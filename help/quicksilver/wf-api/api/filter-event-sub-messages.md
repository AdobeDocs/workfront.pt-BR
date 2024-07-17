---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Filtrar mensagens de assinatura de eventos
description: Filtrar mensagens de assinatura de eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1767'
ht-degree: 0%

---

# Filtrar mensagens de assinatura de eventos

Você pode criar componentes de processamento intermediários que podem ajudá-lo a filtrar e processar apenas as mensagens de assinatura do evento de que sua empresa precisa.

Para saber mais sobre assinaturas de evento, consulte [API de Assinatura de Evento](../../wf-api/general/event-subs-api.md).

## Filtrar mensagens de evento

Esta seção contém trechos de código de filtragem que podem ser implementados para diminuir a carga de mensagens de subscrição de eventos.  Para ajudar a mostrar as diferenças na sintaxe de vários idiomas, esses trechos ilustram o mesmo conjunto de filtros escritos nos seguintes idiomas:

Você pode ver exemplos de filtragem em [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples), onde você pode ver as diferenças na sintaxe de cada idioma e os meios de interação com o SDK do AWS. Esses exemplos são escritos como AWS Lambdas, que é um método comum para empregar filtragem intermediária e componentes de processamento.

Os trechos de código a seguir estão quase prontos para implantação e podem ser usados como ponto de partida para ajudar você a escrever seus próprios filtros e componentes de processamento mais complexos.

### Java

O exemplo a seguir em Java mostra como filtrar cargas do projeto com base na ID de Grupo do projeto, como feito em [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. Estabeleça a ID de grupo que você está procurando e crie-a como uma constante estática.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   Neste exemplo, o método handleRequest, que é um nome de método padrão AWS Lambda, usa um tipo Map como seu primeiro parâmetro, que é o conteúdo da mensagem de subscrição do evento.\
   O segundo parâmetro é o contexto da solicitação atual do Proxy Lambda.\
   O objeto Context é usado para obter um Lambda Logger, que é usado para gravar uma mensagem no CloudWatchLogs.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. Após a invocação do método handleRequest, obtenha o atributo &quot;newState&quot; da mensagem de subscrição do evento, que representa o estado atualizado do recurso.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   Para saber mais sobre o novo formato State, consulte [Formato de mensagem de saída para assinaturas de evento](../../wf-api/api/message-format-event-subs.md).

3. Depois de analisar o mapa &quot;newState&quot; da mensagem, verifique se a ID do grupo do objeto corresponde à ID do grupo identificada na Etapa 1.

4. (Condicional) Se as IDs **não** corresponderem, remova a mensagem para que uma resposta vazia seja retornada.

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
   >Retornar uma resposta vazia e bem-sucedida é essencial. Qualquer coisa além de uma resposta em nível 200 é considerada uma entrega com falha.

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

   O SDK do AWS é usado para invocar outro Lambda, que é responsável por enviar a mensagem filtrada para o endpoint desejado.

   O objetivo de passar a responsabilidade de entregar a mensagem para outro Lambda é evitar um tempo limite da solicitação de entrega proveniente do serviço de Assinatura do evento. Atualmente, o tempo limite permitido para entrega é definido como cinco segundos. Se o filtro levar mais tempo do que o permitido pela configuração, você poderá processar a solicitação, mas o serviço de Assinatura de evento expirará e entrará em um loop de repetição até que receba uma resposta de 200 níveis dentro do período de tempo limite.

   Para saber mais sobre como gerenciar a entrega de mensagens, consulte [Melhorando a Entrega de Mensagens Enquanto Acomoda Tempos Limite](#improving-message-delivery-while-accommodating-timeouts).

### Python

A principal diferença entre os exemplos Java e Python é que no exemplo Java a mensagem de subscrição do evento é recebida como o primeiro parâmetro e no exemplo Python o primeiro parâmetro é um &quot;evento&quot; de proxy Lambda, que contém a mensagem de subscrição do evento juntamente com informações sobre a solicitação de proxy Lambda do AWS.

O exemplo a seguir no Python mostra como filtrar cargas do projeto com base na ID de Grupo do projeto, como feito em [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. Estabeleça a ID de grupo que você está procurando e crie-a como uma constante estática.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   O primeiro parâmetro é o &quot;evento&quot; proxy Lambda, que contém a mensagem de subscrição do evento e algumas informações adicionais que precisam ser analisadas.\
   O segundo parâmetro é o contexto da solicitação atual do Proxy Lambda.\
   Neste exemplo, o objeto Context é usado para obter um Lambda Logger, que é usado para gravar uma mensagem no CloudWatchLogs.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. Analise a mensagem do evento.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. Obtenha o atributo &quot;newState&quot; da mensagem de subscrição do evento.\
   O atributo newState representa o estado atualizado do recurso.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   Para saber mais sobre o novo formato State, consulte [Formato de mensagem de saída para assinaturas de evento](../../wf-api/api/message-format-event-subs.md).

1. Depois de analisar o mapa &quot;newState&quot; da mensagem, verifique se a ID do grupo do objeto corresponde à ID do grupo identificada na Etapa 1.

1. (Condicional) Se as IDs não corresponderem, remova a mensagem para que uma resposta vazia seja retornada.

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
   >Retornar uma resposta vazia e bem-sucedida é essencial. Qualquer coisa além de uma resposta em nível 200 é considerada uma entrega com falha.

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

   O SDK do AWS é usado para invocar outro Lambda, que é responsável por enviar a mensagem filtrada para o endpoint desejado.

   O objetivo de passar a responsabilidade de entregar a mensagem para outro Lambda é evitar um tempo limite da solicitação de entrega proveniente do serviço de Assinatura do evento. Atualmente, o tempo limite para entrega é definido como cinco segundos. Se o filtro levar mais tempo do que o permitido pela configuração, você poderá processar a solicitação, mas o serviço de Assinatura de evento expirará e entrará em um loop de repetição até que receba uma resposta de 200 níveis dentro do período de tempo limite.


### Node.js

O exemplo de Node.js da filtragem de ID de grupo de projeto é semelhante aos exemplos de Java e Python. Assim como no exemplo do Python, o primeiro parâmetro é um evento proxy Lambda e o segundo parâmetro é o Contexto Lambda.

O exemplo a seguir em Node.js mostra como filtrar cargas do projeto com base na ID do Grupo do projeto, como feito em [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. Estabeleça a ID de grupo que você está procurando e crie-a como uma constante estática.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   O primeiro parâmetro é o &quot;evento&quot; proxy Lambda, que contém a mensagem de subscrição do evento e algumas informações adicionais que precisam ser analisadas.\
   O segundo parâmetro é o contexto da solicitação atual do Proxy Lambda.\
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

3. Obtenha a projectGroupID do atributo &quot;newState&quot; da mensagem de subscrição do evento, em seguida, compare-a com a ID do grupo identificado na Etapa 1.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   Para saber mais sobre o novo formato State, consulte [Formato de mensagem de saída para assinaturas de evento](../../wf-api/api/message-format-event-subs.md).

4. (Condicional) Se as IDs não corresponderem, remova a mensagem para que uma resposta vazia seja retornada.\
   O exemplo a seguir mostra IDs de grupo correspondentes:

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
   >Retornar uma resposta vazia e bem-sucedida é essencial. Qualquer coisa além de uma resposta em nível 200 é considerada uma entrega com falha.

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

   O SDK do AWS é usado para invocar outro Lambda, que é responsável por enviar a mensagem filtrada para o endpoint desejado.\
   O objetivo de passar a responsabilidade de entregar a mensagem para outro Lambda é evitar um tempo limite da solicitação de entrega proveniente do serviço de Assinatura do evento. Atualmente, o tempo limite para entrega é definido como cinco segundos. Se o filtro levar mais tempo do que o permitido pela configuração, você poderá processar a solicitação, mas o serviço de Assinatura de evento expirará e entrará em um loop de repetição até que receba uma resposta de 200 níveis dentro do período de tempo limite.\
   Para saber mais sobre como gerenciar a entrega de mensagens, consulte [Melhorando a Entrega de Mensagens Enquanto Acomoda Tempos Limite](#improving-message-delivery-while-accommodating-timeouts).

## Melhorar A Entrega De Mensagens Enquanto Acomoda Os Tempos Limite

O serviço de Assinatura de Eventos tem um tempo limite estrito de **cinco segundos** para todas as solicitações de entrega. Caso a entrega de uma mensagem exceda o tempo permitido, o serviço Assinatura do Evento iniciará um ciclo de nova tentativa para essa mensagem.

Por exemplo, você cria um filtro de ID de grupo de projeto semelhante a um dos exemplos encontrados em [Filtrando Mensagens de Evento](#filtering-event-messages) e inclui uma pesquisa de banco de dados para determinar se a mensagem é necessária. É possível que a pesquisa do banco de dados, juntamente com o tempo necessário para o processamento necessário e para o início forçado do Lambda, demore mais de cinco segundos, fazendo com que o serviço de Assinatura do Evento tente enviar a mensagem novamente.

É possível evitar uma nova tentativa separando as partes demoradas do processo da lógica responsável por determinar se a mensagem é processada e entregue. Ao fazer isso, você pode aceitar a mensagem e enviar uma resposta de 200 níveis para o serviço Assinatura de Evento, enquanto continua de forma assíncrona o processamento ou a filtragem da mensagem em segundo plano (consulte a Etapa 5 no [Java](#java) para obter um exemplo).


Mesmo que o processamento ou a filtragem não exceda o tempo limite de cinco segundos, ainda é vantajoso separar o primeiro ponto de contato da filtragem ou do processamento de mensagens das outras etapas de processamento ou entrega no lado do cliente. Dessa forma, a entrega da mensagem para o destino a partir do serviço de Assinatura do evento tem impacto mínimo no tempo e no desempenho para ambas as partes.

Para saber mais sobre o mecanismo de repetição, consulte [Tentativas de assinatura de evento](../../wf-api/api/event-sub-retries.md).

## Implementação de filtros hospedados na arquitetura sem nuvem

Se você não conseguir aproveitar a arquitetura de nuvem para filtragem de assinaturas de eventos, ainda poderá usar os exemplos em [Filtrar mensagens de evento](#filtering-event-messages) como roteiros de como implementar seus próprios filtros hospedados ou componentes de processamento.

### Ajustar exemplos de filtragem para serviços independentes

Antes de usar os exemplos de filtragem em um ambiente sem nuvem, faça o seguinte:

* Omita as partes específicas de Lambda dos exemplos, como o parâmetro Context.

* Altere as invocações de outros Lambdas nos exemplos para fazer solicitações HTTP assíncronas adicionais para outros filtros ou componentes de processamento que você hospeda.

* Se estiver fazendo referência aos exemplos de Python e Node.js, substitua o primeiro parâmetro de evento pelo primeiro parâmetro de payload mostrado no exemplo de Java. Consulte a Etapa 1 em [Java](#java).

* Implante os filtros ou processadores com uma API baseada na Web.

### Evitando Mensagens de Assinatura de Evento Perdidas

Ocasionalmente, em uma arquitetura sem nuvem, os serviços responsáveis por receber mensagens de assinatura de evento podem estar inacessíveis. Nesse caso, as mensagens podem exceder o limite de novas tentativas e ser perdidas, sem como recuperar as informações nas mensagens.

Recomendamos que durante a inicialização do serviço você implemente uma query solicitando o estado mais recente de todos os recursos que podem ter sido incluídos nas mensagens perdidas. Como mostrado no exemplo a seguir, você pode usar os critérios de filtro para consultar recursos que correspondem a esses critérios e processar seu estado atual.

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

Ao consultar os recursos, você garante que seus sistemas de integração tenham a versão mais recente dos recursos.

### Implementação do processamento assíncrono no delivery de mensagens

Todos os exemplos na seção [Filtering Event Messages](#filtering-event-messages) passam a responsabilidade de entregar mensagens filtradas para outro AWS Lambda. Isso é feito para evitar exceder o tempo limite de cinco segundos na solicitação de delivery, que é imposta pelo serviço de Assinatura de evento que emite a solicitação.

Em uma arquitetura sem nuvem, talvez seja necessário implementar um mecanismo de processamento assíncrono semelhante ao modo como o SDK do AWS permite chamadas assíncronas para outros AWS Lambdas. A maioria das linguagens de programação modernas tem bibliotecas de terceiros ou principais que lidam com o processamento assíncrono, permitindo que você aproveite o estilo assíncrono de processamento implementado em nossos exemplos.
