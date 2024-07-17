---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Visão geral da Restrição de tarefa: datas fixas"
description: Você pode usar a restrição da tarefa Datas fixas quando quiser ser específico sobre a data exata de início e de término de suas tarefas. Para obter mais informações sobre restrições de tarefa, consulte Visão geral de Restrição de Tarefa.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Visão geral de Restrição de tarefa: datas fixas

Você pode usar a restrição da tarefa Datas fixas quando quiser ser específico sobre a data exata de início e de término de suas tarefas. Para obter mais informações sobre restrições de tarefa, consulte [Visão geral da Restrição de Tarefa](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Visão geral da restrição Datas Fixas

Considere o seguinte ao usar a restrição Datas fixas:

* Quando você seleciona a restrição de tarefa Datas Fixas (FIXT), deve especificar a Data Inicial Planejada e a Data de Conclusão Planejada da tarefa. Nesse caso, o relacionamento predecessor da tarefa é ignorado.
* O campo Duração da tarefa não é editável ao usar a restrição FIXT. A duração é calculada como a diferença entre as datas de início e de conclusão planejadas da tarefa.
* Se o Tipo de duração da tarefa for Orientado pelo Esforço, o número de atribuídos na tarefa também afetará a Duração da tarefa.
* Quando você move ou copia uma tarefa com uma restrição FIXT para outro projeto, a restrição da tarefa ou as datas do projeto podem mudar, dependendo de quais são as datas de restrição e quais são as datas de início e de conclusão do projeto. Existem os seguintes cenários:

   * Quando o projeto de destino está agendado do início:

      * Quando qualquer data de restrição da tarefa for anterior à Data inicial do projeto, a restrição da tarefa será alterada para O Mais Breve Possível.
      * Quando alguma ou ambas as datas de restrição da tarefa forem posteriores à Data de conclusão planejada do projeto, a Data de conclusão planejada do projeto será alterada para corresponder à data de restrição de conclusão da tarefa.

   * Quando o projeto de destino estiver agendado A partir da conclusão:

      * Quando qualquer data de restrição da tarefa for posterior à Data de conclusão do projeto, a restrição da tarefa será alterada para O mais tarde possível.
      * Quando alguma ou ambas as datas de restrição da tarefa forem anteriores à Data Inicial Planejada do projeto, a Data Inicial Planejada do projeto será alterada para corresponder à data inicial de restrição da tarefa.

   * Independentemente do cronograma do projeto, quando as datas de restrição da tarefa estiverem dentro das Datas de Início e Término do projeto, não há alterações na Restrição da tarefa ou nas datas do projeto.

  Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md). Para obter informações sobre como copiar tarefas, consulte [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

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
