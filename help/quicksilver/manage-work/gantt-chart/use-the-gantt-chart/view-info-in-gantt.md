---
navigation-topic: use-the-gantt-chart
title: Exibir informações na  [!UICONTROL Gráfico de Gantt]
description: A lista de tarefas Gráfico de Gantt e Gráfico de Gantt da lista de projetos exibe informações sobre projetos e tarefas.
author: Alina
feature: Work Management
exl-id: e6b55699-0831-40d4-a997-6fe3f8828ee1
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 1%

---

# Exibir informações na  [!UICONTROL Gráfico de Gantt]

A lista de tarefas [!UICONTROL Gráfico de Gantt] e lista de projetos [!UICONTROL Gráfico de Gantt] exibir informações sobre projetos e tarefas.

## Requisitos de acesso

Você deve ter o seguinte para seguir as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] visão geral das licenças*</td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>[!UICONTROL View] ou acesso superior a Projetos e tarefas</p> <p><b>Nota</b>

Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>[!UICONTROL View] ou acesso superior ao projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Localize a variável  [!UICONTROL Gráfico de Gantt]

Você pode localizar o gráfico de Gantt da lista de tarefas e a lista de projetos [!UICONTROL Gráfico de Gantt] de várias áreas no Workfront. Para obter mais informações, consulte [Introdução ao [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

## Exibir tarefas na [!UICONTROL Caminho Crítico]

Na lista de projetos [!UICONTROL Gráfico de Gantt], tarefas que não estão no [!UICONTROL Caminho Crítico] exibir como linhas horizontais azuis-claras. Tarefas que estão no [!UICONTROL Caminho Crítico] de um projeto são exibidas como linhas horizontais vermelhas.

Para obter mais informações sobre tarefas na [!UICONTROL Caminho Crítico], consulte [Visão geral do projeto [!UICONTROL Caminho Crítico]](../../../manage-work/tasks/manage-tasks/critical-path.md).

## Exibir informações da tarefa na lista de projetos [!UICONTROL Gráfico de Gantt]

Você pode exibir as informações da tarefa para um projeto diretamente da Lista de projetos. As tarefas são listadas sob o nome de cada projeto.

>[!NOTE]
>
>Não é possível editar tarefas na Lista de projetos [!UICONTROL Gráfico de Gantt].

Você pode exibir as informações da tarefa para um projeto diretamente de uma lista de projetos nas seguintes áreas:

* No [!UICONTROL Projetos] area
* Dentro de um Portfolio
* Dentro de um programa

Para exibir tarefas em um projeto a partir de uma lista de projetos:

1. Vá para uma das áreas mencionadas acima.

   Por exemplo, da variável [!UICONTROL Menu principal], clique em **[!UICONTROL Projetos]**.

   Uma lista de projetos é exibida.

1. Clique no botão **[!UICONTROL Gráfico de Gantt]** ícone ![](assets/gantt-icon-nwe.png) no canto superior direito da tela.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: images conditioned for classic and nwe) <br></p>
   -->

1. Clique no botão **[!UICONTROL Mostrar lista de tarefas]** ícone .

1. Na lista de projetos à esquerda, clique na seta suspensa ao lado do nome do projeto para exibir as tarefas sob o projeto.\
   Isso exibe informações de tarefa no  [!UICONTROL Gráfico de Gantt].\
   ![Show_task_list_enabled_project_expand.png](assets/show-task-list-enabled-project-expanded-350x78.png)

1. (Opcional) Clique no botão **[!UICONTROL Imprimir]** no canto superior direito para exportar o [!UICONTROL Gráfico de Gantt].

   >[!NOTE]
   >
   >A lista de projetos [!UICONTROL Gráfico de Gantt] exporta somente projetos. As informações da tarefa não estão incluídas.

## Altere o período de tempo para o qual as informações são exibidas na [!UICONTROL Gráfico de Gantt]

É possível ajustar o período de tempo mostrado na [!UICONTROL Gráfico de Gantt] para exibir informações em nível granular, ou navegue rapidamente até um dia, semana, mês, trimestre ou exibição anual:

* [Alterar o período de tempo em um nível granular](#change-the-time-period-on-a-granular-level)
* [Exibir informações por dia, semana, mês, trimestre ou ano](#view-information-by-day-week-month-quarter-or-year)

### Alterar o período de tempo em um nível granular {#change-the-time-period-on-a-granular-level}

1. Passe o mouse sobre a linha do tempo do  [!UICONTROL Gráfico de Gantt], em seguida, arraste o indicador de zoom da esquerda para a direita para expandir ou contrair a linha do tempo.\
   ![zoom_tool_in_gantt.png](assets/zoom-tool-in-gantt-350x180.png)

### Exibir informações por dia, semana, mês, trimestre ou ano {#view-information-by-day-week-month-quarter-or-year}

1. No  [!UICONTROL Gráfico de Gantt], clique no menu suspenso de período.

   ![](assets/timeline-options.png)

1. Selecione um intervalo de tempo entre as seguintes opções disponíveis:

   * **[!UICONTROL Ajustar tudo]**: Essa opção exibe a linha do tempo de todo o projeto.
   * **[!UICONTROL Todos os projetos]**: Essa opção está disponível somente no gráfico de Gantt da lista de projetos.
   * **[!UICONTROL Ano]**
   * **[!UICONTROL Trimestre]**
   * **[!UICONTROL Mês]**
   * **[!UICONTROL Semana]**
   * **[!UICONTROL Dia]**

1. (Opcional) Selecione um período de tempo mais granular, como [!UICONTROL Semana] ou [!UICONTROL Dia]e clique e arraste a barra de rolagem horizontal na parte inferior do  [!UICONTROL Gráfico de Gantt] para mover da esquerda para a direita na linha de tempo do projeto.\
   Um instantâneo da linha do tempo do [!UICONTROL Gantt] é exibido para mostrar o projeto inteiro.

   >[!TIP]
   >
   >O instantâneo da linha do tempo é exibido somente depois que você clica na barra de rolagem horizontal.

   ![alongchy_gantt_minimap_with_outline_1_.png](assets/stretchy-gantt-minimap-with-outline--1--350x140.png)

1. (Opcional) Clique em qualquer lugar dentro do instantâneo da linha do tempo para navegar até um ponto específico na vida do projeto.\
   Ou\
   Arraste as alças do visualizador de instantâneos para selecionar um intervalo de linha do tempo específico para exibi-lo no [!UICONTROL Gantt].

## Usar filtros, visualizações e agrupamentos

O [!UICONTROL Gráfico de Gantt] é uma representação visual das informações exibidas atualmente na lista de tarefas. É possível aplicar filtros, visualizações e agrupamentos aos objetos listados em [!UICONTROL Gráfico de Gantt]s.

>[!CAUTION]
>
>Não é possível aplicar filtros, visualizações e agrupamentos ao selecionar [!UICONTROL Manual] salvar [!UICONTROL Planejamento de linha do tempo] para salvar alterações na lista de tarefas. Para obter informações sobre como salvar alterações em tarefas em uma lista, consulte [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Os filtros e agrupamentos aplicados à lista são refletidos na Lista de projetos e na Lista de tarefas  [!UICONTROL Gráfico de Gantt]s e também são incluídos quando os gráficos de Gantt são exportados:

* Filtros\
   Você pode aplicar um Filtro à lista para controlar as informações exibidas no [!UICONTROL Gráfico de Gantt].\
   Para obter informações sobre como aplicar um filtro, consulte  [Visão geral dos filtros em [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Agrupamento\
   Os agrupamentos aplicados à lista são refletidos na variável [!UICONTROL Gráfico de Gantt].\
   Para obter informações sobre como aplicar um Agrupamento, consulte  [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

As exibições não são refletidas na variável [!UICONTROL Gráfico de Gantt]. No entanto, quando você exporta a variável [!UICONTROL Gráfico de Gantt] (conforme descrito em  [Exporte o [!UICONTROL Gráfico de Gantt] para PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)), a lista de tarefas é exportada além do [!UICONTROL Gráfico de Gantt], com a Exibição atual aplicada à lista.

## Configurar opções de exibição

Você pode escolher o tipo de informação que será exibido em [!UICONTROL Gráficos de Gantt]. Para obter mais informações, consulte [Configure como as informações são exibidas no [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).
