---
product-area: resource-management
navigation-topic: resource-pools
title: Associar conjuntos de recursos a usuários
description: Você deve criar um conjunto de recursos antes de associá-lo aos usuários. Você pode associar usuários a conjuntos de recursos ao criar seus conjuntos de recursos.
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 1%

---

# Associar conjuntos de recursos a usuários

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Conjuntos de recursos são coleções de usuários que ajudam você a gerenciar recursos no Adobe Workfront.

Você deve criar um conjunto de recursos antes de associá-lo aos usuários.

Você pode associar usuários a conjuntos de recursos ao criar seus conjuntos de recursos.

Se você criar conjuntos de recursos sem preenchê-los com usuários, poderá associá-los posteriormente aos usuários ao editar ou criar novos usuários.

Para obter informações sobre pools de recursos, consulte [Visão geral sobre pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Para obter informações sobre como criar pools de recursos, consulte [Criar pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td><p>Novo: Qualquer um</p>
       <p>ou</p>
       <p>Atual: Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Gerenciar conjuntos de recursos</p> <p>Editar acesso a projetos, modelos e usuários</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Gerenciar permissões para projetos, modelos e usuários aos quais você deseja associar os Conjuntos de recursos</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Associar conjuntos de recursos a um usuário

{{step-1-to-users}}

1. Marque a caixa ao lado do nome de um usuário da lista e clique em **Editar**.
1. Clique em **Planejamento de recursos**.
1. Comece digitando o nome de um pool de recursos que você deseja associar ao usuário no campo **Pools de Recursos** e selecione-o na lista quando ele for exibido.\
   Você pode associar vários conjuntos de recursos a um usuário.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Clique em **Salvar alterações**.

Para obter mais informações sobre como editar usuários, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Para obter mais informações sobre como criar novos usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Associar conjuntos de recursos a usuários em massa

É possível editar vários usuários em massa e associar os mesmos conjuntos de recursos a todos eles ao mesmo tempo.

Para associar conjuntos de recursos a vários usuários em massa:

{{step-1-to-users}}

1. Selecione vários usuários na lista e clique em **Editar**.
1. Clique em **Planejamento de recursos**.
1. Comece digitando o nome de um pool de recursos que você deseja associar aos usuários no campo **Pools de Recursos** e selecione-o na lista quando ele for exibido.\
   Você pode associar vários conjuntos de recursos a vários usuários.

   >[!NOTE]
   >
   >Somente os conjuntos de recursos comuns a todos os usuários selecionados aparecem nesse campo. Se os usuários selecionados não tiverem conjuntos de recursos compartilhados, esse campo estará vazio. Se esse campo estiver vazio, os conjuntos de recursos especificados aqui substituirão seus conjuntos de recursos individuais.

1. Clique em **Salvar alterações**.

Para obter mais informações sobre como editar usuários em massa, consulte [Editar perfis de usuário em massa](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
