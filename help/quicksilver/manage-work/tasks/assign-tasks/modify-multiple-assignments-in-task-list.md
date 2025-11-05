---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modificar Várias Atribuições de Usuário em uma Lista de Tarefas
description: Ao gerenciar atribuições de tarefas, você pode modificá-las simultaneamente para várias tarefas de uma vez usando o recurso de edição em massa em uma lista de tarefas.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# Modificar atribuições de vários usuários em uma lista de tarefas

<!--Audited: 11/2025-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Ao gerenciar atribuições de tarefas, você pode modificá-las simultaneamente para várias tarefas de uma vez usando o recurso de edição em massa em uma lista de tarefas.

Este artigo se refere à modificação de várias atribuições de usuário para várias tarefas em uma lista de tarefas. Consulte também os seguintes artigos para modificar atribuições em várias tarefas em outras áreas:

* Para obter informações sobre como atribuir tarefas usando o Balanceador de carga de trabalho, consulte [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Para obter informações sobre como atribuir uma tarefa a um recurso em uma lista, consulte [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td> <p>Standard</p>
   <p>Trabalhar ou superior</p>
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

1. Selecione as tarefas para as quais deseja modificar atribuições e clique no ícone **Editar** ![](assets/edit-icon.png).

   A caixa **Editar Tarefas** abre <!--<span class="preview">in the new experience</span>-->.

   <!--1. <span class="preview">(Optional) Click **Switch to old experience** at the bottom of the **Edit Tasks** box.</span> 
   <span class="preview">The **Edit Tasks** box opens in the old experience.</span>-->

1. Vá para a seção **Atribuições**.

   >[!IMPORTANT]
   >
   >A remoção de atribuídos pode afetar as horas da tarefa e as porcentagens de alocação. Para obter mais informações, consulte a seção [Como a remoção de atribuídos afeta as horas da tarefa e as porcentagens de alocação](#how-removing-assignees-affects-task-hours-and-allocation-percentages) neste artigo.
1. Siga um destes procedimentos para adicionar ou remover responsáveis:

   * Para adicionar um novo destinatário:

      1. Na seção **Atribuições**, selecione **Atribuído**.

         As informações comuns em todas as tarefas selecionadas são exibidas. Por exemplo, se o mesmo usuário for atribuído a todas as tarefas, ele será exibido na coluna **Atribuído**. Se as informações não forem comuns nas tarefas selecionadas, nenhuma informação será exibida.

      1. Comece a digitar o nome de um usuário, função ou equipe e selecione-o quando ele for exibido na lista. A atribuição é adicionada e não substitui as atribuições atuais nas tarefas selecionadas.


     >[!TIP]
     >
     > * Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos.
     >   
     > * Ao adicionar uma atribuição de usuário, observe o avatar, a função principal do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados. Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
     >   
     >     * Reatribuir o item de trabalho aos recursos ativos.
     >     * Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.


   * Para remover designados individuais:

      1. Clique no ícone **X** ao lado do nome do destinatário que você deseja remover se ele for exibido na lista Atribuições.

         Ou

         (Condicional) Se o destinatário que você deseja remover não for exibido na seção Atribuições porque o destinatário está atribuído a apenas algumas das tarefas que você selecionou, clique em **Remover destinatário** e comece a digitar o nome do destinatário que você deseja remover, em seguida, clique no nome quando ele aparecer na lista suspensa.

   * Para remover todos os designados existentes:

      1. Clique em **Remover todos os atribuídos existentes** e em **Sim, Excluir todos os atribuídos**.

         Isso remove não somente os atribuídos comuns (atribuídos exibidos na caixa de diálogo de edição), mas também todos os atribuídos em todas as tarefas selecionadas.

     Remover usuários das tarefas pode afetar as horas da tarefa e as porcentagens de alocação.

     Para obter mais informações, consulte [Visão geral da modificação de atribuições de tarefas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. (Opcional) Modifique qualquer uma das seguintes opções para os designados:

   * (Condicional) **Percentual de Alocação ou Horas**: especifique uma nova porcentagem de alocação ou horas.

     >[!NOTE]
     >
     >Essa opção só poderá ser modificada se o Tipo de Duração for o mesmo em todas as tarefas que estão sendo editadas. Quando o Tipo de Duração for Trabalho Calculado ou Orientado pelo Esforço, você poderá atualizar a Alocação %. Quando o Tipo de duração é Simples, você pode atualizar as Horas. Para obter informações sobre o Tipo de Duração, consulte [Visão Geral da Duração e do Tipo de Duração da Tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     >Se o campo estiver em branco, significa que o valor é diferente nas tarefas; no entanto, você ainda poderá modificá-lo.

   * **Proprietário da tarefa**: selecione essa opção para tornar o destinatário o proprietário da tarefa para todas as tarefas que estão sendo editadas.
   * **Função do destinatário**: selecione uma função na lista suspensa. Se não for selecionada, o Adobe Workfront selecionará automaticamente a função principal do usuário.

1. Clique em **Salvar alterações.**

<!--
1. <span class="preview"> (Optional) Click **Try new experience** in the upper-right corner of the **Edit Tasks** box. The Edit Tasks box opens in the new experience. Do one of the following:</span>

   <div class="preview">

   * To add assignees, start typing the name of an assignee in the **Search people, roles, or teams** field, then select them when they display in the list. 
   * To remove assignees, click the **x** icon to the right of their name. Only assignees that are common to all tasks display in the list. 
   * Click Assign to me to assign the selected tasks to yourself.

   </div>
1. <span class="preview">(Conditional) When using the new experience, click **Save**.</span>

-->
