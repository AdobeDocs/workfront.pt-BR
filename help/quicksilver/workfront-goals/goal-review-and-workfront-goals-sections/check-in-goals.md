---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Atualizar progresso da meta nas Metas do Adobe Workfront
description: Você deve revisar suas metas periodicamente e atualizar o progresso delas para garantir que não fiquem para trás ou corram o risco de não serem atingidas.
author: Alina
feature: Workfront Goals
exl-id: 5092f508-e52c-4934-a8c1-d0be04ecce13
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Atualizar progresso da meta nas Metas do Adobe Workfront

Você deve revisar suas metas periodicamente e atualizar o progresso delas para garantir que não fiquem para trás ou corram o risco de não serem atingidas.

<!--And: take this last sentence ^^ out when you update this for goal redesign production.-->

## Requisitos de acesso

Você deve ter o seguinte:

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
  <ul><li>Um plano Ultimate </li>
  Ou
  <li>Uma licença adicional para o Adobe Workfront Goals para os planos Prime ou Select Adobe Workfront. </li></ul> </p>
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
 <td> <p>Editar acesso às Metas</p></td>
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

## Pré-requisitos

Você deve ter uma meta ativa antes de começar.

Não é possível atualizar o progresso das metas rascunhos, inativas ou fechadas.

## Considerações para atualização de metas

Leve em consideração o seguinte ao atualizar o progresso das metas:

* O Workfront Goals calcula automaticamente o progresso de uma meta ao atualizar o progresso de seus indicadores de progresso.

  >[!TIP]
  >
  >Não é possível atualizar o progresso diretamente em uma meta. Você deve atualizar o progresso dos indicadores de progresso da meta (atividades, resultados, projetos conectados) que, por sua vez, atualizam o progresso da meta. Para atualizar o progresso dos projetos, você deve atualizar as tarefas no projeto.

  Consulte também os seguintes artigos:

   * Para obter informações sobre como adicionar atividades às metas, consulte [Adicionar atividades às metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * Para obter informações sobre como adicionar resultados às metas, consulte [Adicionar resultados às metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * Para obter informações sobre como o Workfront Goals calcula o progresso em uma meta, consulte [Visão geral do progresso e da condição da meta no Adobe Workfront Goals](../../workfront-goals/goal-management/calculate-goal-progress.md).

* Você deve criar metas e ativá-las antes de atualizar o progresso delas.

  Consulte também os seguintes artigos:

   * Para obter informações sobre como criar metas, consulte [Criar metas nas Metas do Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
   * Para obter informações sobre como ativar metas, consulte [Ativar metas no Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

  >[!IMPORTANT]
  >
  >Não é possível atualizar o progresso das metas que estão em rascunho, fechadas ou inativas.

* Na primeira vez que você ou outra pessoa atualiza o progresso de um resultado ou atividade em uma meta, o Progresso da meta é alterado de Novas Metas e do Workfront começa a registrar atualizações de progresso e status de progresso na meta.

<!--

## Update goal progress by using Check-in in the Production environment

>[!IMPORTANT]
>
> <span class="preview"> The Check-in functionality has been removed from the Preview environment and will be removed from Workfront Goals with the 23.1 release. See the [Update goal progress in the Preview environment](#update-goal-progress-in-the-preview-environment) section in this article to update goal progress in Preview. </span>


You can check in on goals at the individual goal level, or you can check in on multiple goals from the Check-in section of Workfront Goals.

* [Update individual goals](#update-individual-goals) 
* [Update goals in the Check-in section](#update-goals-in-the-check-in-section)

### Update individual goals {#update-individual-goals}

When you check in on a goal at the goal level, you can update the progress of the results and activities that are assigned to you or other users.

For information about how to update additional information about results and activities, see [Edit results and activities in Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area.

   All goals display by default. 

1. (Optional) Click any of the following sections in the left panel to access a list of goals:

   * Goal Alignment 
   * Pulse 
   * Check-in

   Or

   From the Goal List, click the name of a goal to open the **Goal Details** panel on the right.

   >[!TIP]
   >
   >You must have Edit access to Goals in your Access Level to view the Check-in section or the Check in button.

1. Click **Check in**.

   ![](assets/check-in-link-inside-goal-details-highlighted-350x156.png)

   The progress of results and activities becomes editable.

1. Update the current progress on each of the results. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

1. Update the percent complete on the Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

1. Click **Back to Summary** to return to the Goal Details panel.

   Your goal progress updates as you update the results and activities of your goal. 

1. Click the **X icon** in the upper-right corner of the Goal Details panel to close it.

### Update goals in the Check-in section {#update-goals-in-the-check-in-section}

You can use the Check-in section to check in on goals when you want to quickly provide updates for several goals at the same time.

>[!TIP]
>
>You can access the Check-in section from any of the following sections:
>
>* Goal List 
>* Goal Alignment 
>* Pulse 
>

When you check in on a goal in the Check-in section, you can update the progress of the results and activities that are assigned only to you. You cannot update the progress of results and activities that are assigned to other users in this section.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List section displays by default. 

1. Click Check-in in the left panel.

   Or

   (Conditional) If you are in the Goal List, Goal Alignment, or Pulse sections, click the **Check in** button in the upper-right of the screen. This opens the Check-in section.

   ![](assets/check-in-button-highlighted-350x102.png)

   Goals display in a list and results and activities are listed under each goal.

   ![](assets/check-in-page-with-show-all-aligned-goals-link-350x178.png)

1. (Optional) Click **Show all results**, **Show all activities**, or **Show all aligned goals** to the far right of the goal name to display all results, activities, and aligned goals of a goal whose progress you want to update.

   >[!CAUTION]
   >
   >You cannot directly update aligned goals, but you can update their results and activities.

1. Update the current progress on each of the results assigned to you. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

   The result and the goal progress updated automatically and you receive a confirmation of your changes.

1. Update the percent complete on your Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

   The activity and the goal progress updated automatically and you receive a confirmation of your changes.

1. (Optional) Add a comment for your goal, then click **Post** to save your comment.

-->

Para atualizar o progresso das metas:

1. Clique no ícone ![](assets/main-menu-icon.png) > **Metas** do **Menu Principal** no canto superior direito.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Isso abre a lista de metas. Todas as metas que você tem acesso para visualizar são exibidas por padrão.

   Como alternativa, você pode clicar em Alinhamento de metas no painel esquerdo.

1. Na Lista de Metas, clique no nome de uma meta para abrir a página de metas.
1. Clique em **Indicadores de progresso** no painel esquerdo.

   A lista de Indicadores de Progresso exibe todos os indicadores de progresso para a meta selecionada.

   >[!NOTE]
   >
   >  * Você só pode atualizar resultados e atividades.
   >  * Você deve atualizar os indicadores de progresso das metas secundárias para mostrar o progresso nas metas secundárias.
   >  * Você deve atualizar as tarefas nos projetos conectados para mostrar o progresso nos projetos.
   >   
   >    Por sua vez, o progresso das metas secundárias e o progresso dos projetos impulsionam o progresso da meta selecionada.


1. Para atualizar o progresso de um resultado ou atividade, clique no valor dentro da coluna **Progresso Real** do resultado ou atividade, digite um número para atualizar seu valor e pressione Enter.

   ![](assets/actual-progress-result-updating-highlighted-unshimmed.png)

   A barra de progresso do indicador de progresso na coluna Progresso e o progresso da meta no cabeçalho da meta são atualizados imediatamente.

