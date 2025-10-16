---
product-area: resource-management
navigation-topic: resource-planning
title: Revisar Disponibilidade e Alocação de Recursos usando o Adobe Workfront Resource Planner
description: Você pode visualizar a disponibilidade de seus recursos e a quantidade de trabalho planejado ou orçado para seus projetos no Planejador de recursos. Esses valores são exibidos em Horas, FTE (Equivalente a Tempo Integral) ou quantias de Custo e são organizados em colunas.
author: Lisa
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 4%

---

# Revisar a disponibilidade e a alocação de recursos usando o Planejador de Recursos da Adobe Workfront

Você pode visualizar a disponibilidade de seus recursos e a quantidade de trabalho planejado ou orçado para seus projetos no Planejador de recursos. Esses valores são exibidos em Horas, FTE (Equivalente a Tempo Integral) ou quantias de Custo e são organizados em colunas.

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
   <td><p>Leve ou superior</p>
       <p>Revisar ou superior</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Visualize ou tenha acesso superior ao seguinte:</p> 
    <ul> 
     <li> <p>Gerenciamento de recursos</p> </li> 
     <li> <p>Dados financeiros</p> </li> 
     <li> <p>Usuários</p> </li> 
     <li> <p>Projetos</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Visualize ou tenha permissões mais altas para os projetos que deseja visualizar no Planejador de recursos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você deve atender a todos os pré-requisitos necessários para trabalhar com o Planejador de Recursos. Para obter mais informações, consulte [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>Se qualquer um dos pré-requisitos necessários para a funcionalidade correta do Planejador de recursos estiver ausente, alguns dos números podem ser zero ou as Horas orçadas podem estar esmaecidas.

## Disponibilidade e alocação de recursos

As colunas que exibem a disponibilidade e a alocação dos recursos mudam, dependendo da exibição aplicada ao Planejador de recursos. Para obter informações sobre como exibir as informações no Planejador de Recursos por Projeto, Função ou Usuário, consulte [Visão geral da navegação do Planejador de Recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Considere o seguinte ao alterar sua exibição para o Planejador de recursos:

* Ao aplicar as visualizações **Visualizar por Projeto** ou **Visualizar por Função**, você pode ver as seguintes colunas:

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * Horas Disponíveis, FTE ou Custo
   * Horas planejadas, FTE ou Custo
   * Horas orçadas, FTE ou Custo
   * Horas, FTE ou variação de custo
   * Horas líquidas, FTE ou custo

* Ao aplicar a exibição **Exibir por Usuário**, você poderá ver as seguintes colunas:

   * Horas Disponíveis ou FTE
   * Horas planejadas ou FTE
   * Diferença de Hora ou FTE
   * Porcentagem de Alocação de Horas Planejadas

>[!TIP]
>
>As informações não estão disponíveis como Custo ao aplicar a visualização **Visualizar por Usuário** ao Planejador de Recursos.
>
>Para obter mais informações sobre o que cada coluna exibe, passe o mouse sobre o nome da coluna na qual o número é exibido.\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>Para obter mais informações sobre os dados exibidos em cada coluna, consulte os seguintes artigos:
>
>* [Visão geral de horas, FTE e informações de custo nos modos de exibição Projeto e Função do Planejador de Recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [Exibir Horas Disponíveis, Planejadas e Reais ou FTE no Planejador de Recursos ao usar o modo de exibição Usuário](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>

## Visualizar informações por hora, FTE ou custo

1. Vá até o Planejador de recursos.

   Por padrão, as informações são exibidas por Horas no Planejador de recursos.

1. Expanda o menu suspenso.\
   ![Hours_fte_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. Selecione entre as seguintes opções:

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
      <td> <p>Exibe informações de disponibilidade e alocação em FTE.</p> <p>Para obter mais informações sobre como o FTE é calculado no Planejador de recursos, consulte <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de recursos</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custo</td> 
      <td> <p>Exibe informações de disponibilidade e alocação por custo, se você estiver visualizando o Planejador de Recursos nas visualizações Projeto ou Função. As informações exibem valores na moeda do sistema. O administrador do Workfront define a moeda do sistema. Para obter mais informações sobre como configurar a moeda do sistema no Workfront, consulte <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar taxas de câmbio</a>.</p> <p><b>Nota</b>

   Você deve associar usuários e funções de trabalho às taxas de Custo por Hora para exibir informações de Custo no Planejador de Recursos.<br style="font-style: italic;">Para obter mais informações sobre como associar taxas de Custo por hora a funções de trabalho, consulte <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.<br style="font-style: italic;">Para obter mais informações sobre como associar taxas de Custo por hora a usuários, consulte <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar perfil de usuário</a>.<br style="font-style: italic;">Para obter mais informações sobre como o Custo é calculado no Planejador de Recursos, consulte <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">Calcular custos no Planejador de Recursos </a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Personalizar</td> 
      <td>Cria uma exibição personalizada das colunas exibidas no Planejador de recursos. Selecione as opções que deseja exibir no Planejador de recursos, conforme descrito nas etapas abaixo. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Se você selecionou **Personalizar**, indique as opções na caixa **Personalizar métricas exibidas** para configurar seu modo de exibição personalizado.

   ![Personalizar caixa de exibição](assets/planner-customize-view-box-350x114.png)

1. Na coluna **Tipo de exibição** à esquerda, selecione uma das seguintes exibições:

   * Projeto
   * Função
   * Usuário

1. Na seção **Exibir itens selecionados**, selecione o tipo de informação que deseja exibir nas colunas do modo de exibição selecionado. A tabela a seguir mostra quais opções estão disponíveis em cada exibição:

   | **Opção** | Visualizar Usuários | Visualização do Projeto | Exibição de função |
   |---|---|---|---|
   | Disponível | ✔ | ✔ | ✔ |
   | Planejado | ✔ | ✔ | ✔ |
   | Estimado |   | ✔ | ✔ |
   | Variância |   | ✔ | ✔ |
   | Líquido |   | ✔ | ✔ |
   | Efetivo | ✔ |   |   |
   | Diferença | ✔ |   |   |
   | Porcentagem | ✔ |   |   |

1. Selecione **Usar valores Planejados (PLN) em cálculos LÍQUIDOS** para usar informações Planejadas em vez de Orçadas ao calcular os valores Líquidos nas exibições de Projeto e Função.

   Ao selecionar essa opção, o Workfront calcula os valores Líquidos usando a seguinte fórmula:

   `Net = Available - Planned`

   >[!TIP]
   >
   >**Esta opção é aplicada somente quando você seleciona pelo menos uma opção para personalizar o modo de exibição na seção Exibir itens selecionados.**

1. Clique em **Salvar**.

   A exibição personalizada que inclui as colunas selecionadas é exibida.

   O Planejador de recursos lista a exibição personalizada como Personalizada no menu suspenso Horas.

   >[!NOTE]
   >
   >Você pode ter apenas uma exibição personalizada.

   ![Lista suspensa de horas do planejador](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## Exibir o gráfico de Alocação de Usuários

Você pode exibir a Alocação planejada de usuários em relação à sua disponibilidade em um gráfico.

Para exibir a alocação de usuários em um gráfico:

1. Vá até o Planejador de recursos.

   Para obter mais informações sobre como acessar o Planejador de Recursos, consulte a seção [Localizar o Planejador de Recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) no artigo [Visão geral do Planejador de Recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. Selecione **Exibir por Usuário**.

   >[!TIP]
   >
   >Você pode exibir o Gráfico de Alocação de Usuário apenas na View do Usuário.

1. Clique no **ícone do gráfico de alocação de usuário** ![RP_user_allocation_chart.png](assets/rp-user-allocation-chart.png) para exibir as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">% de disponibilidade sem excesso de alocação de todos os usuários</td> 
      <td>Tempo que todos os usuários ficam disponíveis para trabalhar em um período, mostrado como uma porcentagem do tempo total disponível. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">% de excesso de alocação de todos os usuários </td> 
      <td> <p>É o tempo durante o qual os usuários estão superalocados em um período, mostrado como uma porcentagem do tempo total disponível.</p> <p><b>Nota</b>

   Uma superalocação acontece quando as Horas Planejadas são maiores que as Horas Disponíveis. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">% de subutilização de todos os usuários</td> 
      <td> <p>Essa é a quantidade de tempo em que os usuários são subutilizados em um período, mostrada como uma porcentagem do tempo total disponível.</p> <p><b>Nota</b>

   A subutilização acontece quando as Horas planejadas são inferiores às Horas disponíveis. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Há um excesso de alocações para, pelo menos, um usuário durante este período de tempo</td> 
      <td>Isso indica que há uma superalocação para pelo menos um usuário em um período de tempo, embora a quantidade total de tempo de todos os usuários não esteja superalocada para o período de tempo.<br>Você deve percorrer a lista de usuários e as horas do usuário que está superalocado serão destacadas em vermelho.</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP_user_allocation_chart_Dec_7__2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. (Opcional) Clique na área **Superalocação % para todos os usuários** no gráfico.\
   Todos os usuários superalocados são destacados em vermelho.
1. (Opcional) Clique na área **Subutilização % para todos os usuários** do gráfico.\
   Todos os usuários subutilizados são destacados em azul.

1. (Opcional) Clique no ícone do indicador ![one_user_overallocation_marker.png](assets/one-user-overallocation-marker.png) que mostra onde você tem pelo menos um usuário superalocado.\
   Os usuários superalocados são destacados em vermelho.

1. (Opcional) Atualize a página para recolher o gráfico.
