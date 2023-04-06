---
content-type: api
navigation-topic: api-navigation-topic
title: Atualizar integrações que usam o controle de versão padrão da API
description: Atualizar integrações que usam o controle de versão padrão da API
author: Becky
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 2b9eacc9b2c8f499cdd1794a55879a56224051c8
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Atualizar integrações que usam o controle de versão padrão da API

Lançamos novas versões da API do Adobe Workfront semestralmente. Cada versão é compatível por três anos após seu lançamento, com um ano adicional em um estado obsoleto, onde a versão está disponível, mas não é compatível.

Integrações que não especificam uma versão da API no URI são encaminhadas automaticamente para o Padrão. Se você quiser que sua chamada de API use uma versão específica da API, deverá especificar essa versão nas solicitações de API do Workfront.

>[!NOTE]
>
>Se sua organização estiver usando atualmente a API padrão, o administrador do Workfront recebeu uma mensagem da Central de anúncios com mais instruções relacionadas à API padrão.

Para saber mais sobre como especificar uma versão nas solicitações de API, consulte [Especificar uma versão da API em suas integrações](../../wf-api/api/specify-api-version-integrations.md).

## Considerações ao usar a API padrão

Considere o seguinte ao trabalhar com a API padrão do Workfront:

* A versão padrão da API da versão mais recente. Qualquer chamada de API sem a versão especificada usará a versão padrão. Sempre que o Workfront lançar uma nova versão da API, a versão padrão será atualizada para a versão mais recente. **Portanto, depois que uma nova versão da API do Workfront for lançada, todas as chamadas de API que usam a versão padrão deverão ser verificadas para garantir que a funcionalidade ainda seja suportada**.
* Se sua organização estiver usando atualmente a antiga API padrão obsoleta, o administrador do Workfront recebeu uma mensagem da Central de anúncios com mais instruções relacionadas à API padrão.

Para ver a versão mais recente da API, consulte [Controle de versão da API e cronograma de suporte](../../wf-api/api/api-version-support-schedule.md).

## Atualização de suas integrações para versões de API compatíveis

Se as solicitações da API do Workfront não especificarem uma versão, elas estarão usando Padrão. Recomendamos suas solicitações de API para especificar uma versão compatível da API, de preferência para a API compatível mais recente.

Por exemplo, a seguinte solicitação da API do Workfront não especifica uma versão da API:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Quando essa solicitação é feita, você recebe uma resposta com texto codificado JSON que especifica dados da sua instância do Workfront. Como nenhuma versão da API é especificada neste URI, a chamada vai para Padrão.

Para transformar uma solicitação de API padrão em uma solicitação de API com versão, basta chamar uma versão de API compatível. Por exemplo, o URI a seguir solicita a Versão 15:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Ao atualizar solicitações de API do Workfront, você pode especificar qualquer versão suportada de nossa API. Para saber mais sobre como fazer referência a uma API específica, consulte [Especificar uma versão da API em suas integrações](../../wf-api/api/specify-api-version-integrations.md).

Para garantir a janela de suporte máximo, você deve chamar a versão mais recente. Você pode encontrar uma lista de APIs compatíveis no [Controle de versão da API e cronograma de suporte](../../wf-api/api/api-version-support-schedule.md).

## Histórico da versão padrão da API

A intenção original da &quot;API padrão&quot;, ou Padrão, era mapeá-la para a versão mais recente da API do Workfront. Isso permitiria que os clientes com integrações básicas que chamavam Default nunca precisassem atualizar suas solicitações de API.

Em 2011, a Workfront lançou a versão 3.0 da API. O padrão foi movido automaticamente para a versão 3.0, o que quebrou muitas integrações de clientes que eram muito complexas para utilizar a versão 3.0 sem ser atualizadas. Como resultado, a Workfront reverteu essa alteração e deixou a versão padrão na Versão 2.

Desde 2011, a Workfront aumentou substancialmente a funcionalidade da API. Por causa disso, as versões mais antigas da nossa API foram substituídas. Em 2017, em vez de atualizar Padrão, removemos totalmente o conceito de uma versão padrão. Isso foi para incentivar nossos clientes a usar versões estáveis de nossas APIs e manter suas integrações em um ciclo de, no máximo, três anos.

A Workfront agora está restabelecendo a versão da API padrão. A API padrão é definida como a versão mais recente da API do Workfront e será atualizada para a versão mais recente sempre que uma nova versão for lançada.

