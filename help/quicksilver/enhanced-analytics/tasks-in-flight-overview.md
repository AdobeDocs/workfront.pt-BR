---
title: Visualização das Tarefas em andamento na Análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A visualização Tarefas em andamento mostra quantas tarefas (dentro dos critérios de filtro aplicados) estão em andamento para um projeto, a porcentagem de trabalho concluído para cada tarefa e o cronograma das tarefas.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 4%

---

# Visualização das Tarefas em andamento na Análise aprimorada

>[!IMPORTANT]
>
>O Analytics aprimorado será removido do Workfront na semana de 26 de maio. O Workfront Data Connect é uma solução nova e alternativa e pode ser usada para replicar qualquer visualização do Enhanced Analytics que você usa atualmente. <br>Consulte o [guia de descontinuação do Enhanced Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) para obter mais informações.


A visualização Tarefas em andamento mostra quantas tarefas (dentro dos critérios de filtro aplicados) estão em andamento para um projeto, a porcentagem de trabalho concluído para cada tarefa e o cronograma das tarefas.

![Tarefas em andamento](assets/tasks-in-flight-possible-replacement-350x104.png)

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plano do Adobe Workfront</a>*</td> 
   <td> <p>Business ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">visão geral das licenças do Adobe Workfront</a>*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar acesso aos projetos</p> <p>Acesso de visualização a Tarefas (para atualizar tarefas, você precisa ter acesso de Edição a Tarefas).</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso.<br>Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissão para objetos de projeto e tarefa</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; na [Visão geral do Enhanced Analytics](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender as tarefas na visualização de navegação

A visualização do plano de execução de Tarefas mostra os seguintes detalhes da tarefa:

* **Duração da tarefa planejada**: o comprimento de uma barra de tarefas indica a duração planejada, que se baseia na data de início e na data de conclusão da tarefa.

  ![Duração das tarefas em andamento](assets/tasks-in-flight-duration-350x80.png)

* **Esforço de trabalho concluído**: a cor azul escuro em uma barra de tarefas indica a quantidade de trabalho concluído para uma tarefa. Essa porcentagem de conclusão é exibida à direita da barra de tarefas.

  ![Tarefas em voo com azul escuro](assets/tasks-in-flight-dark-blue-350x35.png)

* **Esforço de trabalho restante**: a cor azul-claro em uma barra de tarefas indica a quantidade de trabalho que precisa ser concluído para uma tarefa.

  ![Tarefas em azul claro de voo](assets/tasks-in-flight-light-blue-350x35.png)

Essas informações podem ajudar você a determinar:

* Onde o esforço de trabalho foi concentrado.
* Quais tarefas podem estar colocando um projeto em risco.
* Quão perto uma tarefa está da conclusão.
* Com quem você precisa falar sobre uma tarefa específica.

Para saber como obter os melhores dados para esta visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualização Exibir as tarefas em andamento

1. Clique no ícone Menu Principal ![ícone Menu principal](assets/main-menu-icon-16x12.png) e selecione **Analytics**.
1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![Selecionar intervalo de datas](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre como usar o filtro de intervalo de datas, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se precisar limitar o conjunto de dados do projeto, selecione e aplique os filtros que deseja usar.

   Para obter mais informações sobre como adicionar filtros na Análise aprimorada, consulte [Aplicar filtros na Análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Depois de adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois de sair da página ou do Workfront.

1. Na visualização do Plano de voo ou Mapa de árvore do projeto, clique em um projeto para exibir mais informações.

   As visualizações Burndown e Tarefas em voo são exibidas.

   >[!NOTE]
   >
   >Para saber mais sobre essas outras visualizações, consulte:
   >
   >   
   >   
   >   * [Exibir a visualização do Plano de voo na análise aprimorada](../enhanced-analytics/flight-plan-overview.md)
   >   * [Exibir a visualização do mapa de árvore do projeto na análise aprimorada](../enhanced-analytics/project-treemap-overview.md)
   >   * [Exibir a visualização de Burndown na análise aprimorada](../enhanced-analytics/burndown-overview.md)
   >   
   >

1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização para o início do intervalo de datas e arraste até o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas e um filtro de período é criado.

   ![Filtro de cronograma](assets/timeframe-filter-350x220.png)

1. (Opcional) Para alterar a forma como as tarefas são classificadas, clique no menu **Classificar por** e selecione uma nova opção de classificação:

   * **Data de conclusão**
   * **Alfabeticamente de A a Z**
   * **Estrutura de detalhamento de trabalho** (Esta opção corresponde à ordem em que as tarefas aparecem no projeto.)

   Todas as outras visualizações na página são atualizadas para corresponder à sua seleção de classificação.

1. Revise o progresso das tarefas no projeto selecionado e passe o mouse sobre uma tarefa específica para ver o número de horas planejadas, a data de vencimento planejada e a porcentagem de conclusão.

   ![Detalhes das tarefas em andamento](assets/tasks-in-flight-task-details-350x242.png)

1. Clique em uma tarefa para abrir os Detalhes da tarefa no lado direito da tela, onde você pode ver mais informações sobre a tarefa, exibir ou inserir atualizações ou fazer alterações na tarefa.

   ![Detalhes da tarefa](assets/task-details-qs-350x675.png)

1. (Opcional) Para exportar os dados de visualização, clique no **ícone Exportar** ![ícone Exportar](assets/export.png) no canto superior direito da visualização e selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de Dados (XSLX)**

