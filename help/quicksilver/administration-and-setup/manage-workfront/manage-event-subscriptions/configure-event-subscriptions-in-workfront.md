---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: Configurar assinaturas de evento no Workfront
description: Os administradores do Workfront podem criar, exibir e excluir assinaturas de eventos da Configuração. Os usuários com o acesso necessário também podem gerenciar assinaturas de eventos dentro do escopo permitido por suas permissões e configuração do sistema.
feature: System Setup and Administration
role: Admin
author: Courtney
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 8%
---

# Configurar assinaturas de evento no Workfront

{{highlighted-preview-article-level}}

Como administrador do Adobe Workfront, você pode criar, exibir e excluir assinaturas de eventos na área Configuração. As assinaturas de evento enviam informações de evento do Workfront para um endpoint externo quando eventos especificados ocorrem.

Você pode criar e excluir assinaturas de evento no Workfront, mas não pode editar uma assinatura existente. Se precisar alterar uma assinatura, exclua-a e crie uma nova.

Os usuários que têm o acesso necessário também podem gerenciar assinaturas de eventos no Workfront, mas somente dentro do escopo permitido por suas permissões e configuração do sistema. Para obter mais informações, consulte [Gerenciar assinaturas de evento como um usuário não administrador](/help/quicksilver/wf-api/general/event-subs-non-admin.md).

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
   <td>
    <p>Você deve ter o acesso apropriado para gerenciar assinaturas de evento.</p>
    <p>Usuários não administradores podem ter acesso somente ao escopo permitido por suas permissões e pela configuração do sistema.</p>
   </td>
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
