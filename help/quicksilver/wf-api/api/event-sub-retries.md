---
content-type: api
navigation-topic: api-navigation-topic
title: Novas tentativas de assinatura de evento
description: Novas tentativas de assinatura de evento
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Novas tentativas de assinatura de evento

Ao implementar um sistema de delivery de mensagens, há algumas limitações que devem ser abordadas para garantir estabilidade, consistência e boa experiência do usuário. Uma das deficiências de um sistema de entrega de mensagens é garantir que as mensagens cheguem ao destino com êxito e saber o que fazer quando as mensagens não chegarem.

Algumas integrações podem aceitar a falha de entrega, descartar a mensagem e passar para a próxima mensagem.  Em outras integrações, a falha ao entregar uma mensagem não pode ser ignorada. Por exemplo, uma integração financeira pode tentar entregar uma mensagem, mas recebe um código de status HTTP 404, que indica que o servidor não pôde encontrar o endpoint para o qual a mensagem deveria ser entregue. Nesses casos, uma mensagem ausente pode significar que alguém não está sendo pago pelo seu tempo ou que uma organização está ultrapassando o orçamento de recursos contratados.

## Estratégia da Adobe Workfront para novas tentativas de assinatura de evento

Como os clientes usam a plataforma Workfront como parte principal de seu trabalho diário de conhecimento, a estrutura Workfront Event Subscription fornece um mecanismo para garantir que a entrega de cada mensagem seja tentada na maior extensão possível.

As mensagens de saída acionadas pelo evento que não são entregues aos endpoints do cliente são reenviadas até que a entrega seja bem-sucedida por um período de até 48 horas. Durante esse período, as tentativas ocorrem com uma frequência cada vez mais reduzida até que o delivery seja bem-sucedido ou até que 48 horas tenham decorrido.

Os clientes precisam garantir que todos os endpoints que consomem mensagens de saída das Assinaturas de eventos da Workfront estejam configurados para retornar uma mensagem de resposta de 200 níveis à Workfront quando a entrega for bem-sucedida.

## Lidar com mensagens de saída disparadas por eventos com falha

O fluxograma a seguir mostra a estratégia para tentar novamente a entrega de mensagens com Assinaturas de Eventos da Workfront:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

As explicações a seguir correspondem às etapas descritas no fluxograma:

1. Falha na entrega da mensagem.
1. As informações de falha de delivery de mensagem são registradas.

   Todas as tentativas falhas de entrega de uma mensagem são registradas para que a depuração possa ser executada para determinar a causa raiz de determinada falha ou série de falhas.

1. Falhas de URL aumentadas.
1. A contagem de tentativas da mensagem é incrementada.
1. Calcule o atraso até que a entrega desta mensagem seja tentada novamente.
1. A mensagem é colocada na fila de mensagens repetidas.

   Como mostrado no fluxograma anterior, a fila de mensagens usada para processar tentativas de delivery de mensagens é uma fila separada daquela que processa a tentativa de delivery inicial para cada mensagem. Isso permite que o fluxo de mensagens quase em tempo real continue desimpedido pela falha de qualquer subconjunto de mensagens.

1. O status do circuito de URL é avaliado. Uma das situações a seguir ocorre:

   * Se o circuito estiver aberto e não permitir deliveries no momento, reinicie o processo na etapa 5.
   * Se o circuito estiver semiaberto, isso implica que nosso circuito está aberto no momento, mas passou tempo suficiente para permitir o teste do URL para ver se o problema com a entrega foi resolvido.
   * Se os limites de tentativa de delivery da mensagem tiverem sido atingidos (48 horas de novas tentativas), a mensagem será descartada

1. Se o circuito de URL estiver fechado e permitindo deliveries, tente entregar a mensagem. Se esse delivery falhar, a mensagem será reiniciada na etapa 1

1. Se o circuito de URL estiver fechado e permitindo deliveries, tente entregar a mensagem. Se esse delivery falhar, a mensagem será reiniciada na etapa 1.

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->
