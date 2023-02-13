---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Compartilhar uma meta na Workfront
description: Ao compartilhar uma meta, você dá permissões de gerenciamento a uma meta para alguém que não a criou.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 2%

---

# Compartilhar uma meta na Adobe Workfront

Ao compartilhar uma meta, você dá permissões de gerenciamento a uma meta para alguém que não a criou.

## Requisitos de acesso

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td> <p>Você deve comprar uma licença adicional para a funcionalidade Metas da Adobe Workfront para acessar descrita neste artigo. </p> <p>Para obter mais informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as metas do Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar o acesso às Metas ou superior</p> <p><b>Nota</b><p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Conceder acesso às Metas da Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> 
    <div> 
     <p>Gerenciar permissões para a meta</p> 
     <p>Para obter informações sobre como compartilhar metas, consulte <a href="#" class="MCXref xref selected">Compartilhar uma meta na Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar, você deve ter o seguinte:

* Um modelo de layout que inclui a área Metas no Menu principal.

## Considerações sobre o compartilhamento de metas

* Os usuários podem ter as seguintes permissões para uma meta:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Permissões de meta</b></p></td> 
      <td>
      <p><b>Descrição</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Exibir</p></td> 
      <td>
      <p>Os usuários têm permissões para visualizar a meta, mas não podem editar informações para a meta, não podem adicionar ou editar informações para resultados ou atividades, atualizar status ou excluir a meta.</p>      
      <p>Por padrão, todos os usuários com acesso às Metas podem visualizar todas as metas no sistema. Os usuários podem copiar a meta, se tiverem o acesso de Edição às Metas em seu nível de acesso.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Gerenciar</p></td> 
      <td> <p>Os usuários podem editar todas as informações para a meta, incluindo os resultados ou as atividades, incluindo excluí-las.</p> 
      <p>Somente criadores de metas ou usuários com permissões de gerenciamento específicas a uma meta podem gerenciar uma meta.</p> 
      Somente usuários com permissões de gerenciamento para uma meta podem compartilhar a meta com outras pessoas para conceder a elas permissões de gerenciamento para a meta. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Você pode compartilhar os seguintes tipos de metas com outras pessoas:

   * Uma meta que você criou
   * Uma meta criada por outra pessoa à qual você recebeu permissões para gerenciar.

* Se você tiver permissões de gerenciamento em uma meta, poderá alterar as permissões na meta do criador da meta. Por padrão, eles têm permissões de Gerenciamento ao criar a meta, mas você pode alterar as permissões para Exibir.

## Compartilhar uma meta

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) > **Metas** no canto superior direito.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   A Lista de metas é exibida.

1. Clique no nome de uma meta na lista. A página de meta é aberta.

1. Clique no botão **Ícone Mais** ao lado do nome da meta, em seguida, clique em **Compartilhar**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   A caixa Acesso à meta é exibida.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Siga um destes procedimentos:

   * Selecione o **Gerenciar todo o sistema** configuração para conceder permissões de gerenciamento a todos no sistema que tenham o acesso de Edição a Metas em seu nível de acesso. Isso é desmarcado por padrão para todas as novas metas.
   * Comece a digitar o nome de um usuário ao qual você deseja conceder permissões de Gerenciamento no **Conceder acesso ao Gerenciar** caixa. Selecione o nome quando ele aparecer na lista.

      >[!TIP]
      >
      >Você só pode compartilhar uma meta com outros usuários. Você não pode compartilhar metas com grupos, equipes ou sua empresa.

1. Clique em **Compartilhar**.

   A meta é compartilhada com os usuários especificados. Um rótulo &quot;Todo o sistema&quot; ou o nome dos usuários que têm permissões de Gerenciamento para a meta são exibidos no campo Acesso a gerenciamento no painel Detalhes da meta .

## Opções de permissão de meta

A tabela a seguir lista as permissões que você pode conceder ao compartilhar uma meta. Para obter mais informações sobre o acesso que os usuários têm com base em sua licença, consulte [Conceder acesso às Metas da Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>Ações</strong> </p> </th> 
   <th> <p><strong>Gerenciar</strong> </p> </th> 
   <th> <p><strong>Exibir</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Meta de visualização</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exibir resultados ou atividades</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Copiar meta* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Converter resultados ou atividades em outras metas*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Exibir projetos adicionados como atividades** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Editar meta</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar resultados ou atividades</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Adicionar resultados ou atividades para a meta</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Associar um projeto como uma atividade à meta**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Excluir meta</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Excluir resultados ou atividades</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Desconectar projetos da meta</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Você deve ter o acesso Editar às Metas em seu nível de acesso para poder converter resultados e atividades em metas.

**Você deve ter acesso à permissão Exibir projetos e Exibir para os projetos adicionados ou que você deseja adicionar à meta para exibi-los.

Para obter informações sobre o nível de acesso do projeto, consulte [Conceder acesso aos projetos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Para obter informações sobre permissões de projeto, consulte [Compartilhar um projeto no Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
