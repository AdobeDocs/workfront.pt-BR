---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modificar atribuições de vários usuários em uma lista de tarefas
description: Ao gerenciar atribuições de tarefas, você pode modificá-las simultaneamente para várias tarefas de uma vez usando o recurso de edição em massa em uma lista de tarefas.
author: Alina
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---

# Modificar atribuições de vários usuários em uma lista de tarefas

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Ao gerenciar atribuições de tarefas, você pode modificá-las simultaneamente para várias tarefas de uma vez usando o recurso de edição em massa em uma lista de tarefas.

Este artigo se refere à modificação de várias atribuições de usuário para várias tarefas em uma lista de tarefas. Consulte também os seguintes artigos para modificar atribuições em várias tarefas em outras áreas:

* Para obter informações sobre como atribuir tarefas usando o Balanceador de carga de trabalho, consulte [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Para obter informações sobre atribuir uma tarefa a um recurso em uma lista, consulte [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalhar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos e tarefas</p> <p>Acesso de visualização ou superior aos usuários</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões ou mais altas para tarefas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

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
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration&nbsp;Types:</p>
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


1. Para filtrar uma função, selecione **Funções das atribuições** e, em seguida, clique em **ID**.

   >[!TIP]
   >
   >Não use o **Atribuído a** campo. Localiza somente o Proprietário principal da tarefa, em vez de qualquer uma das funções que podem ser atribuídas a ele.

   Ou

   Para filtrar um usuário, selecione **Usuários Atribuídos,** e clique em **ID.**

   >[!TIP]
   >
   >Não use o **Atribuído a** campo. Localiza somente o Proprietário principal da tarefa, em vez de qualquer um dos usuários que podem ser atribuídos a ele.

1. Selecione as tarefas para as quais deseja modificar atribuições e clique no botão **Editar** ícone ![](assets/edit-icon.png).

   A página Editar Tarefas é exibida. Os itens editados são exibidos no canto superior esquerdo da página.

1. Vá para a **Atribuições** seção.
1. Siga um destes procedimentos para adicionar ou remover responsáveis:

   >[!IMPORTANT]
   >
   >A remoção de atribuídos pode afetar as horas da tarefa e as porcentagens de alocação. Para obter mais informações, consulte a seção [Como a remoção de atribuídos afeta as horas da tarefa e as porcentagens de alocação](#how-removing-assignees-affects-task-hours-and-allocation-percentages) neste artigo.

   * Para adicionar um novo destinatário:

      1. No **Atribuições** , selecione **Destinatário**.

         As informações comuns em todas as tarefas selecionadas são exibidas. Por exemplo, se o mesmo usuário for atribuído a todas as tarefas, ele será exibido na **Destinatário** coluna. Se as informações não forem comuns nas tarefas selecionadas, nenhuma informação será exibida.

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

      1. Clique em **Ícone X** ao lado do nome do designado que você deseja remover se ele for exibido na lista Atribuições.

         Ou

         (Condicional) Se o destinatário que você deseja remover não for exibido na seção Atribuições porque o destinatário está atribuído a apenas algumas das tarefas selecionadas, clique em **Remover atribuidor** e comece digitando o nome do destinatário que deseja remover, em seguida, clique no nome quando ele aparecer na lista suspensa.

   * Para remover todos os designados existentes:

      1. Clique em **Remover todos os atribuídos existentes** e, em seguida, clique em **Sim, excluir todos os atribuídos**.

         Isso remove não somente os atribuídos comuns (atribuídos exibidos na caixa de diálogo de edição), mas também todos os atribuídos em todas as tarefas selecionadas.

     Remover usuários das tarefas pode afetar as horas da tarefa e as porcentagens de alocação.

     Para obter mais informações, consulte [Visão geral da modificação de atribuições de tarefas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. (Opcional) Modifique qualquer uma das seguintes opções para os designados:

   * (Condicional) **% de Alocação ou Horas**: especifique uma nova porcentagem de alocação ou horas.

     >[!NOTE]
     >
     >Essa opção só poderá ser modificada se o Tipo de Duração for o mesmo em todas as tarefas que estão sendo editadas. Quando o Tipo de Duração for Trabalho Calculado ou Orientado pelo Esforço, você poderá atualizar a Alocação %. Quando o Tipo de duração é Simples, você pode atualizar as Horas. Para obter informações sobre o Tipo de duração, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     Se o campo estiver em branco, significa que o valor é diferente nas tarefas; no entanto, você ainda poderá modificá-lo.

   * **Proprietário da tarefa**: selecione essa opção para tornar o destinatário o proprietário da tarefa para todas as tarefas que estão sendo editadas.
   * **Função do atribuidor**: selecione uma função na lista suspensa. Se não for selecionada, o Adobe Workfront selecionará automaticamente a função principal do usuário.

1. Clique em **Salvar alterações.**
