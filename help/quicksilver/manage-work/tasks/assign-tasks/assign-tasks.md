---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Atribuir tarefas
description: É possível atribuir tarefas a usuários, funções ou equipes para indicar quem é responsável por concluir as tarefas. É possível atribuir uma tarefa a mais de um recurso por vez.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1965'
ht-degree: 1%

---

# Atribuir tarefas

{{highlighted-preview}}

>[!IMPORTANT]
>
>O recurso de substituição de taxa de atribuição foi temporariamente desabilitado na Pré-visualização em 30 de junho de 2023.

É possível atribuir tarefas a usuários, funções de trabalho ou equipes para indicar quem é responsável por concluir as tarefas. É possível atribuir uma tarefa a mais de um recurso por vez.

>[!TIP]
>
>Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos.
>
>Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
>
>* Reatribuir o item de trabalho aos recursos ativos.
>* Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.
>

O número de usuários atribuídos a uma tarefa e o agendamento do Proprietário da tarefa podem modificar as datas planejadas de uma tarefa, o que resulta na alteração da linha do tempo do projeto. Para obter informações sobre o impacto da atribuição de vários usuários a uma tarefa, consulte [Visão geral da modificação de atribuições de tarefas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Além deste artigo, recomendamos que você leia os seguintes artigos para obter mais informações sobre atribuição de tarefas:

* [Visão geral da modificação de atribuições de tarefas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Fazer atribuições inteligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Modificar atribuições de vários usuários em uma lista de tarefas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Planejar uma visão geral do projeto](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Visão geral da Data de conclusão planejada da tarefa](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Definir a data de conclusão planejada do projeto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Requisitos de acesso

<!--drafted for P&P - replace table below with this:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View or higher access to Users</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

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
   <td> <p>Editar acesso a projetos e tarefas</p> <p>Acesso de visualização ou superior aos usuários</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões ou mais altas para tarefas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Considerações para várias atribuições para funções de trabalho, equipes e usuários

Considere o seguinte ao atribuir vários recursos a um item de trabalho:

* Os usuários podem ter mais de uma função de trabalho associada ao seu perfil. Para obter informações sobre como associar usuários a funções de trabalho, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Se você atribuir mais de um usuário a uma tarefa ou problema, o primeiro usuário selecionado será designado automaticamente como o proprietário da tarefa ou problema.
Para obter instruções sobre como alterar isso, consulte as informações sobre a opção Tornar primário no artigo [Criar atribuições avançadas](create-advanced-assignments.md).

* Uma equipe não pode ser um responsável primário em uma tarefa ou problema. Somente um usuário ou uma função de trabalho pode ser designada como Principal em uma tarefa ou problema.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* Tarefas e problemas em um projeto podem ser atribuídos primeiro a uma ou mais equipes ou funções de trabalho. Quando o projeto estiver pronto para ser iniciado, talvez também seja necessário atribuí-lo aos usuários:

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>Equipes</td>
   <td>Se você atribuir uma tarefa a uma equipe e também atribuir um usuário, a tarefa permanecerá atribuída à equipe e ao usuário, mesmo que o usuário não seja membro da equipe.</td>
  </tr>
  <tr>
   <td>Funções de trabalho</td>
   <td><p>Se você atribuir uma tarefa ou um problema a uma ou várias funções e também atribuir um usuário, o decide qual função de trabalho deve ser associada ao usuário adicional (se houver) de acordo com as seguintes regras:</p>
     <ul>
      <li>Se houver apenas uma função de trabalho atribuída e ela corresponder à função principal do usuário (configurada em seu perfil), a tarefa ou o problema será atribuído apenas a esse usuário.</li>
      <li>Se várias funções forem atribuídas e pelo menos uma delas corresponder a uma das outras funções do usuário, a tarefa ou problema será atribuído ao usuário (a função é selecionada aleatoriamente se houver várias correspondências), juntamente com quaisquer funções adicionais atribuídas</li>
      <li>Se pelo menos uma função de trabalho for atribuída e não houver correspondência entre as funções de trabalho do usuário, a tarefa ou problema será atribuída à função ou às funções e ao usuário.</li>
     </ul>
   <p>Para obter informações sobre a função principal de um usuário e outras funções, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Editar o perfil de um usuário</a>.</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## Atribuir uma única tarefa

1. Vá para uma tarefa que você deseja atribuir.
1. Clique em **Atribuir a** no **Atribuições** no cabeçalho da tarefa ou problema.

   Ou

   Clique no nome das atribuições se a tarefa ou problema já estiver atribuído.

   ![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. Siga um destes procedimentos:

   * Comece a digitar o nome de um usuário, função ou equipe que deseja atribuir e clique nele quando ele aparecer na lista.


     >[!TIP]
     >
     >Ao adicionar uma atribuição de usuário, observe o avatar, a função principal do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.
     >
     >Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     >
     ><span class="preview">Ao adicionar uma atribuição de função de trabalho, você pode pesquisar a função de trabalho ou o local. Selecione a Função de Trabalho Sistema/Padrão para usar a taxa de cobrança padrão para a atribuição ou selecione uma Função de Trabalho de Cartão de Taxa para usar a taxa de cobrança do cartão de taxa. Para obter mais informações sobre cartões de taxa, consulte [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


   * (Condicional) Clique em um dos nomes na caixa **Atribuições sugeridas** se essa lista for exibida. Para obter mais informações, consulte [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

   * Clique em **Avançado**

     Para obter informações sobre como fazer atribuições avançadas, consulte [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Clique em **Salvar**.
1. (Opcional e condicional) Clique no link **Ícone X** ao lado do nome da atribuição no painel direito da tarefa para remover uma atribuição, se você clicou em **Avançado**.

## Atribuir uma tarefa em uma lista

É possível atribuir tarefas em uma lista ou um relatório quando qualquer um dos campos de atribuições estiver visível na exibição da lista. Essa é uma maneira mais rápida de atribuir tarefas. Este artigo descreve como modificar atribuições de uma tarefa em uma lista. Para obter informações sobre como modificar várias atribuições para várias tarefas em uma lista, consulte [Modificar atribuições de vários usuários em uma lista de tarefas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Dependendo de qual campo estiver visível na exibição, você poderá atribuir as seguintes entidades à tarefa:

| Campo | Entidades atribuídas |
|---|---|
| **Atribuir a** | Atribuir um usuário |
| **Atribuído** | Atribuir um usuário |
| **Atribuições** | Atribuir usuários, funções de trabalho ou equipes |

Para atribuir tarefas em uma lista:

1. Vá para uma lista de tarefas que tenha os campos Assigned To, Assigned, ou Assignments no modo de exibição.
1. (Opcional) Clique no link **Salvamento automático** e selecione uma das seguintes opções:

   | Opção | Descrição da opção |
   |---|---| 
   | Salvamento automático | As alterações feitas nas tarefas são salvas automaticamente e não podem ser revertidas |
   | Salvamento manual | Você deve salvar manualmente as alterações. Você pode reverter suas alterações antes de salvá-las. |
   | Planejamento da linha do tempo | Você deve salvar manualmente as alterações. Você pode reverter suas alterações antes de salvá-las. Salvar as alterações e todas as dependências do projeto é mais rápido do que selecionar Salvar manualmente. |

   Para obter mais informações sobre como salvar tarefas ao editá-las, consulte [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Para atribuir tarefas, siga um destes procedimentos:

   * Clique dentro do **Atribuído a** ou **Atribuído** e comece a digitar o nome de um usuário ativo que deseja atribuir à tarefa, em seguida, clique nele quando ele for exibido na lista.
   * Clique dentro do **Atribuições** e comece a digitar o nome de um usuário, função de trabalho ou equipe ativos que deseja atribuir à tarefa e, em seguida, clique nele quando ele for exibido na lista.

     >[!TIP]
     >
     >Ao adicionar uma atribuição de usuário, observe o avatar, a função principal do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.
     >
     >Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >
     ><span class="preview">Ao adicionar uma atribuição de função de trabalho, você pode pesquisar a função de trabalho ou o local. Selecione a Função de Trabalho Sistema/Padrão para usar a taxa de cobrança padrão para a atribuição ou selecione uma Função de Trabalho de Cartão de Taxa para usar a taxa de cobrança do cartão de taxa. Para obter mais informações sobre cartões de taxa, consulte [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


1. (Condicional) Quando visível na variável **Atribuições** clique no botão **Pessoas** no canto superior direito da caixa atribuições para abrir a caixa **Atribuições avançadas** e criar atribuições avançadas.

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   Para obter mais informações, consulte [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Não é possível fazer atribuições avançadas nos campos Atribuído a ou Atribuído.

1. Depois de adicionar os atribuídos à tarefa, pressione Enter ou clique em qualquer lugar na página para salvar as alterações se tiver selecionado Salvamento automático. Caso contrário, clique **Salvar**.

## Atribuir várias tarefas a um usuário

1. Vá para uma lista de tarefas que você deseja atribuir em massa.
1. (Condicional) Assegure que o **Salvamento automático** será selecionada se você estiver em uma lista de tarefas em um projeto.

   >[!IMPORTANT]
   >
   >Não é possível editar tarefas em massa ao salvar tarefas manualmente em um projeto.

1. Selecione várias tarefas na lista de tarefas.
1. Clique em **Editar**.

   A variável **Editar Tarefas** é aberta.

1. No **Atribuições** , selecione a **Destinatário** e comece a digitar o nome de um usuário, função de trabalho ou equipe que deseja atribuir a todas as tarefas.

   >[!IMPORTANT]
   >
   >Se qualquer uma das tarefas já estiver atribuída, os recursos que você indicar aqui serão adicionados às tarefas em vez de substituir os recursos existentes nas tarefas.

1. (Opcional) Selecione o botão de opção na caixa **Proprietário da tarefa** para indicar qual recurso é o principal designado ou o Proprietário da tarefa, quando você atribuir mais de um recurso à tarefa. Isto não está disponível para equipes.
1. (Condicional) Especifique a **Alocação %** para cada recurso atribuído à tarefa se todas as tarefas selecionadas tiverem um Tipo de Duração de Atribuição Calculada ou Orientada pelo Esforço. Isso indica quanto tempo esses recursos devem gastar na conclusão da tarefa. Isso só está disponível para usuários e funções de trabalho.

   Ou

   Especificar a quantidade de **Horas** para cada recurso atribuído à tarefa se todas as tarefas selecionadas tiverem um Tipo de Duração Simples. O total de todas as horas de todos os recursos deve ser igual ao número de Horas planejadas da tarefa.

   >[!IMPORTANT]
   >
   >Você não poderá especificar a porcentagem de alocação ou o número de horas por recurso se as tarefas selecionadas tiverem Tipos de Duração diferentes ou se as tarefas selecionadas tiverem Tipos de Duração diferentes.

   Para obter informações sobre o Tipo de duração em tarefas, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Opcional) Selecione uma função que o usuário deve desempenhar na tarefa a partir da **Escolher uma função** menu suspenso no **Função do atribuidor** quando você atribui usuários a tarefas. Se você não selecionar uma função, o Workfront selecionará automaticamente a função principal do usuário.

1. (Opcional) Se você deseja remover os atribuídos existentes de todas as tarefas, execute um dos seguintes procedimentos:

   1. Comece a digitar o nome de um usuário, função ou equipe que deseja remover da tarefa, selecione-o quando ele aparecer na lista e clique em **Remover atribuidor** para remover mais atribuídos.
   1. Clique em **Remover todos os atribuídos existentes** para remover todos os atribuídos da tarefa selecionada.

1. Clique em **Salvar alterações**.
1. (Opcional e condicional) Quando os campos Atribuído a ou Atribuições forem exibidos na lista de tarefas, clique dentro de uma dessas colunas para uma tarefa e, em seguida, clique na guia **Ícone X** ao lado do nome de um destinatário para removê-lo da tarefa.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


