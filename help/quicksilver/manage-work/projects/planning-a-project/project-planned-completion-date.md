---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Definir a data de conclusão do projeto
description: A data de conclusão planejada de um projeto é a data pela qual o projeto está definido para ser concluído.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 996398c5-de92-445e-8e86-36b2efdcf6b5
source-git-commit: fedb0328450896d212081715df4cde7644b169bc
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 1%

---

# Definir a data de conclusão do projeto

<!-- Audited: 4/2025 -->

A data de conclusão planejada de um projeto é a data em que o projeto está definido para ser concluído.

A Início planejada e as datas de conclusão planejadas de um projeto dependem das datas das tarefas do projeto. Este artigo descreve como definir manual ou automaticamente a Data de conclusão planejada de um projeto. Para obter mais informações sobre a Data de conclusão planejada de uma tarefa, consulte [Visão geral da Data de conclusão planejada da tarefa](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

A Data de conclusão planejada de um projeto pode ser definida manual ou automaticamente, dependendo se você agenda o projeto a partir do Início ou da Data de conclusão.

## Requisitos de acesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems plano da Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">licença da Adobe Systems Workfront</td> 
   <td><p>
   Novo: Padrão

Ou

Atual: plano </p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do projeto</p> <p>Para obter informações sobre a solicitação de acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Os requisitos de acesso na documentação](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) da Workfront.

+++

## Definir manualmente a data de conclusão planejada de um projeto

Você deve definir manualmente a data de conclusão planejada de um projeto quando agendar o projeto a partir da Data de conclusão.

>[!NOTE]
>
>Quando você define manualmente a Data de conclusão planejada de um projeto, o Workfront calcula automaticamente a Data inicial planejada do projeto com base na Duração de todas as tarefas.


Para programar um projeto a partir da Data de Término:

{{step1-to-projects}}

1. Clique em **Novo projeto** e selecione **Novo projeto** no menu suspenso exibido.

   Para obter mais informações sobre como criar projetos, consulte o artigo [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

1. Selecione **Detalhes do projeto** no painel esquerdo.

1. Clique no ícone **Editar projeto** ![Editar ícone](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) no canto superior direito e selecione **Visão geral** no menu suspenso exibido.

1. Na seção **Datas do projeto**, clique no campo **Modo de Agendamento** e selecione **Data de Conclusão**.

1. Especifique a **data** de conclusão planejada do projeto.
1. Clique em **Salvar alterações**.

   À medida que start adicionar tarefas ao seu projeto, a **Data** de Início Planejada do projeto é calculada com base na duração total de todas as tarefas.

## Definir automaticamente a data de conclusão planejada de um projeto

A Data de conclusão planejada de um projeto é calculada automaticamente pela Workfront quando você agenda o projeto a partir da Data de início. 

Para programar um projeto a partir da Data Inicial:

{{step1-to-projects}}

1. Clique em **Novo projeto** e selecione **Novo projeto** no menu suspenso exibido.

   Para obter mais informações sobre como criar projetos, consulte o artigo [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

1. Selecione **Detalhes do projeto** no painel esquerdo.

1. Clique no **ícone Editar Projeto** Editar ícone![&#128279;](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) no canto superior direito e selecione **Visão geral** no menu suspenso que aparece.

1. Na seção Datas **do** projeto, clique no **campo Modo** de agendamento e selecione **Início data**.

1. Especifique a **data** de Início planejada do projeto.
1. Clique em **Salvar alterações**.

   À medida que start adicionar tarefas ao seu projeto, a **data** de conclusão planejada do projeto é calculada com base na duração total de todas as tarefas.

   Para obter mais informações sobre a Duração da tarefa, consulte a Visão geral da duração e do tipo[&#128279;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) de duração da tarefa.

   A data de conclusão planejada do projeto coincide, neste caso, com a data de conclusão planejada das últimas tarefa no projeto.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>The Planned Completion Date of a task</h2>
<p>(NOTE: drafted because I created a new article, here: /Content/Manage work/Tasks/Task information/task-planned-completion-date.htm)</p>
<p>You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria.&nbsp;</p>
<ul>
<li><a href="#manually-set-the-planned-completion-date-of-a-task" class="MCXref xref">Manually set the Planned Completion Date of a task</a> </li>
<li><a href="#how-the-planned-completion-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Completion Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Completion Date of a task</strong></p>
<p>Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task.&nbsp;</p>
<p>You can manually set the Planned Completion Date&nbsp;when creating a task, as described in&nbsp;the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Completion Date when you select any of the following Task Constraints:&nbsp;</p>
<table border="1" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th> <p><strong>Task Constraint Type</strong> </p> </th>
<th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td>
<td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Completion Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:</p>
<ul>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Completion Date, when the project is scheduled from Completion Date.</li>
<li> <p>The time off schedule of the Primary&nbsp;Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project&nbsp;Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> or <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Completion Date&nbsp;is determined based on the following calculation:&nbsp;</p>
<p><code>Planned Completion Date = Planned Start Date + Duration</code> </p>
<p>For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.</p> <note type="note">
&nbsp;The Update Type for the project must also be&nbsp;set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically&nbsp;adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
