---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Visualizar o mapa de árvore do projeto no Enhanced Analytics
description: A visualização do mapa de árvore do projeto é uma visualização de horas (ou dias) que foram trabalhadas em uma janela de tempo específica em comparação a outros esforços de trabalho em tamanho. Isso ajuda você a entender o tempo que as pessoas dedicaram a um projeto.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 1%

---

# Visualizar o mapa de árvore do projeto no Enhanced Analytics

A visualização do mapa de árvore do projeto é uma visualização de horas (ou dias) que foram trabalhadas em uma janela de tempo específica em comparação a outros esforços de trabalho em tamanho. Isso ajuda você a entender o tempo que as pessoas dedicaram a um projeto.

![](assets/project-treemap-350x126.png)

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
   <td> <p>Exibir</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender a visualização do mapa de árvore do projeto

As caixas da visualização do mapa de árvore do projeto representam projetos e o tamanho das caixas mostra uma comparação de quanto tempo foi gasto em diferentes projetos. Quanto maior a caixa, mais tempo gasto no projeto.

A visualização do mapa de árvore do projeto é composta de:

* **Caixas azuis leves menores**: Projetos com menos horas - ou dias - são exibidos como caixas menores com uma cor azul clara.

   ![](assets/project-treemap-smaller-box.png)

* **Caixas maiores, azuis escuras**: Projetos com mais horas — ou dias — são exibidos como caixas maiores com uma cor azul escuro.

   ![](assets/project-treemap-larger-box-350x205.png)

* **Caixas azuis de médio porte**: Os projetos que se encaixam entre as duas categorias são exibidos como caixas de tamanho médio com uma sombra de azul entre as cores azul escuro e azul claro. Há três pás possíveis de azul para as caixas de tamanho médio.

A legenda no lado direito mostra um detalhamento de horas concluídas para cada sombra de azul. Essa legenda é dinâmica e é atualizada de acordo com os dados.

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Se você estiver olhando para a visualização do mapa de árvore do projeto por duração em vez de por horas planejadas, esta legenda mostra um detalhamento dos dias trabalhados para cada sombra de azul.\
>![](assets/project-treemap-days-worked.png)>

Ver essas informações ajuda a determinar:

* A prioridade dos itens que estão sendo trabalhados durante o intervalo de datas selecionado.
* Com que equipes estão gastando tempo.
* Se as equipes estão se concentrando nas coisas certas.
* Quando um projeto específico é clicado, o quanto o escopo de um projeto foi alterado durante esse período.

Para saber como obter os melhores dados para essa visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizar o mapa de árvore do projeto

1. Clique no ícone do Menu principal ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre como usar o filtro de intervalo de datas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se precisar limitar o conjunto de dados do projeto, selecione e aplique os filtros que deseja usar.

   Para obter mais informações sobre como adicionar filtros nas Análises aprimoradas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Após adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois que você sai da página ou faz logoff do Workfront.

1. (Opcional) Para alterar a forma como os projetos são classificados, clique no botão **Classificar por** no canto superior direito da visualização do mapa de árvore do projeto, selecione uma nova opção de classificação:

   * **A - Z**
   * **Z - A**
   * **Data de conclusão planejada**
   * **Data de início planejada**

   Todas as outras visualizações na página são atualizadas para corresponder à seleção de classificação.

1. (Condicional) Se houver mais de 50 projetos em seu conjunto de dados, use as setas no canto inferior esquerdo da visualização para navegar de um grupo de 50 projetos para o próximo.

   Todas as outras visualizações na página são atualizadas para corresponder à seleção da página.

   ![](assets/pagination-350x118.png)

1. (Opcional) Altere a exibição de **horas planejadas** para **duration**.

   As horas planejadas são selecionadas por padrão.

1. Passe o mouse sobre um projeto para ver a condição do projeto, bem como o número total de horas planejadas, o número total de horas concluídas e o número médio de horas gastas no projeto por dia.

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Se você selecionou a variável **duration** , você verá os seguintes detalhes de duração:
   >
   >* **Cronograma planejado**: O número de dias planejados para concluir o projeto.
   >* **Dias trabalhados**: A duração planejada para cada tarefa que foi concluída dentro do intervalo de datas selecionado na parte superior, dividido pelo número de horas em um dia.

   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >Para obter mais informações sobre duração, consulte a seção &quot;Visualização de duração&quot; em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Opcional) Para exportar os dados de visualização, clique no botão **Ícone Exportar** ![](assets/export.png) no canto superior direito da visualização, selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de dados (XSLX)**

1. Clique em um projeto para abrir as visualizações de Burndown e Tasks in flight para obter uma visão mais profunda de como as tarefas e horas, ou dias, contribuíram para o tamanho de um projeto.

Para obter mais informações sobre a visualização de Detalhamento, consulte [Visualizar a visualização do Detalhamento na análise aprimorada](../enhanced-analytics/burndown-overview.md). Para obter mais informações sobre as Tarefas em andamento, consulte [Visualizar as Tarefas em andamento na análise aprimorada](../enhanced-analytics/tasks-in-flight-overview.md).

