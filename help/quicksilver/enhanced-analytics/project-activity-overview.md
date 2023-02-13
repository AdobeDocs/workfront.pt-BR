---
title: Exibir a visualização da atividade do projeto no Enhanced Analytics
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A visualização da atividade Projeto mostra uma exibição agregada das atividades no nível do projeto, as atividades de cada pessoa atribuída ao projeto, que ocorreram durante um período específico. É possível limitar o foco para entender as atividades em um projeto ou comparar as atividades do projeto com outros projetos no Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 1%

---

# Exibir a visualização da atividade do projeto no Enhanced Analytics

A visualização da atividade Projeto mostra uma exibição agregada das atividades no nível do projeto, as atividades de cada pessoa atribuída ao projeto, que ocorreram durante um período específico. É possível limitar o foco para entender as atividades em um projeto ou comparar as atividades do projeto com outros projetos no Adobe Workfront.

>[!NOTE]
>
>A visualização Atividade por equipe se comporta de forma semelhante a essa visualização, mas a visualização Atividade por equipe mostra a atividade da equipe inicial para todos os projetos.\
>Para obter informações sobre a visualização Atividade por equipe, consulte [Visualizar a Atividade por equipe na Análise aprimorada](../enhanced-analytics/activity-by-team-overview.md).

<!--WRITER bad link; there is no Activity by Team.png
[![](assets/project-activity-350x114.png)](../Resources/Images/Analytics/Activity by Team.png)
-->

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plano Workfront</a>*</td> 
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

## Entender a visualização da atividade do projeto

As atividades do projeto são exibidas em cores diferentes para resumir eventos específicos em um projeto durante um período de tempo:

* **Usuários conectados**: As caixas roxas mostram que as pessoas atribuídas ao projeto se conectaram no dia. Uma sombra mais escura indica um número maior de pessoas fazendo logon.

   ![](assets/project-activity-users-logged-in.png)

* **Alteração do status da tarefa**: Caixas rosa mostram que as pessoas alteraram o status de uma tarefa para o projeto no dia. Uma sombra mais escura indica um número maior de status de tarefa em alteração.

   ![](assets/project-activity-task-status-changes.png)

* **Tarefas concluídas**: Caixas azuis mostram que as pessoas concluíram uma tarefa para o projeto. Uma sombra mais escura indica um número maior de tarefas que estão sendo concluídas.

   ![](assets/project-activity-tasks-completed.png)

Passar o mouse sobre uma caixa mostra o número exato de vezes que a ação foi concluída em um determinado dia. Você pode selecionar um projeto para ver o detalhamento dessas atividades por cada colaborador individual no projeto.

Ver essas informações ajuda a determinar:

* A atividade em um projeto específico.
* A atividade de um projeto em comparação com outros.
* Quais usuários estão trabalhando em um projeto e com que frequência.

Para saber como obter os melhores dados para essa visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizar a atividade do projeto

1. Clique no ícone do Menu principal ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre como usar o filtro de intervalo de datas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Se você selecionar um intervalo de datas para um período superior a 3 meses, a visualização da atividade do projeto não exibirá dados.

1. (Condicional) Se precisar limitar o conjunto de dados do projeto, selecione e aplique os filtros que deseja usar.

   Para obter mais informações sobre como adicionar filtros nas Análises aprimoradas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Após adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois que você sai da página ou faz logoff do Workfront.

1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização do início do intervalo de datas e arraste até o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas, e um filtro de período é criado.

   ![](assets/timeframe-filter-350x220.png)

1. (Opcional) Para alterar a forma como os projetos são classificados, clique no botão **Classificar por** selecione uma nova opção de classificação:

   * **A - Z**
   * **Z - A**
   * **Data de conclusão planejada**
   * **Data de início planejada**

   Todas as outras visualizações na página são atualizadas para corresponder à seleção de classificação.

1. (Condicional) Se houver mais de 50 projetos em seu conjunto de dados, use as setas no canto inferior esquerdo da visualização para navegar de um grupo de 50 projetos para o próximo.

   Todas as outras visualizações na página são atualizadas para corresponder à seleção da página.

   ![](assets/pagination-350x118.png)

1. Clique em um projeto na visualização para ver mais detalhes do projeto.

   A lista é expandida para exibir as atividades de cada colaborador individual no projeto.

1. Passe o mouse sobre uma caixa para ver a data em que os usuários concluíram uma ação, bem como o número de vezes em que a ação foi concluída nesse dia.

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. (Opcional) Para exportar os dados de visualização, clique no botão **Ícone Exportar** ![](assets/export.png) no canto superior direito da visualização, selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de dados (XSLX)**

