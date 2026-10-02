---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: Configurar assinaturas de evento no Workfront
description: Como administrador do Adobe Workfront, você pode criar, exibir e excluir assinaturas de eventos na área Configuração para enviar eventos do Workfront para um endpoint externo.
feature: System Setup and Administration
role: Admin
author: Courtney
source-git-commit: 5a44679115dcfda871e2fe40c0c8443649fc43cf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 9%
---

# Configurar assinaturas de evento no Workfront

{{highlighted-preview-article-level}}

Como administrador do Adobe Workfront, você pode criar, exibir e excluir assinaturas de eventos na área Configuração. As assinaturas de evento enviam informações de evento do Workfront para um endpoint externo quando eventos especificados ocorrem.

Você pode criar e excluir assinaturas de evento no Workfront, mas não pode editar uma assinatura existente. Se precisar alterar uma assinatura, exclua-a e crie uma nova.

Para obter mais informações sobre assinaturas de eventos, consulte os artigos em [Assinaturas de Eventos](/help/quicksilver/wf-api/api/event-subscriptions.md).

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
   <td>Você deve ser um administrador do Workfront.</td>
  </tr>
 </tbody>
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma assinatura de evento

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **Sistema** e em **Assinaturas de Eventos**.
1. Clique em **Nova assinatura de evento**.
1. No campo **Objeto**, selecione o objeto Workfront que deseja monitorar.
1. No campo **Tipo de evento**, selecione se você deseja que a inscrição de evento acione quando o objeto for criado, atualizado, excluído ou compartilhado.
1. No campo **URL do Webhook**, insira o ponto de extremidade que deve receber a carga do evento.
1. No campo **Token de autenticação**, digite o token usado para autenticar a solicitação no seu ponto de extremidade.
1. Se desejar que o Workfront codifique a carga antes de enviá-la, habilite a opção para enviar a carga como Base64.
1. Se necessário, adicione um ou mais filtros para limitar quais eventos acionam a assinatura. Os filtros disponíveis se baseiam no objeto selecionado.
1. Clique em **Criar**.

Para obter informações sobre requisitos de ponto de extremidade, consulte [requisitos de entrega de Assinatura de Eventos](/help/quicksilver/wf-api/general/setup-event-sub-endpoint.md).

## Exibir assinaturas de evento

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **Sistema** e em **Assinaturas de Eventos**.

Na página Assinaturas de eventos, é possível revisar as assinaturas configuradas para o seu ambiente. Você também pode ver quantas assinaturas sua organização tem e quantas delas estão ativas, desabilitadas ou congeladas.

* **Assinaturas desabilitadas**: essas assinaturas foram desabilitadas automaticamente devido a falhas repetidas de entrega.
* **Assinaturas congeladas**: essas assinaturas estão temporariamente congeladas devido a problemas de entrega.

## Excluir uma assinatura de evento

{{step-1-to-setup}}

1. No painel de navegação esquerdo, clique em **Sistema** e em **Assinaturas de Eventos**.
1. Selecione a inscrição de evento que deseja remover.
1. Clique em **Excluir**.
