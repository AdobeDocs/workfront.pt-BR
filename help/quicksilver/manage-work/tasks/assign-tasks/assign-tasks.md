---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Atribuir tarefas
description: Você pode atribuir tarefas a usuários, funções ou equipes para indicar quem é responsável pela conclusão das tarefas. É possível atribuir uma tarefa a mais de um recurso por vez.
author: Alina
feature: Work Management
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '1789'
ht-degree: 1%

---

# Atribuir tarefas

Você pode atribuir tarefas a usuários, funções de trabalho ou equipes para indicar quem é responsável pela conclusão das tarefas. É possível atribuir uma tarefa a mais de um recurso por vez.

>[!TIP]
>
>Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários ativos, funções de trabalho e equipes.
>
>Se um usuário, uma função de trabalho ou uma equipe tiver sido atribuída antes de ser desativada, ela permanecerá atribuída ao item de trabalho. Nesse caso, recomendamos o seguinte:
>
>* Atribua novamente o item de trabalho aos recursos ativos.
>* Associe os usuários em uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.
>


O número de usuários atribuídos a uma tarefa e o cronograma da tarefa Proprietário pode modificar as datas planejadas de uma tarefa, o que resulta na alteração da linha do tempo do projeto. Para obter informações sobre o impacto da atribuição de vários usuários a uma tarefa, consulte [Visão geral da modificação de atribuições de tarefa](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Além deste artigo, recomendamos que você leia os seguintes artigos para obter mais informações sobre como atribuir tarefas:

* [Visão geral da modificação de atribuições de tarefa](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Visão geral de atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Fazer atribuições inteligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Modificar várias atribuições de usuário em uma lista de tarefas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Planejar uma visão geral do projeto](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Visão geral da data de conclusão planejada da tarefa](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Definir a data de conclusão planejada do projeto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Visão Geral da atribuição de trabalho no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

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
   <td> <p>Editar acesso a Projetos e Tarefas</p> <p>Visualizar ou acessar mais alto os usuários</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir ou aumentar permissões para tarefas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações para várias atribuições em funções, equipes e usuários

Considere o seguinte ao atribuir vários recursos a um item de trabalho:

* Os usuários podem ter mais de uma função de trabalho associada ao perfil. Para obter informações sobre como associar usuários a funções de jobs, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Se você atribuir mais de um usuário a uma tarefa ou problema, o primeiro usuário selecionado será designado automaticamente como o proprietário da tarefa ou problema.
Para obter instruções sobre como alterar isso, consulte as informações sobre a opção Tornar principal no artigo [Criar atribuições avançadas](create-advanced-assignments.md).

* Uma equipe não pode ser um destinatário principal em uma tarefa ou problema. Somente um usuário ou uma função de trabalho pode ser designada como Primária em uma tarefa ou problema.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* Tarefas e problemas em um projeto podem ser atribuídos primeiro a uma ou mais equipes ou funções de trabalho. Quando o projeto estiver pronto para o início, ele também poderá precisar ser atribuído aos usuários:

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
   <td><p>Se você atribuir uma tarefa ou um problema a uma ou várias funções e, em seguida, também atribuir um usuário, decide qual função de trabalho associar ao usuário adicional (se houver) de acordo com as seguintes regras:</p>
     <ul>
      <li>Se houver apenas uma função de trabalho atribuída e ela corresponder à função primária do usuário (configurada em seu perfil), a tarefa ou problema será atribuído somente a esse usuário.</li>
      <li>Se várias funções forem atribuídas e pelo menos uma delas corresponder a uma das outras funções do usuário, a tarefa ou problema será atribuído ao usuário (a função será selecionada aleatoriamente se houver várias correspondências), juntamente com quaisquer funções adicionais atribuídas</li>
      <li>Se pelo menos uma função de trabalho for atribuída e não houver correspondências com as funções de trabalho do usuário, a tarefa ou o problema será atribuído à função ou às funções e ao usuário.</li>
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

1. Vá para uma tarefa que deseja atribuir.
1. Clique em **Atribuir a** no **Atribuições** no cabeçalho da tarefa ou do problema.

   Ou

   Clique no nome das atribuições se a tarefa ou problema já estiver atribuído.

![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. Siga um destes procedimentos:

   * Comece digitando o nome de um usuário, função ou equipe que deseja atribuir e clique nele quando ele for exibido na lista.


      >[!TIP]
      >
      >Ao adicionar uma atribuição de usuário, observe o avatar, a Função primária do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la à medida que você os adiciona.


   * (Condicional) Clique em um dos nomes no **Atribuições sugeridas** , se essa lista for exibida. Para obter mais informações, consulte [Visão geral de atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

   * Clique em **Avançado**

      Para obter informações sobre como fazer atribuições avançadas, consulte [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Clique em **Salvar**.
1. (Opcional e condicional) Clique no botão **Ícone X** ao lado do nome da atribuição no painel direito da tarefa para remover uma atribuição, se você clicar **Avançado**.

## Atribuir uma tarefa a uma lista

É possível atribuir tarefas em uma lista ou em um relatório quando qualquer um dos campos de atribuições estiver visível na exibição da lista. Essa é uma maneira mais rápida de atribuir tarefas. Este artigo descreve como modificar atribuições para uma tarefa em uma lista. Para obter informações sobre como modificar várias atribuições para várias tarefas em uma lista, consulte [Modificar várias atribuições de usuário em uma lista de tarefas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Dependendo de qual campo estiver visível na exibição, é possível atribuir as seguintes entidades à tarefa:

| Campo | Entidades atribuídas |
|---|---|
| **Atribuir a** | Atribuir um usuário |
| **Atribuído** | Atribuir um usuário |
| **Atribuições** | Atribuir usuários, funções de trabalho ou equipes |

Para atribuir tarefas em uma lista:

1. Vá para uma lista de tarefas que tem os campos Atribuído a, Atribuído ou Atribuições na exibição.
1. (Opcional) Clique no botão **Salvar automaticamente** e selecione uma das seguintes opções:

   | Opção | Descrição da opção |
   |---|---| 
   | Salvamento automático | As alterações feitas nas tarefas são salvas automaticamente e não é possível revertê-las |
   | Salvamento manual | Você deve salvar manualmente as alterações. Você pode reverter as alterações antes de salvá-las. |
   | Planejamento da linha do tempo | Você deve salvar manualmente as alterações. Você pode reverter as alterações antes de salvá-las. Salvar as alterações e todas as dependências do projeto é mais rápido do que selecionar Salvar manual . |

   Para obter mais informações sobre como salvar tarefas à medida que você as edita em uma lista, consulte [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Para atribuir tarefas, siga um destes procedimentos:

   * Clique dentro do **Atribuído a** ou **Atribuído** e comece a digitar o nome de um usuário ativo que deseja atribuir à tarefa, em seguida, clique nele quando for exibido na lista.
   * Clique dentro do **Atribuições** e comece a digitar o nome de um usuário ativo, função de trabalho ou equipe que deseja atribuir à tarefa, em seguida, clique nele quando for exibido na lista.

      >[!TIP]
      >Ao adicionar uma atribuição de usuário, observe o avatar, a Função primária do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la à medida que você os adiciona.
      >
      >
   >

1. (Condicional) Quando visível na variável **Atribuições** clique no campo **Pessoas** ícone no canto superior direito da caixa atribuições para abrir o **Atribuições avançadas** e criar atribuições avançadas.

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   Para obter mais informações, consulte [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   Não é possível fazer atribuições avançadas a partir dos campos Atribuído a ou Atribuído.

1. Depois de adicionar seus destinatários à tarefa, pressione Enter ou clique em qualquer lugar na página para salvar as alterações, se você selecionou Salvar automaticamente. Caso contrário, clique em **Salvar**.

## Atribuir várias tarefas a um usuário

1. Vá para uma lista de tarefas que deseja atribuir em massa.
1. (Condicional) Certifique-se de que a variável **Salvar automaticamente** é selecionada se você estiver em uma lista de tarefas em um projeto.

   >[!IMPORTANT]
   Não é possível editar tarefas em massa ao salvar tarefas manualmente em um projeto.

1. Selecione várias tarefas na lista de tarefas.
1. Clique em **Editar**.

   O **Editar Tarefas** será aberta.

1. No **Atribuições** selecione a **Destinatário** em seguida, comece a digitar o nome de um usuário, função de trabalho ou equipe que deseja atribuir a todas as tarefas.

   >[!IMPORTANT]
   Se alguma das tarefas já estiver atribuída, os recursos que você indicar aqui serão adicionados às tarefas em vez de substituir os recursos existentes nas tarefas.

1. (Opcional) Selecione o botão de opção no **Proprietário da Tarefa** para indicar qual recurso é o destinatário principal ou o Proprietário da tarefa, ao atribuir mais de um recurso à tarefa. Isso não está disponível para equipes.
1. (Condicional) Especifique a variável **% de alocação** para cada recurso atribuído à tarefa se todas as tarefas selecionadas tiverem um Tipo de duração de atribuição direcionada ou calculada. Isso indica quanto tempo esses recursos devem gastar na conclusão da tarefa. Isso só está disponível para usuários e funções de trabalho.

   Ou

   Especifique a quantidade de **Horas** para cada recurso atribuído à tarefa se todas as tarefas selecionadas tiverem um Tipo de duração Simples. O total de horas para todos os recursos deve ser igual ao número de Horas Planejadas para a tarefa.

   >[!IMPORTANT]
   Não é possível especificar a porcentagem de alocação ou o número de horas por recurso se as tarefas selecionadas tiverem Tipos de duração diferentes ou se as tarefas selecionadas tiverem Tipos de duração diferentes.

   Para obter informações sobre Tipo de duração em tarefas, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Opcional) Selecione uma função que o usuário deve atender à tarefa na **Escolha uma função** no menu suspenso da **Função do destinatário** quando você atribui usuários a tarefas. Se você não selecionar uma função, o Workfront seleciona automaticamente a Função primária do usuário.

1. (Opcional) Se você deseja remover os destinatários existentes de todas as tarefas, siga um destes procedimentos:

   1. Comece digitando o nome de um usuário, função ou equipe que deseja remover da tarefa, depois selecione-o quando ele for exibido na lista e clique em **Remover Destinatário** para remover mais destinatários.
   1. Clique em **Remover todos os destinatários existentes** para remover todos os destinatários de todas as tarefas selecionadas.

1. Clique em **Salvar alterações**.
1. (Opcional e condicional) Quando os campos Atribuído a ou Atribuições forem exibidos na lista de tarefas, clique dentro de uma dessas colunas para uma tarefa e, em seguida, clique no botão **Ícone X** ao lado do nome de um destinatário para removê-lo da tarefa.

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


