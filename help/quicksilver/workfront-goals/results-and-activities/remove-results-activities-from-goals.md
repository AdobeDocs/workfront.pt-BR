---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Remova indicadores de progresso das metas no Adobe Workfront Metas
description: Você pode remover resultados, atividades e projetos de metas nas Metas da Adobe Workfront, quando eles não forem mais relevantes.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Remova indicadores de progresso das metas no Adobe Workfront Metas

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Você pode remover resultados, atividades e projetos de metas se eles não forem mais relevantes.

Para obter informações sobre como criar metas e adicionar resultados e atividades a elas, consulte os seguintes artigos:

* [Criar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
* [Adicionar atividades às metas em Metas da Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Adicionar resultados às metas em Metas da Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Editar resultados e atividades nas Metas da Adobe Workfront](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

As metas também podem ser alinhadas às metas principais, tornando-se metas infantis. As metas das crianças são também indicadores de progresso das metas principais.

Você pode remover o alinhamento entre as metas removendo a conexão entre elas. Para obter mais informações, consulte [Remova o alinhamento da meta nas Metas da Adobe Workfront](../goal-alignment/remove-goal-alignment.md).

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
     <p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta na Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve ter o seguinte antes de começar:

* Um modelo de layout que inclui a área Metas no Menu principal.
* Uma meta com resultados, atividades ou projetos.

## Considerações para remover resultados, atividades e desconectar projetos de metas

* Você pode remover resultados e atividades somente de metas ativas.
* Você pode remover resultados e atividades de uma meta, excluindo-os. Os resultados e as atividades excluídos não podem ser recuperados.
* Quando você remove o resultado ou a atividade de uma meta, o progresso do resultado removido ou a atividade afeta o progresso geral da meta.
* Não é possível excluir um projeto de uma meta, mas você pode desconectá-lo da meta. Ao desconectar o projeto da meta, a porcentagem completa do projeto não afeta mais o progresso da meta.

   Para obter informações sobre como os projetos afetam o progresso da meta, consulte [Adicionar projetos às metas em Metas da Adobe Workfront](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Não é possível remover um resultado ou uma atividade de uma meta e não é possível desconectar uma meta-filho ou um projeto, se eles forem o último indicador de progresso da meta.
* Se um projeto for excluído da área Projetos e for o último indicador de progresso de uma meta, a meta se tornará Inativa.

## Excluir resultados e atividades de metas

Remova resultados e atividades de uma meta ao excluí-los. A exclusão de resultados e atividades de uma meta é idêntica.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito, em seguida, clique em **Metas**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Isso abre a área Metas do Workfront e a Lista de metas é exibida por padrão.

1. Clique no nome de uma meta da qual deseja remover os resultados e as atividades.

   Isso abre a página da meta.

1. Clique em **Indicadores de progresso** no painel esquerdo.

1. Selecione um resultado ou atividade e clique no botão **Excluir** ícone ![](assets/delete-icon.png) na parte superior da lista.

1. Clique em **Excluir** para confirmar a exclusão. O resultado ou a atividade é excluída e não pode ser recuperada. A porcentagem completa da meta é atualizada para excluir a atividade ou resultado excluído.


## Remover projetos de metas

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. Clique no botão **Menu principal** no canto superior direito e clique em **Metas**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Isso abre a área Metas do Workfront e a Lista de metas é exibida por padrão.

1. Clique no nome de uma meta da qual deseja remover os resultados e as atividades.

   Isso abre a página da meta.
1. Clique em **Indicadores de progresso** no painel esquerdo.
1. Selecione um projeto e clique no botão **Desconectar** ícone ![](assets/disconnect-icon.png) na parte superior da lista.
1. Clique em **Desconectar** para confirmar.

   O projeto não está mais conectado à meta. A porcentagem completa da meta é atualizada para excluir o projeto desconectado.

