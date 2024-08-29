---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Gerenciar metas na Lista de metas do Adobe Workfront
description: Depois que você ou outros usuários criam metas, é possível revisar o progresso e as informações na Lista de metas. Para obter informações sobre como criar metas, consulte Criar metas no Adobe Workfront Goals.
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 2%

---

# Gerenciar metas na Lista de metas do Adobe Workfront

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

Depois que você ou outros usuários criam metas, é possível revisar o progresso e as informações na Lista de metas. Para obter informações sobre como criar metas, consulte [Criar metas nas Metas do Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as ações descritas neste artigo:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> 
   <p>Para o novo plano e estrutura de licença:
  <ul><li>Um plano Ultimate </li></ul>
   </p>
<p>Para o plano e a estrutura de licença atuais: 
<ul><li> A Pro ou superior </li>
  <li>Uma licença do Adobe Workfront Goals, além de uma licença da Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licença da Adobe Workfront*</td>
 <td>
 <p>Nova licença: Contributor ou superior</p>
 Ou
 <p>Licença atual: Solicitação ou superior</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">visão geral das licenças da Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produto*</td>
 <td>
 <p> Novo requisito de produto, um dos seguintes: </p>
<ul>
<li>Um plano Select ou Prime do Adobe Workfront e uma licença adicional do Adobe Workfront Goals.</li>
<li>Um plano do Ultimate Workfront que inclui o Workfront Goals por padrão. </li></ul>
 <p>Ou</p>
 <p>Requisito atual do produto: um plano do Workfront e uma licença adicional para o Adobe Workfront Goals. </p> <p>Para obter informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as Metas do Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Nível de acesso</td>
 <td> <p>Editar acesso às Metas</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permissões de objeto</td>
 <td>
  <div>
  <p>Exibir permissões ou mais altas para a meta para exibi-la</p>
  <p>Gerenciar permissões para a meta para editá-la</p>
  <p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta no Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclui a área Metas no Menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Gerenciar metas na Lista de metas

Você pode visualizar e gerenciar metas nas seguintes seções do Workfront Goals:

* Lista de metas
* Alinhamento de metas

Cada seção exibe metas em formatos ligeiramente diferentes. A seção usada depende do propósito que você deseja atingir ao trabalhar com metas.

Para obter mais informações, consulte [seções de Visão Geral das Metas do Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

Este artigo descreve como analisar metas na Lista de metas.

Considere o seguinte ao revisar a Lista de metas:

* Você pode exibir metas que você ou qualquer outra pessoa em sua organização criou na Lista de metas. Você deve ter permissões de gerenciamento nas metas para poder editá-las.

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List section displays by default. You can view goals regardless of their status, period, or owner, by default.

   The list of goals contains the following columns with information about each goal, result, or activity: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 
       <div> 
        <p role="rowheader">Name </p> 
       </div> </td> 
      <td>The name of the goal, result, or activity.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Owner</td> 
      <td>The name of the goal, result, or activity owner. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Period</td> 
      <td>The time period for which the goal is scheduled.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress </td> 
      <td> <p>The progress indicator for the goal includes the following:</p> 
       <ul> 
      <li> <p>The progress label. </p> <p>For information, see <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Overview of goal progress and condition in Adobe Workfront Goals</a>. </p> </li> 
      <li> <p>The percent complete of the goal, activity, or result. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Status (includes alignment icon)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
      <td> <p>The status of the goal which can be one of the following:</p> 
       <ul> 
        <li>Active</li> 
        <li>Draft</li> 
        <li>Inactive</li> 
        <li>Closed</li> 
       </ul> <p>For information about goal status, see <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Goal status overview in Adobe Workfront Goals</a>. </p> <p>The alignment icon appears on goals that are aligned to other goals. For information about aligning goals, see <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Align goals by connecting them in Adobe Workfront Goals</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Use the filters in the upper-right corner of the goal list to select only goals that are important to you. For information about using filters in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md)
1. Click any of the fields in the column headers to sort it by that field.

   An arrow displays to the right of the field by which the list is sorted.

   ![](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

   * Results names, owners, and progress

     For information about results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   
   * Activity names, owners, and progress

     For information about activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

1. Click the name of a goal to open the **Goal Details** panel on the right and review more information about the goal as well as manage it. For information about reviewing individual goals, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Optional) Expand the **Goals per page** drop-down menu and select from the following options to display additional goals:

   * 20  
      
      This is the default selection. 
   * 50
   * 100

1. Click **Print** to export a list of goals, results, and activities to a .pdf file.

   >[!TIP]
   >
   >* When printing a list of goals, the file produced contains only the information displayed on the screen. Items eliminated by filtering a list of goals do not display in the .pdf file.
   >* When you do not expand the goals in the list before printing the list, the .pdf file displays only goals without their results and activities.

   For more information, see [Print the Goal List in Adobe Workfront Goals](../../workfront-goals/goal-management/print-the-goal-list.md). 

1. Click the **Alignment icon** ![](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

Para gerenciar metas na Lista de metas:

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal** no canto superior direito e clique em **Metas**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   A seção Lista de metas é exibida por padrão. Você pode exibir metas independentemente de seu status, período ou proprietário, por padrão.

   A lista de metas contém os seguintes campos com informações sobre cada meta:

   * **Nome**: o nome da meta.
   * **Proprietário**: o nome do proprietário da meta.
   * **Período**: o período para o qual a meta é agendada.
   * **Status**: o status da meta pode ser um dos seguintes:
      * Ativo
      * Rascunho
      * Inativo
      * Fechado

     Para obter informações sobre o status da meta, consulte [Visão geral do status da meta no Adobe Workfront Goals](../goal-management/goal-status-overview.md).

     O ícone de alinhamento aparece nas metas alinhadas a outras metas. Para obter informações sobre como alinhar metas, consulte [Alinhar metas ao conectá-las às Metas do Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md).

   * **Condição**: uma representação visual de como a meta está progredindo dentro do período alocado para que ela seja concluída.

     A condição de uma meta pode ser uma das seguintes:

      * Novo(a)
      * No Prazo
      * Em Risco
      * Com problemas

     Para obter informações sobre as condições da meta, consulte [Visão geral do progresso da meta e da condição nas Metas do Adobe Workfront](../goal-management/calculate-goal-progress.md).

   * **Progresso**: o indicador de progresso da meta como um valor percentual. A cor do indicador de progresso corresponde à cor da Condição da meta.

     Para obter informações, consulte [Calcular progresso da meta em Metas do Adobe Workfront](../goal-management/calculate-goal-progress.md).

1. Clique no ícone de filtro ![](assets/filter-icon.png) no canto superior direito da lista de metas e aplique filtros para exibir somente as metas que são importantes para você.

   Para obter informações sobre como usar filtros nas Metas do Workfront, consulte [Informações de filtro nas Metas do Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Clique em qualquer um dos campos nos cabeçalhos da coluna para classificar a lista por esse campo.
Uma seta é exibida à direita do campo pelo qual a lista é classificada.

1. (Opcional) Clique no campo na coluna novamente para classificar a mesma coluna em uma ordem decrescente.
1. Clique no nome de uma meta para abrir a página da meta.
1. Selecione uma meta na lista e clique em uma das seguintes opções na parte superior da lista:
   * **Editar** ícone ![](assets/edit-icon.png) para editar informações sobre a meta. Para obter informações, consulte [Editar metas nas Metas da Adobe Workfront](../goal-management/edit-goals.md).
   * **Compartilhar** ícone ![](assets/share-icon.png) para compartilhar a meta com outras pessoas. Para obter informações, consulte [Compartilhar uma meta no Adobe Workfront Goals](../workfront-goals-settings/share-a-goal.md).
   * **Abrir alinhamento** ícone ![](assets/align-icon-unshimmed.png) para abrir a área Alinhamento de Meta. Essa opção é exibida somente quando a meta selecionada está alinhada a outra meta.
   * **Excluir** ícone ![](assets/delete-icon.png) para excluir a meta, em seguida, clique em **Excluir** para confirmar.  Para obter informações, consulte [Excluir e desativar metas nas Metas do Adobe Workfront](../goal-management/delete-and-deactivate-goals.md).





