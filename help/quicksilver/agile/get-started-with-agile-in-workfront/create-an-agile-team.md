---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Criar uma equipe Agile
description: O Adobe Workfront permite que as equipes do Agile concluam o trabalho de forma incremental e organizada.
author: Jenny
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 2%

---

# Criar uma equipe Agile

<!--Audited: 01/2024-->

O [!DNL Adobe Workfront] permite que as equipes Agile concluam o trabalho de forma incremental e organizada.

Qualquer usuário na organização pode ver a equipe Agile e visualizar todos os componentes Agile da equipe, incluindo o backlog, as iterações, o storyboard e as histórias individuais. No entanto, somente membros da equipe com acesso de [!UICONTROL Edição] ao trabalho podem fazer alterações no trabalho atribuído à equipe.

O [!DNL Workfront] oferece suporte às seguintes metodologias Agile:

* **[!UICONTROL Scrum]**: as equipes têm uma lista de pendências de trabalho que precisa ser feito. Quando a equipe está pronta para trabalhar em uma parte específica do trabalho, o trabalho é movido da lista de pendências para uma iteração. Para obter informações mais detalhadas sobre o gerenciamento de uma equipe Scrum, consulte [Scrum em uma equipe Agile](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** as equipes movem o trabalho na exibição Kanban entre status predeterminados. Os status padrão são: backlog, em andamento e concluído. Para obter informações mais detalhadas sobre o gerenciamento de uma equipe Kanban, consulte [Kanban em uma equipe Agile](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p>
   <p>Planejar a criação de uma nova equipe Agile</p>
  <p>Trabalhar ou mais para converter uma equipe em uma equipe Agile</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Decida sobre uma metodologia Agile

Você pode usar uma metodologia Agile Scrum ou Kanban para sua equipe Agile. Cada metodologia oferece vários benefícios. A forma como sua equipe Agile funciona determina a metodologia Agile que você escolhe usar.

As metodologias Scrum e Kanban Agile em [!DNL Workfront] permitem mover histórias por um storyboard para indicar uma alteração de status e o progresso da história.

As metodologias Scrum e Kanban Agile em [!DNL Workfront] diferem das seguintes maneiras:

### Benefícios do uso do Kanban em [!DNL Workfront]

A metodologia Agile [!DNL Kanban] no [!DNL Workfront] permite mover mais facilmente histórias por um storyboard Agile, limitando a quantidade de trabalho em andamento. Não há datas de início e término ao usar a metodologia Agile [!DNL Kanban].

A seguinte funcionalidade é compatível com essa metodologia:

* Exibir o backlog no storyboard Agile [!DNL Kanban].
Para obter mais informações, consulte [Adicionar o backlog ao quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configure os itens na lista de pendências a serem adicionados automaticamente ao [!UICONTROL Kanban] do storyboard Agile quando outros itens forem movidos para um status que equivale a Concluído.
Para obter mais informações, consulte a seção [Configurar histórias que serão adicionadas automaticamente da lista de pendências](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) no artigo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configure um limite de Trabalho em andamento (WIP) a ser exibido no storyboard Agile [!UICONTROL Kanban].
Para obter mais informações, consulte [Gerenciar o limite de trabalhos em andamento (WIP) no quadro Kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Benefícios do uso do Scrum em [!DNL Workfront]

A metodologia Scrum Agile em [!DNL Workfront] permite adicionar um conjunto de histórias a uma iteração Agile e criar um storyboard para essa iteração. A iteração é baseada nas datas inicial e final definidas por você.

A seguinte funcionalidade é compatível com essa metodologia:

* Incluir problemas no storyboard [!UICONTROL Scrum]
* Incluir problemas na lista de pendências de uma equipe Agile
* Subtarefas podem ser exibidas no storyboard [!UICONTROL Scrum]
* Exibir um gráfico de burndown para ver o progresso em relação às histórias durante a iteração
Para obter mais informações, consulte [Visão geral do gráfico de burndown ágil](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Criar uma equipe Agile

{{step1-to-team}}

1. Clique no ícone **[!UICONTROL Alternar equipes]** ![Ícone Alternar equipe](assets/switch-team-icon.png) e clique em **[!UICONTROL Criar nova equipe]**.

   ![Selecione Criar nova equipe](assets/create-new-team.png)

   A caixa Nova equipe é exibida.

1. Especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nome da Equipe]</strong> </td> 
      <td>Digite um nome para a nova equipe Agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Esta é uma Equipe Ágil]</strong> </td> 
      <td>Selecione esta opção para configurar esta nova equipe para ser uma Equipe Agile.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL Está Ativo]</strong> </td> 
      <td>Selecione esta opção para ativar esta equipe. Equipes inativas não estão visíveis para outros usuários para atribuir ao trabalho. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Grupo]</strong> </td> 
      <td> <p>Comece a digitar o nome de um grupo para adicionar ao grupo e selecione o nome quando ele aparecer na lista suspensa.</p> <p><b>Nota</b></p> <p> Quando uma equipe é atribuída a um grupo ou subgrupo, os administradores desse grupo ou subgrupo podem gerenciar a equipe sem ser um membro da equipe. Os administradores de grupo podem ir para a área [!UICONTROL Equipes] no [!UICONTROL Menu Principal] e clicar na seta [!UICONTROL Trocar Equipes] <img src="assets/switch-team-icon.png" alt="Ícone Trocar equipe"> para listar todas as equipes atribuídas aos grupos que eles gerenciam.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Membros da Equipe]</strong> </td> 
      <td>Comece a digitar o nome de um usuário para fazer parte da equipe e selecione o nome quando ele aparecer na lista suspensa.<br>Repita esse processo para adicionar vários usuários à equipe.<br>Como os usuários podem pertencer a mais de uma equipe, eles podem pertencer a equipes Agile e não-Agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descrição]</strong> </td> 
      <td><p>Digite uma descrição para a equipe.</p> <p>A descrição é exibida na parte superior direita da área [!UICONTROL Equipes] quando o grupo é selecionado.</p>
      <p>Se a descrição for longa, clique nela para exibir a descrição completa em um pop-up. Se você tiver acesso para editar as [!UICONTROL configurações da equipe], também poderá editar a descrição diretamente na janela pop-up.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar]**.

   Para obter informações sobre como configurar uma Equipe Agile, consulte os seguintes artigos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Converter uma equipe existente em uma equipe Agile

É possível converter uma equipe existente em uma Equipe Agile:

{{step1-to-team}}

1. Clique no ícone **[!UICONTROL Equipe de comutação]** ![Ícone Equipe de comutação](assets/switch-team-icon.png) e selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a equipe que você deseja converter em uma equipe Agile.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com uma licença [!UICONTROL Padrão], [!UICONTROL Plano] ou [!UICONTROL Trabalho] podem ver esta opção.
   ![Selecionar Editar](assets/edit-team-settings.png)

1. Na seção **[!UICONTROL Agile]**, selecione **[!UICONTROL Equipe Agile]**.

1. Na seção **[!UICONTROL Metodologia]**, selecione se a equipe usará uma metodologia Agile **[!UICONTROL Scrum]** ou **[!UICONTROL Kanban]**.

1. Clique em **Salvar alterações**.

   A equipe é salva como uma equipe Agile. Você pode configurar a nova equipe como um Scrum ou uma equipe Kanban ao editá-la.

   Para obter mais informações, consulte os seguintes artigos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
