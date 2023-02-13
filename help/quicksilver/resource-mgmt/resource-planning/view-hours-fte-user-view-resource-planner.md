---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: Exibir Horas Disponíveis, Planejadas e Reais ou FTE no Planejador de Recursos ao usar a exibição Usuário
description: Exibir Horas Disponíveis, Planejadas e Reais ou FTE no Planejador de Recursos ao usar o Planejamento de Visualização do Usuário no RP" - talvez "orçando recursos no RP" ou "Gerenciando Recursos no RP". etc... - ou talvez precise ser redefinida de outro PDV?!)"
author: Alina
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 1%

---

# Exibir Horas Disponíveis, Planejadas e Reais ou FTE no Planejador de Recursos ao usar a exibição Usuário

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

Além de orçar recursos nas exibições Projeto e Função, você pode usar a Exibição de Usuário do Planejador de Recursos do Adobe Workfront para exibir informações sobre os valores de Horas Planejadas, Disponíveis e Real ou FTE para projetos e recursos.

## Visão Geral da Exibição de Usuário no Planejador de Recursos

Considere o seguinte ao exibir as informações de Horas ou FTE no Planejador de Recursos:

* Você pode exibir as informações de Horas Disponíveis e Planejadas ou do FTE para usuários, funções de cargo e projetos em todas as exibições do Planejador de Recursos.
* Você pode exibir as seguintes informações somente na Visualização de usuário:

   * A diferença entre a quantidade de Horas Planejadas ou de TEF e a quantidade de Horas Disponíveis ou de TEF. Em seguida, é possível orçar a alocação de seus usuários de acordo com essa diferença nas exibições Projeto e Função.
   * As Horas reais ou FTE.

* Você pode exibir a diferença entre o Usuário Disponível e a quantidade de Horas Planejadas ou FTE como um número ou como um valor percentual na exibição Usuário.
* Não é possível exibir as informações na exibição Usuário por Custo.
* O Adobe Workfront preenche as Horas Disponíveis ou o FTE de acordo com o tempo de trabalho associado aos usuários em suas programações.\
   Os usuários não associados a um agendamento mostram a disponibilidade de acordo com o Agendamento padrão.\
   Para obter informações sobre a Programação Padrão, consulte [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* O Workfront preenche as Horas Planejadas ou o FTE das Horas Planejadas com as informações sobre as tarefas e problemas dos projetos.
* O Workfront preenche as Horas reais com o tempo real registrado para tarefas e problemas pelos usuários atribuídos a eles. Isso inclui o tempo de logon em um projeto.
* Na exibição Usuário, é possível fazer o seguinte:

   * Expanda cada usuário para exibir uma lista de projetos nos quais esse usuário está atribuído.

      >[!NOTE]
      >
      >Somente os usuários associados aos projetos incluídos nos filtros podem ser expandidos.

   * Expanda cada projeto para exibir uma lista de funções de trabalho que o usuário pode atender a esses projetos.
   * Expanda cada função para exibir uma lista de tarefas às quais o usuário nessa função está atribuído.

   Se os usuários não tiverem funções de trabalho associadas a eles, suas Disponíveis, Planejadas e Horas Reais ou FTE serão listadas na **Sem função** seção.\
   Para obter informações sobre quais campos e itens são exibidos ao aplicar a exibição Usuário ao Planejador de Recursos, consulte a seção &quot;Projeto/Função/Seleção de Exibição de Usuário&quot; em [Visão geral da navegação do Planejador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Visão geral dos campos visíveis na Visualização de usuário do Planejador de Recursos

Consulte as tabelas a seguir para entender as informações exibidas na exibição Usuário do Planejador de Recursos. As informações são exibidas em valores de Horas ou FTE.

* [A coluna AVL (Disponível)](#the-avl-available-column)
* [Coluna PLN (planejada)](#the-pln-planned-column)
* [A coluna ACT (Real)](#The%C2%A0ACT)
* [A coluna DIF (Diferença)](#the-dif-difference-column)
* [A coluna % (Porcentagem de Alocação de Horas Planejadas)](#the-planned-hours-allocation-percentage-column)

### A coluna AVL (Disponível) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Exibido por</strong> </td> 
   <td> <p><strong>Descrição</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td>O total de Horas Disponíveis ou FTE para o usuário de acordo com seu cronograma. </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>Essas informações não estão disponíveis para o Projeto ao aplicar a exibição Usuário ao Planejador de Recursos. </td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>O total de Horas Disponíveis ou FTE para a função de acordo com o cronograma do usuário e o <strong>Porcentagem de disponibilidade de FTE</strong> do papel.</p> </td> 
  </tr> 
  <tr> 
   <td>Tarefa ou problema</td> 
   <td>Essas informações não estão disponíveis para a Tarefa ou o Problema. </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações sobre como a disponibilidade de usuário e função é calculada com base no agendamento do usuário e na Porcentagem da disponibilidade de FTE da função, consulte [Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de Recursos](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### Coluna PLN (planejada) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Exibido por</strong> </td> 
   <td> <p><strong>Descrição</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> O total de Horas Planejadas ou FTE de todas as tarefas ou problemas atribuídos ao usuário em todos os projetos.<br><p>Isso inclui tarefas e problemas que são atribuídos ao usuário, mas não estão associados a nenhuma função de trabalho, tarefas ou problemas que não estão em projetos que você tem acesso a Gerenciar.</p><p>Quando a alocação de usuários para horas tiver sido modificada usando o Balanceador de Carga de Trabalho, os dados no Planejador de Recursos poderão ser afetados se as datas selecionadas contiverem apenas uma parte de uma tarefa ou problema. Para obter informações sobre como modificar alocações para usuários, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gerenciar alocações de usuários no Balanceador de Carga de Trabalho</a> . </p></td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td> O total de Horas Planejadas ou FTE de todas as tarefas e problemas atribuídos a um usuário específico no projeto.<br><p>Observação: Isso não inclui as Horas Planejadas ou o FTE de tarefas ou problemas que não são atribuídos a nenhum usuário. </p></td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>O total de Horas Planejadas ou FTE de todas as tarefas e problemas atribuídos ao usuário nesta função no projeto.</p> <p> <p>Observação: Isso não inclui as Horas Planejadas ou o FTE de tarefas ou problemas que são atribuídos a essa função, mas não a esse usuário nessa função. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Tarefa ou problema</td> 
   <td>As Horas Planejadas ou o FTE associado à tarefa ou ao problema no projeto.</td> 
  </tr> 
 </tbody> 
</table>

Considere o seguinte ao exibir as Horas Planejadas:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* As Horas Planejadas são igualmente distribuídas para cada dia dentro da Duração das tarefas e problemas , para cada recurso atribuído a elas. A tarefa ou emissão Duração é baseada em suas Datas de Início e Conclusão Planejadas e inclui todos os dias de calendário dentro desse período de tempo.\
   A Workfront leva em conta o agendamento do usuário ou do projeto ao distribuir as Horas Planejadas para usuários ou projetos. Nesse caso, as Horas Planejadas são igualmente distribuídas para cada dia dentro da Duração das tarefas ou problemas, excluindo fins de semana, dias de folga e exceções de programação.

   Por exemplo, se você exibir o Planejador de Recursos por Semana e tiver tarefas que abrangem várias semanas em projetos, o número de Horas Planejadas por semana dependerá do número de dias nessa semana que fazem parte da Duração da tarefa. Isso funciona de forma semelhante ao exibir o Planejador de Recursos por Mês ou Trimestre e quando as tarefas abrangem vários meses ou trimestres.\
   Dias de fim de semana, exceções de agendamento e dias de folga são excluídos desta distribuição.

* As seguintes categorias de tarefas são incluídas no cálculo das Horas Planejadas para cada recurso:

   * tarefas atribuídas aos usuários em Grupos de Recursos, funções de trabalho ou equipes no projeto.

      >[!TIP]
      >
      >Se tarefas forem atribuídas a equipes, sua alocação será exibida em **Sem função** e **Sem usuário** seções. Você pode ver as Horas Planejadas associadas às equipes, mas não pode calcular as horas, pois nenhuma função ou usuário está associado às tarefas.

* As Horas Planejadas no Planejador de Recursos não incluem as Horas Planejadas associadas ao seguinte:

   * tarefas pai
   * tarefas não atribuídas
   * problemas, quando a variável **Incluir horas de problemas** está desativada.

* As Horas Planejadas não são exibidas no Planejador de Recursos se a tarefa ou emissão Duração for zero.
* As Horas Planejadas associadas a usuários desativados não são exibidas.

Para obter mais informações sobre Horas Planejadas e FTE no Planejador de Recursos, consulte [Visão geral de horas, FTE e informações de custo nas exibições Projeto e Função do Planejador de Recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### A coluna ACT (Real)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Exibido por</strong> </td> 
   <td> <p><strong>Descrição</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuário </td> 
   <td> <p>O tempo registrado pelo usuário em todas as tarefas ou problemas atribuídos a ele.</p> <p>Isso inclui o seguinte:</p> 
    <ul> 
     <li>Tarefas e problemas que são atribuídos ao usuário, mas não estão associados a nenhuma função de trabalho.</li> 
     <li>Tarefas e problemas que não estão em projetos para os quais você tem acesso a Gerenciar. </li> 
    </ul> <p>Isso inclui o tempo de logon no projeto somente quando o usuário é atribuído a tarefas ou problemas nesse projeto.  </p> </td> 
  </tr> 
  <tr> 
   <td>Projeto </td> 
   <td> <p>O tempo registrado pelo usuário em todas as tarefas e problemas atribuídos a ele no projeto.</p> <p>Isso inclui qualquer momento em que eles fizeram logon diretamente no projeto.</p> <p>Isso não inclui o seguinte:</p> 
    <ul> 
     <li> <p>Tempo conectado em tarefas e problemas que não são atribuídos a nenhum usuário. </p> </li> 
     <li> <p>Tempo conectado nas tarefas pai. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>O tempo de logon em todas as tarefas ou problemas atribuídos ao usuário nesta função. </p> <p>Isso não inclui o seguinte:</p> 
    <ul> 
     <li>Tempo conectado em tarefas e problemas atribuídos a esta função, mas não a este usuário nesta função.</li> 
     <li>Tempo registrado diretamente no projeto ou nas tarefas principais. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Tarefa ou problema </td> 
   <td> <p>O tempo em que as tarefas foram conectadas e os problemas foram resolvidos pelo usuário que também foi atribuído a ele. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>O tempo registrado é exibido no período correspondente à Data de entrada da hora, independentemente do período da tarefa, problema ou projeto em que as horas são registradas.

Para obter mais informações sobre Horas Reais, consulte [Exibir Horas Reais](../../manage-work/tasks/task-information/actual-hours.md).

### A coluna DIF (Diferença) {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Exibido por</strong> </td> 
   <td> <p><strong>Descrição</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> <p>A diferença entre as Horas Disponíveis e Planejadas ou FTE do usuário. </p> <p>A diferença Hour ou FTE é calculada usando a seguinte fórmula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>Observação: Se o valor for exibido em números vermelhos negativos, o usuário estará sobrealocado. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>Essas informações não estão disponíveis para o Projeto. </td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>A diferença entre as Horas Disponíveis e Planejadas ou FTE da função de cargo. </p> <p>A diferença Hour ou FTE é calculada usando a seguinte fórmula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>Observação: Se o valor for exibido em números vermelhos negativos, a função será sobrealocada. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Tarefa ou problema</td> 
   <td>Estas informações não estão disponíveis para a Tarefa, Ocorrência ou Projeto. </td> 
  </tr> 
 </tbody> 
</table>

### A coluna % (Porcentagem de Alocação de Horas Planejadas) {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Exibido por</strong> </td> 
   <td> <p><strong>Descrição</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> <p>A alocação das Horas Planejadas ou do FTE como uma porcentagem das Horas Disponíveis. A porcentagem da Alocação de Horas Planejadas é calculada usando a seguinte fórmula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>O mesmo cálculo é usado para valores FTE. </p> </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>Estas informações não estão disponíveis para o Projeto ao aplicar a variável <strong>Exibir por usuário</strong> exibir para o Planejador de Recursos.</td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> A alocação das Horas Planejadas ou do FTE como uma porcentagem das Horas Disponíveis. <p>A porcentagem da Alocação de Horas Planejadas é calculada usando a seguinte fórmula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>O mesmo cálculo é usado para valores FTE.</p></td> 
  </tr> 
  <tr> 
   <td>Tarefa ou problema</td> 
   <td>Estas informações não estão disponíveis para a Tarefa, Ocorrência ou Projeto. </td> 
  </tr> 
 </tbody> 
</table>

Se o valor de Horas Planejadas ou FTE for zero, a Alocação de Porcentagem será de 0%. Se o valor de Horas Disponíveis ou FTE for zero, a Alocação de Porcentagem não poderá ser calculada.

Para obter mais informações sobre Horas Planejadas e FTE e como elas são exibidas no Planejador de Recursos, consulte [Recursos de orçamento no Planejador de Recursos usando as exibições Projeto e Função](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->
