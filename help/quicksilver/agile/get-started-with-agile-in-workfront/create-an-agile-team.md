---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Criar uma equipe ágil
description: O Adobe Workfront permite que equipes ágeis concluam o trabalho de forma incremental e organizada.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# Criar uma equipe ágil

[!DNL Adobe Workfront] permite que as equipes ágeis concluam o trabalho de forma incremental e organizada.

Qualquer usuário na organização pode ver a equipe ágil e visualizar todos os componentes ágeis da equipe, incluindo o registro retroativo, iterações, quadro de histórias e histórias individuais. No entanto, somente membros da equipe com [!UICONTROL Editar] o acesso ao trabalho pode fazer alterações no trabalho atribuído à equipe.

[!DNL Workfront] suporta as seguintes metodologias ágeis:

* **[!UICONTROL Scrum]**: As equipes têm um atraso de trabalho que precisa ser feito. Quando a equipe está pronta para trabalhar em um pedaço específico de trabalho, o trabalho é movido do backlog para uma iteração. Para obter informações mais detalhadas sobre como gerenciar uma equipe de Soma, consulte [Soma em uma equipe ágil](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** As equipes movem o trabalho na exibição Kanban entre status predeterminados. Os status padrão são: backlog, em andamento e concluído. Para obter informações mais detalhadas sobre o gerenciamento de uma equipe kanban, consulte [Kanban em uma equipe ágil](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Plan] para criar uma nova equipe ágil; [!UICONTROL Trabalho] ou superior para converter uma equipe em uma equipe ágil</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano ou tipo de licença você possui, entre em contato com seu [!DNL Workfront] administrador.

## Decidir sobre uma metodologia ágil

Você pode usar uma metodologia ágil Scrum ou Kanban para sua equipe ágil. Cada metodologia oferece vários benefícios. A maneira como sua equipe ágil funciona determina a metodologia ágil que você escolhe usar.

Metodologias ágicas de Scrum e Kanban em [!DNL Workfront] permitir que você mova histórias para um quadro de histórias para indicar uma mudança de status e o progresso da história.

Metodologias ágicas de Scrum e Kanban em [!DNL Workfront] diferem das seguintes maneiras:

### Benefícios do uso do Kanban em [!DNL Workfront]

O [!DNL Kanban] metodologia ágil em [!DNL Workfront] permite que você mova histórias com mais facilidade em um quadro de histórias ágil, além de limitar a quantidade de trabalho em andamento. Não há datas de início e término ao usar a variável [!DNL Kanban] metodologia ágil.

A funcionalidade a seguir suporta essa metodologia:

* Exibir o backlog na [!DNL Kanban] quadro de histórias ágeis.\
   Para obter mais informações, consulte [Adicione o backlog ao [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configure os itens no backlog a serem adicionados automaticamente ao [!UICONTROL Kanban] quadro de história ágil quando outros itens são movidos para um status que equivale a Concluído.\
   Para obter mais informações, consulte a seção [Configure histórias para serem adicionadas automaticamente do backlog](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) no artigo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configurar um limite de Trabalho em Andamento (WIP) a ser exibido no [!UICONTROL Kanban] quadro de histórias ágeis.\
   Para obter mais informações, consulte [Gerenciar o limite de trabalho em andamento (WIP) no quadro Kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Benefícios do uso do Scrum em [!DNL Workfront]

A metodologia ágil do Scrum em [!DNL Workfront] permite adicionar um conjunto de histórias a uma iteração ágil e criar um quadro de histórias para essa iteração. A iteração é baseada nas datas de início e término definidas por você.

A funcionalidade a seguir suporta essa metodologia:

* Inclua problemas na [!UICONTROL Scrum] quadro de histórias
* Incluir problemas no backlog de uma equipe ágil
* As subtarefas podem ser exibidas na [!UICONTROL Scrum] quadro de histórias
* Exibir um gráfico de detalhamento para ver o progresso em relação a histórias durante a iteração\
   Para obter mais informações, consulte [Visão geral do gráfico de detalhamento ágil](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Criar uma nova equipe ágil

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Equipes]**.
1. Clique no botão **[!UICONTROL Trocar equipes]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), depois clique em **[!UICONTROL Criar novo grupo]**.

   ![Selecione Criar nova equipe.](assets/create-new-team-350x198.png)

1. Especifique as seguintes informações no [!UICONTROL Nova equipe] caixa de diálogo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nome da equipe]</strong> </td> 
      <td>Digite um nome para a nova equipe ágil.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Esta é uma equipe ágil]</strong> </td> 
      <td>Selecione esta opção para configurar esta nova equipe para ser uma equipe ágil.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Grupo]</strong> </td> 
      <td> <p>Comece digitando o nome de um grupo a ser adicionado à equipe e selecione o nome quando ele for exibido na lista suspensa.</p> <p>Observação: Quando uma equipe é atribuída a um grupo ou subgrupo, qualquer administrador de grupo desse grupo ou subgrupo pode gerenciar a equipe sem ser membro dele. Os administradores de grupo podem ir para a área [!UICONTROL Equipes] no [!UICONTROL Main Menu] e clicar na seta [!UICONTROL Switch Teams] <img src="assets/switch-team-icon.png" alt="Ícone Alternar equipe"> para listar todas as equipes atribuídas aos grupos que gerenciam.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Membros da equipe]</strong> </td> 
      <td>Comece digitando o nome de um usuário que deve estar no grupo e selecione o nome quando ele for exibido na lista suspensa.<br>Repita esse processo para adicionar vários usuários à equipe.<br>Como os usuários podem fazer parte de mais de uma equipe, eles podem fazer parte de equipes ágeis e não ágeis.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descrição]</strong> </td> 
      <td><p>Digite uma descrição para a equipe.</p> <p>A descrição é exibida na parte superior direita da área [!UICONTROL Equipes] quando a equipe é selecionada.</p>
      <p>Se a descrição for longa, você pode clicar nela para exibir a descrição completa em um pop-up. Se você tiver acesso para editar as configurações da [!UICONTROL equipe], também poderá editar a descrição diretamente na pop-up.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar]**.

   Para obter informações sobre como configurar uma equipe do Agile, consulte os seguintes artigos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Converter uma equipe existente em uma equipe ágil

Você pode converter uma equipe existente em uma equipe ágil:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Equipes]**.
1. Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. Selecione a equipe que deseja converter em uma equipe ágil.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.\
   ![](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Ágil]** seção , selecione **[!UICONTROL Esta é uma equipe ágil]**.

1. No **[!UICONTROL Metodologia]** selecione se a equipe usará uma **[!UICONTROL Scrum]** ou **[!UICONTROL Kanban]** metodologia ágil.

1. Clique em **Salvar alterações.**

   Para obter informações sobre como configurar uma equipe do Agile, consulte os seguintes artigos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
