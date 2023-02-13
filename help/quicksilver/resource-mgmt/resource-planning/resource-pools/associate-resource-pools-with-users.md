---
product-area: resource-management
navigation-topic: resource-pools
title: Associar pools de recursos a usuários
description: Associar pools de recursos a usuários
author: Alina
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Associar pools de recursos a usuários

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Os pools de recursos são coleções de usuários que ajudam a gerenciar recursos no Adobe Workfront.

Você deve criar um pool de recursos antes de associá-lo aos usuários.

Você pode associar usuários a pools de recursos ao criar pools de recursos.

Se você criar pools de recursos sem preenchê-los com usuários, poderá associá-los posteriormente a eles durante a edição ou criação de novos usuários.

Para obter informações sobre pools de recursos, consulte [Visão geral dos pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Para obter informações sobre a criação de pools de recursos, consulte [Criar pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro e superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Gerenciar conjuntos de recursos</p> <p>Editar acesso a Projetos, Modelos e Usuários</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões para projetos, modelos e usuários aos quais você associou os pools de recursos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Associar pools de recursos a um usuário

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Usuários**.
1. Marque a caixa ao lado do nome de um usuário da lista e clique em **Editar**.
1. Clique em **Planejamento de recursos**.
1. Comece a digitar o nome de um pool de recursos que deseja associar ao usuário no **Pools de Recursos** , selecione-o na lista, quando aparecer.\
   Você pode associar vários pools de recursos a um usuário.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Clique em **Salvar alterações**.

Para obter mais informações sobre edição de usuários, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Para obter mais informações sobre como criar novos usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Associar pools de recursos a usuários em massa

É possível editar vários usuários em massa e associar os mesmos pools de recursos a todos ao mesmo tempo.

Para associar pools de recursos a vários usuários em massa:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Usuários**.
1. Selecione vários usuários na lista e clique em **Editar**.
1. Clique em **Planejamento de recursos**.
1. Comece a digitar o nome de um pool de recursos que deseja associar aos usuários no **Pools de Recursos** , selecione-o na lista, quando aparecer.\
   Você pode associar vários pools de recursos a vários usuários.

   >[!NOTE]
   >
   >Apenas os pools de recursos comuns a todos os usuários selecionados aparecem neste campo. Se os usuários selecionados não tiverem pools de recursos compartilhados, esse campo estará vazio. Se este campo estiver vazio, os pools de recursos especificados aqui substituirão os pools de recursos individuais.

1. Clique em **Salvar alterações**.

Para obter mais informações sobre como editar usuários em massa, consulte [Editar perfis de usuário em massa](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
