---
content-type: api
navigation-topic: general-api
title: Requisitos de entrega de Assinatura de Evento
description: Requisitos de entrega de Assinatura de Evento
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Requisitos de entrega de Assinatura de Evento

As mensagens de assinatura de evento são notificações que podem ser configuradas para notificar os usuários quando determinados eventos ocorrem. Para saber mais sobre o que são Assinaturas de Eventos, consulte [Perguntas frequentes - Assinaturas de Eventos](../../wf-api/general/event-subs-faq.md).

## Padrões para entrega de mensagem de Assinatura de Evento

Os endpoints de serviço que consomem mensagens de assinatura de eventos do Adobe Workfront devem atender aos seguintes requisitos básicos para garantir que as mensagens sejam enviadas e recebidas corretamente:

* O ponto de extremidade do serviço deve aceitar solicitações HTTP POST. HTTP POST é o método de solicitação usado em todas as entregas de mensagens de assinatura de eventos, incluindo mensagens de validação.

* Para que o sistema de delivery de subscrição do evento confirme que a mensagem foi recebida com êxito, o endpoint deve retornar um status HTTP de nível 200 (por exemplo, 200 OK ou 202) para todas as mensagens recebidas.

* Se um status de nível 200 não for retornado, o sistema de assinatura de eventos presumirá que a mensagem não foi entregue com êxito e começará a aplicar a política de repetição apropriada. Para saber mais sobre a política de novas tentativas do Workfront, consulte [Novas tentativas de assinatura de evento](../../wf-api/api/event-sub-retries.md).

* Juntamente com o retorno de um status de nível 200 como status de resposta, a resposta HTTP deve ser recebida dentro de cinco segundos após o início da tentativa de delivery. Essa restrição garante que os processos de negócios do consumidor ou as limitações de infraestrutura não atrasem o delivery de outras mensagens com entrega pendente.

* Se um processo de negócios de longa duração for acionado a partir de uma mensagem de assinatura de evento, a Workfront recomenda  que

   1. o endpoint salva as informações da mensagem no recebimento e responde imediatamente com um status de nível 200.
   1. Depois que um endpoint responde a uma solicitação de delivery de subscrição de evento, as mensagens salvas podem ser processadas.
