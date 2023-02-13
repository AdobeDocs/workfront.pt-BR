---
product-area: resource-management
navigation-topic: resource-planning
title: Calcular custos no Planejador de Recursos
description: "Alina: ***Vinculado ao Planejamento no artigo Planejador de Recursos, Noções Gerais das áreas do Planejador de Recursos. - não mover/ alterar/ excluir.)"
author: Alina
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '1373'
ht-degree: 0%

---

# Calcular custos no Planejador de Recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

Você pode orçar seus recursos no Planejador de Recursos do Adobe Workfront usando valores de Custo, em vez de Valores de Horas ou FTE. Os valores de custo não estão disponíveis para a variável **Exibir por usuário** no Planejador de recursos.

>[!IMPORTANT]
>
>Você deve associar usuários e funções de cargo às taxas de Custo por Hora para exibir as informações de Custo no Planejador de Recursos.\
>Para obter mais informações sobre como associar as taxas de Custo por Hora às funções de cargo, consulte [Criar e gerenciar funções de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>Para obter mais informações sobre como associar as taxas de Custo por Hora aos usuários, consulte [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Antes de orçar seus recursos, certifique-se de ter uma boa compreensão do trabalho que precisa ser feito (Horas Planejadas, FTE ou Custo) e de que tempo seus usuários estão abertos para trabalhar (Horas Disponíveis, FTE ou Custo).\
Para obter mais informações sobre como entender as informações no Planejador de Recursos ao fazer o orçamento por Horas ou FTE, consulte [Visão geral de horas, FTE e informações de custo nas exibições Projeto e Função do Planejador de Recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro e superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Edite o acesso ao Gerenciamento de Recursos que inclui acesso a Editar prioridades e horas orçamentárias no Planejador de Recursos</p> <p>Editar acesso a dados financeiros, projetos e usuários</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões dos projetos para os quais deseja obter informações de orçamento com a capacidade de Gerenciar finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Exibir informações no Planejador de Recursos por Custo

Por padrão, as informações de disponibilidade e alocação são exibidas em Horas no Planejador de Recursos.

Para exibir informações Disponíveis, Planejadas e Orçadas por Custo no Planejador de Recursos:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Recursos**.
1. Vá para .
1. (Condicional) Selecionar **Exibir por projeto** ou **Exibir por função**.\
   Por padrão **Exibir por projeto** está selecionada.\
   As informações de alocação e disponibilidade são exibidas em Horas.

1. No **Horas** , selecione **Custo**.

   Se você não tiver acesso aos Dados financeiros em seu nível de acesso, essa opção não estará disponível.\
   Se os projetos tiverem uma moeda diferente da moeda do sistema, o Custo desses projetos será exibido no Planejador de Recursos convertido na moeda do sistema. O administrador do sistema define a moeda do sistema.\
   Para obter mais informações sobre como configurar a moeda do sistema no Workfront e as taxas de conversão, consulte [Configurar taxas de câmbio](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![cost_in_the_planejer_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Calcular Custo Disponível no Planejador de Recursos

Para exibir os valores de Custo Disponível no Planejador de Recursos, você deve ter o seguinte:

* Taxas de custo por hora para usuários e funções
* Informações sobre a disponibilidade do usuário.

   A obtenção de informações sobre a disponibilidade do usuário depende de como o administrador do Workfront configura as Preferências de gerenciamento de recursos.\
   Para obter mais informações sobre como calcular a disponibilidade do usuário e definir Preferências do Gerenciamento de Recursos, consulte [Configurar preferências do Gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

A tabela a seguir ilustra como o Custo Disponível é calculado no Planejador de Recursos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Custo disponível</strong> </th> 
   <th><strong>Cálculo</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Custo Disponível do Usuário</td> 
   <td> <p>O Custo Disponível por Usuário é calculado usando a seguinte fórmula:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>Nota</b>

Se o usuário não tiver uma taxa de Custo por Hora em seu perfil, a taxa de Custo por Hora da função de cargo sob a qual está listado será usada no cálculo. Se o usuário não tiver nenhuma função associada a ele, o Custo Disponível do Usuário será de $0. </p> </td>
</tr> 
  <tr> 
   <td>Custo da Função Disponível</td> 
   <td> <p>O Custo Disponível por função é calculado usando a seguinte fórmula:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>Nota</b>

Se a função não tiver uma taxa de Custo por Hora, o Custo da Função Disponível será de $0.</p> </td>
</tr> 
  <tr> 
   <td>Custo Disponível do Projeto</td> 
   <td> <p>O Custo Disponível por projeto é calculado usando a seguinte fórmula:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Calcular Custo Planejado no Planejador de Recursos

Embora você não possa exibir as informações da tarefa no Planejador de Recursos, os Custos Planejados para usuários, funções e projetos são calculados levando em conta as seguintes informações da tarefa:

* O tipo de atribuição na tarefa.\
   Você pode deixar uma tarefa não atribuída ou atribuir as seguintes entidades a uma tarefa:

   * Um usuário (com ou sem uma função de trabalho)
   * Uma função
   * Uma equipe\
      Uma tarefa atribuída a uma Equipe é considerada não atribuída, da perspectiva do Planejador de Recursos.

* O **Tipo de custo** das tarefas do projeto.\
   Para obter mais informações sobre o Tipo de Custo de uma tarefa, consulte [Rastrear custos](../../manage-work/projects/project-finances/track-costs.md).

>[!NOTE]
>
>Os Custos Planejados pelo Usuário não influenciam o Custo Planejado do Projeto. Somente os custos da Função Planejada afetam os Custos Planejados do Projeto, no Planejador de Recursos.

Os seguintes cenários existem ao calcular o Custo Planejado para usuários, funções e o projeto:

* Quando a variável **Tipo de custo** é **Por hora do usuário **e há um **sem atribuição** na tarefa:

   * **Função e custo planejado do usuário**:

      A função e os custos planejados do usuário são de US$ 0,00.

   * **Custo Planejado do Projeto**:

      O Custo Planejado do Projeto é de $0,00.

* Quando a variável **Tipo de custo** é **Por hora do usuário** e há um **atribuição de usuário** na tarefa:

   * **Função e custo planejado do usuário**:

      O Custo Planejado do Usuário é calculado usando a seguinte fórmula:



      ```
      User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate
      ```

      Se um usuário tiver uma taxa de custo em seu perfil, essa taxa será usada para calcular o Custo Planejado. Caso contrário, a taxa de Custo por Hora do nível do sistema de sua Função Principal será usada.

      >[!NOTE]
      >
      >O usuário pode ser atribuído à tarefa com uma de suas funções de trabalho secundárias, mas a taxa da função de trabalho principal é usada aqui.

      O Custo Planejado da Função é calculado usando a seguinte fórmula:

      ```
      Role Planned Cost = SUM(User Planned Cost)
      ```

   * **Custo Planejado do Projeto**:

      O Custo Planejado do Projeto é de $0,00.

* Quando a variável **Tipo de custo** é **Por hora do usuário** e há um **atribuição de função de trabalho** na tarefa:

   * **Função e custo planejado do usuário**:

      O Custo Planejado do Usuário é de US$ 0,00.

      O Custo Planejado da Função é calculado usando a seguinte fórmula:

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      A taxa de Custo por Hora no nível do sistema da função de trabalho atribuída à tarefa é usada para calcular o Custo Planejado.

   * **Custo Planejado do Projeto**:

      O Custo Planejado do Projeto é de $0,00.

* Quando a variável **Tipo de custo** é **Função por hora** e há **sem atribuição** na tarefa:

   * **Função e custo planejado do usuário**:

      A função e os custos planejados do usuário são de US$ 0,00.

   * **Custo Planejado do Projeto**:

      O Custo Planejado do Projeto é de $0,00.

* Quando a variável **Tipo de custo** é **Função por hora** e há um **atribuição de usuário** na tarefa:

   * **Função e custo planejado do usuário**:

      O Custo Planejado do Usuário é de US$ 0,00.

      O Custo Planejado da Função é calculado pela seguinte fórmula:

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      A Workfront observa a função de trabalho que o usuário cumpre na tarefa para calcular o Custo Planejado da função.

      Se o usuário não estiver associado a nenhuma função na tarefa, o Custo Planejado será de US$ 0,00.

   * **Custo Planejado do Projeto**:

      O Custo Planejado do Projeto é calculado usando a seguinte fórmula:

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

* Quando a variável **Tipo de custo** é **Função por hora** e há um **atribuição de função de trabalho** na tarefa:

   * **Função e custo planejado do usuário**:

      O Custo Planejado do Usuário é de US$ 0,00.

      O Custo Planejado da Função é calculado pela seguinte fórmula:

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      A Workfront observa a função de trabalho que o usuário cumpre na tarefa para calcular o Custo Planejado da função.

   * **Custo Planejado do Projeto**:

      O Custo Planejado do Projeto é calculado usando a seguinte fórmula:

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

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

Para exibir valores de Custo Orçado no Planejador de Recursos, você deve ter o seguinte:

* Horas Orçadas para funções, usuários e projetos.
* Taxas de custo por hora para usuários e funções.

>[!NOTE]
>
>As Horas Orçamentadas dos projetos são calculadas com base nas Horas Orçadas para as Funções, não para as de usuários.

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
   <td>Custo orçado do Usuário</td> 
   <td> <p>O Custo Orçado por Usuário é calculado usando a seguinte fórmula:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>Nota</b>

Se o usuário não tiver uma taxa de Custo por Hora em seu perfil, o Custo do Usuário Orçado será de $0,00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Custo da Função Orçada</td> 
   <td> <p>O Custo da Função Orçada é calculado usando a seguinte fórmula:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>Nota</b>

Se a função não tiver uma taxa de Custo por Hora, o Custo da Função Orçada será de $0,00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Custo orçado do projeto</td> 
   <td> <p>O Custo por projeto orçado é calculado usando a seguinte fórmula:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
