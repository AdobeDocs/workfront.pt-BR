---
content-type: api
navigation-topic: api-navigation-topic
title: Novas tentativas de assinatura de evento
description: Novas tentativas de assinatura de evento
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 0325d305c892c23046739feff17d4b1fc11100cc
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Novas tentativas de assinatura de evento

Ao implementar um sistema de delivery de mensagens, há algumas limitações que devem ser abordadas para garantir estabilidade, consistência e boa experiência do usuário. Uma das deficiências de um sistema de entrega de mensagens é garantir que as mensagens cheguem ao destino com êxito e saber o que fazer quando as mensagens não chegarem.

Algumas integrações podem aceitar a falha de entrega, descartar a mensagem e passar para a próxima mensagem.  Em outras integrações, a falha ao entregar uma mensagem não pode ser ignorada. Por exemplo, uma integração financeira pode tentar entregar uma mensagem, mas recebe um código de status HTTP 404, que indica que o servidor não pôde encontrar o endpoint para o qual a mensagem deveria ser entregue. Nesses casos, uma mensagem ausente pode significar que alguém não está sendo pago pelo seu tempo ou que uma organização está ultrapassando o orçamento de recursos contratados.

## Estratégia da Adobe Workfront para novas tentativas de assinatura de evento

Como os clientes usam a plataforma Workfront como parte principal de seu trabalho diário de conhecimento, a estrutura Workfront Event Subscription fornece um mecanismo para garantir que a entrega de cada mensagem seja tentada na maior extensão possível.

As mensagens de saída acionadas pelo evento que não são entregues aos endpoints do cliente são reenviadas até que a entrega seja bem-sucedida por um período de até 48 horas. Durante esse período, as tentativas ocorrem com uma frequência incrementalmente aumentada até que o delivery seja bem-sucedido ou até que 11 tentativas sejam feitas.

A fórmula para essas novas tentativas é:

`((2^attempt) - 1) * 84800ms`

A primeira tentativa ocorre após 1,5 minuto, a segunda em quase 5 minutos e a 11ª em cerca de 48 horas.

Os clientes precisam garantir que todos os endpoints que consomem mensagens de saída das Assinaturas de eventos da Workfront estejam configurados para retornar uma mensagem de resposta de 200 níveis à Workfront quando a entrega for bem-sucedida.

## Regras de assinatura desabilitadas e congeladas

* Uma URL de assinatura está **desabilitada** se tiver uma taxa de falha superior a 70% com mais de 100 tentativas OU se tiver 2.000 falhas consecutivas
* Uma URL de assinatura está **congelada** se tiver mais de 2.000 falhas consecutivas e o último sucesso tiver ocorrido há mais de 72 horas OU se tiver 50.000 falhas consecutivas em qualquer período.
* Uma URL de assinatura **desabilitada** continuará tentando entregar a cada 10 minutos e será reabilitada com uma entrega bem-sucedida.
* Uma URL de assinatura **congelada** nunca tentará a entrega, a menos que seja habilitada manualmente fazendo uma solicitação de API.



<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

The following explanations correspond with the steps depicted in the flowchart:

1. Message fails to be delivered. 
1. Message delivery failure information is logged.

   All failed attempts to deliver a message are logged so that debugging may be performed to determine the root cause of a given failure or series of failures. 

1. URL failures incremented. 
1. Message attempt count is incremented. 
1. Calculate the delay until this message's delivery will be attempted again. 
1. Message is placed onto the message retry queue.

   As shown in the preceding flowchart, the message queue used for processing message delivery retries is a separate queue from the one that processes the initial delivery attempt for each message. This allows the near real-time flow of messages to continue unimpeded by the failure of any subset of messages. 

1. URL circuit status is evaluated. One of the following occurs:

   * If the circuit is open and not allowing deliveries at this time, restart the process at step 5.
   * If the circuit is half-open, this implies that our circuit is currently open, but enough time has passed to allow testing of the URL to see if the problem with delivering to it has been resolved.
   * If the message delivery attempt limits have been reached (48 hours of retrying) then the message is dropped

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1 

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1.
   -->
