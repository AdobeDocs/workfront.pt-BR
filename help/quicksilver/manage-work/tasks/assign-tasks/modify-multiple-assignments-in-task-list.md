---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modificar várias atribuições de usuário em uma lista de tarefas
description: Ao gerenciar atribuições de tarefas, você pode modificá-las simultaneamente para várias tarefas de cada vez usando o recurso de edição em massa em uma lista de tarefas.
author: Alina
feature: Work Management
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 0%

---

# Modificar várias atribuições de usuário em uma lista de tarefas

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Ao gerenciar atribuições de tarefas, você pode modificá-las simultaneamente para várias tarefas de cada vez usando o recurso de edição em massa em uma lista de tarefas.

Este artigo se refere à modificação de várias atribuições de usuário para várias tarefas em uma lista de tarefas. Consulte também os seguintes artigos para modificar atribuições em várias tarefas em outras áreas:

* Para obter informações sobre a atribuição de tarefas usando o Balanceador de Carga de Trabalho, consulte [Visão Geral da atribuição de trabalho no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Para obter informações sobre como atribuir uma tarefa a um recurso em uma lista, consulte [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos e Tarefas</p> <p>Visualizar ou acessar mais alto os usuários</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir ou aumentar permissões para tarefas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

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

1. Vá para a lista que contém as tarefas em que deseja modificar atribuições.
1. (Opcional) Crie um filtro para exibir somente as tarefas atribuídas ao destinatário que você deseja modificar.

   Por exemplo, se o projeto contiver uma função específica como o destinatário padrão de várias tarefas, você poderá criar um filtro para exibir somente as tarefas com essa função como o destinatário. Em seguida, é possível substituir a função por um usuário específico.

   Para obter informações sobre como criar um filtro, consulte [Criar ou editar filtros](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Para filtrar em uma função, selecione **Funções de Atribuição**, depois clique em **ID**.

   >[!TIP]
   >
   >Não utilize o **Atribuído a** campo. Isso localiza somente o Proprietário Principal da tarefa em vez de qualquer uma das funções que poderiam ser atribuídas a ele.

   Ou

   Para filtrar um usuário, selecione **Usuários da Atribuição,** em seguida, clique em **ID.**

   >[!TIP]
   >
   >Não utilize o **Atribuído a** campo. Isso encontra somente o Proprietário principal da tarefa em vez de qualquer um dos usuários que poderiam ser atribuídos a eles.

1. Selecione as tarefas para as quais deseja modificar atribuições e clique no botão **Editar** ícone ![](assets/edit-icon.png).

   A página Editar Tarefas é exibida. Os itens editados são exibidos no canto superior esquerdo da página.

1. Vá para o **Atribuições** seção.
1. Siga um destes procedimentos para adicionar ou remover destinatários:

   >[!IMPORTANT]
   >
   >A remoção de destinatários pode afetar as horas da tarefa e as porcentagens de alocação. Para obter mais informações, consulte a seção [Como a remoção de destinatários afeta as horas da tarefa e as porcentagens de alocação](#how-removing-assignees-affects-task-hours-and-allocation-percentages) neste artigo.

   * Para adicionar um novo destinatário:

      1. No **Atribuições** seção , selecione **Destinatário**.

         As informações comuns em todas as tarefas selecionadas são exibidas. Por exemplo, se o mesmo usuário for atribuído a todas as tarefas, esse usuário será exibido no **Destinatário** coluna. Se as informações não forem comuns nas tarefas selecionadas, nenhuma informação será exibida.

      1. Comece a digitar o nome de um usuário, função ou equipe e selecione-o quando for exibido na lista. A atribuição é adicionada e não substitui as atribuições atuais nas tarefas selecionadas.
      >[!TIP]
      >
      > * Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários ativos, funções de trabalho e equipes.
      >   
      > * Ao adicionar uma atribuição de usuário, observe o avatar, a Função primária do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la à medida que você os adiciona.

         > 
         >   Se um usuário, uma função de trabalho ou uma equipe tiver sido atribuída antes de ser desativada, ela permanecerá atribuída ao item de trabalho. Nesse caso, recomendamos o seguinte:
         >   
         >     * Atribua novamente o item de trabalho aos recursos ativos.
         >     * Associe os usuários em uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.



   * Para remover destinatários individuais:

      1. Clique no botão **Ícone X** ao lado do nome do destinatário que você deseja remover se o destinatário for exibido na lista Atribuições.

         Ou

         (Condicional) Se o destinatário que você deseja remover não for exibido na seção Atribuições porque o destinatário está atribuído a apenas algumas das tarefas que você selecionou, clique em **Remover Destinatário** e comece a digitar o nome do destinatário que deseja remover, em seguida, clique no nome quando ele for exibido na lista suspensa.
   * Para remover todos os destinatários existentes:

      1. Clique em **Remover todos os destinatários existentes**, depois clique em **Sim, Excluir Todos os Atributos**.

         Isso remove não apenas os destinatários comuns (destinatários que são exibidos na caixa de diálogo de edição), mas também todos os destinatários em todas as tarefas selecionadas.
      A remoção de usuários de tarefas pode afetar as horas da tarefa e as porcentagens de alocação.

      Para obter mais informações, consulte [Visão geral da modificação de atribuições de tarefa](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).





1. (Opcional) Modifique qualquer uma das seguintes opções para destinatários:

   * (Condicional) **Alocação % ou Horas**: Especifique uma nova porcentagem ou horas de alocação.

      >[!NOTE]
      >
      >Essa opção pode ser modificada somente se o Tipo de duração for o mesmo em todas as tarefas que estão sendo editadas. Quando o Tipo de duração é Trabalho calculado ou Impulsionado por esforço, você pode atualizar a % de alocação. Quando o Tipo de duração é Simples, você pode atualizar as Horas. Para obter informações sobre Tipo de duração, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      Se o campo estiver em branco, significa que o valor é diferente entre tarefas; no entanto, você ainda poderá modificá-lo.

   * **Proprietário da Tarefa**: Selecione essa opção para tornar o destinatário o proprietário da tarefa para todas as tarefas que estão sendo editadas.
   * **Função do destinatário**: Selecione uma função na lista suspensa. Se não for selecionada, o Adobe Workfront selecionará automaticamente a Função primária do usuário.

1. Clique em **Salvar alterações.**
