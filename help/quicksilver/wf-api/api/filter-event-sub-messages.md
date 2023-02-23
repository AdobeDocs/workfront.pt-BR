---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Filtrar mensagens de assinatura do evento
description: Filtrar mensagens de assinatura do evento
author: John
feature: Workfront API
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# Filtrar mensagens de assinatura do evento

Você pode criar componentes de processamento intermediários que podem ajudar você a filtrar e processar apenas as mensagens de assinatura do evento que sua empresa precisa.

Para saber mais sobre assinaturas de evento, consulte [API de assinatura de evento](../../wf-api/general/event-subs-api.md).

## Filtro de mensagens de evento

Esta seção contém trechos de código da filtragem que você pode implementar para diminuir a carga das mensagens de assinatura de evento.  Para ajudar a mostrar as diferenças na sintaxe de vários idiomas, esses trechos ilustram o mesmo conjunto de filtros escritos nos seguintes idiomas:

Você pode exibir exemplos de filtragem em [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples), onde é possível ver as diferenças na sintaxe de cada idioma e os meios de interação com o SDK do AWS.Esses exemplos são escritos como AWS Lambdas, que é um método comum para empregar a filtragem intermediária e os componentes de processamento.

Os seguintes fragmentos de código estão quase prontos para implantação e podem ser usados como ponto de partida para ajudá-lo a escrever seus próprios filtros mais complexos e componentes de processamento.

### Java

O exemplo a seguir em Java mostra como filtrar cargas de projeto com base na ID de grupo do projeto, conforme feito em [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. Estabeleça a ID de grupo que você está procurando e crie-a como uma constante estática.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   Neste exemplo, o método handleRequest, que é um nome de método padrão AWS Lambda, assume um tipo de Map como seu primeiro parâmetro, que é o conteúdo da mensagem de assinatura de evento.\
   O segundo parâmetro é o contexto da solicitação de Proxy Lambda atual.\
   O objeto Context é usado para obter um Lambda Logger, que é usado para gravar uma mensagem no CloudWatchLogs.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. Após a invocação do método handleRequest , obtenha o atributo &quot;newState&quot; da mensagem de assinatura do evento, que representa o estado atualizado do recurso.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   Para saber mais sobre o novo formato de Estado, consulte [Formato de mensagem de saída para assinaturas de eventos](../../wf-api/api/message-format-event-subs.md).

3. Após analisar o mapa &quot;newState&quot; na mensagem, verifique se a ID de grupo do objeto corresponde à ID de grupo identificada na Etapa 1.

4. (Condicional) Se as IDs **não** correspondência, solte a mensagem para que uma resposta vazia seja retornada.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);    
    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
      }
    return "";
   }
   ```

   >[!NOTE]
   >
   >Retornar uma resposta vazia e bem-sucedida é fundamental. Qualquer coisa além de uma resposta de nível 200 é considerada um delivery com falha.

5. Processar a mensagem.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");
   
        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
      }
    ... 
   }
   ```

   O SDK do AWS é usado para chamar outro Lambda, que é responsável por fornecer a mensagem filtrada ao terminal desejado.

   A finalidade de transferir a responsabilidade de entregar a mensagem a outro Lambda é evitar um tempo limite da solicitação de delivery proveniente do serviço de Assinatura de evento. No momento, o tempo limite permitido para a entrega é definido como cinco segundos. Se o filtro demorar mais do que o permitido pela configuração, você poderá processar a solicitação, mas o serviço de Assinatura de evento expirará e entrará em um loop de tentativas até receber uma resposta de nível 200 dentro do período limite.

   Para saber mais sobre como gerenciar o delivery de mensagens, consulte [Aprimoramento Do Delivery De Mensagens Ao Acomodar Os Timeouts](#improving-message-delivery-while-accommodating-timeouts).

### Python

A principal diferença entre os exemplos de Java e Python é que no exemplo de Java a mensagem de assinatura do evento é recebida como o primeiro parâmetro e no exemplo de Python o primeiro parâmetro é um &quot;evento&quot; de proxy Lambda, que contém a mensagem de assinatura do evento junto com informações sobre a solicitação de proxy AWS Lambda.

O exemplo a seguir em Python mostra como filtrar cargas de projeto com base na ID do grupo do projeto, como feito em  [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. Estabeleça a ID de grupo que você está procurando e crie-a como uma constante estática.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   O primeiro parâmetro é o &quot;event&quot; do proxy Lambda, que contém a mensagem de assinatura do evento e algumas informações adicionais que precisam ser analisadas.\
   O segundo parâmetro é o contexto da solicitação de Proxy Lambda atual.\
   Neste exemplo, o objeto Context é usado para obter um Lambda Logger, que é usado para gravar uma mensagem no CloudWatchLogs.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. Analise a mensagem do evento.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. Obtenha o atributo &quot;newState&quot; da mensagem de assinatura do evento.\
   O atributo newState representa o estado atualizado do recurso.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   Para saber mais sobre o novo formato de Estado, consulte [Formato de mensagem de saída para assinaturas de eventos](../../wf-api/api/message-format-event-subs.md).

1. Após analisar o mapa &quot;newState&quot; na mensagem, verifique se a ID de grupo do objeto corresponde à ID de grupo identificada na Etapa 1.

1. (Condicional) Se as IDs não corresponderem, solte a mensagem para que uma resposta vazia seja retornada.

   ```
   if new_state['groupID'] == DESIRED_GROUP_ID:
      # Process the message
      print('matched group ID')
      process_message(event_subscription_message)
   
   return {
   'statusCode': 200
   ```

   >[!NOTE]
   >
   >Retornar uma resposta vazia e bem-sucedida é fundamental. Qualquer coisa além de uma resposta de nível 200 é considerada um delivery com falha.

1. Processar a mensagem.

   ```
   def process_message(event_subscription_message):
      aws_lambda.invoke(
         FunctionName='forwardMessageOntoMyEndpoint',
         InvocationType='Event',
         LogType='None',
         Payload=event_subscription_message
      )
   ```

   O SDK do AWS é usado para chamar outro Lambda, que é responsável por fornecer a mensagem filtrada ao terminal desejado.

   A finalidade de transferir a responsabilidade de entregar a mensagem a outro Lambda é evitar um tempo limite da solicitação de delivery proveniente do serviço de Assinatura de evento. No momento, o tempo limite para a entrega é definido como cinco segundos. Se o filtro demorar mais do que o permitido pela configuração, você poderá processar a solicitação, mas o serviço de Assinatura de evento expirará e entrará em um loop de tentativas até receber uma resposta de nível 200 dentro do período limite.


### Node.js

O exemplo do Node.js da filtragem da ID do grupo de projetos é semelhante aos exemplos de Java e Python. Assim como no exemplo Python, o primeiro parâmetro é um evento de proxy Lambda e o segundo parâmetro é o Contexto Lambda.

O exemplo a seguir em Node.js mostra como filtrar cargas de projeto com base na ID de grupo do projeto, conforme feito em  [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. Estabeleça a ID de grupo que você está procurando e crie-a como uma constante estática.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   O primeiro parâmetro é o &quot;event&quot; do proxy Lambda, que contém a mensagem de assinatura do evento e algumas informações adicionais que precisam ser analisadas.\
   O segundo parâmetro é o contexto da solicitação de Proxy Lambda atual.\
   Neste exemplo, o objeto Context é usado para obter um Lambda Logger, que é usado para gravar uma mensagem no CloudWatchLogs.

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. Analise a mensagem do evento.

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. Obtenha a projectGroupID do atributo &quot;newState&quot; da mensagem de assinatura do evento e, em seguida, corresponda a ela à ID do grupo identificado na Etapa 1.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   Para saber mais sobre o novo formato de Estado, consulte [Formato de mensagem de saída para assinaturas de eventos](../../wf-api/api/message-format-event-subs.md).

4. (Condicional) Se as IDs não corresponderem, solte a mensagem para que uma resposta vazia seja retornada.\
   O exemplo a seguir mostra as IDs de grupo correspondentes:

   ```
   if (projectGroupId === DESIRED_GROUP_ID) {
      // Process the message
      console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
      forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
   } else {
      endLambdaRequest(context);
   }
   ```

   >[!NOTE]
   >
   >Retornar uma resposta vazia e bem-sucedida é fundamental. Qualquer coisa além de uma resposta de nível 200 é considerada um delivery com falha.

5. Processar a mensagem.

   ```
   function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
      let lambdaParams = {
         FunctionName: 'forwardMessageOntoMyEndpoint',
         InvocationType: 'Event',
         LogType: 'None',
         Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
      };
   
      lambda.invoke(lambdaParams, function (err, data) {
         if (err) {
            console.error(err, err.stack);
         } else {
            console.log('data = ' + data);
         }
         endLambdaRequest(context);
      });
   }
   ```

   O SDK do AWS é usado para chamar outro Lambda, que é responsável por fornecer a mensagem filtrada ao terminal desejado.\
   A finalidade de transferir a responsabilidade de entregar a mensagem a outro Lambda é evitar um tempo limite da solicitação de delivery proveniente do serviço de Assinatura de evento. No momento, o tempo limite para a entrega é definido como cinco segundos. Se o filtro demorar mais do que o permitido pela configuração, você poderá processar a solicitação, mas o serviço de Assinatura de evento expirará e entrará em um loop de tentativas até receber uma resposta de nível 200 dentro do período limite.\
   Para saber mais sobre como gerenciar o delivery de mensagens, consulte [Aprimoramento Do Delivery De Mensagens Ao Acomodar Os Timeouts](#improving-message-delivery-while-accommodating-timeouts).

## Aprimoramento Do Delivery De Mensagens Ao Acomodar Os Timeouts

O serviço de Assinatura de evento tem um tempo limite estrito de **cinco segundos** para todas as solicitações de delivery. No caso de o delivery de uma mensagem exceder o tempo permitido, o serviço de Assinatura de evento inicia um ciclo de nova tentativa para essa mensagem.

Por exemplo, você cria um filtro de ID de grupo de projeto semelhante a um dos exemplos encontrados em [Filtro de mensagens de evento](#filtering-event-messages) e inclua uma pesquisa de banco de dados para determinar se a mensagem é necessária. É possível que a pesquisa do banco de dados juntamente com o tempo necessário para o processamento necessário e para o início frio do Lambda possa levar mais de cinco segundos, fazendo com que o serviço de Assinatura de evento tente novamente entregando a mensagem.

Você pode evitar uma nova tentativa separando as partes demoradas do processo da lógica responsável por determinar se a mensagem é uma mensagem que você deseja processar e entregar. Ao fazer isso, você pode aceitar a mensagem e enviar uma resposta de nível 200 para o serviço de Assinatura do evento, enquanto continua de forma assíncrona a processar ou filtrar a mensagem em segundo plano (consulte a Etapa 5 em [Java](#java) para um exemplo).


Mesmo que o processamento ou a filtragem não exceda o tempo limite de cinco segundos, ainda é vantajoso separar o primeiro ponto de contato da filtragem ou do processamento de mensagens das outras etapas de processamento ou entrega no lado do cliente. Dessa forma, o handoff da mensagem para o destino a partir do serviço de Assinatura de evento tem impacto mínimo no tempo e no desempenho para ambas as partes.

Para saber mais sobre o mecanismo de repetição, consulte [Tentativas de assinatura do evento](../../wf-api/api/event-sub-retries.md).

## Implementação de filtros hospedados na arquitetura sem nuvens

Se você não conseguir aproveitar uma arquitetura de nuvem para a filtragem de assinatura de evento, ainda poderá usar os exemplos em [Filtro de mensagens de evento](#filtering-event-messages) como roteiros de como implementar seus próprios filtros hospedados ou componentes de processamento.

### Ajustar exemplos de filtragem para serviços independentes

Antes de usar os exemplos de filtragem em um ambiente sem nuvens, faça o seguinte:

* Omita as partes específicas do Lambda dos exemplos, como o parâmetro Context .

* Altere as invocações de outros Lambdas nos exemplos para fazer solicitações HTTP assíncronas adicionais para outros filtros ou componentes de processamento que você hospeda.

* Se estiver fazendo referência aos exemplos de Python e Node.js , substitua o primeiro parâmetro de evento pelo primeiro parâmetro de carga mostrado no exemplo de Java. Consulte a Etapa 1 em [Java](#java).

* Implante os filtros ou processadores com uma API baseada na Web.

### Evitando Mensagens de Assinatura de Evento Ausentes

Ocasionalmente, em uma arquitetura sem nuvens, os serviços responsáveis por receber mensagens de assinatura de evento podem estar inacessíveis. Nesse caso, as mensagens podem exceder o limite de tentativas e serem perdidas, sem como recuperar as informações nas mensagens.

Recomendamos que, durante a inicialização do serviço, você implemente um query solicitando o estado mais recente de todos os recursos que podem ter sido incluídos nas mensagens perdidas. Como mostrado no exemplo a seguir, você pode usar os critérios de filtro para buscar recursos que correspondam a esses critérios e, em seguida, processar seu estado atual.

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v15.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;
    try 
    {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
      } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}
```

Ao consultar recursos, você garante que seus sistemas integradores tenham a versão mais recente dos recursos.

### Implementação de processamento assíncrono na entrega de mensagens

Todos os exemplos na [Filtro de mensagens de evento](#filtering-event-messages) passe a responsabilidade de enviar mensagens filtradas para outro AWS Lambda. Isso é feito para evitar exceder o tempo limite de cinco segundos na solicitação de delivery, que é imposta pelo serviço de Assinatura de evento que emite a solicitação.

Em uma arquitetura sem nuvens, talvez seja necessário implementar um mecanismo de processamento assíncrono semelhante à forma como o SDK da AWS permite chamadas assíncronas para outros AWS Lambdas. A maioria das linguagens de programação modernas tem bibliotecas principais ou de terceiros que lidam com processamento assíncrono, permitindo aproveitar o estilo assíncrono de processamento implementado em nossos exemplos.
