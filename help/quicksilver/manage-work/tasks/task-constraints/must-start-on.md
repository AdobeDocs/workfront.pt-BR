---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão geral da restrição de tarefa: Deve Iniciar Em'
description: Use a Restrição de Tarefa Deve Iniciar em (MSO) para agendar uma tarefa para iniciar exatamente em uma data específica.
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Visão geral da restrição de tarefa: Deve Iniciar em

Use a Restrição de Tarefa Deve Iniciar em (MSO) para agendar uma tarefa para iniciar exatamente em uma data específica.

A restrição Deve iniciar em agenda uma tarefa para iniciar exatamente na hora e na data especificadas na **Data de início planejada** campo.

>[!TIP]
>
>A atualização manual da Data de início planejada de uma tarefa altera a restrição da tarefa para Deve iniciar em.

## Visão Geral da Restrição de Tarefa Deve Iniciar

Considere o seguinte ao agendar uma tarefa com uma restrição Deve Iniciar em:

* As relações antecessoras não forçam a reprogramação desta tarefa. A Workfront ignora basicamente qualquer relacionamento antecessor da tarefa com essa restrição.
* A tarefa não mostra **Em Risco** se os antecessores começarem a ficar para trás ou atrasados.

* Ao mover ou copiar uma tarefa com uma restrição MSO para outro projeto, a restrição da tarefa ou as datas do projeto podem mudar, dependendo das datas de restrição e das datas de início e conclusão do projeto. Os seguintes cenários existem:

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
