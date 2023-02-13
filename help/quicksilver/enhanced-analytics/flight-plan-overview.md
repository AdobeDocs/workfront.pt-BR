---
title: Exibir a visualização do Plano de voo na análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A visualização do plano de voo mostra quantos projetos (dentro dos critérios de filtragem aplicados) estavam em andamento, quais mudanças de condição ocorreram ao longo da vida desses projetos e o grau de cumprimento dos prazos de conclusão previstos por esses projetos.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# Exibir a visualização do Plano de voo na análise aprimorada

A visualização do plano de voo mostra quantos projetos (dentro dos critérios de filtragem aplicados) estavam em andamento, quais mudanças de condição ocorreram ao longo da vida desses projetos e o grau de cumprimento dos prazos de conclusão previstos por esses projetos.

![](assets/flight-plan-350x132.png)

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
   <td> <p>Visualizar o acesso a Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso.<br>Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar o acesso ao projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender a visualização do plano de voo

Na duração real de um projeto, você pode ver apenas as seguintes condições do projeto:

* No Prazo
* Em Risco
* Com problemas

Para saber mais sobre as condições do projeto, consulte [Visão geral da condição do projeto e do tipo de condição](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

A visualização Plano de voo mostra os seguintes detalhes do projeto:

* **Duração planejada**: A linha azul horizontal representa o comprimento planejado do projeto, com os triângulos em qualquer extremidade da linha indicando a data inicial e a data final.

   ![](assets/planned-duration-line-350x37.png)

* **Duração real**: A linha espessa e colorida abaixo da duração planejada representa a duração real do projeto. A cor da linha muda de acordo com a condição do projeto nesse momento específico da vida do projeto.

   ![](assets/actual-duration-line.png)

* **Condição real**: A linha espessa e colorida também mostra a condição de um projeto em momentos diferentes no tempo. A cor da linha muda de acordo com a condição do projeto:

   * **Verde**: No Target
   * **Laranja**: Em Risco
   * **Vermelho**: Em problemas

   ![](assets/actual-condition-color.png)

Ao passar o cursor do mouse sobre uma linha de projeto na visualização Plano de voo, você pode ver informações sobre o período planejado do projeto, a condição do projeto atual e, se aplicável, a condição personalizada. Para obter uma visualização mais detalhada do que pode ter afetado a duração ou a condição, consulte as outras visualizações na área de Análise aprimorada .

Ver essas informações ajuda a determinar:

* Quais eventos estendem um projeto após a data original de conclusão planejada.
* Quando um projeto começa a enfrentar problemas.
* Quantos projetos estão abertos no mesmo período de tempo.
* Quantos projetos estão ativos.
* Quais projetos necessitam de mais atenção ou apoio.

Para obter informações sobre como obter os melhores dados para esta visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Exibir a visualização do plano de voo

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre como usar o filtro de intervalo de datas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se precisar limitar o conjunto de dados do projeto, selecione e aplique os filtros que deseja usar.

   Para obter mais informações sobre como adicionar filtros nas Análises aprimoradas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Após adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois que você sai da página ou faz logoff do Workfront.

1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização do início do intervalo de datas e arraste até o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas, e um filtro de período é criado.

   ![](assets/timeframe-filter-350x220.png)

1. (Opcional) Para alterar a forma como os projetos são classificados, clique no botão **Classificar por** no canto superior direito da visualização Plano de voo, selecione uma nova opção de classificação:

   * **A - Z**
   * **Z - A**
   * **Data de conclusão planejada**
   * **Data de início planejada**

   Todas as outras visualizações na página são atualizadas para corresponder à seleção de classificação.

1. (Condicional) Se houver mais de 50 projetos em seu conjunto de dados, use as setas no canto inferior esquerdo da visualização para navegar de um grupo de 50 projetos para o próximo.

   Todas as outras visualizações na página são atualizadas para corresponder à seleção da página.

   ![](assets/pagination-350x118.png)

1. Passe o mouse sobre o gráfico de barras do projeto para ver a linha de data azul, bem como os seguintes detalhes:

   * Linha do tempo planejada
   * Condição atual
   * Condição personalizada (se aplicável)

   ![](assets/project-bar-graph-350x143.png)

1. (Opcional) Para exportar os dados de visualização, clique no botão **Exportar** ícone ![](assets/export.png) no canto superior direito da visualização, selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de dados (XSLX)**

1. Para ver mais informações do projeto, clique em um projeto na visualização para abrir as visualizações de Burndown e Tasks in flight .

   Essas visualizações podem ajudar você a obter mais informações sobre o que fez com que o projeto saísse do controle. Também facilitam o check-in de um projeto em andamento.\
   Para obter mais informações sobre a visualização de Detalhamento, consulte [Visualizar a visualização do Detalhamento na análise aprimorada](../enhanced-analytics/burndown-overview.md). Para obter mais informações sobre as Tarefas em andamento, consulte [Visualizar as Tarefas em andamento na análise aprimorada](../enhanced-analytics/tasks-in-flight-overview.md).

