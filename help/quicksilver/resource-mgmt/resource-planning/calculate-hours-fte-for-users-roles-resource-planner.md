---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de recursos
description: Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de recursos
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 4331917d133c52cf727f148b75a213853c1e5679
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

Você pode exibir a alocação e a disponibilidade de seus recursos no Planejador de Recursos por Horas, FTE ou Custo.\
Para obter mais informações sobre o cálculo de Custos no Planejador de Recursos, consulte [Calcular custos no Planejador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

&quot;FTE&quot; significa Equivalente a Tempo Integral. É uma medida de tempo que representa a quantidade de horas dedicadas ao trabalho real durante um dia ou semana para um usuário ou função de trabalho.

Os conjuntos de informações de recursos a seguir são calculados de forma diferente no Planejador de recursos:

* Os valores de Horas Disponíveis ou FTE são calculados com base na forma como o Administrador do Sistema configura as preferências de Gerenciamento de Recursos no sistema.\
  Para obter mais informações sobre como os valores de Horas Disponíveis e FTE são calculados, consulte [Calcular Horas Disponíveis ou FTE para usuários e funções de trabalho no Planejador de Recursos](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  Para obter mais informações sobre como definir as preferências de Gerenciamento de Recursos para o sistema Adobe Workfront, consulte [Configurar preferências de gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* Todos os outros valores de FTE são calculados com base no agendamento Padrão do sistema.\
  Para obter mais informações sobre como todos os outros valores são exibidos no Planejador de recursos ao usar FTE, consulte a seção [Calcular todos os outros valores de hora e FTE para usuários e funções de trabalho no Planejador de recursos](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) neste artigo.

É importante entender o que é o FTE para cada um dos usuários e suas funções de trabalho para gerenciar com precisão os recursos à medida que você os atribui para trabalhar.

## Calcular Horas Disponíveis ou FTE para usuários e funções de trabalho no Planejador de Recursos {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [Calcular as Horas Disponíveis e o FTE de um usuário no Planejador de Recursos](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [Calcular as Horas Disponíveis e o FTE para uma função de trabalho no Planejador de Recursos](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [Calcular as Horas Disponíveis e o FTE de um usuário no Planejador de Recursos (Exemplo)](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### Calcular as Horas Disponíveis e o FTE de um usuário no Planejador de Recursos {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

O administrador do Workfront determina como o tempo disponível para um usuário é calculado ao selecionar para usar um dos seguintes itens na área Gerenciamento de recursos em Configuração:

* O Cronograma Padrão do sistema e o FTE do usuário.
* A programação do usuário.

Para obter mais informações, consulte [Configurar preferências de gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><br></p>
<p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p>
<p>(NOTE: The determines how to calculate resource availability at the system level.For more information about defining the Resource Management preferences for the system, see Configure Resource Management preferences.)</p>
<p>Based on how this setting is configured, the availability of the users in the Resource Planner (hours as well as FTE availability) is calculated by using the following methods: </p>
<ul>
<li><strong>The Default Schedule</strong>: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the Resource Planner. The Schedule of the user is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE value</code> <span style="color: #dc143c;">( NOTE: this is the correct value. If this shows as a division in other articles, that is wrong. It's a multiplication between these 2 values).</span><br>For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Resource Planner.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a></li>
<li style="font-weight: normal;"> The <strong>Available FTE</strong> for the user in the<strong>Resource Planner</strong> is the same as the user FTE specified in the user settings. <br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner. For more information about the value of the user FTE as it displays in the user settings, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><strong>The User's Schedule</strong>: The Schedule of the user is used to determine the availability of the user in the Resource Planner. The value of the user FTE is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the Resource Planner. </li>
<li> The <strong>Available FTE</strong> in the<strong>Resource Planner</strong> is calculated by the following formula:<br><em><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul></li>
</ul> <note type="note">
If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note>
</div>
-->

### Calcular as Horas Disponíveis e o FTE para uma função de trabalho no Planejador de Recursos {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

Primeiro, é necessário calcular a disponibilidade do usuário e, em seguida, calcular a disponibilidade de cada uma de suas funções de trabalho.

A disponibilidade de funções de trabalho no Planejador de recursos leva em conta a disponibilidade total do usuário e a **Porcentagem de Disponibilidade de FTE** associado a cada função do usuário.\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

Para obter mais informações sobre como associar uma **Porcentagem de Disponibilidade de FTE** com uma função de trabalho para um usuário, consulte [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Por exemplo, se o valor de Horas Disponíveis para um usuário for 40 e ele puder cumprir uma Função Principal por 75% desse tempo e uma Outra Função por 25% desse tempo, o Planejador de Recursos mostrará que **Horas Disponíveis** para a Função principal por uma semana é de 30 horas e que o valor **Horas Disponíveis** para a Outra função é 10 horas. Nesse caso, o FTE da Função principal é 0,75 e o FTE da outra função é 0,25.

>[!NOTE]
>
>O tempo total disponível para o usuário é calculado por um dos dois métodos descritos no [Calcular as Horas Disponíveis e o FTE de um usuário no Planejador de Recursos](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) neste artigo.

Ao visualizar o Planejador de recursos na visualização Função, a disponibilidade de uma função de trabalho é um total da disponibilidade de todos os usuários que podem desempenhar essa função de trabalho.\
Para obter mais informações sobre a disponibilidade de recursos no Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Calcular as Horas Disponíveis e o FTE de um usuário no Planejador de Recursos (Exemplo) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

A tabela a seguir ilustra como as Horas Disponíveis e o FTE Disponível são calculados para o usuário no Planejador de Recursos, dependendo de qual método é usado pelo administrador do sistema para o cálculo do FTE nas Preferências de Gerenciamento de Recursos.

Neste exemplo, estamos usando os seguintes números:

* Um calendário padrão do sistema de 40 horas
* Uma programação de usuário de 20 horas
* Um FTE de usuário de 0,75

| Método de Cálculo de FTE (Configuração do Sistema) | **Horas a partir do Cronograma do Usuário** | **Horas a partir do calendário padrão** | **Campo FTE do usuário** | **Horas Disponíveis no Planejador de Recursos** | **FTE disponível no Planejador de recursos** |
|---|---|---|---|---|---|
| **O Cronograma Padrão** | Ignorada | 40 | 0.75 | **30** (calculado) | **0.75** |
| **O Cronograma do Usuário** | 20 | 40 | Ignorada | **20** | **0,5** (calculado) |

Exceções de cronograma e folga podem afetar a quantidade de Horas planejadas ou FTE. Para obter mais informações, consulte [Configurar preferências de gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Calcular todos os outros valores de hora e FTE para usuários e funções de trabalho no Planejador de recursos {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

Além das Horas Disponíveis ou FTE, as seguintes informações de tempo também são exibidas no Planejador de Recursos:

* Horas planejadas
* Horas orçadas
* Variação de Hora
* Horas líquidas\
  Para obter mais informações sobre esses valores, consulte [Visão geral de horas, FTE e informações de custo nas visualizações Projeto e Função do Planejador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* Diferença de Hora\
  Para obter mais informações sobre o que esse valor representa, consulte [Visão geral de horas, FTE e informações de custo nas visualizações Projeto e Função do Planejador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

Você pode exibir as mesmas informações no Planejador de recursos que o FTE ou as horas.

O Workfront usa a seguinte fórmula para exibir todos os outros valores como FTE no Planejador de Recursos:

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>O cronograma do usuário é ignorado ao calcular o FTE para todos os valores, exceto para os valores de FTE Disponíveis (AVL) no Planejador de recursos. Somente o Cronograma Padrão é considerado para o cálculo.

Esse cálculo se aplica aos seguintes valores:

* ETC planejado (PLN)
* FTE orçado (BDG)
* Variação FTE (VAR)
* FTE LÍQUIDO
* Diferença FTE (DIF)
