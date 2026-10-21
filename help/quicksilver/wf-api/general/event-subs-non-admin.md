---
content-type: api
navigation-topic: general-api
title: Gerenciar assinaturas de evento como um usuário não administrador
description: Se o acesso ao Workfront permitir, será possível criar, exibir e excluir assinaturas de eventos que estejam dentro do escopo permitido por suas permissões e pela configuração do sistema.
author: Courtney
feature: Workfront API
role: Developer
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 10%
---

# Gerenciar assinaturas de evento como um usuário não administrador

Se o acesso ao Workfront permitir, você poderá criar, exibir e excluir assinaturas de eventos da área Configuração. No entanto, seu acesso é limitado às assinaturas e ações autorizadas para sua função e pela configuração do sistema de sua organização.

Esse recurso não está disponível para todos os usuários da mesma forma que para os administradores do Workfront. Os usuários com o acesso necessário podem gerenciar assinaturas de eventos somente no escopo concedido a eles.

Por exemplo, suas permissões podem permitir gerenciar apenas determinados tipos de objeto, tipos de evento ou assinaturas para um conjunto definido de trabalho. Não é possível gerenciar assinaturas de eventos fora do escopo permitido pelo seu acesso e configuração.

Para obter a configuração gerenciada pelo administrador, consulte [Configurar assinaturas de evento no Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md).

Para obter informações sobre a API de Assinaturas de Eventos, consulte [API de Assinatura de Eventos](/help/quicksilver/wf-api/general/event-subs-api.md).

>[!NOTE]
>
>Os usuários podem gerenciar assinaturas de eventos somente no escopo permitido por suas permissões e pela configuração do sistema da organização. O acesso não é automaticamente equivalente ao acesso de administrador.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Pacote do Adobe Workfront</td>
   <td>Qualquer</td>
  </tr>
  <tr>
   <td role="rowheader">Licença do Adobe Workfront</td>
   <td>
    <p>Padrão</p>
    <p>Plano</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Configurações de nível de acesso</td>
   <td>
    <p>Você deve ter o acesso apropriado para gerenciar assinaturas de evento.</p>
    <p>Seu acesso é limitado às assinaturas e ações permitidas por suas permissões e pela configuração do sistema de sua organização.</p>
   </td>
  </tr>
 </tbody>
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Trabalhar com assinaturas de evento

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **Sistema** e em **Assinaturas de Eventos**.
1. Revise as assinaturas disponíveis para você.
1. Crie, exiba ou exclua somente as assinaturas que se enquadram no escopo autorizado.

Se você não vir as opções esperadas ou se não conseguir criar ou gerenciar uma assinatura, entre em contato com o administrador do Workfront para confirmar se o acesso é limitado por função, permissões ou configuração do sistema.

## Artigos relacionados

* [Configurar assinaturas de evento no Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)
* [API de Assinatura de evento](/help/quicksilver/wf-api/general/event-subs-api.md)
