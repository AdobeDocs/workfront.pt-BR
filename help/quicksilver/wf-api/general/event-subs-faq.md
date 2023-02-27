---
content-type: api;faq
navigation-topic: general-api
title: Perguntas frequentes - Assinaturas de eventos
description: Perguntas frequentes - Assinaturas de eventos
author: Becky
feature: Workfront API
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 0%

---

# Perguntas frequentes - Assinaturas de eventos

<!--
{{highlighted-preview}}
-->

As perguntas a seguir são frequentes sobre assinaturas de evento:

## O que é uma assinatura?

Uma assinatura é um conjunto de dados usado para corresponder e fornecer eventos do Adobe Workfront ao endpoint HTTP de um cliente. Esse recurso é composto de 4 atributos primários:

* customer_id
* obj_code
* obj_id
* url

Uma assinatura também pode ter outros atributos, como sua própria ID exclusiva e a data de criação, mas os atributos listados acima são usados principalmente para corresponder eventos e entregá-los aos clientes.

## Posso selecionar quais eventos são enviados para um endpoint com base em determinados critérios em um payload do evento?

Os filtros de assinatura de evento são uma maneira pela qual os subs de evento podem ser classificados de acordo com critérios especificados. É recomendável aplicar filtros a assinaturas de eventos, pois pode reduzir significativamente o número de mensagens que um endpoint precisa consumir. Para obter mais informações, consulte [Filtragem de assinatura de evento](../../wf-api/general/event-subs-api.md#event).

## Por que a API retorna um código de resposta de conflito 409?

Se você tentar criar uma assinatura de evento e receber um código de resposta: Em conflito 409, a assinatura que você tentou criar é duplicada. A Workfront não permite a criação de assinaturas duplicadas.

## O que devo fazer se minhas mensagens não forem enviadas para o meu terminal?

Procure os seguintes cenários e use a solução recomendada:

* Certifique-se de que o terminal de assinatura seja definido pela variável **url** campo—está retornando um código de resposta HTTP 2XX. Caso contrário, entre em contato com o Suporte da Workfront ou consulte [Requisitos de delivery de assinatura de evento](../../wf-api/general/setup-event-sub-endpoint.md).

* A solicitação de entrega de evento pode estar expirando antes de ser concluída. Certifique-se de que o terminal responda de maneira consistente em 5 segundos. Esse é o tempo limite padrão definido para a solicitação HTTP para entregar uma mensagem de Assinatura de evento. Se o terminal não responder em 5 segundos, entre em contato com o Suporte da Workfront ou consulte [Requisitos de delivery de assinatura de evento](../../wf-api/general/setup-event-sub-endpoint.md).
* Os eventos podem não gerar a maneira como você pensa. Certifique-se de que você não esteja fazendo suposições sobre como ou quando os eventos devem e são acionados. Por exemplo, você pode pensar que a atualização de um documento em uma tarefa gera um evento de atualização de tarefa, mas, em vez disso, gera um evento de criação de documento ou de atualização de documento.
* Sua assinatura pode não estar configurada conforme o esperado. Você pode criar assinaturas de eventos em diferentes ambientes e esperar que elas sejam transferidas como seus outros dados do Workfront. No entanto, os dados de Assinatura de evento não estão configurados para serem copiados ou promovidos para outros ambientes. Certifique-se de que você está emitindo solicitações de API para o ambiente correto e que as assinaturas desse ambiente estejam configuradas conforme esperado.
* A carga útil não foi recebida porque o endereço IP Workfront necessário não foi adicionado à  lista de permissões no firewall. Os eventos de assinatura de evento são enviados somente de alguns endereços IP. Certifique-se de que a rede de destino tenha todas as exceções de IP necessárias para receber cargas das Assinaturas de eventos do Workfront.

## Por que está levando um tempo excessivo para minhas mensagens chegarem ao meu terminal?

Alguns dos seguintes cenários podem ser responsáveis:

* Uma operação grande — como uma atualização em massa — no sistema pode fazer com que um grande volume de mensagens seja enfileirado de uma só vez, o que pode levar algum tempo para ser processado.
* Cálculos de longa duração ou cálculos de linha do tempo em projetos grandes podem estar causando um atraso na publicação de mensagens para o consumo de Assinaturas de eventos.
* A assinatura pode ter sido desabilitada.

   * Após um período de carência de 100 mensagens, se um URL específico — que pode ser associado a uma ou mais assinaturas — falhar mais de 70% do tempo ou se o URL falhar no delivery após 2000 tentativas consecutivas, todas as mensagens correspondentes a assinaturas com o mesmo URL não serão tentadas para entrega. Em vez disso, essas mensagens são imediatamente enfileiradas para uma nova tentativa.

      A cada 10 minutos depois que um URL é desativado, tentamos entregar a próxima mensagem que aparece para processamento. Se essa mensagem tiver êxito, reativamos esse URL e, subsequentemente, qualquer assinatura correspondente. Se essa mensagem não for enviada, o cronômetro de 10 minutos será redefinido e tentaremos novamente depois que expirar.

      Esse comportamento pode ser percebido como entregas inconsistentes ou atrasadas, mas simplesmente segue as políticas de como as mensagens de Assinatura de evento são tratadas.

   * Um URL de assinatura de evento será desativado se uma das seguintes condições for atendida:

      * O URL de assinatura falhou por 7 dias e falhou pelo menos 2000 tentativas consecutivas de delivery nas últimas 72 horas.
      * O URL de assinatura falhou ao entregar 50.000 tentativas consecutivas.

## O que devo fazer se estiver recebendo um status de resposta 500 ao tentar chamar a API de assinatura de evento?

Entre em contato com o Suporte da Workfront. Para saber como entrar em contato com o suporte, consulte [Entre em contato com o Suporte ao cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Quais tipos diferentes de autenticação posso usar com as Assinaturas de evento do Workfront?

Você pode usar qualquer autenticação que use um token portador. O **authToken** campo de uma assinatura é uma string que representa um token portador OAuth2 usado para autenticar com o URL especificado na variável **url** campo. Em teoria, esse valor de token pode ser qualquer coisa, desde que o endpoint de destino esteja ciente de como lidar com sua codificação, que é **utf-8**.

## Quanto tempo deve demorar até que eu receba meu payload do evento das Assinaturas de eventos do Workfront?

Em geral, você pode esperar receber solicitações de entrega de evento de assinatura de evento em menos de 5 segundos a partir da alteração de dados que está sendo registrada. Em média, as notificações do webhook são recebidas em menos de 1 segundo a partir do momento em que a alteração de dados é feita. No entanto, o serviço pode receber mensagens em quantidades tão grandes que também pode demorar mais.

## Recursos adicionais

* **Documentação da API**: [API de assinatura de evento](../../wf-api/general/event-subs-api.md)

* **Práticas recomendadas**: [Práticas recomendadas de assinatura de evento](../../wf-api/general/event-sub-best-practice.md)

* **Campos que acionam cargas de assinatura de evento**: [Campos de recurso de assinatura de evento](../../wf-api/api/event-sub-resource-fields.md)

* **Noções básicas sobre tentativas de assinatura de evento**: [Tentativas de assinatura do evento](../../wf-api/api/event-sub-retries.md)

* **Configuração do firewall para Workfront**: [Configurar a  lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
