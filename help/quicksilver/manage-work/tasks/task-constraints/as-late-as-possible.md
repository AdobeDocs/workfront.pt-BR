---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''Visão geral da restrição de tarefa: O Mais Tarde Possível"'
description: O Mais Tarde Possível (ALAP) é uma Restrição de Tarefa do Adobe Workfront que coloca o tempo de conclusão da tarefa o mais próximo possível do final do projeto.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Visão geral da restrição de tarefa: O Mais Tarde Possível

O Mais Tarde Possível (ALAP) é uma Restrição de Tarefa do Adobe Workfront que coloca o tempo de conclusão da tarefa o mais próximo possível do final do projeto.

O uso dessa restrição pode fazer com que o antecessor ou as Tarefas dependentes sejam reprogramadas.

Para obter mais informações sobre os relacionamentos do antecessor, consulte [Usar predecessores de tarefa](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

O Mais Tarde Possível é a restrição padrão se um projeto usar um modo de programação de Programação a partir da Data de Conclusão e o padrão do sistema ou grupo para a Data Inicial de uma tarefa for Baseado na Data Planejada do Projeto.

Para obter informações sobre onde definir a Restrição padrão para uma nova tarefa, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Para obter informações sobre como atualizar a Restrição de Tarefa em uma tarefa, consulte [Atualizar a Restrição de Tarefa de uma tarefa](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible:&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click&nbsp;<strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the&nbsp;<strong>Overview</strong>&nbsp;section, expand the&nbsp;<strong>Task Constraint</strong>&nbsp;drop-down menu.</p> </li>
<li value="4"> <p>Select&nbsp;<strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.&nbsp;</li>
</ol>
</div>
-->

## A diferença entre o Horário Disponível Mais Recente e O Mais Tarde Possível

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

A restrição de Tempo Disponível Mais Recente difere da restrição As Late As Possible quando os seguintes critérios existem:

* O projeto está programado desde a data inicial
* As tarefas no projeto têm uma relação predecessora
* A tarefa sucessora tem uma restrição de tarefa flexível

Nesta situação:

* **Hora Disponível Mais Recente:** Usar a restrição de Tempo Disponível Mais Recente na tarefa predecessora dá prioridade à restrição flexível do sucessor.

   **Exemplo:** Por exemplo, a Tarefa A é antecessora da Tarefa B. A Tarefa A tem a Restrição de Tempo Disponível Mais Recente e a Tarefa B tem a restrição O Mais Rápido Possível. Nessa situação, a Tarefa A é agendada o mais próximo possível do início do projeto.

   ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **O Mais Tarde Possível:** Nesse cenário, o uso da restrição As Late As Possible na tarefa predecessora dá prioridade à tarefa predecessora.

   **Exemplo:** Por exemplo, a Tarefa A é um antecessor da Tarefa B. A Tarefa A tem a restrição As Late As Possible e a Tarefa B tem a restrição O Mais Rápido Possível. Nessa situação, a Tarefa A é agendada o mais próximo possível do final do projeto.

   ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

 

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest&nbsp;Available Time constraint differs from the As Late&nbsp;As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest&nbsp;Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest&nbsp;Available Time constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close&nbsp;to the start&nbsp;of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late&nbsp;As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late&nbsp;As Possible&nbsp;constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close to the end&nbsp;of the project as possible.</p> </li>
</ul>
</div>
-->
