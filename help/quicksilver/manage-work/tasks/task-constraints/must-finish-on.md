---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão Geral Da Restrição Da Tarefa: Deve Terminar Em'
description: Você pode usar a Restrição de Tarefa Deve Terminar em (MFO) para programar uma tarefa para terminar em uma data específica.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
TQID: https://experienceleague.adobe.com/qo-JdIbfFijhpa7-kI22hYe7gZ6DvJb8e2ycBiKTU7I
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 395
ht-degree: 1%

---

# Visão geral de restrição de tarefa: deve terminar em

Você pode usar a Restrição de Tarefa Deve Terminar em (MFO) para programar uma tarefa para terminar em uma data específica.

A restrição Deve Terminar Em programa uma tarefa para terminar exatamente na hora e data que você especificar no campo **Data de Conclusão Planejada**.

>[!TIP]
>
>A atualização manual da Data de conclusão planejada de uma tarefa altera a restrição da tarefa para Precisa ser concluída em.

## Visão Geral da Restrição Deve Ser Concluída na Tarefa

Considere o seguinte ao programar uma tarefa com uma restrição Deve ser concluída em:

* As relações de predecessoras não forçam a tarefa a ser reagendada. O Adobe Workfront ignora essencialmente as relações predecessoras.
* A tarefa será exibida como **Em Risco** se os predecessores começarem a ser executados atrasados ou estiverem atrasados.

* Quando você move ou copia uma tarefa com uma restrição MFO para outro projeto, a restrição da tarefa ou as datas do projeto podem mudar dependendo de quais são as datas de restrição e quais são as datas de início e de conclusão do projeto. Existem os seguintes cenários:

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
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
