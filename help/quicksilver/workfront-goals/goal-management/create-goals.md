---
product-previous: workfront-goals
navigation-topic: goal-management
title: Criar metas no Adobe Workfront Goals
description: Seja você um CEO, um gerente ou um colaborador individual, é possível criar metas no Adobe Workfront Goals para alinhar seu trabalho às suas metas e às metas que descrevem a estratégia de sua organização.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 5%

---

# Criar metas no Adobe Workfront Goals

<!--Audited for P&P only: 4/2025-->

Seja você um CEO, um gerente ou um colaborador individual, é possível criar metas no Adobe Workfront Goals para alinhar seu trabalho às suas metas e às metas que descrevem a estratégia de sua organização.

## Requisitos de acesso

>[!NOTE]
>
>Sua empresa pode optar por continuar usando o Adobe Workfront Goals se ele comprou esse pacote no passado. Você precisa falar com o seu representante de conta para obter mais detalhes.
>
>O Adobe Workfront Goals não está mais disponível para compra.

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

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
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
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

## Diretrizes para a criação de metas

Antes de começar com as Metas do Workfront, recomendamos que você leia sobre as práticas recomendadas e as diretrizes para gerenciar metas de maneira eficaz. Para obter mais informações sobre as diretrizes para criar e gerenciar metas, consulte [visão geral das Metas do Adobe Workfront](../../workfront-goals/goal-management/wf-goals-overview.md).

## Criar metas

Este artigo descreve como criar uma meta estratégica no Workfront Goals. Para obter informações sobre como criar uma meta do Business Case, consulte [Criar metas do Business Case](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

Você pode criar uma meta estratégica de uma das seguintes maneiras:

* [Criar uma meta do zero](#create-a-goal-from-scratch)
* [Copiar uma meta existente](#copy-an-existing-goal)
* [Converter um resultado ou atividade em uma meta](#convert-a-result-or-activity-to-a-goal)

### Criar uma meta do zero {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![Add goal box](assets/add-goal-box-350x235.png)

   >[!TIP]
   >
   >You can add a goal from any section in Workfront Goals. The process for creating a goal is identical regardless of the section you choose to add the goal from.

1. Start typing what you want to achieve in the **Goal** field. This is the name of the goal and a required field. 
1. Select a time period when the goal should be executed in the **Period** drop-down menu. This is a pre-filled field. The default is the current quarter.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a **Start date** and an **End date** for your goal, if you clicked **Define custom dates**.

   >[!TIP]
   >
   >* You can create a goal with dates in any time period, including up to 2 years in the past. 
   >* When defining custom dates, they are constrained by the initial date you selected. So if you select quarter and then custom dates, you can't go beyond that quarter.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same timeframes for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your over-arching strategy.

1. (Optional) Click your name in the **Owner** field, if you want to indicate someone else as the owner of the goal. By default, you are the owner of goals you create. 
1. Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. (Optional) Enter a **Description** for the goal. This field is optional. 
1. Click **Save**.

   The status of the new goal is Draft.

   >[!IMPORTANT]
   >
   >You must associate a goal with a progress indicator to activate it and start working on it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >
   >* Add a Result
   >
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

-->

1. Clique no ícone **Menu Principal** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito e clique em **Metas**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   A lista de metas é exibida.
1. Clique em **Nova meta**.

   A caixa Nova meta é exibida.

   ![Nova caixa de meta](assets/new-goal-box-unshimmed.png)

1. Especifique informações nos seguintes campos:
   * **Nome da meta**: insira um nome para a meta. Este campo é obrigatório.
   * **Período**: selecione um trimestre ou ano predefinido no campo suspenso **Período**

     Ou

     Selecione a opção **Habilitar datas personalizadas** e selecione uma **Data inicial** e uma **Data final** para a meta.

     Os anos anterior, atual e seguinte e seus respectivos trimestres são listados como opções predefinidas no campo suspenso Período.

     O Período da meta indica o período em que você espera que a meta seja concluída.

   * **Proprietário da meta**: comece digitando o nome de um usuário, equipe, grupo ou de sua organização para indicar quem é o proprietário da meta. Você está selecionado como o proprietário da meta por padrão.
   * **Descrição**: insira informações adicionais sobre a meta.
1. Clique em **Criar meta**.

   A nova meta está listada na Lista de metas e tem o status de **Rascunho**.

   Você deve associar uma meta a um indicador de progresso para ativá-la e começar a trabalhar nela.

   Siga pelo menos um destes procedimentos para preparar uma meta a ser ativada:
   * Adicionar um resultado

     Para obter informações sobre como adicionar resultados, consulte [Adicionar resultados às metas no Adobe Workfront Goals](../results-and-activities/add-results-to-goals.md).
   * Adicionar uma atividade

     Para obter informações sobre como adicionar atividades, consulte [Adicionar atividades às metas no Adobe Workfront Goals](../results-and-activities/add-activities-to-goals.md).
   * Alinhar outra meta a ela

     Para obter informações sobre como alinhar metas, consulte [Alinhar metas ao conectá-las às Metas do Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md).


### Copiar uma meta existente {#copy-an-existing-goal}

Você pode criar uma meta copiando uma existente.

Para obter informações sobre como copiar metas, consulte [Copiar metas nas Metas da Adobe Workfront](../../workfront-goals/goal-management/copy-goals.md).

### Converter um resultado ou atividade em uma meta {#convert-a-result-or-activity-to-a-goal}

Você pode criar uma meta convertendo o resultado ou a atividade de uma meta existente em uma meta. A nova meta fica alinhada à meta original.

Para obter informações sobre como converter resultados e atividades em metas, consulte [Alinhar metas convertendo resultados e atividades em metas](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

