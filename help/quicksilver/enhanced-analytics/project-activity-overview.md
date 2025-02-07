---
title: Exibir a visualização da atividade Projeto na Análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A visualização da atividade Projeto mostra uma exibição agregada das atividades no nível do projeto (as atividades de cada pessoa atribuídas ao projeto) que ocorreram durante um período específico. Você pode limitar seu foco para entender as atividades em um projeto ou pode comparar as atividades do projeto com outros projetos no Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 325334010d5f1206931cc9ace67f9511d614ffca
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 8%

---

# Exibir a visualização da atividade Projeto na Análise aprimorada

<!-- Audited: 12/2023 -->

A visualização da atividade Projeto mostra uma exibição agregada das atividades no nível do projeto (as atividades de cada pessoa atribuídas ao projeto) que ocorreram durante um período específico. Você pode limitar seu foco para entender as atividades em um projeto ou pode comparar as atividades do projeto com outros projetos no Adobe Workfront.

>[!NOTE]
>
>A visualização Atividade por equipe se comporta de forma semelhante a essa visualização, mas a visualização Atividade por equipe mostra a atividade da equipe inicial para todos os projetos.\
>Para obter informações sobre a visualização Atividade por equipe, consulte [Exibir a visualização Atividade por equipe na análise aprimorada](../enhanced-analytics/activity-by-team-overview.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plano do Workfront</a></td> 
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

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; na [Visão geral do Enhanced Analytics](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender a visualização da atividade de Projeto

As atividades do projeto são exibidas em cores diferentes para resumir eventos específicos em um projeto durante um período de tempo:

* **Usuários conectados**: as caixas roxas mostram que as pessoas atribuídas ao projeto estão conectadas nesse dia. Um tom mais escuro indica um número maior de pessoas que fizeram logon.

  ![Usuários logados](assets/project-activity-users-logged-in.png)

* **Alteração do status da tarefa**: as caixas de cor-de-rosa mostram que as pessoas alteraram o status de uma tarefa para o projeto nesse dia. Um tom mais escuro indica um número maior de alterações de status de tarefas.

  ![Alteração do status da tarefa](assets/project-activity-task-status-changes.png)

* **Tarefas concluídas**: as caixas azuis mostram que as pessoas concluíram uma tarefa para o projeto. Um tom mais escuro indica um maior número de tarefas concluídas.

  ![Tarefas concluídas](assets/project-activity-tasks-completed.png)

Passar o mouse sobre uma caixa mostra o número exato de vezes que a ação foi concluída em um determinado dia. Você pode selecionar um projeto para ver um detalhamento dessas atividades por cada colaborador individual no projeto.

Essas informações ajudam a determinar:

* A atividade em um projeto específico.
* A atividade de um projeto em comparação a outros projetos.
* Quais usuários estão trabalhando em um projeto e com que frequência.

Para saber como obter os melhores dados para esta visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Exibir a visualização da atividade Projeto

1. Clique no ícone Menu Principal ![ícone Menu principal](assets/main-menu-icon-16x12.png) e selecione **Analytics**.
1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![Selecionar intervalo de datas](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre como usar o filtro de intervalo de datas, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Se você selecionar um intervalo de datas para um período superior a 3 meses, a visualização da atividade Projeto não exibirá dados.

1. (Condicional) Se precisar limitar o conjunto de dados do projeto, selecione e aplique os filtros que deseja usar.

   Para obter mais informações sobre como adicionar filtros na Análise aprimorada, consulte [Aplicar filtros na Análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Depois de adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois de sair da página ou do Workfront.

1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização para o início do intervalo de datas e arraste até o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas e um filtro de período é criado.

   ![Filtro de cronograma](assets/timeframe-filter-350x220.png)

1. (Opcional) Para alterar a forma como os projetos são classificados, clique no menu **Classificar por** e selecione uma nova opção de classificação:

   * **A - Z**
   * **Z - A**
   * **Data de conclusão planejada**
   * **Data de início planejada**

   Todas as outras visualizações na página são atualizadas para corresponder à sua seleção de classificação.

1. (Condicional) Se houver mais de 50 projetos no seu conjunto de dados, use as setas no canto inferior esquerdo da visualização para navegar de um grupo de 50 projetos para o próximo.

   Todas as outras visualizações na página são atualizadas para corresponder à seleção da página.

   ![Paginação](assets/pagination-350x118.png)

1. Clique em um projeto na visualização para ver mais detalhes do projeto.

   A lista é expandida para exibir as atividades de cada colaborador individual no projeto.

1. Passe o mouse sobre uma caixa para ver a data em que os usuários concluíram uma ação, bem como o número de vezes que a ação foi concluída para esse dia.

   ![Pop-up de atividade](assets/project-activity-activity-pop-up-350x137.png)

1. (Opcional) Para exportar os dados de visualização, clique no **ícone Exportar** ![ícone Exportar](assets/export.png) no canto superior direito da visualização e selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de Dados (XSLX)**

