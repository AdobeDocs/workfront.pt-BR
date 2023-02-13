---
product-area: resource-management
navigation-topic: resource-planning
title: Revise a disponibilidade e alocação de recursos usando o Adobe Workfront Resource Planner
description: Você pode visualizar a disponibilidade de seus recursos e a quantidade de trabalho planejado ou orçado para seus projetos no Planejador de Recursos. Esses valores são exibidos em Horas, FTE (Equivalente de Tempo Total) ou Quantias de Custo e são organizados em colunas.
author: Alina
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 4%

---

# Revise a disponibilidade e alocação de recursos usando o Adobe Workfront Resource Planner

Você pode visualizar a disponibilidade de seus recursos e a quantidade de trabalho planejado ou orçado para seus projetos no Planejador de Recursos. Esses valores são exibidos em Horas, FTE (Equivalente de Tempo Total) ou Quantias de Custo e são organizados em colunas.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

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
   <td> <p>Revisar ou superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso ao seguinte:</p> 
    <ul> 
     <li> <p>Gerenciamento de recursos</p> </li> 
     <li> <p>Dados financeiros</p> </li> 
     <li> <p>Usuários</p> </li> 
     <li> <p>Projetos</p> </li> 
    </ul> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou permissões superiores aos projetos que você deseja visualizar no Planejador de Recursos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

<!--note from the table about the license: Review or higher: 
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (waiting on Vazgen to confirm - working differenly in classic)
      </MadCap:conditionalText>
     -->

## Pré-requisitos

Você deve atender a todos os pré-requisitos necessários para trabalhar com o Planejador de Recursos. Para obter mais informações, consulte [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>Se algum dos pré-requisitos necessários para a funcionalidade correta do Planejador de Recursos estiver ausente, alguns dos números poderão ser zero ou as Horas Orçadas poderão estar esmaecidas.

## Disponibilidade e afetação de recursos

As colunas que exibem a disponibilidade e alocação de seus recursos mudam, dependendo de qual exibição você se aplica ao Planejador de Recursos. Para obter informações sobre como exibir as informações no Planejador de Recursos por Projeto, Função ou Usuário, consulte [Visão geral da navegação do Planejador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Considere o seguinte ao alterar sua exibição para o Planejador de Recursos:

* Quando você aplica a variável **Exibir por projeto** ou **Exibir por função** for exibido, você poderá ver as seguintes colunas:

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * Horas, FTE ou Custo Disponíveis
   * Horas, FTE ou Custo Planejado
   * Horas, FTE ou Custo Orçadas
   * Horas, FTE ou Variação de Custo
   * Horas, FTE ou Custo Líquidos

* Quando você aplica a variável **Exibir por usuário** você pode ver as seguintes colunas:

   * Horas ou FTE disponíveis
   * Horas Planejadas ou FTE
   * Hora ou diferença de FTE
   * Porcentagem de Alocação de Horas Planejadas

>[!TIP]
>
>As informações não estão disponíveis como Custo ao aplicar a variável **Exibir por usuário** exibir para o Planejador de Recursos.
>
>Para obter mais informações sobre o que cada coluna exibe, passe o mouse sobre o nome da coluna na qual o número é exibido.\
>![Net_hours_res_planejer_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>Para obter mais informações sobre os dados exibidos em cada coluna, consulte os seguintes artigos:
>
>* [Visão geral de horas, FTE e informações de custo nas exibições Projeto e Função do Planejador de Recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [Exibir Horas Disponíveis, Planejadas e Reais ou FTE no Planejador de Recursos ao usar a exibição Usuário](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>


## Exibir informações por Hora, FTE ou Custo

1. Vá para o Planejador de Recursos.

   Por padrão, as informações são exibidas por Horas no Planejador de Recursos.

1. Expanda o menu suspenso.\
   ![Hours_fte_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. Selecione dentre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Horas</td> 
      <td>Exibe informações de disponibilidade e alocação em Horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">FTE</td> 
      <td> <p>Exibe informações de disponibilidade e alocação em FTE.</p> <p>Para obter mais informações sobre como o FTE é calculado no Planejador de Recursos, consulte <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de Recursos</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custo</td> 
      <td> <p>Exibe informações de disponibilidade e alocação por custo, se você estiver exibindo o Planejador de Recursos nas exibições Projeto ou Função. As informações exibem valores na moeda do seu sistema. O administrador do Workfront define a moeda do sistema. Para obter mais informações sobre como configurar a moeda do sistema no Workfront, consulte <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar taxas de câmbio</a>.</p> <p><b>Nota</b>

   Você deve associar usuários e funções de cargo às taxas de Custo por Hora para exibir as informações de Custo no Planejador de Recursos.<br style="font-style: italic;">Para obter mais informações sobre como associar as taxas de Custo por Hora às funções de cargo, consulte <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.<br style="font-style: italic;">Para obter mais informações sobre como associar as taxas de Custo por Hora aos usuários, consulte <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar o perfil de um usuário</a>.<br style="font-style: italic;">Para obter mais informações sobre como o Custo é calculado no Planejador de Recursos, consulte <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">Calcular custos no Planejador de Recursos </a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Personalizar</td> 
      <td>Cria uma exibição personalizada das colunas exibidas no Planejador de Recursos. Selecione as opções que deseja exibir no Planejador de Recursos, conforme descrito nas etapas abaixo. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Se você selecionou **Personalizar**, indique as opções na **Personalizar métricas exibidas** para configurar sua exibição personalizada.

   ![](assets/planner-customize-view-box-350x114.png)

1. No **Tipo de exibição** à esquerda, selecione uma das seguintes exibições:

   * Projeto
   * Função
   * Usuário

1. No **Exibir itens selecionados** selecione o tipo de informação que deseja exibir nas colunas da exibição selecionada. A tabela a seguir mostra quais opções estão disponíveis em cada exibição:

   | **Opção** | Visualizar Usuários | Visualização do Projeto | Exibição da função |
   |---|---|---|---|
   | Disponível | ✔ | ✔ | ✔ |
   | Planejado | ✔ | ✔ | ✔ |
   | Estimado |   | ✔ | ✔ |
   | Variação |   | ✔ | ✔ |
   | Líquido |   | ✔ | ✔ |
   | Efetivo | ✔ |   |   |
   | Diferença | ✔ |   |   |
   | Percentual | ✔ |   |   |

1. Selecionar **Usar valores planejados (PLN) em cálculos LÍQUIDOS** para usar informações Planejadas em vez de Orçadas ao calcular os valores Líquidos nas exibições Projeto e Função.

   Ao selecionar essa opção, o Workfront calcula os valores de Net usando a seguinte fórmula:

   ```
   Net = Available - Planned
   ```

   >[!TIP]
   >
   >**Essa opção é aplicada somente quando você seleciona pelo menos uma opção para personalizar a exibição na seção Exibir itens selecionados .**

1. Clique em **Salvar**.

   A exibição personalizada que inclui as colunas selecionadas é exibida.

   O Planejador de Recursos lista a exibição personalizada como Personalizada no menu suspenso Horas.

   >[!NOTE]
   >
   >Você pode ter apenas uma exibição personalizada.

   ![](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## Exibir o gráfico Alocação de usuários

Você pode exibir a Alocação planejada de usuários em relação à disponibilidade em um gráfico.

Para exibir a alocação de usuários em um gráfico:

1. Vá para o Planejador de Recursos.

   Para obter mais informações sobre como acessar o Planejador de Recursos, consulte o [Localizar o Planejador de Recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) no artigo [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. Selecionar **Exibir por usuário**.

   >[!TIP]
   >
   >Você pode exibir o Gráfico de Alocação de Usuário somente na Exibição de Usuário.

1. Clique no botão **Gráfico de alocação de usuários** ícone ![RP_user_allocate_chart.png](assets/rp-user-allocation-chart.png) para exibir as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">% de disponibilidade sem excesso de alocação de todos os usuários</td> 
      <td>Esse é o tempo que todos os usuários estão disponíveis para trabalhar em um período de tempo, mostrado como uma porcentagem de seu tempo total disponível. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">% de excesso de alocação de todos os usuários </td> 
      <td> <p>Essa é a quantidade de tempo em que os usuários são alocados em excesso em um período, mostrada como uma porcentagem do tempo total disponível.</p> <p><b>Nota</b>

   Uma atribuição excessiva acontece quando as Horas Planejadas são maiores que as Horas Disponíveis. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">% de subutilização de todos os usuários</td> 
      <td> <p>Esse é o tempo em que os usuários são subutilizados em um período, mostrado como uma porcentagem do tempo total disponível.</p> <p><b>Nota</b>

   A subutilização acontece quando as Horas Planejadas são inferiores às Horas Disponíveis. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Há um excesso de alocações para, pelo menos, um usuário durante este período de tempo</td> 
      <td>Isso indica que há uma sobrealocação para pelo menos um usuário em um período de tempo, embora a quantidade total de tempo de todos os usuários não esteja sobrealocada para o período de tempo.<br>Você deve percorrer a lista de usuários e as horas para o usuário que está sobrealocado são destacadas em vermelho.</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP_user_allocate_chart_Dec._7_2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. (Opcional) Clique no botão **% de atribuição excessiva para todos os usuários** no gráfico.\
   Todos os usuários com alocação excessiva são destacados em vermelho.
1. (Opcional) Clique no botão **% de subutilização para todos os utilizadores** no gráfico.\
   Todos os usuários subutilizados são destacados em azul.

1. (Opcional) Clique no ícone do indicador ![one_user_overallocate_marker.png](assets/one-user-overallocation-marker.png) que mostra onde você tem pelo menos um usuário com alocação excessiva.\
   Os usuários com alocação excessiva são destacados em vermelho.

1. (Opcional) Atualize a página para recolher o gráfico.
