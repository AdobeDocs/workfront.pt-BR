---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão geral da restrição de tarefa: Datas fixas'
description: Você pode usar a restrição de tarefa Datas fixas quando quiser ser específico sobre a data de início e a data de término exatas das suas tarefas. Para obter mais informações sobre restrições de tarefa, consulte Visão geral da Restrição de Tarefa.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Visão geral da restrição de tarefa: Datas fixas

Você pode usar a restrição de tarefa Datas fixas quando quiser ser específico sobre a data de início e a data de término exatas das suas tarefas. Para obter mais informações sobre restrições de tarefa, consulte [Visão geral da restrição de tarefa](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Visão geral da restrição Datas fixas

Considere o seguinte ao usar a restrição Datas fixas :

* Ao selecionar a restrição de tarefa Datas fixas (FIXT), você deve especificar a Data inicial planejada e a Data de conclusão planejada da tarefa. Nesse caso, o relacionamento antecessor da tarefa é ignorado.
* O campo Duration da tarefa não é editável ao usar a restrição FIXT. A Duração é calculada como a diferença entre as Datas de Início Planejado e de Conclusão Planejada da tarefa.
* Se o Tipo de duração da tarefa for Orientada ao Esforço, o número de designados à tarefa também afetará a Duração da tarefa.
* Ao mover ou copiar uma tarefa com uma restrição FIXT para outro projeto, a restrição da tarefa ou as datas do projeto podem mudar, dependendo das datas de restrição e das datas de início e conclusão do projeto. Os seguintes cenários existem:

   * Quando o projeto de destino é agendado desde o início:

      * Quando qualquer data de restrição da tarefa for anterior à Data de Início do Projeto, a restrição de tarefa será alterada para Assim que possível.
      * Quando qualquer ou ambas as datas de restrição da tarefa forem posteriores à Data de Conclusão Planejada do projeto, a Data de Conclusão Planejada do projeto será alterada para corresponder à data de restrição de conclusão da tarefa.
   * Quando o projeto de destino é agendado a partir da conclusão:

      * Quando qualquer data de restrição da tarefa for posterior à Data de conclusão do projeto, a restrição da tarefa será alterada para O mais tarde possível.
      * Quando qualquer ou ambas as datas de restrição da tarefa forem anteriores à Data Inicial Planejada do projeto, a Data Inicial Planejada do projeto será alterada para corresponder à data de restrição inicial da tarefa.
   * Independentemente do agendamento do projeto, quando as datas de restrição da tarefa estão dentro das Datas de Início e Conclusão do projeto, não há alterações na Restrição de Tarefa ou nas datas do projeto.

   Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md). Para obter informações sobre cópia de tarefas, consulte [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obter informações sobre como atualizar a Restrição de Tarefa em uma tarefa, consulte [Atualizar a Restrição de Tarefa de uma tarefa](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
