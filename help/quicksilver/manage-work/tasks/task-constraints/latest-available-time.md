---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Visão geral da Restrição de Tarefa: Último Tempo Disponível"
description: O Último Tempo Disponível (LAT) é um tipo de Restrição de Tarefa no Adobe Workfront.
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: c3abb5dce14c0b19ab2e5b82f159cd29f80f79e4
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Visão geral de Restrição de Tarefa: Último Tempo Disponível

O Último Tempo Disponível (LAT) é um tipo de Restrição de Tarefa no Adobe Workfront.

## Usar a Restrição de Tarefa de Tempo Mais Recente Disponível

Você pode usar a restrição LAT quando quiser agendar uma tarefa para começar no último horário disponível depois de considerar as relações predecessor-sucessor no projeto.

Essa restrição difere de Assim que Possível, pois não forçará predecessores ou sucessores a serem reagendados. Em vez disso, afetará somente o agendamento da tarefa à qual está associada, definindo-o para o horário mais recente disponível com base em sua relação com outras tarefas.

Para obter informações sobre como atualizar a Restrição de Tarefa em uma tarefa, consulte [Atualizar a Restrição de Tarefa de uma tarefa](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE: replaced with new article linked above) </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## A diferença entre o Último Horário Disponível e o Mais Tarde Possível

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
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
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
