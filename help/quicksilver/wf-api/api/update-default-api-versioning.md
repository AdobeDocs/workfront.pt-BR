---
content-type: api
navigation-topic: api-navigation-topic
title: Atualizar integrações que usam o controle de versão da API padrão
description: Atualizar integrações que usam o controle de versão da API padrão
author: Becky
feature: Workfront API
role: Developer
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Atualizar integrações que usam o controle de versão da API padrão

Lançamos novas versões da API do Adobe Workfront semestralmente. Cada versão é compatível por três anos após seu lançamento, com um ano adicional em um estado obsoleto, em que a versão está disponível, mas não é compatível.

Integrações que não especificam uma versão da API no URI são automaticamente roteadas para Padrão. Se quiser que sua chamada de API use uma versão específica da API, você deve especificar essa versão em suas solicitações de API do Workfront.

>[!NOTE]
>
>Se sua organização estiver usando a API padrão no momento, o administrador do Workfront receberá uma mensagem do Centro de notificações com mais instruções sobre a API padrão.

Para saber mais sobre como especificar uma versão em suas solicitações de API, consulte [Especificar uma versão de API em suas integrações](../../wf-api/api/specify-api-version-integrations.md).

## Considerações ao usar a API padrão

Considere o seguinte ao trabalhar com a API padrão do Workfront:

* A versão padrão da API é a versão mais recente. Qualquer chamada de API sem a versão especificada usará a versão padrão. Cada vez que o Workfront lança uma nova versão da API, a versão padrão será atualizada para a versão mais recente. **Portanto, depois que uma nova versão da API do Workfront for lançada, todas as chamadas de API que usam a versão padrão deverão ser verificadas para garantir que a funcionalidade ainda tenha suporte**.
* Se sua organização estiver usando a API padrão obsoleta anteriormente, o administrador do Workfront receberá uma mensagem do Centro de notificações com mais instruções sobre a API padrão.

Para ver a versão mais recente da API, consulte [Controle de versão da API e agendamento de suporte](../../wf-api/api/api-version-support-schedule.md).

## Atualização das integrações para versões de API compatíveis

Se as solicitações de API do Workfront não especificarem uma versão, elas usarão o padrão. Recomendamos suas solicitações de API para especificar uma versão compatível da API, de preferência para a API compatível mais recente.

Por exemplo, a seguinte solicitação de API do Workfront não especifica uma versão da API:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Quando essa solicitação é feita, você recebe uma resposta com texto codificado em JSON que especifica os dados da sua instância do Workfront. Como nenhuma versão da API é especificada nesse URI, a chamada vai para Padrão.

Para transformar uma solicitação de API padrão em uma solicitação de API com versão, basta chamar uma versão de API compatível. Por exemplo, o seguinte URI solicita a versão 15:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Ao atualizar suas solicitações de API do Workfront, você pode especificar qualquer versão compatível da nossa API. Para saber mais sobre como fazer referência a uma API específica, consulte [Especificar uma Versão da API em suas integrações](../../wf-api/api/specify-api-version-integrations.md).

Para garantir a janela de suporte máxima, você deve chamar a versão mais recente. Você pode encontrar uma lista de APIs compatíveis em [Controle de versão da API e programação de suporte](../../wf-api/api/api-version-support-schedule.md).

## Histórico da versão padrão da API

A intenção original da &quot;API padrão&quot;, ou Padrão, era mapeá-la para a versão mais recente da API do Workfront. Isso permitiria que os clientes com integrações básicas chamadas de Padrão nunca precisassem atualizar suas solicitações de API.

Em 2011, o Workfront lançou a versão 3.0 da API. O padrão foi movido automaticamente para a versão 3.0, o que prejudicou muitas integrações de clientes que eram muito complexas para utilizar a versão 3.0 sem serem atualizadas. Como resultado, o Workfront reverteu essa alteração e deixou a versão padrão na Versão 2.

Desde 2011, o Workfront aumentou substancialmente a funcionalidade da API. Por causa disso, substituímos versões mais antigas da API. Em 2017, em vez de atualizar o Padrão, removemos completamente o conceito de uma versão padrão. Isso incentivava nossos clientes a usar versões estáveis de nossas APIs e a manter suas integrações em um ciclo de, no máximo, três anos.

Agora, o Workfront está restabelecendo a versão da API padrão. A API padrão está definida como a versão mais recente da API do Workfront e será atualizada para a versão mais recente sempre que uma nova versão for lançada.

