---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modificar Várias Atribuições de Usuário em uma Lista de Tarefas
description: Ao gerenciar atribuições de tarefas, você pode modificá-las simultaneamente para várias tarefas de uma vez usando o recurso de edição em massa em uma lista de tarefas.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 3%

---

# Modificar atribuições de vários usuários em uma lista de tarefas

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).  

</div>-->

Ao gerenciar atribuições de tarefas, você pode modificá-las simultaneamente para várias tarefas de uma vez usando o recurso de edição em massa em uma lista de tarefas.

Este artigo se refere à modificação de várias atribuições de usuário para várias tarefas em uma lista de tarefas. Consulte também os seguintes artigos para modificar atribuições em várias tarefas em outras áreas:

* Para obter informações sobre como atribuir tarefas usando o Balanceador de carga de trabalho, consulte [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Para obter informações sobre como atribuir uma tarefa a um recurso em uma lista, consulte [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p>
   <p>Trabalho ou maior</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos e tarefas</p> <p>Acesso de visualização ou superior aos usuários</p> </td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td>
   <td>Contribute ou tenha permissões mais altas para as tarefas</td>
  </tr>
 </tbody>
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Modificar atribuições para várias tarefas

1. Vá para a lista que contém as tarefas nas quais você deseja modificar as atribuições.
1. (Opcional) Crie um filtro para exibir somente as tarefas atribuídas ao destinatário que você deseja modificar.

   Por exemplo, se o seu projeto contiver uma função específica como o destinatário padrão para várias tarefas, você poderá criar um filtro para exibir somente tarefas com essa função como o destinatário. Em seguida, você pode substituir a função por um usuário específico.

   Para obter informações sobre como criar um filtro, consulte [Criar ou editar filtros](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Para filtrar uma função, selecione **Funções de atribuição** e clique em **ID**.

   >[!TIP]
   >
   >Não use o campo **Atribuído a**. Localiza somente o Proprietário principal da tarefa, em vez de qualquer uma das funções que podem ser atribuídas a ele.

   Ou

   Para filtrar por um usuário, selecione **Usuários de Atribuição,** e clique em **ID.**

   >[!TIP]
   >
   >Não use o campo **Atribuído a**. Localiza somente o Proprietário principal da tarefa, em vez de qualquer um dos usuários que podem ser atribuídos a ele.

1. Selecione as tarefas para as quais deseja modificar atribuições e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png).

   1. Para adicionar ou remover responsáveis, siga um destes procedimentos:

      * Para adicionar responsáveis, comece digitando o nome de um responsável no campo **Pesquisar pessoas, funções ou equipes** e, em seguida, selecione-os quando eles forem exibidos na lista.

        O novo destinatário é adicionado aos existentes nas tarefas selecionadas.
      * Para remover responsáveis, clique no nome de um responsável na caixa **Remover responsável**

        Ou

        Clique em **Remover todos os atribuídos existentes**.

        Os responsáveis são removidos de todas as tarefas selecionadas.

        Remover usuários das tarefas pode afetar as horas da tarefa e as porcentagens de alocação.

        Para obter mais informações, consulte [Visão geral da modificação de atribuições de tarefas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).


        >[!TIP]
        >
        >* Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos.
        >   
        >* Ao adicionar uma atribuição de usuário, observe o avatar, a função principal do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados. Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
        > 
        >   Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
        >   
        >* Reatribuir o item de trabalho aos recursos ativos.
        >* Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.


   1. (Opcional) Modifique qualquer uma das seguintes opções para os designados:

      * (Condicional) **Percentual de Alocação ou Horas**: especifique uma nova porcentagem de alocação ou horas.

      >[!NOTE]
      >
      >Essa opção só poderá ser modificada se o Tipo de Duração for o mesmo em todas as tarefas que estão sendo editadas. Quando o Tipo de Duração for Trabalho Calculado ou Orientado pelo Esforço, você poderá atualizar a Alocação %. Quando o Tipo de duração é Simples, você pode atualizar as Horas. Para obter informações sobre o Tipo de Duração, consulte [Visão Geral da Duração e do Tipo de Duração da Tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      >
      >
      >Se o campo estiver em branco, significa que o valor é diferente nas tarefas; no entanto, você ainda poderá modificá-lo.

      * **Tornar Primário**: passe o mouse sobre as tarefas selecionadas e selecione esta opção para tornar o destinatário o proprietário da tarefa para todas as tarefas que estão sendo editadas.
      * **Função do destinatário**: selecione uma função na lista suspensa. Se não for selecionada, o Adobe Workfront selecionará automaticamente a função principal do usuário.
      * **Tipo de Duração**
      * **Duração**
      * **Horas planejadas**

   1. Clique em **Salvar**.

<!-- temporary content - for Assignments redesign:

Editing assignments on tasks differs depending on which environment you choose. 

1. (Conditional) If you are using the Production environment to assign tasks, the **Edit Tasks** box opens in the new experience. Do the following in the Production environment: 

   1. To add or remove assignees, do one of the following:

      * To add assignees, start typing the name of an assignee in the **Search people, roles, or teams** field, then select them when they display in the list. 
      * To remove assignees, click the **x** icon to the right of their name. Only assignees that are common to all tasks display in the list. 
      * Click Assign to me to assign the selected tasks to yourself.

   1. (Conditional) When using the new experience, click **Save**.

   1. (Optional) Click **Switch to old experience** at the bottom of the **Edit Tasks** box.
      
      The **Edit Tasks** box opens in the old experience.

   1. (Conditional) In the old experience, do the following to modify the assignees:

      1. Go to the **Assignments** section.

         >[!IMPORTANT]
         >
         >Removing assignees can affect the task hours and allocation percentages. For more information, see the section [How removing assignees affects task hours and allocation percentages](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in this article.

      1. Do one of the following to add or remove assignees:

         * To add a new assignee:

            1. In the **Assignments** section, select **Assignee**.

               Information that is common across all tasks selected displays. For example, if the same user is assigned to all tasks, that user displays in the **Assignee** column. If information is not common across the tasks selected, no information displays.
            
            1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected tasks.

            >[!TIP]
            >
            > * You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
            >   
            > * When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them. You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
            > 
            >   If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
            >   
            >     * Reassign the work item to active resources.
            >     * Associate the users in a deactivated team with an active team and reassign the work item to the active team.


         * To remove individual assignees:

            1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.

               Or

               (Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the tasks that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.

         * To remove all existing assignees:

            1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.

               This removes not only common assignees (assignees that are displayed in the edit dialog box), but also all assignees on all the selected tasks.

            Removing users from tasks can affect task hours and allocation percentages.
            
            For more information, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

      1. (Optional) Modify any of the following options for assignees:

         * (Conditional) **Allocation % or Hours**: Specify a new allocation percentage or hours.

         >[!NOTE]
         >
         >This option can be modified only if the Duration Type is the same across all tasks that are being edited. When the Duration Type is Calculated Work or Effort Driven you can update the Allocation %. When the Duration Type is Simple you can update the Hours. For information about Duration Type, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
         >
         >
         >If the field is blank, this means that the value is different across tasks; however, you are still able to modify it.

         * **Task Owner**: Select this option to make the assignee the owner of the task for all tasks being edited.
         * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Adobe Workfront automatically selects the Primary Role of the user. 

      1. Click **Save Changes.**
        

1. <span class="preview">(Conditional) If you are using the Preview environment to assign tasks, the **Edit Tasks** box opens. Do the following in the Preview environment: </span>

   <div class="preview">-->





