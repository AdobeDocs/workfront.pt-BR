---
title: Visualizar as Tarefas em andamento na análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A visualização Tarefas em andamento mostra quantas tarefas (dentro dos critérios de filtro aplicados) estão em andamento para um projeto, a porcentagem de trabalho concluído para cada tarefa e como as tarefas são agendadas.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# Visualizar as Tarefas em andamento na análise aprimorada

A visualização Tarefas em andamento mostra quantas tarefas (dentro dos critérios de filtro aplicados) estão em andamento para um projeto, a porcentagem de trabalho concluído para cada tarefa e como as tarefas são agendadas.

![](assets/tasks-in-flight-possible-replacement-350x104.png)

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plano Adobe Workfront</a>*</td> 
   <td> <p>Empresa ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar o acesso a Projetos</p> <p>Exibir o acesso às Tarefas (Para atualizar tarefas, é necessário Editar acesso às Tarefas.)</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso.<br>Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissão para objetos de projeto e tarefa</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender as Tarefas em andamento

A visualização Tarefas no plano de voo mostra os seguintes detalhes da tarefa:

* **Duração da tarefa planejada**: O comprimento de uma barra de tarefas indica a duração planejada, que se baseia na data de início e na data de conclusão da tarefa.

   ![](assets/tasks-in-flight-duration-350x80.png)

* **Trabalho concluído**: A cor azul escuro em uma barra de tarefas indica a quantidade de trabalho concluído para uma tarefa. Essa porcentagem de conclusão é exibida à direita da barra de tarefas.

   ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **Trabalho restante**: A cor azul claro em uma barra de tarefas indica a quantidade de trabalho que precisa ser concluída para uma tarefa.

   ![](assets/tasks-in-flight-light-blue-350x35.png)

Essas informações podem ajudar você a determinar:

* Onde o esforço de trabalho foi focado.
* Que tarefas poderiam estar a pôr em risco um projeto.
* A proximidade de uma tarefa em relação à conclusão.
* Com quem você precisa falar sobre uma tarefa específica.

Para saber como obter os melhores dados para essa visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizar as Tarefas em andamento

1. Clique no ícone do Menu principal ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre como usar o filtro de intervalo de datas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se precisar limitar o conjunto de dados do projeto, selecione e aplique os filtros que deseja usar.

   Para obter mais informações sobre como adicionar filtros nas Análises aprimoradas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Após adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois que você sai da página ou faz logoff do Workfront.

1. Na visualização Plano de voo ou Mapa de árvore do projeto , clique em um projeto para exibir mais informações.

   As visualizações Burndown e Tasks in flight são exibidas.

   >[!NOTE]
   >
   >Para saber mais sobre essas outras visualizações, consulte:
   >
   >   
   >   
   >   * [Exibir a visualização do Plano de voo na análise aprimorada](../enhanced-analytics/flight-plan-overview.md)
   >   * [Visualizar o mapa de árvore do projeto no Enhanced Analytics](../enhanced-analytics/project-treemap-overview.md)
   >   * [Visualizar a visualização do Detalhamento na análise aprimorada](../enhanced-analytics/burndown-overview.md)


1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização do início do intervalo de datas e arraste até o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas, e um filtro de período é criado.

   ![](assets/timeframe-filter-350x220.png)

1. (Opcional) Para alterar como as tarefas são classificadas, clique no botão **Classificar por** selecione uma nova opção de classificação:

   * **Data de término**
   * **Alfabeticamente de A a Z**
   * **Estrutura de detalhamento do trabalho** (Essa opção corresponde à ordem em que as tarefas aparecem no projeto.)

   Todas as outras visualizações na página são atualizadas para corresponder à seleção de classificação.

1. Revise o progresso das tarefas no projeto selecionado e passe o mouse sobre uma tarefa específica para ver o número de horas planejadas, a data de vencimento planejada e a porcentagem de conclusão.

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. Clique em uma tarefa para abrir os Detalhes da tarefa no lado direito da tela, onde você pode ver mais informações sobre a tarefa, visualizar ou inserir atualizações, ou fazer alterações na tarefa.

   ![](assets/task-details-qs-350x675.png)

1. (Opcional) Para exportar os dados de visualização, clique no botão **Ícone Exportar** ![](assets/export.png) no canto superior direito da visualização, selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de dados (XSLX)**

