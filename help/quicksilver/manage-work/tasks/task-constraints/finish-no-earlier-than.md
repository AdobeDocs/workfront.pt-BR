---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão geral da restrição de tarefa: Concluir Não Antes De'
description: Concluir não antes de (FNET) é uma Restrição de Tarefa que agenda uma tarefa para ser concluída após a data especificada.
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Visão geral da restrição de tarefa: Concluir não antes de

Concluir não antes de (FNET) é uma Restrição de Tarefa que agenda uma tarefa para ser concluída após a data especificada.

## Visão geral da restrição Concluir não é anterior a

Considere o seguinte ao usar a restrição Concluir não anterior a (FNET) para uma tarefa:

* Você deve usar essa restrição quando o projeto for programado a partir da data de conclusão. Nesse caso, você pode fornecer uma restrição suave na tarefa antes de forçar outras tarefas dependentes a serem exibidas em risco.
* Quando você usa o FNET em um projeto agendado **Data inicial**, a restrição agendará a tarefa da maneira que a agendaria se a restrição fosse tão rápida quanto possível.
* Quando você move ou copia uma tarefa com uma restrição FNET para outro projeto, a restrição da tarefa ou as datas do projeto podem ser alteradas dependendo das datas da restrição e das datas de início e conclusão do projeto. Os seguintes cenários existem:

   * Quando o projeto de destino é agendado desde o início:

      * Quando a data de restrição da tarefa é anterior à Data Inicial Planejada do projeto, a restrição da tarefa é alterada para Assim que possível.
      * Quando a data de restrição da tarefa é posterior à Data de Conclusão Planejada do projeto, a Data de Conclusão Planejada do projeto muda para corresponder à data de restrição de conclusão da tarefa.
   * Quando o projeto de destino é agendado a partir da conclusão:

      * Quando a data de restrição da tarefa for posterior à Data de conclusão do projeto, a restrição da tarefa será alterada para O mais tarde possível.
      * Quando a data de restrição da tarefa é anterior à Data Inicial Planejada do projeto, a Data Inicial Planejada do projeto muda para corresponder à data de restrição inicial da tarefa.
   * Independentemente da programação do projeto, quando a data de restrição da tarefa estiver dentro das Datas de Início e Conclusão do projeto, não há alterações na Restrição de Tarefa ou nas datas do projeto.

   Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md). Para obter informações sobre cópia de tarefas, consulte [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

   Para obter informações sobre como atualizar a Restrição de Tarefa em uma tarefa, consulte [Atualizar a Restrição de Tarefa de uma tarefa](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Finish No Earlier Than constraint</h2>
<p>(NOTE: replaced with new article linked above)&nbsp;</p>
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
