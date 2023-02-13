---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão geral da restrição de tarefa: Iniciar Não Mais Tarde Que'
description: Iniciar Não Mais Tarde que (SNLT) é uma Restrição de Tarefa que agenda uma tarefa para iniciar antes da data especificada.
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Visão geral da restrição de tarefa: Iniciar Não Mais Tarde

Iniciar Não Mais Tarde que (SNLT) é uma Restrição de Tarefa que agenda uma tarefa para iniciar antes da data especificada.

Considere o seguinte ao trabalhar com a restrição SNLT:

* Você deve usar a restrição Iniciar não mais tarde do que quando o projeto for programado a partir da data de conclusão. Nesse caso, você pode fornecer uma restrição suave em uma tarefa antes que ela force outras tarefas dependentes a serem exibidas como Em Risco.
* Iniciar não mais tarde do que é a restrição padrão se um projeto usar um modo de programação de Programação a partir da data de conclusão e o padrão do sistema ou grupo para a Data inicial de uma tarefa for Hoje. Para obter informações sobre onde definir a Restrição padrão para uma nova tarefa, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Quando você usa a restrição SNLT com um projeto de Data Inicial da Programação, o Adobe Workfront agenda a tarefa como uma tarefa o Mais rápido possível.
* Ao mover ou copiar uma tarefa com uma restrição SNLT para outro projeto, a restrição da tarefa ou as datas do projeto podem mudar, dependendo das datas de restrição e das datas de início e conclusão do projeto. Os seguintes cenários existem:

   * Quando o projeto de destino é agendado desde o início:

      * Quando a data de restrição da tarefa é anterior à Data Inicial Planejada do projeto, a restrição da tarefa é alterada para Assim que possível.
      * Quando a data de restrição da tarefa é posterior à Data de Conclusão Planejada do projeto, a Data de Conclusão Planejada do projeto muda para corresponder à data de restrição de conclusão da tarefa.

      * Quando o projeto de destino é agendado a partir da conclusão:

         * Quando a data de restrição da tarefa for posterior à Data de conclusão do projeto, a restrição da tarefa será alterada para O mais tarde possível.
         * Quando a data de restrição da tarefa é anterior à Data Inicial Planejada do projeto, a Data Inicial Planejada do projeto muda para corresponder à data de restrição inicial da tarefa.
      * Independentemente da programação do projeto, quando a data de restrição da tarefa estiver dentro das Datas de Início e Conclusão do projeto, não há alterações na Restrição de Tarefa ou nas datas do projeto.

   Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

   Para obter informações sobre cópia de tarefas, consulte [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

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
