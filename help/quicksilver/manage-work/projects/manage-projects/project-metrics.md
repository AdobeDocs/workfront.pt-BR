---
content-type: overview;how-to-procedural
product-area: projects
keywords: analytics,métricas,projeto,tarefas,destinatário,concluído,status,vencido,futuro
navigation-topic: manage-projects
title: Entender as métricas do projeto
description: As métricas do projeto oferecem uma visualização do que está acontecendo em um projeto, permitindo que você avalie rapidamente as necessidades e o status de um projeto. Saiba como interpretar a área Métricas no painel esquerdo de um projeto.
author: Alina
feature: Work Management
exl-id: 54c2a59d-9f6b-4126-9526-5169aeda8517
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1206'
ht-degree: 2%

---

# Entender as métricas do projeto

As métricas do projeto fornecem uma visualização geral em formato de gráfico sobre o desempenho de um projeto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Leve ou superior</p>
   <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualizar acesso aos projetos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para um projeto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>New: Light or higher </p>
   <p>Current: Review or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>View access to Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a project</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Pré-requisitos

Para acessar a área Métricas no painel esquerdo de um projeto, você deve:

* Ative a opção Métricas do painel esquerdo na área Projetos do modelo de layout.

  Para saber como um administrador do Workfront ou um administrador de grupo pode personalizar o painel esquerdo com um Modelo de Layout, consulte [Personalizar o painel esquerdo usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Visão geral da área Métricas do projeto

As métricas do projeto oferecem uma visualização do que está acontecendo em um projeto, permitindo que você avalie rapidamente as necessidades e o status de um projeto.

![Métricas do projeto](assets/project-metrics-full-screen-350x238.png)

Na área Métricas, você pode ver o estado geral de um projeto, bem como:

* Onde o trabalho está ativo ou paralisado
* Quem tem itens de trabalho em aberto atribuídos a eles
* Detalhes sobre tarefas ou problemas que estão vencidos ou próximos da Data de conclusão planejada

Você também pode detalhar cada gráfico para analisar mais detalhadamente tarefas ou problemas em uma categoria específica.

Para saber mais sobre essas tarefas ou problemas, consulte [Exibir detalhes de métricas](#view-metrics-details).

<!--this was deprecated: 
>[!TIP]
>
>To see metrics at a higher level for a group of projects within a program, portfolio, etc., navigate to the Enhanced analytics area.  
>To learn more about Enhanced analytics, see [Enhanced analytics overview](../../../enhanced-analytics/enhanced-analytics-overview.md).-->

## KPIs do projeto

Os indicadores-chave de desempenho (KPIs) são exibidos na parte superior da área Métricas.

![Métricas do projeto](assets/project-metrics-kpis-350x52.png)

Esses KPIs estão divididos nas seguintes categorias:

| Tarefas concluídas | **Tarefas concluídas** mostra o número de tarefas com status Concluído. Esse número também inclui tarefas que têm um status personalizado igual a Concluído. |
|---|---|
| Tarefas incompletas | **Tarefas incompletas** mostra o número de tarefas que não estão com status Concluído ou Fechado ou com status igual a Concluído. |
| Tarefas vencidas | **Tarefas atrasadas** mostra o número de tarefas que passaram da Data de conclusão planejada e que não estão com status Concluído ou Fechado ou com status igual a Concluído ou Fechado. |
| Total de tarefas | **Total de tarefas** mostra o número total de tarefas no projeto. |

>[!TIP]
>
>Para exibir uma lista de itens de trabalho para um KPI específico, clique nesse KPI. Nessa lista, você pode clicar em um item de trabalho específico para exibir mais detalhes em uma nova guia.\
>![Tarefas concluídas](assets/completed-tasks-dialog-350x75.png)\
>Para obter mais informações, consulte [Exibir detalhes de métricas](#view-metrics-details).

## Gráfico de barras de tarefas ou problemas

No gráfico de barras que aparece abaixo dos KPIs do projeto, você pode verificar o status ou a prioridade dos itens de trabalho no projeto. A visualização da tarefa é selecionada por padrão.

Quando o status é selecionado neste gráfico, você pode exibir todos os status de tarefas ou problemas em um projeto. Cada status é agrupado em uma barra no gráfico. Todos os status de sistema padrão e personalizados são exibidos neste gráfico.

![Problema de tarefa por status](assets/project-metrics-task-issue-by-status-350x120.png)

Quando a prioridade é selecionada neste gráfico, você pode exibir todas as prioridades de tarefas ou problemas em um projeto.

![Tarefas e problemas por prioridade](assets/project-metrics-task-issue-by-priority-350x121.png)

>[!TIP]
>
>Para exibir uma lista de itens de trabalho com um status ou prioridade específica, clique em uma barra no gráfico. Nessa lista, você pode clicar em um item de trabalho específico para exibir mais detalhes em uma nova guia.\
>![Caixa Tarefas concluídas](assets/completed-tasks-dialog-350x75.png)\
>Para obter mais informações, consulte [Exibir detalhes de métricas](#view-metrics-details).

## Gráfico de rosca

O gráfico de rosca localizado abaixo dos KPIs do projeto permite que você verifique a proporção de itens de trabalho concluídos versus itens de trabalho incompletos em um projeto.

![Tarefas ou problemas por status concluído](assets/tasks-issues-by-complete-status-350x250.png)

No menu suspenso acima do gráfico, você pode selecionar:

| Todas as tarefas | Selecionar **tarefas** mostra o número total de tarefas no projeto, bem como a proporção entre tarefas concluídas e incompletas. |
|---|---|
| Todos os problemas | Selecionar **problemas** mostra o número total de problemas no projeto, bem como a proporção entre problemas concluídos e incompletos. |

>[!TIP]
>
>Para exibir uma lista de itens de trabalho concluídos ou incompletos, clique nessa seção no gráfico de rosca. Nessa lista, você pode clicar em um item de trabalho específico para exibir mais detalhes em uma nova guia.\
>![Caixa Tarefas concluídas](assets/completed-tasks-dialog-350x75.png)\
>Para obter mais informações, consulte [Exibir detalhes de métricas](#view-metrics-details).

## Gráfico de barras do responsável

O gráfico de barras do responsável mostra o número de tarefas atribuídas a cada pessoa no projeto. Esse número varia de acordo com a categoria selecionada no menu suspenso.

![Tarefas e problemas por destinatário](assets/tasks-issues-by-assignee-350x104.png)

Você pode optar por verificar as atribuições de tarefas de um projeto nas seguintes categorias:

| Completo | Selecionar **Concluído** mostra o número de tarefas atribuídas a cada usuário que foram concluídas. |
|---|---|
| Incompleto | Selecionar **Incompleto** mostra o número de tarefas atribuídas a cada usuário que ainda não foram concluídas. |
| Breve | Selecionar **No futuro** mostra o número de tarefas atribuídas a cada usuário que ainda não atingiram a Data de Início Planejada. |
| Atrasado | Selecionar **Vencidas** mostra o número de tarefas atribuídas a cada usuário que estão além da Data de Conclusão Planejada e ainda não foram concluídas. |

>[!TIP]
>
>Para exibir uma lista de itens de trabalho na categoria selecionada que são atribuídos a um usuário específico, clique na barra ao lado do nome do usuário no gráfico. Nessa lista, você pode clicar em um item de trabalho específico para exibir mais detalhes em uma nova guia.\
>![Caixa Tarefas concluídas](assets/completed-tasks-dialog-350x75.png)\
>Para obter mais informações, consulte [Exibir detalhes de métricas](#view-metrics-details).

## Exibir detalhes de métricas {#view-metrics-details}

Você pode interagir com os gráficos na área Métricas para analisar diferentes aspectos de um gráfico ou observar mais detalhadamente as tarefas e problemas em um gráfico.

1. Vá para o projeto para o qual deseja ver as métricas.
1. No painel esquerdo, clique em **Métricas**.\
   Os gráficos na área Métricas exibem informações para tarefas por padrão.\
   ![Seção de métricas](assets/metrics-section-350x298.png)

1. (Condicional) Se uma seta suspensa for exibida em um gráfico, clique no ícone **Seta suspensa** ![Seta suspensa](assets/dropdown-arrow.png) no gráfico e selecione a opção desejada no menu.\
   Para obter informações sobre as opções exibidas nos menus de cada gráfico, consulte a seção relevante acima.

1. (Opcional) Para examinar mais detalhadamente as tarefas ou problemas de qualquer métrica na página, faça o seguinte:

   1. Clique no elemento, como tarefas atribuídas a um usuário específico, problemas com alta prioridade ou todas as tarefas vencidas, para o qual você deseja ver detalhes.

      Uma lista de tarefas ou problemas é exibida.

      ![Caixa Tarefas concluídas](assets/completed-tasks-dialog-350x75.png)

   1. Use as setas na parte inferior da lista para localizar a tarefa ou o problema que deseja examinar.

      Ou

      Selecione um número específico para exibir tarefas ou problemas em uma página específica.

      ![Paginação](assets/pagination-300x152.png)

   1. Selecione uma tarefa ou problema para ver mais detalhes.

      A tarefa ou problema é aberto em uma nova guia.

1. (Opcional) Para exportar o painel de métricas do projeto para um arquivo .png, clique no **ícone Exportar** ![ícone Exportar](assets/export.png) e selecione **Exportar como PNG** no menu suspenso.

   >[!TIP]
   >
   >Ao exportar o painel, o arquivo exportado inclui somente o que é exibido atualmente no visor. Para incluir certos itens no arquivo exportado, talvez seja necessário rolar para cima ou para baixo na página ou ajustar as configurações de zoom do navegador.
