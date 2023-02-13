---
content-type: api
navigation-topic: api-navigation-topic
title: Atualizar integrações que usam o controle de versão padrão da API
description: Atualizar integrações que usam o controle de versão padrão da API
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Atualizar integrações que usam o controle de versão padrão da API

Lançamos novas versões da API do Adobe Workfront semestralmente. Cada versão é compatível por três anos após seu lançamento, com um ano adicional em um estado obsoleto, onde a versão está disponível, mas não é compatível.

Integrações que não especificam uma versão da API no URI são encaminhadas automaticamente para o Padrão, que foi substituído. Para que as integrações do Workfront sejam válidas, você deve especificar uma versão da API compatível nas solicitações da API do Workfront.

Para saber mais sobre como especificar uma versão nas solicitações de API, consulte [Especificar uma versão da API em suas integrações](../../wf-api/api/specify-api-version-integrations.md).

## Noções básicas sobre a versão padrão da API

A intenção original da &quot;API padrão&quot;, ou Padrão, era mapeá-la para a versão mais recente da API do Workfront. Isso permitiria que os clientes com integrações básicas que chamavam Default nunca precisassem atualizar suas solicitações de API.

Em 2011, a Workfront lançou a versão 3.0 da API. O padrão foi movido automaticamente para a versão 3.0, o que quebrou muitas integrações de clientes que eram muito complexas para utilizar a versão 3.0 sem ser atualizadas. Como resultado, a Workfront reverteu essa alteração e deixou a versão padrão na Versão 2.

Infelizmente, esse tópico nunca foi revisitado e, agora que planejamos aumentar substancialmente a funcionalidade da API, somos forçados a rejeitar versões mais antigas da nossa API, incluindo Padrão. Em vez de atualizar Padrão, o que certamente quebraria mais integrações, estamos removendo o conceito de uma versão padrão totalmente. Isso incentiva nossos clientes a usar versões estáveis de nossas APIs e a manter suas integrações em um ciclo de, no máximo, três anos.

## Descontinuar padrão

Em um esforço para melhorar a API do Workfront, estamos removendo versões de API mais antigas que excederam nossa janela de suporte de três anos. Uma dessas versões é a versão 2, para a qual o Padrão é mapeado. Essa versão foi lançada em 2010 e grande parte da lógica compatível com o aplicativo Attask/Workfront naquela época não existe mais ou mudou substancialmente.

Substituímos o Padrão em julho de 2017 e não designaremos mais uma versão específica da API para ser a versão padrão. Em vez disso, todas as solicitações da API do Workfront devem especificar uma versão específica da API.

>[!IMPORTANT]
>
> Até 1º de julho de 2018, todas as integrações do Workfront que usam Padrão devem ser atualizadas para chamar uma versão específica da API compatível. Após essa data, todas as solicitações da API do Workfront usadas por integrações que não especificam uma versão falharão.

Para saber mais sobre a cadência de desativação do Workfront, consulte [Controle de versão da API e cronograma de suporte](../../wf-api/api/api-version-support-schedule.md).

## Atualização de suas integrações para versões de API compatíveis

Se as solicitações da API do Workfront não especificarem uma versão, elas estarão usando Padrão. Você deve atualizar as solicitações de API para especificar uma versão compatível da API, de preferência para a API compatível mais recente.

Por exemplo, a seguinte solicitação da API do Workfront não especifica uma versão da API:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Quando essa solicitação é feita, você recebe uma resposta com texto codificado JSON que especifica dados da sua instância do Workfront. Como nenhuma versão da API é especificada neste URI, a chamada vai para Padrão.

Para transformar uma solicitação de API padrão em uma solicitação de API com versão, basta chamar uma versão de API compatível. Por exemplo, o URI a seguir solicita a Versão 9:

`https://davidwhite.my.workfront.com/attask/api/`**v9.0**`/project/metadata`

Ao atualizar solicitações de API do Workfront, você pode especificar qualquer versão suportada de nossa API. Para saber mais sobre como fazer referência a uma API específica, consulte [Especificar uma versão da API em suas integrações](../../wf-api/api/specify-api-version-integrations.md).

Para garantir a janela de suporte máximo, você deve chamar a versão mais recente (Versão 9). Você pode encontrar uma lista de APIs compatíveis no [Controle de versão da API e cronograma de suporte](../../wf-api/api/api-version-support-schedule.md).

É fundamental atualizar as integrações que você tem que usam Padrão. Caso tenha integrações que não especificam uma versão, poderá receber uma notificação do vendedor da Workfront, do gerente de sucesso do cliente ou do representante de suporte, ou uma mensagem do centro de anúncios.

Assim que possível, certifique-se de que suas integrações sejam atualizadas para chamar uma versão compatível de nossa API.
