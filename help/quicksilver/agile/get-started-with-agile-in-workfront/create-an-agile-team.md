---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Crie uma equipe ágil
description: O Adobe Workfront permite que as equipes da Agile concluam o trabalho de maneira incremental e organizada.
author: Courtney
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 5%

---

# Criar uma equipe ágil

<!--Audited: 01/2024-->

O [!DNL Adobe Workfront] permite que as equipes Ágeis concluam o trabalho de maneira incremental e organizada.

Qualquer usuário na organização pode ver a equipe Ágil e visualizar todos os componentes Ágeis da equipe, incluindo a lista de pendências, iterações, quadro de matérias e matérias individuais. No entanto, somente membros da equipe com acesso de [!UICONTROL Edição] ao trabalho podem fazer alterações no trabalho atribuído à equipe.

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
   <p>Planeje a criação de uma nova equipe Ágil</p>
  <p>Trabalhe ou superior para converter uma equipe em uma equipe ágil</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Decidir sobre uma metodologia ágil

Você pode usar uma metodologia Ágil Scrum ou Kanban para sua equipe Ágil. Cada metodologia oferece vários benefícios. A forma como sua equipe Agile funciona determina a metodologia Agile que você escolhe usar.

As metodologias Scrum e Kanban Agile em [!DNL Workfront] permitem mover matérias em um quadro de matérias para indicar uma alteração de status e o progresso da matéria.

As metodologias Scrum e Kanban Agile em [!DNL Workfront] diferem das seguintes maneiras:

### Benefícios do uso do Kanban em [!DNL Workfront]

A metodologia Ágil [!DNL Kanban] em [!DNL Workfront] permite mover com mais facilidade matérias em um quadro de matérias Ágil, limitando a quantidade de trabalho em andamento. Não há datas de início e término ao usar a metodologia Ágil [!DNL Kanban].

A seguinte funcionalidade é compatível com essa metodologia:

* Exibir o backlog no storyboard Agile [!DNL Kanban].
Para obter mais informações, consulte [Adicionar o backlog ao quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configure os itens na lista de pendências a serem adicionados automaticamente ao [!UICONTROL Kanban] do storyboard Agile quando outros itens forem movidos para um status que equivale a Concluído.
Para obter mais informações, consulte a seção [Configurar histórias que serão adicionadas automaticamente da lista de pendências](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) no artigo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configure um limite de Trabalho em andamento (WIP) a ser exibido no storyboard Agile [!UICONTROL Kanban].
Para obter mais informações, consulte [Gerenciar o limite de trabalhos em andamento (WIP) no quadro Kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Benefícios do uso do Scrum em [!DNL Workfront]

A metodologia Scrum Agile em [!DNL Workfront] permite adicionar um conjunto de histórias a uma iteração Ágil e criar um quadro de histórias para essa iteração. A iteração é baseada nas datas de início e término que você definir.

A seguinte funcionalidade suporta essa metodologia:

* Incluir problemas no storyboard [!UICONTROL Scrum]
* Incluir problemas na lista de pendências de uma equipe Agile
* As subtarefas podem ser exibidas no quadro de matérias [!UICONTROL Trilha]
* Exibir um gráfico de burndown para ver o progresso em relação às matérias durante a iteração
Para obter mais informações, consulte [Visão geral do gráfico de detalhamento ágil](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Criar uma equipe ágil

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
      <td role="rowheader"><strong>[!UICONTROL Nome da Equipe do]</strong> </td> 
      <td>Digite um nome para o novo grupo Agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Esta é uma Equipe Ágil]</strong> </td> 
      <td>Selecione esta opção para configurar o novo grupo para ser um grupo Ágil.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL Está Ativo]</strong> </td> 
      <td>Selecione esta opção para ativar a equipe. Equipes inativas não são visíveis para outros usuários para atribuir ao trabalho. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Grupo]</strong> </td> 
      <td> <p>Comece a digitar o nome de um grupo para adicionar ao grupo e, em seguida, selecione o nome quando ele aparecer na lista suspensa.</p> <p><b>Nota</b></p> <p> Quando uma equipe é atribuída a um grupo ou subgrupo, qualquer administrador desse grupo ou subgrupo pode gerenciar a equipe sem ser um membro da equipe. Os administradores de grupo podem ir para a área [!UICONTROL Teams] no menu principal  e clicar na seta [!UICONTROL Switch Teams] <img src="assets/switch-team-icon.png" alt="Ícone Alternar equipe"> para listar todas as equipes atribuídas aos grupos que eles gerenciam.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Membros da Equipe do]</strong> </td> 
      <td>Comece a digitar o nome de um usuário para fazer parte da equipe e selecione o nome quando ele aparecer na lista suspensa.<br>Repita este processo para adicionar vários usuários à equipe.<br>Como os usuários podem estar em mais de uma equipe, eles podem estar em equipes ágeis e não ágeis.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descrição]</strong> </td> 
      <td><p>Digite uma descrição para a equipe.</p> <p>A descrição é exibida no canto superior direito da área [!UICONTROL Teams] quando o grupo é selecionado.</p>
      <p>Se a descrição for longa, clique nela para exibir a descrição completa em uma janela pop-up. Se você tiver acesso para editar as [!UICONTROL configurações da equipe], você também pode editar a descrição diretamente no pop-up.</p></td>
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

1. Clique no ícone **[!UICONTROL Alternar equipe]** ![Ícone Alternar equipe](assets/switch-team-icon.png) e, em seguida, selecione uma nova equipe no menu suspenso ou pesquise uma equipe na barra de pesquisa.

1. Selecione a equipe que deseja converter em uma equipe ágil.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com uma licença [!UICONTROL Padrão], [!UICONTROL Plano] ou [!UICONTROL Trabalho] veem esta opção.
   ![Selecionar Editar](assets/edit-team-settings.png)

1. Na seção **[!UICONTROL Agile]**, selecione **[!UICONTROL Equipe Agile]**.

1. Na seção **[!UICONTROL Metodologia]**, selecione se a equipe usará uma metodologia ágil **[!UICONTROL Scrum]** ou **[!UICONTROL Kanban]**.

1. Clique em **Salvar alterações**.

   O grupo é salvo como um grupo Ágil. Você pode configurar a nova equipe como um Scrum ou uma equipe Kanban ao editar a equipe.

   Para obter mais informações, consulte os seguintes artigos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
