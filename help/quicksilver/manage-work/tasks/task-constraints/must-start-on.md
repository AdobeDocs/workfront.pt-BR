---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão Geral De Restrição De Tarefa: Deve Iniciar Em'
description: Use a Restrição de Tarefa Obrigatória Iniciar em (MSO) para programar uma tarefa para iniciar exatamente em uma data específica.
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Visão geral de Restrição de Tarefa: Deve Iniciar em

Use a Restrição de Tarefa Obrigatória Iniciar em (MSO) para programar uma tarefa para iniciar exatamente em uma data específica.

A restrição Deve Iniciar em programa uma tarefa para iniciar exatamente na hora e data que você especificar no campo **Data de Início Planejada**.

>[!TIP]
>
>A atualização manual da Data Inicial Planejada de uma tarefa altera a restrição da tarefa para Deve Iniciar em.

## Visão Geral da Restrição Deve Iniciar na Tarefa

Considere o seguinte ao programar uma tarefa com uma restrição Deve iniciar em:

* As relações de predecessoras não forçam essa tarefa a ser reagendada. O Workfront ignora basicamente qualquer relação predecessora da tarefa com essa restrição.
* A tarefa mostra **Em Risco** se os predecessores começarem a ser executados atrasados ou atrasados.

* Quando você move ou copia uma tarefa com uma restrição MSO para outro projeto, a restrição da tarefa ou as datas do projeto podem mudar dependendo de quais são as datas de restrição e quais são as datas de início e de conclusão do projeto. Existem os seguintes cenários:

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
<h2>Use the Must Start On Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Must Start On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Start On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start by this date, and no later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
