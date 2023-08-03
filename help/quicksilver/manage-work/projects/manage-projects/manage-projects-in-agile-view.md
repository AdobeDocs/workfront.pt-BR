---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Gerenciar um projeto na visualização Agile
description: Planos, tipos de licença e acesso necessários Adobe Workfront Plan Team, Pro, Business ou Enterprise Workfront License Type Review, Work ou Plan Permissions no modelo de acesso Editar acesso e capacidade para criar relatórios, painéis e calendários
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 0b6b71fae698d34e9c96ba5a699006b3df294a5c
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# Gerenciar um projeto na visualização Agile

{{preview-and-fast-release}}

<!--
Required plans, license types, and access

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront Plan</a> </p> </td> 
   <td> <p>Team, Pro, Business, or Enterprise </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront License Type</p> </td> 
   <td> <p>Review, Work, or Plan </p> </td> 
  </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
 </tbody> 
</table>
-->

Você pode aproveitar a funcionalidade ágil para o seu projeto sem os desafios administrativos que normalmente acompanham as práticas ágeis (como gerenciar um backlog da equipe ou criar iterações).

Se você quiser trabalhar em um ambiente ágil que use um backlog de equipe e permita criar iterações de tarefas no backlog, siga as instruções em [Trabalhe em um ambiente ágil](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso às seguintes áreas:</p> 
    <ul> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Relatórios, painéis, calendários</p> </li> 
     <li> <p>Filtros, Visualizações, Agrupamentos</p> </li> 
    </ul> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Entender projetos Agile

>[!NOTE]
>
>Esta seção se aplica somente à visualização Agile herdada, não à visualização de quadro de um projeto.

* [Funcionalidade Agile em um projeto](#agile-functionality-in-a-project)
* [Diferenças ao usar a visualização Agile em um projeto ou em uma iteração](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Funcionalidade Agile em um projeto {#agile-functionality-in-a-project}

A seguinte funcionalidade ágil está disponível ao gerenciar um projeto em uma visualização ágil:

* Status de Término\
  Para obter informações mais detalhadas sobre o status de conclusão, consulte [Visão geral do status de conclusão da iteração](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Storyboard\
  Para obter informações mais detalhadas sobre o storyboard, consulte o [Quadro Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) seção.

Há algumas diferenças ao usar visualizações ágeis em um projeto em vez de trabalhar em um ambiente puramente ágil (com registros pendentes e iterações). Para obter mais informações, consulte [Diferenças ao usar a visualização Agile em um projeto ou em uma iteração](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) neste artigo.

### Diferenças ao usar a visualização Agile em um projeto ou em uma iteração {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [As tarefas e subtarefas seguem regras de exibição diferentes no Storyboard](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [As listas de pendências e iterações não são usadas](#backlogs-and-iterations-are-not-used)
* [A ordem das tarefas é mantida na visualização Agile e não pode ser reordenada](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [As tarefas são medidas somente em Horas planejadas](#tasks-are-measured-only-in-planned-hours)
* [A Equipe Agile não é usada](#the-agile-team-is-not-used)
* [Cada usuário no projeto pode visualizar o projeto em uma visualização Agile diferente](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### As tarefas e subtarefas seguem regras de exibição diferentes no Storyboard {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* As tarefas que não têm uma tarefa pai nem uma subtarefa são sempre exibidas como um único storyboard no storyboard.\
  Por exemplo, essas tarefas aparecem da seguinte maneira na exibição de lista do projeto:

  ![Lista de projetos Agile - tarefas sem tarefas principais ou secundárias](assets/agile-project-single-list-nwe.png) Essas tarefas aparecem da seguinte maneira na exibição ágil do projeto:

  ![Visualização Agile do projeto - tarefas sem tarefas principais ou secundárias](assets/agile-project-singlecard-nwe.png)

* As tarefas pai que têm subtarefas são sempre exibidas na variável **Histórias** coluna do storyboard. As subtarefas são exibidas na raia da tarefa pai.\
  Por exemplo, essas tarefas aparecem da seguinte maneira na exibição de lista do projeto:

  ![Lista de projetos Agile - tarefas com pais e subtarefas](assets/agile-project-parent-list-nwe.png)\
  Essas tarefas aparecem da seguinte maneira na exibição ágil do projeto:

  ![Visualização de projeto Agile - tarefas com pais e subtarefas](assets/agile-project-parent-nwe.png)

* Subtarefas de segundo nível (subtarefas de subtarefas) são exibidas como um cartão cinza suspenso da tarefa pai imediata.
* Subtarefas de terceiro nível (subtarefas de subtarefas) nunca são exibidas no storyboard.

#### As listas de pendências e iterações não são usadas {#backlogs-and-iterations-are-not-used}

Ao visualizar um projeto em uma visualização ágil, os seguintes componentes ágeis não são usados:

* **Backlog:** Nenhuma lista de pendências é usada porque qualquer tarefa no projeto é exibida automaticamente como histórias.
* **Iterações:** Em vez de criar iterações para definir as datas em que o trabalho será realizado, os dias atualmente designados na linha do tempo do projeto se tornam os dias úteis.

#### A ordem das tarefas é mantida na visualização Agile e não pode ser reordenada {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

A ordem em que as tarefas aparecem em um projeto é mantida ao exibi-lo em um storyboard ágil.

Não é possível reordenar tarefas no projeto ao visualizar o projeto em uma exibição ágil. Como a modificação da ordem da tarefa pode afetar outras tarefas que possam ter dependências, você deve exibir o projeto em uma exibição padrão para modificar a ordem da tarefa.

#### As tarefas são medidas somente em Horas planejadas {#tasks-are-measured-only-in-planned-hours}

As tarefas em um projeto são sempre medidas em Horas planejadas.

Em uma iteração, as tarefas (histórias) podem ser medidas em horas ou pontos.

#### A Equipe Agile não é usada {#the-agile-team-is-not-used}

Como as equipes ágeis concluem o trabalho nas iterações atribuídas a elas, as equipes ágeis não são usadas ao visualizar um projeto em uma visualização ágil.

Em vez disso, os usuários do projeto basicamente se tornam a equipe ágil desse projeto.

#### Cada usuário no projeto pode visualizar o projeto em uma visualização Agile diferente {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

Diferentemente de uma iteração ágil, os usuários de um projeto podem personalizar a exibição ágil para eles mesmos, enquanto outros usuários usam uma exibição ágil diferente.

Em uma iteração ágil, as informações disponíveis no storyboard de agile (como colunas de status disponíveis) são determinadas no nível da equipe.

Para obter informações sobre como personalizar uma visualização ágil, consulte [Criar ou personalizar uma visualização Agile](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Exibir um projeto na exibição Agile

1. <span class="preview">Vá para o projeto que deseja visualizar em uma visualização Agile, na lista de tarefas ou na lista de problemas.</span>
1. Clique em **Quadro** ícone ![Ícone do painel](assets/board-icon-for-agile-view.png).

   A exibição de quadro do projeto é exibida por padrão.

   ![Exibição do painel do projeto](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. (Opcional) Clique em **Configurar** para definir opções para as colunas e cartões.

   Para obter mais informações, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) e [Personalizar quais campos são exibidos em um cartão](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md). Observe que você não pode definir políticas de coluna na exibição de quadro de um projeto.

1. (Opcional) Clique em **Usar ágil legado** para usar a visualização ágil herdada em vez da visualização de quadro.

1. (Opcional - somente visualização ágil herdada) Se você tiver criado uma visualização ágil personalizada ou se outro usuário tiver criado uma visualização ágil personalizada e a compartilhou com você, você poderá visualizá-la em vez da visualização ágil padrão.

   Clique em **Exibir** e clique na exibição ágil personalizada que deseja visualizar.

   A exibição ágil personalizada será usada na próxima vez que você clicar no botão **Agile** ícone.

   Para obter informações sobre como criar uma nova visualização ágil, consulte [Criar e personalizar visualizações Agile](#create-and-customize-agile-views).

   O projeto é exibido na visualização ágil personalizada.

1. (Condicional - somente visualização Agile herdada) Se as tarefas no seu projeto estiverem usando status diferentes de &quot;Novo&quot;, &quot;Em andamento&quot; ou &quot;Concluído&quot; (os status padrão da visualização Agile), você deverá adicionar os status adicionais à visualização Agile para que todas as tarefas nesses status sejam exibidas.

   Se as tarefas tiverem um status que não seja exibido no storyboard Agile, a própria tarefa não será exibida no storyboard Agile (no entanto, o Percentual concluído dessas tarefas ainda contribuirá para o Percentual concluído de qualquer tarefa pai e o Percentual concluído do projeto geral).

   Para adicionar status à visualização Agile, crie uma nova visualização Agile ou personalize uma visualização Agile existente, conforme descrito na seção &quot;Criar ou personalizar uma visualização Agile&quot; no artigo [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (Opcional) Para retornar à exibição em lista, clique no link **Lista** ícone.

## Criar e personalizar visualizações Agile {#create-and-customize-agile-views}

>[!NOTE]
>
>Esta seção se aplica somente à visualização Agile herdada, não à visualização de quadro de um projeto.

Assim como com as exibições padrão no Workfront, você pode personalizar Exibições ágeis existentes ou criar novas Exibições ágeis do zero. Diferentemente das exibições padrão, não é possível criar novas Exibições ágeis com base em Exibições ágeis existentes.

Para obter mais informações sobre como criar e personalizar exibições Agile, consulte a seção &quot;Criar ou personalizar uma exibição Agile&quot; no artigo [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Compartilhar uma visualização Agile existente

>[!NOTE]
>
>Esta seção se aplica somente à visualização Agile herdada, não à visualização de quadro de um projeto.

Para obter informações sobre como compartilhar uma visualização ágil, consulte [Compartilhar um filtro, uma exibição ou um agrupamento](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Remover uma visualização Agile existente

>[!NOTE]
>
>Esta seção se aplica somente à visualização Agile herdada, não à visualização de quadro de um projeto.

Para obter informações sobre como excluir uma exibição, consulte a seção &quot;Remover uma exibição&quot; no artigo [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
