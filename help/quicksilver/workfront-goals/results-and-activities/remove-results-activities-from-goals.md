---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Remover indicadores de progresso das metas no Adobe Workfront Goals
description: Você pode remover resultados, atividades e projetos das metas nas Metas do Adobe Workfront, quando elas não forem mais relevantes.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 2%

---

# Remover indicadores de progresso das metas no Adobe Workfront Goals

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Você pode remover resultados, atividades e projetos das metas se eles não forem mais relevantes.

Para obter informações sobre como criar metas e adicionar resultados e atividades a elas, consulte os seguintes artigos:

* [Criar metas nas Metas do Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
* [Adicionar atividades às metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Adicionar resultados às metas nas Metas do Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Editar resultados e atividades no Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

As metas também podem ser alinhadas às metas principais, tornando-se metas secundárias. As metas secundárias também são indicadores de progresso das metas principais.

Você pode remover o alinhamento entre metas removendo a conexão entre elas. Para obter informações, consulte [Remover alinhamento da meta nas Metas do Adobe Workfront](../goal-alignment/remove-goal-alignment.md).

## Requisitos de acesso

>[!NOTE]
>
>Sua empresa pode optar por continuar usando o Adobe Workfront Goals se ele comprou esse pacote no passado. Você precisa falar com o seu representante de conta para obter mais detalhes.
>
>O Adobe Workfront Goals não está mais disponível para compra.

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Pacote do Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licença do Adobe Workfront</td>
 <td>
 <p>Colaborador ou superior</p>
<p>Solicitação ou superior</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuração do nível de acesso</td>
 <td> <p>Editar acesso às Metas</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permissões de objeto</td>
 <td>
  <div>
  <p>Exibir permissões ou mais altas para a meta para exibi-la</p>
  <p>Gerenciar permissões para a meta para editá-la</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo Administradores do sistema, devem receber um modelo de layout que inclua a área Metas no Menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Pré-requisitos

Você deve ter uma meta associada a resultados, atividades ou projetos.

## Considerações para remover resultados, atividades e desconectar projetos das metas

* Você pode remover resultados e atividades somente de metas ativas.
* Você pode remover resultados e atividades de uma meta excluindo-os. Os resultados e as atividades excluídos não podem ser recuperados.
* Quando você remove o resultado ou a atividade de uma meta, o progresso do resultado removido ou da atividade afeta o progresso geral da meta.
* Não é possível excluir um projeto de uma meta, mas você pode desconectá-lo da meta. Ao desconectar o projeto da meta, a porcentagem concluída do projeto não afeta mais o progresso da meta.

  Para obter informações sobre como os projetos afetam o progresso da meta, consulte [Adicionar projetos às metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Não é possível remover um resultado ou uma atividade de uma meta e não é possível desconectar uma meta secundária ou um projeto, se eles forem o último indicador de progresso para a meta.
* Se um projeto for excluído da área Projetos e for o último indicador de progresso de uma meta, a meta se tornará Inativa.

## Excluir resultados e atividades das metas

Você remove os resultados e as atividades de uma meta ao excluí-los. A exclusão de resultados e atividades de uma meta é idêntica.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![Delete result](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

{{step1-to-goals}}

Isso abre a área Metas do Workfront e a Lista de metas é exibida por padrão.

1. Clique no nome de uma meta da qual deseja remover resultados e atividades.

   Isso abre a página de meta.

1. Clique em **Indicadores de progresso** no painel esquerdo.

1. Selecione um resultado ou uma atividade e clique no ícone **Excluir** ![Ícone Excluir](assets/delete-icon.png) na parte superior da lista.

1. Clique em **Excluir** para confirmar a exclusão. O resultado ou a atividade é excluído e não pode ser recuperado. A porcentagem concluída das atualizações de meta para excluir a atividade ou resultado excluído.


## Remover projetos das metas

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![Disconnect](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


{{step1-to-goals}}

Isso abre a área Metas do Workfront e a Lista de metas é exibida por padrão.

1. Clique no nome de uma meta da qual deseja remover resultados e atividades.

   Isso abre a página de meta.
1. Clique em **Indicadores de progresso** no painel esquerdo.
1. Selecione um projeto e clique no ícone **Desconectar** ![Ícone Desconectar](assets/disconnect-icon.png) na parte superior da lista.
1. Clique em **Desconectar** para confirmar.

   O projeto não está mais conectado à meta. A porcentagem concluída das atualizações de meta para excluir o projeto desconectado.

