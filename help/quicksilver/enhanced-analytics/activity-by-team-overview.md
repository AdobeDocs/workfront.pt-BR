---
title: Visualizar a Atividade por equipe na Análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A visualização Atividade por equipe mostra atividades que acontecem durante um período específico para uma equipe inicial, permitindo que você entenda como diferentes equipes residenciais gastaram seu tempo no Adobe Workfront. Dependendo de como sua equipe inicial está configurada no Workfront, essa visualização pode oferecer diferentes insights e responder a perguntas diferentes.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Visualizar a Atividade por equipe na Análise aprimorada

A visualização Atividade por equipe mostra atividades que acontecem durante um período específico para uma equipe inicial, permitindo que você entenda como diferentes equipes residenciais gastaram seu tempo no Adobe Workfront. Dependendo de como sua equipe inicial está configurada no Workfront, essa visualização pode oferecer diferentes insights e responder a perguntas diferentes.

>[!NOTE]
>
>A visualização da atividade Projeto é semelhante a essa visualização, mas exibe a atividade com base nas pessoas atribuídas aos projetos em vez das pessoas atribuídas a uma equipe inicial.\
>Para obter informações sobre a visualização da atividade do projeto, consulte [Exibir a visualização da atividade do projeto no Enhanced Analytics](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png)

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

## Entender a atividade por visualização de equipe

As diferentes atividades são exibidas em cores diferentes para resumir eventos específicos durante o período de tempo filtrado:

* **Usuários conectados**: Caixas roxas mostram que pessoas na equipe de casa fizeram logon naquele dia. Uma sombra mais escura indica um número maior de pessoas fazendo logon.

   ![](assets/project-activity-users-logged-in.png)

* **Alteração do status da tarefa**: Caixas rosa mostram que as pessoas na equipe inicial alteraram o status de uma tarefa nesse dia. Uma sombra mais escura indica um número maior de status de tarefa em alteração.

   ![](assets/project-activity-task-status-changes.png)

* **Tarefas concluídas**: Caixas azuis mostram que as pessoas da equipe de casa concluíram uma tarefa naquele dia. Uma sombra mais escura indica um número maior de tarefas que estão sendo concluídas.

   ![](assets/project-activity-tasks-completed.png)

Passar o mouse sobre uma caixa mostra o número exato de vezes que a ação foi concluída em um determinado dia. Você pode selecionar uma equipe para ver o detalhamento dessas atividades por cada pessoa na equipe inicial.

Ver essas informações ajuda a determinar:

* Quais atividades estão ocorrendo dentro de uma equipe doméstica e a que taxa.
* As equipes domésticas estão sendo sobretrabalhadas ou estão usando mais o sistema.
* Se a distribuição do trabalho for apropriada para a equipe doméstica.

Para saber como obter os melhores dados para essa visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualização da atividade por equipe

1. Clique no ícone do Menu principal ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. No painel esquerdo, selecione **Pessoas**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre como usar o filtro de intervalo de datas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se você não definiu seu filtro Equipe , adicione o filtro Equipe e selecione cada equipe para a qual deseja visualizar os dados.

   Para obter mais informações sobre como adicionar filtros nas Análises aprimoradas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Após adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois que você sai da página ou faz logoff do Workfront.

1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização do início do intervalo de datas e arraste até o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas, e um filtro de período é criado.

   ![](assets/timeframe-filter-350x220.png)

1. Clique em um nome de equipe

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   para ver mais detalhes das atividades concluídas pela equipe inicial.

   A lista é expandida para exibir as atividades de cada pessoa atribuída à equipe inicial.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. Passe o mouse sobre uma caixa colorida para ver a data em que os usuários concluíram uma ação, bem como o número de vezes em que a ação foi concluída nesse dia.

   As cores mais escuras indicam maior atividade.

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Opcional) Para exportar os dados de visualização, clique no ícone Exportar ![](assets/export.png) no canto superior direito da visualização, selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de dados (XSLX)**

