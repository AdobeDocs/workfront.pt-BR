---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão Geral Da Restrição De Tarefa: Não Iniciar Antes De'
description: Use a Restrição de Tarefa Iniciar Não Antes de (SNET) para programar uma tarefa para iniciar após a data especificada.
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
TQID: https://experienceleague.adobe.com/2YS0JaxRwYAAN5ZqNzPO7kGyQ876UlJ5b-X4MY4bT6c
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 492
ht-degree: 1%

---

# Visão geral de restrição de tarefa: não iniciar antes de

Use a Restrição de Tarefa Iniciar Não Antes de (SNET) para programar uma tarefa para iniciar após a data especificada.

## Visão Geral da Restrição Iniciar Não Antes da Tarefa

Considere o seguinte ao usar a Restrição Não Iniciar Antes da Tarefa:

* Você deve usar a restrição Não iniciar antes de quando o projeto estiver programado a partir da data inicial. Nesse caso, você pode fornecer uma restrição leve em uma tarefa antes que ela force outras tarefas dependentes a serem exibidas como Em Risco.
* Não Iniciar Antes de É a restrição padrão se um projeto estiver agendado A Partir da Data Inicial e se a data inicial padrão do sistema ou grupo para uma nova tarefa estiver definida como Hoje. Para obter informações sobre como configurar padrões para tarefas, consulte [Configurar preferências de tarefas e problemas do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Se você programar a Data Inicial Inicial Inicial do Projeto e a data inicial padrão do sistema para uma nova tarefa for definida como Baseado na Data Planejada do Projeto, a restrição padrão para uma nova tarefa será O Mais Breve Possível.
* Se você programar o projeto A Partir da Data de Conclusão e a data inicial padrão do sistema para uma nova tarefa for definida como Hoje, a restrição Iniciar Não Antes de Que agendará a tarefa como seria uma tarefa O Mais Tarde Possível.
* Quando você move ou copia uma tarefa com uma restrição SNET para outro projeto, a restrição da tarefa ou as datas do projeto podem mudar dependendo de quais são as datas de restrição e quais são as datas de início e conclusão do projeto. Existem os seguintes cenários:

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
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Earlier Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
