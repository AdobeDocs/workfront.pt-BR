---
title: Exibir a visualização de Plano de voo na Análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A visualização do Plano de voo mostra quantos projetos (dentro dos critérios de filtro aplicados) estavam em andamento, quais alterações de condição ocorreram durante a vida desses projetos e o quão próximos esses projetos respeitaram os prazos de conclusão planejados.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 4%

---

# Exibir a visualização de Plano de voo na Análise aprimorada

>[!IMPORTANT]
>
>O Analytics aprimorado será removido do Workfront na semana de 26 de maio. O Workfront Data Connect é uma solução nova e alternativa e pode ser usada para replicar qualquer visualização do Enhanced Analytics que você usa atualmente. <br>Consulte o [guia de descontinuação do Enhanced Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) para obter mais informações.


A visualização do Plano de voo mostra quantos projetos (dentro dos critérios de filtro aplicados) estavam em andamento, quais alterações de condição ocorreram durante a vida desses projetos e o quão próximos esses projetos respeitaram os prazos de conclusão planejados.

![Plano de voo](assets/flight-plan-350x132.png)

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
   <td> <p>Visualizar acesso aos projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso.<br>Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar acesso ao projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; na [Visão geral do Enhanced Analytics](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender a visualização do plano de voo

Na duração real de um projeto, você pode ver apenas as seguintes condições do projeto:

* No Prazo
* Em Risco
* Com problemas

Para saber mais sobre as condições do projeto, consulte [Visão Geral da Condição do Projeto e do Tipo de Condição](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

A visualização Plano de voo mostra os seguintes detalhes do projeto:

* **Duração planejada**: a linha azul horizontal representa o comprimento planejado do projeto, com os triângulos em cada extremidade da linha indicando a data inicial e a data final.

  ![Duração planejada](assets/planned-duration-line-350x37.png)

* **Duração real**: a linha espessa colorida abaixo da duração planejada representa a duração real do projeto. A cor da linha muda dependendo da condição do projeto naquele momento específico da vida útil do projeto.

  ![Duração real](assets/actual-duration-line.png)

* **Condição real**: a linha espessa e colorida também mostra a condição de um projeto em momentos diferentes. A cor da linha muda dependendo da condição do projeto:

   * **Verde**: No Destino
   * **Laranja**: Em Risco
   * **Vermelho**: Com Problemas

  ![Condição real](assets/actual-condition-color.png)

Ao passar o mouse sobre uma linha do projeto na visualização Plano de voo, é possível ver informações sobre o período planejado do projeto, a condição atual do projeto e, se aplicável, a condição personalizada. Para obter uma visualização mais detalhada do que pode ter afetado a duração ou a condição, você pode consultar as outras visualizações na área Analítica aprimorada.

Essas informações ajudam a determinar:

* Quais eventos estendem um projeto além da data de conclusão planejada original.
* Quando um projeto começa a ter problemas.
* Quantos projetos estão abertos no mesmo período.
* Quantos projetos estão ativos.
* Quais projetos precisam de mais atenção ou suporte.

Para obter informações sobre como obter os melhores dados para esta visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Exibir a visualização de Plano de voo

1. Clique no ícone **Menu principal** ![Ícone do menu principal](assets/main-menu-icon-16x12.png) e selecione **Analytics**.
1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![Selecionar intervalo de datas](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre como usar o filtro de intervalo de datas, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se precisar limitar o conjunto de dados do projeto, selecione e aplique os filtros que deseja usar.

   Para obter mais informações sobre como adicionar filtros na Análise aprimorada, consulte [Aplicar filtros na Análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Depois de adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois de sair da página ou do Workfront.

1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização para o início do intervalo de datas e arraste até o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas e um filtro de período é criado.

   ![Filtro de cronograma](assets/timeframe-filter-350x220.png)

1. (Opcional) Para alterar a forma como os projetos são classificados, clique no menu **Classificar por** no canto superior direito da visualização Plano de voo e selecione uma nova opção de classificação:

   * **A - Z**
   * **Z - A**
   * **Data de conclusão planejada**
   * **Data de início planejada**

   Todas as outras visualizações na página são atualizadas para corresponder à sua seleção de classificação.

1. (Condicional) Se houver mais de 50 projetos no seu conjunto de dados, use as setas no canto inferior esquerdo da visualização para navegar de um grupo de 50 projetos para o próximo.

   Todas as outras visualizações na página são atualizadas para corresponder à seleção da página.

   ![Paginação](assets/pagination-350x118.png)

1. Passe o mouse sobre o gráfico de barras do projeto para ver a linha de data azul, bem como os seguintes detalhes:

   * Linha do tempo planejada
   * Condição atual
   * Condição personalizada (se aplicável)

   ![Gráfico de barras do projeto](assets/project-bar-graph-350x143.png)

1. (Opcional) Para exportar os dados de visualização, clique no ícone **Exportar** ![Ícone Exportar](assets/export.png) no canto superior direito da visualização e selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de Dados (XSLX)**

1. Para ver mais informações do projeto, clique em um projeto na visualização para abrir as visualizações Burndown e Tarefas em andamento.

   Essas visualizações podem ajudar você a obter um insight mais profundo sobre o que fez o projeto sair do caminho. Elas também facilitam o check-in de um projeto em andamento.\
   Para obter mais informações sobre a visualização de Burndown, consulte [Exibir a visualização de Burndown na análise aprimorada](../enhanced-analytics/burndown-overview.md). Para obter mais informações sobre as Tarefas na visualização em andamento, consulte [Exibir as Tarefas na visualização em andamento na análise aprimorada](../enhanced-analytics/tasks-in-flight-overview.md).

