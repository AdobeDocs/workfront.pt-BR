---
product-area: resource-management
navigation-topic: resource-planning
title: Calcular Custos no Planejador de Recursos
description: Você pode estimar seus recursos no Planejador de Recursos da Adobe Workfront usando valores de Custo, em vez de valores de Horas ou FTE. Os valores de custo não estão disponíveis para a visualização **Exibir por usuário** no Planejador de recursos.
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 0%

---

# Calcular custos no Planejador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

Você pode estimar seus recursos no Planejador de Recursos da Adobe Workfront usando valores de Custo, em vez de valores de Horas ou FTE. Os valores de custo não estão disponíveis para a exibição **Visualizar por Usuário** no Planejador de Recursos.

>[!IMPORTANT]
>
>Você deve associar usuários e funções de trabalho às taxas de Custo por Hora para exibir informações de Custo no Planejador de Recursos.\
>Para obter mais informações sobre como associar taxas de Custo por hora a funções de trabalho, consulte [Criar e gerenciar funções de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>Para obter mais informações sobre como associar taxas de Custo por hora a usuários, consulte [Editar perfil de usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Antes de estimar seus recursos, certifique-se de ter um bom entendimento de qual trabalho precisa ser feito (Horas planejadas, FTE ou Custo) e que horas seus usuários estão abertos para trabalhar (Horas disponíveis, FTE ou Custo).\
Para obter mais informações sobre como entender as informações no Planejador de Recursos ao fazer o orçamento por Horas ou FTE, consulte [Visão geral de horas, FTE e informações de custo nas exibições de Projeto e Função do Planejador de Recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td>
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Editar prioridades e horas de orçamento no Planejador de recursos</p> <p>Editar acesso a Dados Financeiros, Projetos e Usuários</p></td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para os projetos para os quais você deseja orçar informações com a capacidade de Gerenciar Finanças</p></td>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir informações no Planejador de Recursos por Custo

Por padrão, as informações de disponibilidade e alocação são exibidas em Horas no Planejador de recursos.

Para exibir informações Disponíveis, Planejadas e Orçadas por Custo no Planejador de Recursos:

{{step1-to-resourcing}}

1. Vá até o Planejador de recursos.
1. (Condicional) Selecione **Exibir por Projeto** ou **Exibir por Função**.\
   Por padrão, **Exibir por Projeto** está selecionado.\
   As informações de alocação e disponibilidade são exibidas em Horas.

1. No menu suspenso **Horas**, selecione **Custo**.

   Se você não tiver acesso a Dados Financeiros em seu nível de acesso, essa opção não estará disponível.\
   Se os projetos tiverem uma moeda diferente da moeda do sistema, o Custo desses projetos será exibido no Planejador de recursos convertido na moeda do sistema. O administrador do sistema define a moeda do sistema.\
   Para obter mais informações sobre como configurar a moeda do sistema no Workfront e as taxas de conversão, consulte [Configurar taxas de câmbio](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![custos_no_planejador_com_no_orçamento.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Calcular Custo Disponível no Planejador de Recursos

Para exibir os valores de Custo Disponível no Planejador de Recursos, você deve ter o seguinte:

* Taxas de custo por hora para usuários e funções
* Informações sobre a disponibilidade do usuário.

  A obtenção de informações sobre a disponibilidade de usuários depende de como o administrador do Workfront configura as Preferências de gerenciamento de recursos.\
  Para obter mais informações sobre como calcular a disponibilidade de usuários e definir Preferências de Gerenciamento de Recursos, consulte [Configurar preferências de Gerenciamento de Recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

A tabela a seguir ilustra como o Custo Disponível é calculado no Planejador de Recursos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Custo Disponível</strong> </th> 
   <th><strong>Cálculo</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Custo Disponível do Usuário</td> 
   <td> <p>O Custo Disponível por usuário é calculado usando a seguinte fórmula:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>Nota</b>

Se o usuário não tiver uma taxa de Custo por hora em seu perfil, a taxa de Custo por hora da função de trabalho na qual ele está listado será usada no cálculo. Se o usuário não tiver nenhuma função associada a ele, o Custo de Usuário Disponível será de $0. </p> </td>
</tr> 
  <tr> 
   <td>Custo Disponível da Função</td> 
   <td> <p>O Custo Disponível por função é calculado usando a seguinte fórmula:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>Nota</b>

Se a função não tiver uma taxa de Custo por hora, o Custo da Função Disponível será $0.</p> </td>
</tr> 
  <tr> 
   <td>Custo Disponível do Projeto</td> 
   <td> <p>O Custo Disponível por projeto é calculado usando a seguinte fórmula:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Calcular Custo Planejado no Planejador de Recursos

Embora não seja possível exibir as informações da tarefa no Planejador de Recursos, os Custos Planejados para usuários, funções e projetos são calculados levando-se em conta as seguintes informações da tarefa:

* O tipo de atribuição na tarefa.\
  Você pode deixar uma tarefa não atribuída ou atribuir as seguintes entidades a uma tarefa:

   * Um usuário (com ou sem uma função de trabalho)
   * Uma Função
   * Uma equipe\
     Uma tarefa atribuída a uma Equipe é considerada não atribuída, da perspectiva do Planejador de Recursos.

* O **Tipo de Custo** das tarefas no projeto.\
  Para obter mais informações sobre o Tipo de Custo de uma tarefa, consulte [Rastrear custos](../../manage-work/projects/project-finances/track-costs.md).

* As datas efetivas das taxas de custo para funções de trabalho e usuários.

  Por exemplo, se a função ou o usuário tiver 10 horas planejadas em fevereiro e 10 horas planejadas em março, mas a taxa de custo tiver sido alterada de US$ 12 para US$ 20 em março, o valor do Custo Planejado em fevereiro será de US$ 120 e em março o Custo Planejado será de US$ 200.

>[!NOTE]
>
>Os Custos planejados do usuário não influenciam o Custo planejado do projeto. Somente os custos Planejados da Função afetam os Custos Planejados do Projeto, no Planejador de Recursos.

Existem os seguintes cenários ao calcular o Custo Planejado para usuários, funções e o projeto:

* Quando o **Tipo de Custo** for **De Hora em Hora do Usuário &#x200B;** e não houver **nenhuma atribuição** na tarefa:

   * **Custo Planejado de Função e Usuário**:

     Os custos planejados da função e do usuário são de US$ 0,00.

   * **Custo Planejado do Projeto**:

     O custo planejado do projeto é de US$ 0,00.

* Quando o **Tipo de Custo** é **Usuário por Hora** e há uma **atribuição de usuário** na tarefa:

   * **Custo Planejado de Função e Usuário**:

     O Custo Planejado do Usuário é calculado usando a seguinte fórmula:

     `User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate`

     Se um usuário tiver uma taxa de custo em seu perfil, essa taxa será usada para calcular o Custo Planejado. Caso contrário, a taxa de Custo por hora em nível de sistema da Função principal será usada.

     >[!NOTE]
     >
     >O usuário pode ser atribuído à tarefa com uma de suas funções de trabalho secundárias, mas a taxa da função de trabalho principal é usada aqui.

     O Custo Planejado da Função é calculado usando a seguinte fórmula:

     `Role Planned Cost = SUM(User Planned Cost)`

   * **Custo Planejado do Projeto**:

     O custo planejado do projeto é de US$ 0,00.

* Quando o **Tipo de Custo** é **Usuário por Hora** e há uma **atribuição de função de trabalho** na tarefa:

   * **Custo Planejado de Função e Usuário**:

     O custo planejado do usuário é de US$ 0,00.

     O Custo Planejado da Função é calculado usando a seguinte fórmula:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     A taxa de Custo por Hora em nível de sistema da função de trabalho atribuída à tarefa é usada para calcular o Custo Planejado.

   * **Custo Planejado do Projeto**:

     O custo planejado do projeto é de US$ 0,00.

* Quando o **Tipo de Custo** é **Função por Hora** e não há **nenhuma atribuição** na tarefa:

   * **Custo Planejado de Função e Usuário**:

     Os custos planejados da função e do usuário são de US$ 0,00.

   * **Custo Planejado do Projeto**:

     O custo planejado do projeto é de US$ 0,00.

* Quando o **Tipo de Custo** é **Função por Hora** e há uma **atribuição de usuário** na tarefa:

   * **Custo Planejado de Função e Usuário**:

     O custo planejado do usuário é de US$ 0,00.

     O Custo Planejado da Função é calculado pela seguinte fórmula:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     A Workfront analisa a função de trabalho que o usuário desempenha na tarefa para calcular o Custo planejado da função.

     Se o usuário não estiver associado a nenhuma função na tarefa, o Custo Planejado será de US$ 0,00.

   * **Custo Planejado do Projeto**:

     O Custo Planejado do Projeto é calculado usando a seguinte fórmula:

     `Project Planned Cost = SUM(Role Planned Costs)`

* Quando o **Tipo de Custo** é **Função por Hora** e há uma **atribuição de função de trabalho** na tarefa:

   * **Custo Planejado de Função e Usuário**:

     O custo planejado do usuário é de US$ 0,00.

     O Custo Planejado da Função é calculado pela seguinte fórmula:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     A Workfront analisa a função de trabalho que o usuário desempenha na tarefa para calcular o Custo planejado da função.

   * **Custo Planejado do Projeto**:

     O Custo Planejado do Projeto é calculado usando a seguinte fórmula:

     `Project Planned Cost = SUM(Role Planned Costs)`

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(table below ideal but drafted because it does not display correctly in Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td rowspan="2">&nbsp;</td>
<td colspan="3"> <p><strong>Cost Type = User Hourly</strong> </p><strong>User Planned Cost</strong> </td>
<td colspan="3"> <p><strong>Cost Type = Role Hourly</strong> </p><strong>Role Planned Cost</strong> </td>
</tr>
<tr>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>User and Role Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td rowspan="2"> <p><strong>Project Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td colspan="2"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td>
</tr>
<tr>
<td colspan="6"> <note type="note">
User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the Resource Planner.
</note> </td>
</tr>
</tbody>
</table>
-->

## Calcular Custo Orçado no Planejador de Recursos

Para exibir os valores de Custo Orçado no Planejador de Recursos, você deve ter o seguinte:

* Horas orçadas para funções, usuários e projetos.
* Taxas de custo por hora para usuários e funções.

>[!NOTE]
>
>As horas orçadas dos projetos são calculadas com base nas horas orçadas das funções, não das de usuários.

A tabela a seguir ilustra como o Custo Orçado é calculado no Planejador de Recursos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Custo Orçado</strong> </th> 
   <th><strong>Cálculo</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Custo orçado do usuário</td> 
   <td> <p>O Custo orçado por usuário é calculado usando a seguinte fórmula:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>Nota</b>

Se o usuário não tiver uma taxa de Custo por hora em seu perfil, o Custo de usuário orçado será de US$ 0,00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Custo orçado da função</td> 
   <td> <p>O Custo orçado da função é calculado usando a seguinte fórmula:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>Nota</b>

Se a função não tiver uma taxa de Custo por hora, o Custo da função orçada será de US$ 0,00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Custo orçado do projeto</td> 
   <td> <p>O Custo orçado por projeto é calculado usando a seguinte fórmula:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
