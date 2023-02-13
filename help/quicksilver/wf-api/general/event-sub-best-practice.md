---
content-type: api
navigation-topic: general-api
title: Práticas recomendadas de assinatura de evento
description: Práticas recomendadas de assinatura de evento
author: John
feature: Workfront API
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 50675b7af3fcd2188a18391732a93a7b67454db9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Práticas recomendadas de assinatura de evento

As mensagens de Assinatura de evento do Adobe Workfront são enviadas automaticamente do Workfront após a configuração correta do serviço e a criação de uma Assinatura de evento para acionar esses deliveries de mensagem. Para saber mais sobre como configurar corretamente assinaturas de evento, consulte [Requisitos de delivery de assinatura de evento](../../wf-api/general/setup-event-sub-endpoint.md).


Veja abaixo algumas práticas recomendadas para ajudá-lo a criar assinaturas de evento com eficácia.

## Fornecer todos os campos de corpo de solicitação necessários

Verifique se todos os campos de corpo da solicitação necessários foram fornecidos para a API. Para obter informações sobre todos os atributos de solicitação necessários, consulte [API de assinatura de evento](../../wf-api/general/event-subs-api.md).

## Evite incluir campos de corpo extras

Não inclua campos de corpo extras na solicitação, pois isso resultará na falha da API ao criar uma assinatura.

## Concluir o teste dentro do período de carência

Tente realizar todos os testes de assinatura dentro do período de carência de 100 mensagens. Para saber mais sobre esse período de carência, consulte [Perguntas frequentes - Assinaturas de eventos](../../wf-api/general/event-subs-faq.md).

## Satisfazer os requisitos padrão de entrega de mensagem de assinatura do evento

Certifique-se de que o terminal de subscrição está em conformidade com os Requisitos Padrão de Entrega da Mensagem de Subscrição de Eventos. Para saber mais sobre esses requisitos, consulte [Requisitos de delivery de assinatura de evento](../../wf-api/general/setup-event-sub-endpoint.md).

## lista de permissões endereços IP por região global

Para receber cargas de assinatura de evento por meio do firewall, é necessário adicionar os endereços IP à lista de permissões por região global. Para saber mais, consulte [API de assinatura de evento](../../wf-api/general/event-subs-api.md).

## Ter o nível de acesso correto e uma chave de API

Para criar, consultar ou excluir uma Assinatura de evento, o usuário do Workfront precisa:

* Um nível de acesso de **Administrador do sistema**
Para saber mais, consulte [Conceder ao usuário acesso administrativo total](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) ou [Conceder aos usuários acesso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Uma chave de API

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
