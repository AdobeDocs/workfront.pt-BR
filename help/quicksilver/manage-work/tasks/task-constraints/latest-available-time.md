---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão geral da restrição de tarefa: Hora Disponível Mais Recente'
description: O Último Tempo Disponível (LAT) é um tipo de Restrição de Tarefa no Adobe Workfront.
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Visão geral da restrição de tarefa: Hora Disponível Mais Recente

O Último Tempo Disponível (LAT) é um tipo de Restrição de Tarefa no Adobe Workfront.

## Usar a Restrição de Tarefa de Tempo Disponível Mais Recente

Você pode usar a restrição LAT quando quiser agendar uma tarefa para começar no horário mais recente disponível após considerar os relacionamentos predecessor-sucessor no projeto.

Esta restrição difere do Mais Rápido Possível, na medida em que não obrigará os antecessores ou sucessores a serem reagendados. Em vez disso, ele só afetará o agendamento da tarefa à qual está associado, definindo-o para o último horário disponível com base em seu relacionamento com outras tarefas.

Para obter informações sobre como atualizar a Restrição de Tarefa em uma tarefa, consulte [Atualizar a Restrição de Tarefa de uma tarefa](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## A diferença entre o Horário Disponível Mais Recente e O Mais Tarde Possível

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
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
<p>(NOTE:&nbsp;this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
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
