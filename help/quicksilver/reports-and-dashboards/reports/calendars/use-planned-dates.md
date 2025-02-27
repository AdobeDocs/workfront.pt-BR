---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Usar datas planejadas em um relatório de calendário
description: Um relatório de calendário é um relatório dinâmico que fornece uma representação visual do seu trabalho. Você pode usar os campos Data planejada em um relatório de calendário para tarefas, problemas e projetos.
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: 78cfafe4c9a0fb846533c04da392a09dc1dbc9f1
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 2%

---

# Usar [!UICONTROL Datas planejadas] em um relatório de calendário

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span> 
-->

Um relatório de calendário é um relatório dinâmico que fornece uma representação visual do seu trabalho. Você pode usar os campos [!UICONTROL Data Planejada] em um relatório de calendário para os seguintes objetos:

* Tarefas
* Problemas
* Projetos

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Novo: Padrão</p>
       <p>ou</p>
       <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>[!UICONTROL Editar] acesso a [!UICONTROL Relatórios], [!UICONTROL Painéis] e [!UICONTROL Calendários]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Acesso [!UICONTROL Gerenciar] ao relatório de calendário</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar o grupo de itens na Produção

Você pode escolher como deseja que o grupo de itens seja exibido no calendário.

{{step1-to-calendars}}

1. Selecione o calendário ao qual deseja adicionar um novo grupo de itens.
Ou
Clique em **[!UICONTROL + Novo calendário]** e digite o nome do calendário.

   >[!NOTE]
   >
   >Você deve ter acesso de Edição a Relatórios, Painéis e Calendários no seu nível de acesso para criar um relatório de calendário.

1. À esquerda, clique em **[!UICONTROL Adicionar ao Calendário]** e em **[!UICONTROL Adicionar itens avançados]**.

1. Especifique o seguinte:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nomear este grupo de itens]</strong></td>
      <td>Digite um nome para o grupo de itens.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Cor]</strong></td>
      <td>Selecione uma cor para o grupo de itens. Todos os itens são exibidos na cor selecionada no relatório de calendário.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Campo de Data]</strong></td>
      <td><p>Escolha <strong>[!UICONTROL Datas planejadas]</strong>. Para obter mais informações sobre datas planejadas, consulte </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Visão geral da Data de início planejada do projeto</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Visão geral da Data de Início Planejada da tarefa</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Visão geral da Data de conclusão planejada da tarefa</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Definir a data de conclusão planejada do projeto</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>No calendário, mostrar</strong></td>
      <td><p>Escolha como deseja que as datas sejam exibidas:</p>
       <ul>
        <li><strong>[!UICONTROL Somente Data de Início]</strong>: o calendário exibe o objeto em uma única data.</li>
        <li><strong>[!UICONTROL Somente Data de Término]</strong>: o calendário exibe o objeto em uma única data.</li>
        <li><strong>[!UICONTROL Duration] (Início ao Fim)</strong>: o calendário exibe o objeto durante um período de dias.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Alternar para datas reais quando disponível]</strong></td>
      <td><p>O calendário alterna automaticamente para datas reais quando elas estão disponíveis. <br>Escolha <strong>[!UICONTROL Sim]</strong> ou <strong>[!UICONTROL Não]</strong> para alternar para datas reais quando disponíveis. Para obter mais informações sobre Datas Reais, consulte</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Visão Geral da Data de Início Efetivo do projeto </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Visão geral da Data de Término Efetivo do projeto </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Prossiga para a seção a seguir.

## Adicionar objetos ao grupo de itens na produção

Depois de configurar como deseja que os itens sejam exibidos, você precisa adicionar os objetos que deseja ver no calendário ao agrupamento.

1. No **[!UICONTROL O que você deseja adicionar ao calendário?seção]**, selecione

   * **[!UICONTROL Tarefas]**
   * **[!UICONTROL Projetos]**
   * **[!UICONTROL Problemas]**

1. Clique em **[!UICONTROL Adicionar Tarefas]**, **[!UICONTROL Adicionar Projetos]** ou **[!UICONTROL Adicionar Problemas]**, dependendo do tipo de objeto que você está adicionando ao calendário.
   ![Selecionar objeto para o calendário](assets/field-name.png)

1. No menu suspenso, comece digitando o nome do campo e selecione a origem do campo do objeto que deseja exibir no calendário (por exemplo, **[!UICONTROL Tarefas atrasadas]**).
1. Definir uma declaração de condição para o agrupamento de calendário.

   ![Declaração de condição](assets/condition-statement-calendar.png)

   Para saber mais sobre como definir condições, consulte [Filtro e modificadores de condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Opcional) Especifique objetos adicionais para o agrupamento de calendário repetindo as Etapas de 1 a 4.
1. No campo **[!UICONTROL Definir os rótulos de Tarefas/Projetos/Problemas para...]**, selecione como os objetos neste agrupamento de calendário são rotulados no calendário.

   >[!NOTE]
   >
   >Se as opções de rótulo padrão não estiverem disponíveis para um determinado objeto, o nome do objeto será exibido. Por exemplo, quando o rótulo [!UICONTROL Tarefa pai] é selecionado e não há nenhuma tarefa pai associada ao objeto, [!DNL Adobe Workfront] exibe o nome do objeto que você está visualizando no calendário.

1. Clique em **[!UICONTROL Salvar]**.

<!--

## Set up the group of items in Preview

You can choose how you want the group of items to display on your calendar.

{{step1-to-calendars}}

1. Select the calendar you want to add a new group of items to.
   Or
   Click **[!UICONTROL + New Calendar]** and enter the calendar name.

   >[!NOTE]
   >
   >You must have Edit access to Reports, Dashboards, and Calendars in your access level to create a calendar report.

1. On the left, click **[!UICONTROL Add to Calendar]**, then click **[!UICONTROL Add advanced items]**.

1. Specify the following:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Type a name for the group of items.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Select a color for the group of items. All items display in the selected color on the calendar report.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><p>Choose <strong>[!UICONTROL Planned dates]</strong>. For more information on planned dates, see </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Overview of the project Planned Start Date</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Overview of the task Planned Start Date</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overview of the task Planned Completion Date</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Set the project Planned Completion Date</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>On the calendar, show</strong></td>
      <td><p>Choose how you want the dates to show:</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong>: The calendar displays the object on a single date.</li>
        <li><strong>[!UICONTROL End Date Only]</strong>: The calendar displays the object on a single date.</li>
        <li><strong>[!UICONTROL Duration] (Start to End)</strong>: The calendar displays the object over a span of days.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to actual dates when available]</strong></td>
      <td><p>The calendar automatically switches to actual dates when they are available. <br>Choose <strong>[!UICONTROL Yes]</strong> or <strong>[!UICONTROL No]</strong> to switch to actual dates when available. For more information on Actual Dates, see</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Overview of the project Actual Start Date </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Overview of the project Actual Completion Date </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Continue to the following section.

## Add objects to the group of items in Preview

After you set up how you want items to display, you need to add the objects you want to see on the calendar to the grouping.

1. In the **[!UICONTROL What would you like to add to the calendar?]** section, select

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**

1. Click **[!UICONTROL Add Tasks]**, **[!UICONTROL Add Projects]**, or **[!UICONTROL Add Issues]**, depending on the object type you are adding to the calendar.
   ![Select object for calendar](assets/field-name.png)

1. In the drop-down menu, begin typing the field name, then select the field source of the object you want to display on the calendar (for example, **[!UICONTROL Late Tasks]**).
1. Set a condition statement for the calendar grouping.

   ![Condition statement](assets/condition-statement-calendar.png)

   To learn about setting conditions, see [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optional) Specify additional objects for the calendar grouping by repeating Steps 1-4.
1. In the **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** field, select how the objects in this calendar grouping are labeled in the calendar.

   >[!NOTE]
   >
   >If the default label options are not available for a certain object, the object name is shown instead. For example, when the [!UICONTROL Parent Task] label is selected and there is no parent task associated with the object, [!DNL Adobe Workfront] displays the object name you are viewing in the calendar.

1. Click **[!UICONTROL Save]**. 

-->