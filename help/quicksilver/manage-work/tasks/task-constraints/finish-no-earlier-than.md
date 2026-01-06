---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão Geral Da Restrição De Tarefa: Não Terminar Antes De'
description: Não Terminar Antes de (FNET) é uma Restrição de Tarefa que programa uma tarefa para ser concluída após a data especificada.
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Visão geral de Restrição de Tarefa: Não Concluir Antes de

Não Terminar Antes de (FNET) é uma Restrição de Tarefa que programa uma tarefa para ser concluída após a data especificada.

## Visão geral da restrição Não Terminar Antes de

Considere o seguinte ao usar a restrição Não Terminar Antes de (FNET) para uma tarefa:

* Você deve usar essa restrição quando o projeto estiver agendado a partir da data de conclusão. Nesse caso, você pode fornecer uma restrição leve na tarefa antes de forçar outras tarefas dependentes a serem mostradas Em Risco.
* Quando você usa FNET em um projeto agendado **Da Data de Início**, a restrição agenda a tarefa da maneira que agendaria se a restrição fosse o Mais Breve Possível.
* Quando você move ou copia uma tarefa com uma restrição FNET para outro projeto, a restrição da tarefa ou as datas do projeto podem mudar dependendo de quais são as datas de restrição e quais são as datas de início e conclusão do projeto. Existem os seguintes cenários:

   * Quando o projeto de destino está agendado do início:

      * Quando a data de restrição da tarefa for anterior à Data de início planejada do projeto, a restrição da tarefa será alterada para O Mais Breve Possível.
      * Quando a data de restrição da tarefa for posterior à Data de Conclusão Planejada do projeto, a Data de Conclusão Planejada do projeto será alterada para corresponder à data de restrição da conclusão da tarefa.

   * Quando o projeto de destino estiver agendado A partir da conclusão:

      * Quando a data de restrição da tarefa for posterior à Data de conclusão do projeto, a restrição da tarefa será alterada para O mais tarde possível.
      * Quando a data de restrição da tarefa for anterior à Data Inicial Planejada do projeto, a Data Inicial Planejada do projeto será alterada para corresponder à data inicial de restrição da tarefa.

   * Independentemente do cronograma do projeto, quando a data de restrição da tarefa estiver dentro das datas de início e conclusão do projeto, não há alterações na restrição da tarefa ou nas datas do projeto.

  Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md). Para obter informações sobre como copiar tarefas, consulte [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

  Para obter informações sobre como atualizar a Restrição de Tarefa em uma tarefa, consulte [Atualizar a Restrição de Tarefa de uma tarefa](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Finish No Earlier Than constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Earlier Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>Finish No Earlier Than</strong>.</p> <p> <img src="assets/fnet-350x267.png" alt="FNET.png" style="width: 350;height: 267;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete no earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes.</strong> </li>
</ol>
</div>
-->
