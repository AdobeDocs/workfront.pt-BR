---
content-type: api;faq
navigation-topic: general-api
title: Perguntas frequentes - Assinaturas de eventos
description: Perguntas frequentes - Assinaturas de eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 0%

---

# Perguntas frequentes - Assinaturas de eventos

<!--
{{highlighted-preview}}
-->

As perguntas a seguir são frequentes sobre Inscrições em eventos:

## O que é uma assinatura?

Uma assinatura é um conjunto de dados usado para corresponder e entregar eventos do Adobe Workfront para o endpoint HTTP de um cliente. Este recurso é composto de quatro atributos principais:

* customer_id
* obj_code
* obj_id
* url

Uma assinatura também pode ter outros atributos, como sua própria ID exclusiva e a data de criação, mas os atributos listados acima são usados principalmente para corresponder eventos e entregá-los aos clientes.

## Posso selecionar quais eventos são enviados para um endpoint com base em determinados critérios em uma carga do evento?

Os filtros de assinatura de evento são uma maneira de os subs de evento serem classificados por critérios especificados. É recomendável aplicar filtros às assinaturas de evento, pois isso pode reduzir significativamente o número de mensagens que um endpoint precisa consumir. Para obter mais informações, consulte [Filtragem de assinatura de evento](../../wf-api/general/event-subs-api.md#event).

## Por que a API está retornando um código de resposta de conflito 409?

Se você tentar criar uma assinatura de evento e receber um código de resposta: Conflito 409, a assinatura que você tentou criar está duplicada. O Workfront não permite a criação de assinaturas duplicadas.

## O que devo fazer se minhas mensagens não estiverem sendo entregues ao meu endpoint?

Procure os seguintes cenários e use a solução recomendada:

* Certifique-se de que o endpoint de subscrição — definido pelo **url** campo — está retornando um código de resposta HTTP 2XX. Caso contrário, entre em contato com o Suporte da Workfront ou consulte [Requisitos de entrega de Assinatura de Evento](../../wf-api/general/setup-event-sub-endpoint.md).

* A solicitação de entrega de evento pode estar expirando antes de ser concluída. Certifique-se de que o endpoint responda de forma consistente em 5 segundos. Esse é o tempo limite padrão definido para a solicitação HTTP para entregar uma mensagem de Assinatura de evento. Se o terminal não responder em 5 segundos, entre em contato com o Suporte da Workfront ou consulte [Requisitos de entrega de Assinatura de Evento](../../wf-api/general/setup-event-sub-endpoint.md).
* Os eventos podem não gerar o que você pensa. Certifique-se de que você não esteja fazendo suposições sobre como ou quando os eventos devem ser disparados. Por exemplo, você pode pensar que a atualização de um documento em uma tarefa gera um evento de atualização de tarefa, mas em vez disso, gera um evento de criação de documento ou atualização de documento.
* Sua assinatura pode não estar configurada conforme o esperado. Você pode criar assinaturas de evento em diferentes ambientes e esperar que elas sejam transferidas como seus outros dados do Workfront. No entanto, os dados de Assinatura de evento não estão configurados para serem copiados ou promovidos para outros ambientes. Verifique se você está emitindo solicitações de API para o ambiente correto e se as assinaturas nesse ambiente estão configuradas conforme esperado.
* A carga não foi recebida porque o endereço IP necessário do Workfront não foi adicionado ao arquivo de inclui na lista de permissões do firewall. Os eventos de Assinatura de eventos são enviados de apenas alguns endereços IP. Verifique se a rede de destino tem todas as exceções de IP necessárias para receber cargas das Assinaturas de Eventos da Workfront.

## Por que está demorando muito para que minhas mensagens cheguem ao meu terminal?

Alguns dos seguintes cenários podem ser responsáveis:

* Uma operação grande, como uma atualização em massa, no sistema pode fazer com que um grande volume de mensagens seja enfileirado de uma só vez, o que pode levar algum tempo para ser processado.
* Cálculos de longa duração ou cálculos de linha do tempo em projetos grandes podem estar causando um atraso na publicação de mensagens para o consumo de Assinaturas de eventos.
* A assinatura pode ter sido desabilitada.

   * Após um período de carência de 100 mensagens, se um URL específico, que pode estar associado a uma ou mais assinaturas, falhar mais de 70% do tempo ou se o URL falhar ao ser entregue após 2000 tentativas consecutivas, nenhuma tentativa de entrega será feita para todas as mensagens que correspondam às assinaturas com o mesmo URL. Em vez disso, essas mensagens são imediatamente enfileiradas para uma nova tentativa.

     A cada 10 minutos depois que um URL é desativado, tentamos enviar a próxima mensagem que aparece para processamento. Se essa mensagem for bem-sucedida, reativaremos esse URL e, subsequentemente, quaisquer assinaturas correspondentes. Se essa mensagem não for enviada, esse cronômetro de 10 minutos será redefinido e tentaremos novamente depois que expirar.

     Esse comportamento pode ser percebido como deliveries inconsistentes ou atrasados, mas simplesmente segue nossas políticas para a maneira como as mensagens de Assinatura de evento são tratadas.

   * Um URL de Assinatura de Evento será desabilitado permanentemente se uma das seguintes condições for atendida:

      * O URL de assinatura não foi entregue por 7 dias e falhou em pelo menos 2.000 tentativas de entrega consecutivas nas últimas 72 horas.
      * O URL de assinatura não entregou 50.000 tentativas consecutivas.

## O que devo fazer se estiver recebendo um status de resposta 500 ao tentar chamar a API de assinatura de evento?

Entre em contato com o Suporte da Workfront. Para saber como entrar em contato com o suporte, consulte [Entre em contato com o Suporte ao cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Que tipos diferentes de autenticação posso usar com as assinaturas de evento da Workfront?

Você pode usar qualquer autenticação que use um token de portador. A variável **authToken** o campo de uma subscrição é uma string que representa um token de portador OAuth2 usado para a autenticação com o URL especificado no **url** campo. Em teoria, esse valor de token pode ser qualquer coisa, desde que o endpoint de destino esteja ciente de como lidar com sua codificação, que é **utf-8**.

## Quanto tempo deve levar até que eu receba minha carga de evento das Assinaturas de Evento do Workfront?

Em geral, você pode esperar receber solicitações de entrega de eventos de Assinatura de eventos em menos de 5 segundos a partir da alteração de dados que está sendo registrada. Em média, as notificações de webhook são recebidas em menos de 1 segundo a partir do momento em que a alteração de dados é feita. No entanto, o serviço pode receber mensagens em quantidades tão grandes que também pode levar mais tempo.

## Recursos adicionais

* **Documentação da API**: [API de assinatura de evento](../../wf-api/general/event-subs-api.md)

* **Práticas recomendadas**: [Práticas recomendadas de assinatura de evento](../../wf-api/general/event-sub-best-practice.md)

* **Campos que acionam cargas de Assinatura de evento**: [Campos de recurso de assinatura do evento](../../wf-api/api/event-sub-resource-fields.md)

* **Noções básicas sobre novas tentativas de assinatura de evento**: [Novas tentativas de assinatura de evento](../../wf-api/api/event-sub-retries.md)

* **Configuração do firewall para o Workfront**: [Incluir na lista de permissões Configurar o arquivo de pesquisa do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
