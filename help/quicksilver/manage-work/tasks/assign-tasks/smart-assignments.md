---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Visão geral das atribuições inteligentes
description: Ao gerenciar atribuições de tarefas e problemas, você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho. As atribuições inteligentes são sugestões que o Adobe Workfront apresenta ao atribuir itens de trabalho a recursos com base em um algoritmo que determina o recurso mais apropriado para o trabalho.
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Visão geral das atribuições inteligentes

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>   
  
<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> 
-->

Ao gerenciar atribuições de tarefas e problemas, você pode usar atribuições inteligentes para identificar quem é o melhor usuário para concluir o trabalho. As atribuições inteligentes são sugestões que o Adobe Workfront apresenta ao atribuir itens de trabalho a recursos com base em um algoritmo que determina o recurso mais apropriado para o trabalho.

>[!NOTE]
>
>As atribuições inteligentes não levam em conta a disponibilidade do usuário. No entanto, sua disponibilidade de acordo com seus agendamentos afeta as Datas Planejadas e Projetadas das tarefas e problemas quando são atribuídas. Para obter informações sobre cronogramas, consulte o artigo [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Este artigo contém informações gerais sobre atribuições inteligentes. Para obter informações sobre como usar atribuições inteligentes para atribuir tarefas e problemas a usuários, consulte [Fazer atribuições inteligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## Visão geral das atribuições inteligentes

Considere o seguinte ao trabalhar com atribuições inteligentes:

* O algoritmo funciona independentemente para tarefas e problemas. Isso significa que a lista de usuários sugeridos para problemas pode ser diferente da lista de usuários sugeridos para uma tarefa, pois o Workfront cria as listas de acordo com critérios relacionados a problemas e tarefas separadamente.
* As atribuições inteligentes não recomendam funções de trabalho ou equipes. Em vez disso, são sugestões de usuários que se encaixam melhor para concluir uma tarefa ou um problema.
* As atribuições sugeridas são sempre usuários ativos.
* O usuário listado primeiro deve ser a melhor correspondência para a tarefa.

## Localizar sugestões de atribuição inteligente

Você pode ver as atribuições inteligentes nas seguintes áreas onde pode atribuir tarefas ou problemas:

* Uma lista de tarefas ou problemas ou um relatório <!--edit this to say just issue list or report and update screen shot - add new one-->

  ![](assets/smart-assignments-task-list-nwe-350x280.png)

<!--
* <span class="preview">A task list or report (******insert shot here*****)</span>
-->

* Um cabeçalho de tarefa ou problema

  ![](assets/smart-assignments-task-header-nwe-350x302.png)

* O painel Resumo de tarefas ou problemas

  ![](assets/smart-assignments-summary-panel-nwe-350x332.png)

* O campo Atribuições de um item listado na área Página inicial

  ![](assets/smart-assignments-in-home-nwe-350x216.png)


<!--removed for scheduling deprecation: 

* Resource Scheduling

  ![](assets/smart-assignments-scheduling-350x219.png)

  >[!CAUTION]
  >
  >Resource Scheduling is a deprecated feature. For more information, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* Balanceador de carga de trabalho

  ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## Critérios de atribuições inteligentes

<!--
<div class="preview">

Smart assignments work differently for tasks than for issues.  

### Smart assignments criteria for tasks

Task smart assignments work in two phases:  

#### First phase of smart assignment calculation criteria for tasks 

Workfront calculates a similarity score for every assignment. The calculation for the similarity score and the order in which the assignments are listed take into account the following:  

* A score of 100% is given to an existing assignment where the task, project, and portfolio names are identical to the task you're trying to assign. The project and portfolio names of the task of an existing assignment must also match the project and portfolio of the task you are trying to assign.   

* If only some of this information from other assignments matches on the existing tasks, the score might be lower.  

  For example, if you are assigning a task called "My second task" on a project called "My project" in a portfolio called "My portfolio" and you have an existing task called "My task" in another project called "My project" in a portfolio called "My portfolio", the user assigned to "My task" might get a score of 95% because the name of the existing task and the task you're trying to assign now are similar, but not identical.  
 
    >[!TIP]
    >
    >  Workfront looks for matches only in the Name fields of tasks, projects, and portfolios and not in any other fields. 

* An assignment could get a higher score when they are assigned to a lot of tasks in the system that are similar in names. For example, if a team called "Development" is assigned to 50% of the tasks in the system containing "AI" in the name and you are now assigning another task with "AI" in the name, the score of the "Development" team is higher. In this case, the names of  projects and portfolios are not as important.  

* Taking into account this scoring system, the first 7 suggestions are listed as smart assignments, in the descending order of their scores. Assignments with scores lower than 40% do not display.  

* If several assignments have identical scores, they display in descending order of the date on which the assignments were made.  
For example, if Rick was assigned to a similar task earlier today and Jennifer was assigned to a similar task two days ago, Rick displays first.  

* If there are no matches using this calculation, the second step of smart assignments applies which is calculated using a different algorithm.  

#### Second phase of smart assignment calculation criteria for tasks

If the first step of task smart assignments has found no matches, Workfront calculates smart assignments for tasks in the same way that it calculates them for issues.  

### Smart assignments criteria for tasks and issues 

</div> 

>[!NOTE]
>
><span class="preview">The following criteria applies for tasks only when the first phase of the task smart assignment calculation did not find any matches. The following criteria always applies for issues, by default. </span>

-->

Os usuários são recomendados na lista suspensa atribuições inteligentes com base em uma combinação dos seguintes critérios (listados na ordem do mais importante para o menos importante):

1. Usuários atribuídos a outros itens de trabalho nos últimos 30 dias pelo usuário que fez a atribuição. Os primeiros 50 usuários que correspondem a esse critério são exibidos. O usuário atribuído com mais frequência é exibido primeiro.

2. Se o item de trabalho for atribuído a uma equipe ou função, a lista de usuários sugeridos será filtrada ainda mais levando em conta as atribuições existentes abaixo. Nesse caso, somente os seguintes usuários são exibidos na lista de sugestões:

   * Usuários cuja Equipe inicial é a equipe atribuída ao item de trabalho.
   * Usuários cuja função principal é a função atribuída ao item de trabalho.

>[!TIP]
>
>* Se não houver nenhuma função ou equipe atribuída na tarefa ou problema, o Workfront exibirá todos os usuários atribuídos nos últimos 30 dias, até 50 usuários.
>
>* Se você não tiver feito nenhuma atribuição nos últimos 30 dias, somente os usuários que pertencem à equipe atribuída ou têm a função atribuída ao item de trabalho serão exibidos na lista de atribuições inteligentes.

<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
