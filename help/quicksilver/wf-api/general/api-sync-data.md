---
content-type: api
keywords: API,dados,sincronização,diário,entrada,objeto
navigation-topic: general-api
title: Usar a API para sincronizar dados de programas e serviços
description: Usar a API para sincronizar dados de programas e serviços
author: Becky
feature: Workfront API
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# Usar a API para sincronizar dados de programas e serviços

Essas são algumas maneiras comuns de utilizar a API para sincronizar dados de programas e serviços.

## Atualizações quase em tempo real

O Adobe Workfront usa &quot;Assinaturas de eventos&quot; (também comumente chamadas de webhooks) para enviar atualizações quase em tempo real sobre objetos e ações compatíveis, por meio da API, aos endpoints desejados. Você pode esperar receber uma atualização em relação a novos objetos e ações em 5 segundos, mas, em média, as atualizações chegam em aproximadamente 1 segundo. Para obter mais informações sobre que tipo de objetos são aceitos, quais tipos de ações são aceitas, detalhes técnicos e exemplos para configurar assinaturas de eventos, consulte [API de assinatura de evento](../../wf-api/general/event-subs-api.md) e [Requisitos de delivery de assinatura de evento](../../wf-api/general/setup-event-sub-endpoint.md).

## Atualizações em lote

As atualizações em lote são uma maneira de configurar o sistema para atualizações, fazendo solicitações periódicas para os servidores da Workfront. Há muitas maneiras de fazer isso, mas geralmente o processo consiste em fazer com que seu serviço faça uma solicitação aos servidores de API da Workfront e procure objetos que foram criados ou modificados desde a última chamada de solicitação. Para obter informações sobre possíveis chamadas de solicitações e parâmetros úteis, consulte [Comportamento do GET](../../wf-api/general/api-basics.md#get-behavior) da seção [Noções básicas da API](../../wf-api/general/api-basics.md) artigo 10. o

Como você está configurando seu serviço para atualizações em lote, lembre-se de algumas coisas importantes:

### Datas da entrada

As datas de entrada são armazenadas utilizando a formatação ISO 8601. Esse padrão inclui informações de data, hora e fuso horário.

**Exemplo:** Formato de data ISO 8601

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

A data em que um objeto é criado e a última data em que o objeto foi modificado são armazenadas como &quot;entryDate&quot; e &quot;lastUpdateDate&quot;, respectivamente. Para obter informações detalhadas sobre objetos Workfront, seus campos associados e nomes de campos, consulte o [API Explorer](../../wf-api/general/api-explorer.md). Observe que entryDate para qualquer objeto Workfront específico não é alterado, onde, à medida que lastUpdatedDate for alterado sempre que o objeto for modificado.

**Exemplo:** Solicitação de GET para um objeto de problema, utilizando o **lastUpdateDate** campo. Essa solicitação retornaria todos os problemas atualizados desde essa data especificada.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Objeto de entrada de diário

Se você estiver interessado em obter alterações em relação a um campo específico em um objeto, poderá consultar o objeto &quot;Entrada de diário&quot;. O objeto Entrada de diário do Workfront pode ser configurado para registrar informações sobre campos de objeto específicos sempre que esses campos forem modificados, consulte [Configurar atualizações do sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) para obter mais detalhes.

Quando um campo é configurado para ser registrado como parte do objeto Entrada de Diário, uma Entrada de Diário correspondente será criada sempre que esse campo for modificado. Em seguida, você pode consultar o objeto Entrada de diário usando uma chamada de API semelhante ao seguinte:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot; é usado para examinar um lançamento de uma alteração, em vez de analisar o próprio objeto alterado.
