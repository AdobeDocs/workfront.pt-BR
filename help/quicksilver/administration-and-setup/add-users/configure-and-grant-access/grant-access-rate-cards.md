---
title: Conceder acesso aos cartões de tarifa
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Como administrador do Adobe Workfront, você pode definir o acesso de um usuário a dados financeiros no Workfront por meio de seu nível de acesso.
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
exl-id: b21e65d3-3c9f-4f3d-95d3-de4c09199622
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 10%
---
# Conceder acesso aos cartões de taxa

Como administrador do Adobe Workfront, você pode definir o acesso de um usuário a cartões de taxa por meio do nível de acesso do usuário, conforme explicado na [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Para obter informações sobre cartões de taxa, consulte [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Padrão</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações para conceder acesso a cartões de taxa

Considere o seguinte ao conceder aos usuários acesso aos cartões de taxa no Workfront:

* Os usuários devem ter acesso de edição a cartões de taxa, projetos e dados financeiros para anexar um cartão de taxa a um projeto.
* Usuários sem acesso a cartões de taxa e com acesso de edição a dados financeiros não podem anexar um cartão de taxa a um projeto, mas podem editar outras taxas de cobrança no projeto provenientes de outras fontes.

## Configurar o acesso do usuário aos cartões de taxa usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, conforme explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no botão **Exibir** ou **Editar** à direita de Cartões de Taxa e selecione as capacidades que deseja conceder em **Ajustar suas configurações**.

   ![Ajustar o acesso ao cartão](assets/rate-card-access-fine-tune.png)

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configurar acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso às tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Quando terminar, clique em **Salvar**.

   Após criar o nível de acesso, você pode atribuí-lo a um usuário. Para obter mais informações, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acesso a cartões de taxa compartilhados

Você pode compartilhar um cartão de taxa com outros usuários concedendo a eles permissões, conforme explicado em [Compartilhar um cartão de taxa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md).

Quando você compartilha qualquer objeto com outro usuário, os direitos do recipient sobre ele são determinados por uma combinação de dois itens:

* As permissões concedidas ao destinatário para o objeto
* As configurações de nível de acesso do destinatário para o tipo do objeto
