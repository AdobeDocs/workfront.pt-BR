---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão Geral Da Restrição De Tarefa: O Mais Tarde Possível'
description: O Mais Tarde Possível (ALAP) é uma Restrição de Tarefa do Adobe Workfront que coloca o tempo de conclusão da tarefa o mais próximo possível do final do projeto.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Visão geral de Restrição de tarefa: o mais tarde possível

O Mais Tarde Possível (ALAP) é uma Restrição de Tarefa do Adobe Workfront que coloca o tempo de conclusão da tarefa o mais próximo possível do final do projeto.

O uso dessa restrição pode fazer com que tarefas predecessoras ou dependentes sejam reagendadas.

Para obter mais informações sobre as relações de predecessoras, consulte [Usar predecessoras da tarefa: índice do artigo](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

A restrição padrão Mais Tarde Possível será a restrição padrão se um projeto usar o modo de programação Programação da Data de Conclusão e o padrão do sistema ou do grupo para a Data Inicial de uma tarefa for Baseado na Data Planejada do Projeto.

Para obter informações sobre onde definir a Restrição padrão para uma nova tarefa, consulte [Configurar preferências de tarefas e problemas do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Para obter informações sobre como atualizar a Restrição de Tarefa em uma tarefa, consulte [Atualizar a Restrição de Tarefa de uma tarefa](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## A diferença entre o Último Horário Disponível e o Mais Tarde Possível

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

A restrição Último Tempo Disponível difere da restrição O Mais Tarde Possível quando existem os seguintes critérios:

* O projeto está agendado a partir da data de início
* As tarefas no projeto têm um relacionamento predecessor
* A tarefa sucessora tem uma restrição de tarefa flexível

Nesta situação:

* **Último Tempo Disponível:** Usar a última restrição de Tempo Disponível na tarefa predecessora dá prioridade à restrição flexível da sucessora.

  **Exemplo:** Por exemplo, a Tarefa A é predecessora da Tarefa B. A Tarefa A tem a restrição Tempo Disponível Mais Recente e a Tarefa B tem a restrição O Mais Breve Possível. Nessa situação, a Tarefa A é agendada o mais próximo possível do início do projeto.

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **O Mais Tarde Possível:** neste cenário, usar a restrição O Mais Tarde Possível na tarefa predecessora dá prioridade à tarefa predecessora.

  **Exemplo:** Por exemplo, a Tarefa A é predecessora da Tarefa B. A Tarefa A tem a restrição O Mais Tarde Possível e a Tarefa B tem a restrição O Mais Breve Possível. Nessa situação, a Tarefa A é agendada o mais próximo possível do final do projeto.

  ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)



<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
