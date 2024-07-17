---
content-type: api
keywords: API,dados,sincronização,diário,entrada,objeto
navigation-topic: general-api
title: Usar a API para sincronizar dados de programas e serviços
description: Usar a API para sincronizar dados de programas e serviços
author: Becky
feature: Workfront API
role: Developer
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Uso da API para sincronizar dados de programas e serviços

Essas são algumas maneiras comuns de utilizar a API para sincronizar dados de programas e serviços.

## Atualizações quase em tempo real

O Adobe Workfront usa &quot;Assinaturas de eventos&quot; (também comumente chamadas de webhooks) para enviar atualizações quase em tempo real sobre objetos e ações compatíveis, por meio da API, para os endpoints desejados. Você pode esperar receber uma atualização sobre novos objetos e ações em 5 segundos, mas, em média, as atualizações chegam em aproximadamente 1 segundo. Para obter informações adicionais sobre que tipo de objetos são aceitos, que tipo de ações são aceitas, detalhes técnicos e exemplos de como configurar assinaturas de evento, consulte a [API de Assinatura de Evento](../../wf-api/general/event-subs-api.md) e os [requisitos de entrega de Assinatura de Evento](../../wf-api/general/setup-event-sub-endpoint.md).

## Atualizações em lote

As atualizações em lote são uma maneira de configurar o sistema para atualizações, fazendo solicitações periódicas aos servidores do Workfront. Há várias maneiras de fazer isso, mas geralmente o processo consiste em fazer com que seu serviço faça uma solicitação aos servidores de API do Workfront e procure objetos que foram criados ou modificados desde a última chamada de solicitação. GET Para obter informações sobre chamadas de solicitações potenciais e parâmetros úteis, consulte a seção [Comportamento](../../wf-api/general/api-basics.md#get-behavior) do artigo [noções básicas sobre API](../../wf-api/general/api-basics.md).

Ao configurar seu serviço para atualizações em lote, lembre-se das seguintes informações importantes:

### Datas de entrada

As datas de entrada são armazenadas utilizando a formatação ISO 8601. Esse padrão inclui informações de data, hora e fuso horário.

**Exemplo:** formato de data ISO 8601

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

Tanto a data em que um objeto é criado quanto a última data em que o objeto foi modificado são armazenadas como &quot;entryDate&quot; e &quot;lastUpdateDate&quot;, respectivamente. Para obter informações detalhadas sobre objetos Workfront, seus campos associados e nomes de campo, consulte o [API Explorer](../../wf-api/general/api-explorer.md). Observe que a entryDate de um determinado objeto do Workfront não é alterada, enquanto a lastUpdatedDate é alterada sempre que o objeto é modificado.

**Exemplo:** GET para um objeto de problema, utilizando o campo **lastUpdateDate**. Essa solicitação retornaria todos os problemas atualizados desde a data especificada.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Objeto de entrada do diário

Se você estiver interessado em obter alterações referentes a um campo específico em um objeto, poderá consultar o objeto &quot;Lançamento do diário&quot;. O objeto de Entrada do Diário do Workfront pode ser configurado para registrar informações sobre campos de objeto específicos sempre que esses campos forem modificados. Consulte [Configurar atualizações do sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) para obter detalhes adicionais.

Quando um campo é configurado para ser registrado como parte do objeto de Lançamento no Diário, uma Entrada no Diário correspondente será criada toda vez que o campo for modificado. Em seguida, você pode consultar o objeto Lançamento do diário usando uma chamada de API semelhante ao seguinte:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot; é usada para verificar uma entrada de diário de uma alteração, em vez de verificar o próprio objeto alterado.
