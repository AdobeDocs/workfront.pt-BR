---
content-type: api
navigation-topic: general-api
title: Práticas recomendadas de assinatura de evento
description: Práticas recomendadas de assinatura de evento
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 19e0b792bc49ede0504af479952fdbdf384dc73c
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# Práticas recomendadas de assinatura de evento

As mensagens de Assinatura de evento do Adobe Workfront são enviadas automaticamente pelo Workfront depois de configurar corretamente o serviço e criar uma Assinatura de evento para acionar essas entregas de mensagem. Para saber mais sobre como configurar corretamente Assinaturas de Eventos, consulte [Requisitos de entrega de Assinatura de Eventos](../../wf-api/general/setup-event-sub-endpoint.md).


Veja abaixo algumas práticas recomendadas para ajudá-lo a criar assinaturas de evento de maneira eficiente.

## Forneça todos os campos de corpo de solicitação obrigatórios

Verifique se todos os campos obrigatórios do corpo da solicitação foram fornecidos para a API. Para obter informações sobre todos os atributos de solicitação necessários, consulte a [API de Assinatura de Evento](../../wf-api/general/event-subs-api.md).

## Evite incluir campos de corpo extras

Não inclua campos de corpo extras na solicitação, pois isso resultará na falha da API ao criar uma assinatura.

## Concluir o teste dentro do período de carência

Tente concluir todos os testes de assinatura dentro do período de carência de 100 mensagens. Para saber mais sobre este período de carência, consulte [Perguntas frequentes - Assinaturas de Eventos](../../wf-api/general/event-subs-faq.md).

## Atender aos requisitos padrão de entrega de mensagens de assinatura de eventos

Verifique se o endpoint de sua assinatura está em conformidade com os Requisitos de Entrega de Mensagem de Assinatura de Evento Padrão. Para saber mais sobre esses requisitos, consulte [Requisitos de entrega de assinatura de evento](../../wf-api/general/setup-event-sub-endpoint.md).

## ➡ Incluir na lista de permissões endereços IP por região global

Para receber payloads de subscrições de evento por meio do firewall, você deve adicionar os endereços IP à inclui na lista de permissões por região global. Para saber mais, consulte [API de Assinatura de Evento](../../wf-api/general/event-subs-api.md).

## Ter o nível de acesso e a autenticação certos

Para criar, consultar ou excluir uma Assinatura de Evento, o usuário do Workfront precisa:

* Um nível de acesso de **Administrador do Sistema**
Para saber mais, consulte [Conceder a um usuário acesso administrativo total](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) ou [Conceder aos usuários acesso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Um cabeçalho `sessionID` é necessário para usar a API de Assinaturas de Eventos

  Para obter mais informações, consulte [Autenticação](api-basics.md#authentication) em [Noções básicas sobre API](api-basics.md).
