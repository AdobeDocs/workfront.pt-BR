---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão Geral Da Restrição De Tarefa: Não Terminar Depois De'
description: Não Terminar Depois de (FNLT) é uma Restrição de Tarefa que programa uma tarefa para ser concluída antes da data especificada.
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Visão geral da restrição de tarefas: não terminar depois de

Não Terminar Depois de (FNLT) é uma Restrição de Tarefa que programa uma tarefa para ser concluída antes da data especificada.

## Visão geral da restrição Não Terminar Depois de

Considere o seguinte ao usar a restrição Não Terminar Depois de (FNLT) para uma tarefa:

* Você deve usar essa restrição quando o projeto está agendado a partir da data inicial. Nesse caso, você pode fornecer uma restrição leve em uma tarefa antes que ela force outras tarefas dependentes a serem exibidas como Em Risco.
* Quando você usa a restrição FNLT com um projeto Programar da Data de Conclusão, essa restrição programa a tarefa da mesma maneira que uma tarefa o Mais Tarde Possível.
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
<h2>Use the Finish No Later Than constraint</h2>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Finish No Later Than</strong>.</p> <p> <img src="assets/fnlt-350x266.png" alt="FNLT.png" style="width: 350;height: 266;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>You must complete the task on and not later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
