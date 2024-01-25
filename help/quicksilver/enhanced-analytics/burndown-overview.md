---
title: Exibir a visualização de Burndown na análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A visualização de Burndown mostra o burndown de um projeto específico ao longo do tempo e ajuda você a entender a relação entre a condição do projeto, a velocidade e as horas—ou dias restantes.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Exibir a visualização de Burndown na análise aprimorada

<!-- Audited: 12/2023 -->

A visualização de Burndown mostra o burndown de um projeto específico ao longo do tempo e ajuda você a entender a relação entre a condição do projeto, a velocidade e as horas—ou dias restantes.

![Exemplo de burndown de análise aprimorado](assets/burndown120623.png)

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>
      <p>Novo: Qualquer um</p>
      <p>ou</p>
      <p>Atual: Comercial ou superior</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
      <p>Novo: Claro ou superior</p>
      <p>ou</p>
      <p>Atual: revisão ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualizar acesso aos projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir</p> </td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender a visualização de Burndown

A linha azul sólida mostra a velocidade planejada desde a data de início até a data de conclusão planejada. Essa linha é ajustada à medida que o trabalho é adicionado, removido ou atualizado, e é alterada para uma linha vertical tracejada quando o projeto atinge a data de conclusão planejada.

![Velocidade planejada](assets/burndown-planned-line.png)

A linha real mostra o número de horas ou dias gastos no projeto ao longo do tempo. A cor dessa linha indica a condição do projeto a cada dia:

* **Verde**: o projeto está no destino.

  ![No destino](assets/burndown-green.png)

* **Laranja**: o projeto está em risco.

  ![Em risco](assets/burndown-orange.png)

* **Vermelho**: o projeto está com problemas.

  ![Com problemas](assets/burndown-red.png)

Para obter mais informações sobre essas condições do projeto, consulte [Visão geral da condição do projeto e do tipo de condição](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Quando a linha real se move verticalmente para cima, o trabalho foi adicionado ao projeto. Quando a linha se move verticalmente para baixo, o trabalho foi removido ou concluído para o projeto.

Abaixo do eixo x da visualização, você pode ver mais informações sobre como as tarefas e as horas (ou dias) foram alteradas em um determinado dia (o valor adicionado, o valor concluído e a diferença entre os dois).

Ver todas essas informações na visualização de Burndown ajuda a determinar:

* A integridade do projeto individual ao longo do tempo
* Como os problemas que surgiam (ou que afetavam o trabalho não planejado) afetaram o trabalho planejado
* Quais eventos estenderam seu projeto além da data de conclusão original

Para saber como obter os melhores dados para essa visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Exibir a visualização de Burndown

{{step1-to-analytics}}

1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![Selecionar datas](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre o uso do filtro de intervalo de datas, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se precisar limitar o conjunto de dados do projeto, selecione e aplique os filtros que deseja usar.

   Para obter mais informações sobre como adicionar filtros na Análise aprimorada, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Depois de adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois de sair da página ou do Workfront.

1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização para o início do intervalo de datas e arraste-o para o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas, e um filtro de período é criado automaticamente.

   ![Filtro de cronograma](assets/timeframe-filter-350x220.png)

1. Na visualização do Plano de voo ou Mapa de árvore do projeto, clique em um projeto para exibir mais informações.

   As visualizações Burndown e Tarefas em voo são exibidas.

   >[!NOTE]
   >
   >Para saber mais sobre essas outras visualizações, consulte:
   >
   >   * [Exibir a visualização de Plano de voo na Análise aprimorada](../enhanced-analytics/flight-plan-overview.md)
   >   * [Visualização do mapa de árvore do projeto na Análise aprimorada](../enhanced-analytics/project-treemap-overview.md)
   >   * [Visualização das Tarefas em andamento na Análise aprimorada](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. (Opcional) Altere a exibição de horas planejadas para **duração**.

   As horas planejadas são selecionadas por padrão.

   >[!NOTE]
   >
   >Selecionar **duração** altera todas as informações de horas para dias.\
   >![Burndown de duração](assets/duration-burndown-350x112.png)\
   >Para obter mais informações sobre duração na área Analítica aprimorada, consulte a seção &quot;Visualização de duração&quot; em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md#duration-view).

1. Clique em qualquer ponto no gráfico de linhas.

   A data exata é exibida, juntamente com informações adicionais sobre tarefas e horas, ou dias, para o dia selecionado, abaixo do gráfico.

   ![Detalhes do burndown](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Se a velocidade real for uma linha plana que roda ao longo do eixo x (em linha com 0 horas ou 0 dias) da visualização, isso significa que nenhuma hora planejada (ou dias) foi adicionada ao projeto.\
   >Se a velocidade real for uma linha plana acima do eixo x (em linha com um número de horas ou número de dias) que nunca cai, significa que nenhuma tarefa foi concluída dentro do período filtrado.

1. (Opcional) Para exportar os dados de visualização, clique no link **Exportar** ícone ![Ícone Exportar](assets/export.png) no canto superior direito da visualização e selecione o formato de exportação:

   * Gráfico (PNG)
   * Tabela de dados (XSLX)

1. (Opcional) Para ver detalhes sobre o progresso das tarefas no projeto selecionado, verifique a visualização Tarefas em andamento que aparece abaixo da visualização Burndown. Para obter mais informações, consulte [Visualização das Tarefas em andamento na Análise aprimorada](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md).
