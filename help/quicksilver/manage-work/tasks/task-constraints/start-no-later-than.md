---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão Geral Da Restrição De Tarefa: Não Iniciar Depois De'
description: Não Iniciar Depois de (SNLT) é uma Restrição de Tarefa que programa uma tarefa para ser iniciada antes da data especificada.
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
TQID: https://experienceleague.adobe.com/eX2KAzQkOb0AmYcR5Zc6SPeySBTDKjM74QYi7ox4A0w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 436
ht-degree: 1%

---

# Visão geral de restrição de tarefa: não iniciar depois de

Não Iniciar Depois de (SNLT) é uma Restrição de Tarefa que programa uma tarefa para ser iniciada antes da data especificada.

Considere o seguinte ao trabalhar com a restrição SNLT:

* Você deve usar a restrição Iniciar não mais tarde do que quando o projeto estiver agendado a partir da data de conclusão. Nesse caso, você pode fornecer uma restrição leve em uma tarefa antes que ela force outras tarefas dependentes a serem exibidas como Em Risco.
* Não Iniciar Depois de É a restrição padrão se um projeto usar um modo de programação de Programação a partir da Data de Conclusão e o padrão do sistema ou grupo para a Data de Início de uma tarefa for Hoje. Para obter informações sobre onde definir a Restrição padrão para uma nova tarefa, consulte [Configurar preferências de tarefas e problemas do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Quando você usa a restrição SNLT com um projeto Programar da Data Inicial, o Adobe Workfront programa a tarefa da mesma maneira que uma tarefa O Mais Breve Possível.
* Quando você move ou copia uma tarefa com uma restrição SNLT para outro projeto, a restrição da tarefa ou as datas do projeto podem mudar dependendo de quais são as datas de restrição e quais são as datas de início e de conclusão do projeto. Existem os seguintes cenários:

   * Quando o projeto de destino está agendado do início:

      * Quando a data de restrição da tarefa for anterior à Data de início planejada do projeto, a restrição da tarefa será alterada para O Mais Breve Possível.
      * Quando a data de restrição da tarefa for posterior à Data de Conclusão Planejada do projeto, a Data de Conclusão Planejada do projeto será alterada para corresponder à data de restrição da conclusão da tarefa.

      * Quando o projeto de destino estiver agendado A partir da conclusão:

         * Quando a data de restrição da tarefa for posterior à Data de conclusão do projeto, a restrição da tarefa será alterada para O mais tarde possível.
         * Quando a data de restrição da tarefa for anterior à Data Inicial Planejada do projeto, a Data Inicial Planejada do projeto será alterada para corresponder à data inicial de restrição da tarefa.

      * Independentemente do cronograma do projeto, quando a data de restrição da tarefa estiver dentro das datas de início e conclusão do projeto, não há alterações na restrição da tarefa ou nas datas do projeto.

  Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

  Para obter informações sobre como copiar tarefas, consulte [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obter informações sobre como atualizar a Restrição de Tarefa em uma tarefa, consulte [Atualizar a Restrição de Tarefa de uma tarefa](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Start No Later Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Later Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>.<br></li>
</ol>
</div>
-->
