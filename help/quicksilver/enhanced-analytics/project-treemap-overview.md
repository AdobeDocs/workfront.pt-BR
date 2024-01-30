---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Visualização do mapa de árvore do projeto na Análise aprimorada
description: A visualização do mapa de árvore do projeto é uma exibição de horas, ou dias, que foram trabalhadas em uma janela de tempo específica em comparação a outros esforços de trabalho em tamanho. Isso ajuda você a entender quanto tempo as pessoas dedicaram a um projeto.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Visualização do mapa de árvore do projeto na Análise aprimorada

<!-- Audited: 12/2023 -->

A visualização do mapa de árvore do projeto é uma exibição de horas, ou dias, que foram trabalhadas em uma janela de tempo específica em comparação a outros esforços de trabalho em tamanho. Isso ajuda você a entender quanto tempo as pessoas dedicaram a um projeto.

![](assets/project-treemap-350x126.png){width="700"}

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plano do Adobe Workfront</a></td> 
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

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender a visualização do mapa de árvore do projeto

As caixas na visualização do mapa de árvore do projeto representam projetos e o tamanho das caixas mostra uma comparação de quanto tempo foi gasto em projetos diferentes. Quanto maior a caixa, mais tempo é gasto com o projeto.

A visualização do mapa de árvore do projeto é composta de:

* **Caixas menores, azuis claras**: projetos com menos horas ou dias são exibidos como caixas menores com uma cor azul-claro.

  ![](assets/project-treemap-smaller-box.png)

* **Caixas azuis escuras e maiores**: os projetos com mais horas ou dias são exibidos como caixas maiores com uma cor azul escura.

  ![](assets/project-treemap-larger-box-350x205.png)

* **Caixas azuis de tamanho médio**: os projetos que se encaixam entre as duas categorias são exibidos como caixas de tamanho médio com uma sombra de azul entre as cores azul escuro e azul claro. Há 3 tons possíveis de azul para as caixas de tamanho médio.

A legenda no lado direito mostra um detalhamento de horas concluídas para cada sombra de azul. Essa legenda é dinâmica e é atualizada de acordo com os dados.

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Se você estiver observando a visualização do mapa de árvore do projeto por duração em vez de por horas planejadas, essa legenda mostra um detalhamento dos dias trabalhados para cada sombra de azul.\
>![](assets/project-treemap-days-worked.png)>

Ver essas informações ajuda a determinar:

* A prioridade dos itens sendo trabalhados durante o intervalo de datas selecionado.
* Em que equipes estão gastando tempo.
* Se as equipes estão focadas nas coisas certas.
* Quando um projeto específico é clicado, quanto o escopo de um projeto mudou nesse período de tempo.

Para saber como obter os melhores dados para essa visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Exibir a visualização do mapa de árvore do projeto

1. Clique no ícone Menu principal ![](assets/main-menu-icon-16x12.png)e selecione **Analytics**.
1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre o uso do filtro de intervalo de datas, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se precisar limitar o conjunto de dados do projeto, selecione e aplique os filtros que deseja usar.

   Para obter mais informações sobre como adicionar filtros na Análise aprimorada, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Depois de adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois de sair da página ou do Workfront.

1. (Opcional) Para alterar a forma como os projetos são classificados, clique no **Classificar por** no canto superior direito da visualização Mapa de árvore do projeto, em seguida, selecione uma nova opção de classificação:

   * **A - Z**
   * **Z - A**
   * **Data de término planejada**
   * **Data de início planejada**

   Todas as outras visualizações na página são atualizadas para corresponder à sua seleção de classificação.

1. (Condicional) Se houver mais de 50 projetos no seu conjunto de dados, use as setas no canto inferior esquerdo da visualização para navegar de um grupo de 50 projetos para o próximo.

   Todas as outras visualizações na página são atualizadas para corresponder à seleção da página.

   ![](assets/pagination-350x118.png)

1. (Opcional) Altere a exibição de de **horas planejadas** para **duração**.

   As horas planejadas são selecionadas por padrão.

1. Passe o mouse sobre um projeto para ver a condição do projeto, bem como o número total de horas planejadas, o número total de horas concluídas e o número médio de horas gastas no projeto por dia.

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Se você selecionou a variável **duração** você verá os seguintes detalhes de duração:
   >
   >* **Cronograma planejado**: O número de dias planejados para concluir o projeto.
   >* **Dias trabalhados**: a duração planejada para cada tarefa que foi concluída dentro do intervalo de datas selecionado na parte superior, dividida pelo número de horas em um dia.
   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >Para obter mais informações sobre duração, consulte a seção &quot;Exibição de duração&quot; em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Opcional) Para exportar os dados de visualização, clique no link **Ícone Exportar** ![](assets/export.png) no canto superior direito da visualização, selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de dados (XSLX)**

1. Clique em um projeto para abrir as visualizações Burndown e Tarefas em andamento para obter um insight mais profundo sobre como as tarefas e as horas ou dias contribuíram para o tamanho de um projeto.

Para obter mais informações sobre a visualização de Burndown, consulte [Exibir a visualização de Burndown na análise aprimorada](../enhanced-analytics/burndown-overview.md). Para obter mais informações sobre a visualização Tarefas em andamento, consulte [Visualização das Tarefas em andamento na Análise aprimorada](../enhanced-analytics/tasks-in-flight-overview.md).

