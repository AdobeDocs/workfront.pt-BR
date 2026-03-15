---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Add Stories to an Existing Iteration
description: É possível adicionar histórias a uma iteração de várias maneiras.
author: Courtney
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 7%

---

# Adicionar stories a uma iteração existente

É possível adicionar matérias a uma iteração de qualquer uma das seguintes maneiras:

* Da lista de pendências após a criação da iteração, conforme descrito na seção [Mover matérias da lista de pendências para uma iteração ou para o quadro [!UICONTROL Kanban]](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) em [Gerenciar a lista de pendências ágil](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* From the [!UICONTROL Details] page of the individual task or issue
* From a task or issue list
* From a report
* From a dashboard

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p> 
   <p>Trabalho ou maior</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Gerenciar acesso ao projeto em que a história se encontra </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Understand how adding stories affects task dates

By default, when you add an existing task to an iteration, the task&#39;s [!UICONTROL Planned Start Date] and [!UICONTROL Planned Completion Date] are set as follows:

### Task [!UICONTROL Planned Start Date]

* The task uses the iteration&#39;s Start Date when:

   * O projeto não tem uma [!UICONTROL Data de Início Planejada] definida.
   * A [!UICONTROL Data de Início Planejada] do projeto é *antes* ou *no* da data de início da iteração.

* A tarefa usa a [!UICONTROL Data de Início Planejada] do projeto quando:

   * A [!UICONTROL Data de Início Planejada] do projeto é *depois* da data de início da iteração.

### Task [!UICONTROL Planned Completion Date]

* The task uses the iteration&#39;s End Date when:

   * The project does not have a [!UICONTROL Planned Completion Date] set.
   * The project&#39;s [!UICONTROL Planned Start Date] is *before or on* the iteration&#39;s Start Date or the Project&#39;s [!UICONTROL Planned Completion Date] is *before or on* the iteration&#39;s End Date.

* The task uses the project&#39;s [!UICONTROL Planned Completion Date] when:

   * The project&#39;s [!UICONTROL Planned Start Date] is *after* the iteration&#39;s Start Date and the project&#39;s [!UICONTROL Planned Completion Date] is *after* the iteration&#39;s End Date.

Você pode configurar equipes individuais do Scrum para usar as datas do projeto por padrão, em vez das datas de iteração. Para obter informações, consulte a seção [Configurar como as datas são aplicadas ao adicionar itens de trabalho a uma iteração](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) no artigo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Adicionar uma matéria a uma iteração existente

Você pode adicionar qualquer tarefa ou problema a qualquer iteração se tiver acesso de Gerenciamento ao projeto. Lembre-se do seguinte ao mover uma tarefa ou ocorrência para uma iteração:

* Se você adicionar várias equipes, a tarefa ou ocorrência poderá ser exibida somente na iteração de uma equipe. This is the iteration you choose in step 3 below.
* If the task or issue is assigned to an Agile team and moved to another team&#39;s iteration, the team assignment does not change.
* If the task or issue is not assigned to a team, the task or issue is assigned to the team who owns the iteration.
* You can&#39;t add parent tasks to the iteration. If you add any child tasks, the parent task appears on the Scrum board as a swimlane.

>[!IMPORTANT]
>
>After the task moves to the iteration, you cannot update the [!UICONTROL Duration Type] or [!UICONTROL Task Constraint]. [!UICONTROL Duration Type] is set to [!UICONTROL Simple] and [!UICONTROL Task Constraint] is set to [!UICONTROL Fixed Dates] to keep the task timeline consistent with the iteration&#39;s timeline.

1. Open the task or issue you want to add to an iteration.
Ou
Acesse o projeto, relatório ou painel que contém a tarefa ou ocorrência que você deseja adicionar a uma iteração. Depois, selecione uma ou mais tarefas ou ocorrências.

1. Clique no ícone **[!UICONTROL Mais]** ![Mais](assets/more-icon.png) > **[!UICONTROL Adicionar à Iteração]**.
Não é possível atribuir tarefas ou problemas atribuídos a equipes não ágeis.

1. Na caixa **[!UICONTROL Adicionar a]**, comece a digitar o nome da iteração e selecione-o quando ele aparecer na lista.

   >[!NOTE]
   >
   >É possível mover uma matéria de uma iteração existente para uma nova iteração.

1. Clique em **[!UICONTROL Adicionar]**.
