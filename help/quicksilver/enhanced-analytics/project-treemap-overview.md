---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Visualização do mapa de árvore do projeto na Análise aprimorada
description: A visualização do mapa de árvore do projeto é uma exibição de horas, ou dias, que foram trabalhadas em uma janela de tempo específica em comparação a outros esforços de trabalho em tamanho. Isso ajuda você a entender quanto tempo as pessoas dedicaram a um projeto.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 2%

---

# Visualização do mapa de árvore do projeto na Análise aprimorada

>[!IMPORTANT]
>
>O Analytics aprimorado foi removido do Workfront em 27 de maio. O Workfront Data Connect é uma solução nova e alternativa e pode ser usada para replicar qualquer visualização do Enhanced Analytics que você usa atualmente. <br>Consulte o [guia de descontinuação do Enhanced Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) para obter mais informações.


<!-- Audited: 12/2023 -->

A visualização do mapa de árvore do projeto é uma exibição de horas, ou dias, que foram trabalhadas em uma janela de tempo específica em comparação a outros esforços de trabalho em tamanho. Isso ajuda você a entender quanto tempo as pessoas dedicaram a um projeto.

![Mapa de árvore do projeto](assets/project-treemap-350x126.png){width="700"}

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">plano do Adobe Workfront</a></td> 
   <td> <p>Business ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a></td> 
   <td>   <p>Novo:</p> 
   <ul><li>Leve ou Superior</li></ul>
   <p>Atual:</p>
   <ul><li>Revisar ou superior</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualizar acesso aos projetos</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; na [Visão geral do Enhanced Analytics](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender a visualização do mapa de árvore do projeto

As caixas na visualização do mapa de árvore do projeto representam projetos e o tamanho das caixas mostra uma comparação de quanto tempo foi gasto em projetos diferentes. Quanto maior a caixa, mais tempo é gasto com o projeto.

A visualização do mapa de árvore do projeto é composta de:

* **Caixas menores e azuis claras**: os projetos que têm menos horas ou dias são exibidos como caixas menores com uma cor azul-claro.

  ![Caixa menor](assets/project-treemap-smaller-box.png)

* **Caixas azuis escuras e maiores**: os projetos que têm mais horas ou dias são exibidos como caixas maiores com uma cor azul escura.

  ![Caixa maior](assets/project-treemap-larger-box-350x205.png)

* **Caixas azuis de tamanho Medium**: os projetos que se encaixam entre as duas categorias são exibidos como caixas de tamanho médio com uma sombra de azul entre as cores azul escuro e azul claro. Há 3 tons possíveis de azul para as caixas de tamanho médio.

A legenda no lado direito mostra um detalhamento de horas concluídas para cada sombra de azul. Essa legenda é dinâmica e é atualizada de acordo com os dados.

![Horas do mapa de árvore concluídas](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Se você estiver observando a visualização do mapa de árvore do projeto por duração em vez de por horas planejadas, essa legenda mostra um detalhamento dos dias trabalhados para cada sombra de azul.\
>![Dias trabalhados do Treemap](assets/project-treemap-days-worked.png)>

Essas informações ajudam a determinar:

* A prioridade dos itens nos quais se trabalhou durante o intervalo de datas selecionado.
* Em que equipes estão gastando tempo.
* Se as equipes estão focadas nas coisas certas.
* Quando um projeto específico é clicado, quanto o escopo de um projeto mudou nesse período de tempo.

Para saber como obter os melhores dados para esta visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Exibir a visualização do mapa de árvore do projeto

1. Clique no ícone Menu Principal ![ícone Menu principal](assets/main-menu-icon-16x12.png) e selecione **Analytics**.
1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![Selecionar intervalo de datas](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre como usar o filtro de intervalo de datas, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se precisar limitar o conjunto de dados do projeto, selecione e aplique os filtros que deseja usar.

   Para obter mais informações sobre como adicionar filtros na Análise aprimorada, consulte [Aplicar filtros na Análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Depois de adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois de sair da página ou do Workfront.

1. (Opcional) Para alterar a forma como os projetos são classificados, clique no menu **Classificar por** no canto superior direito da visualização do mapa de árvore do projeto e selecione uma nova opção de classificação:

   * **A - Z**
   * **Z - A**
   * **Data de conclusão planejada**
   * **Data de início planejada**

   Todas as outras visualizações na página são atualizadas para corresponder à sua seleção de classificação.

1. (Condicional) Se houver mais de 50 projetos no seu conjunto de dados, use as setas no canto inferior esquerdo da visualização para navegar de um grupo de 50 projetos para o próximo.

   Todas as outras visualizações na página são atualizadas para corresponder à seleção da página.

   ![Paginação](assets/pagination-350x118.png)

1. (Opcional) Altere a exibição de **horas planejadas** para **duração**.

   As horas planejadas são selecionadas por padrão.

1. Passe o mouse sobre um projeto para ver a condição do projeto, bem como o número total de horas planejadas, o número total de horas concluídas e o número médio de horas gastas no projeto por dia.

   ![Detalhes do projeto do Treemap](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Se você selecionou a exibição **duração**, verá os seguintes detalhes de duração:
   >
   >* **Período planejado**: o número de dias planejados para concluir o projeto.
   >* **Dias trabalhados**: a duração planejada para cada tarefa que foi concluída dentro do intervalo de datas selecionado na parte superior, dividida pelo número de horas em um dia.
   >   
   >![Duração do Treemap](assets/duration-treemap-350x159.png)
   >
   >Para obter mais informações sobre duração, consulte a seção &quot;Exibição de duração&quot; na [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Opcional) Para exportar os dados de visualização, clique no **ícone Exportar** ![ícone Exportar](assets/export.png) no canto superior direito da visualização e selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de Dados (XSLX)**

1. Clique em um projeto para abrir as visualizações Burndown e Tarefas em andamento para obter uma insight mais profunda de como as tarefas e as horas — ou dias — contribuíram para o tamanho de um projeto.

Para obter mais informações sobre a visualização de Burndown, consulte [Exibir a visualização de Burndown na análise aprimorada](../enhanced-analytics/burndown-overview.md). Para obter mais informações sobre as Tarefas na visualização em andamento, consulte [Exibir as Tarefas na visualização em andamento na análise aprimorada](../enhanced-analytics/tasks-in-flight-overview.md).

