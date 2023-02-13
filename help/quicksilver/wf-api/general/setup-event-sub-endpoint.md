---
content-type: api
navigation-topic: general-api
title: Requisitos de delivery de assinatura de evento
description: Requisitos de delivery de assinatura de evento
author: John
feature: Workfront API
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Requisitos de delivery de assinatura de evento

As mensagens de assinatura de evento são notificações que podem ser configuradas para notificar os usuários quando determinados eventos ocorrerem. Para saber mais sobre o que são Assinaturas de eventos, consulte [Perguntas frequentes - Assinaturas de eventos](../../wf-api/general/event-subs-faq.md).

## Padrões para entrega de mensagem de assinatura de evento

Os endpoints de serviço que consomem mensagens de assinatura de evento do Adobe Workfront devem atender aos seguintes requisitos básicos, para garantir que as mensagens sejam enviadas e recebidas corretamente:

* O endpoint de serviço deve aceitar solicitações HTTP POST. HTTP POST é o método de solicitação usado em todos os deliveries de mensagens de assinatura de eventos, incluindo mensagens de validação.

* Para que o sistema de delivery de assinatura de evento reconheça que a mensagem foi recebida com êxito, o endpoint deve retornar um status HTTP de nível 200 (por exemplo, 200 OK ou 202) para todas as mensagens recebidas.

* Se um status de nível 200 não for retornado, o sistema de assinatura de eventos presumirá que a mensagem não foi entregue com êxito e começará a aplicar a política de repetição apropriada. Para saber mais sobre a política de tentativas do Workfront, consulte [Tentativas de assinatura do evento](../../wf-api/api/event-sub-retries.md).

* Juntamente com o retorno de um status de nível 200 como status de resposta, a resposta HTTP deve ser recebida dentro de cinco segundos após o início da tentativa de delivery. Essa restrição garante que os processos de negócios do consumidor ou as limitações de infraestrutura não atrasem o delivery de outras mensagens pendentes.

* Se um processo de negócios de longa duração disparar de uma mensagem de assinatura de evento, a Workfront recomenda que

   1. o endpoint salva as informações da mensagem no recebimento e responde imediatamente com um status de nível 200.
   1. Depois que um endpoint responde a uma solicitação de delivery de delivery de assinatura de evento, as mensagens salvas podem ser processadas.
