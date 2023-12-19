---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Criar uma equipe ágil
description: O Adobe Workfront permite que equipes ágeis concluam o trabalho de forma incremental e organizada.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 0%

---

# Criar uma equipe ágil

[!DNL Adobe Workfront] O permite que equipes ágeis concluam o trabalho de forma incremental e organizada.

Qualquer usuário na organização pode ver a equipe ágil e visualizar todos os componentes ágeis da equipe, incluindo a lista de pendências, as iterações, o storyboard e as histórias individuais. No entanto, apenas os membros da equipe com [!UICONTROL Editar] o acesso ao trabalho pode fazer alterações no trabalho atribuído à equipe.

[!DNL Workfront] O oferece suporte às seguintes metodologias ágeis:

* **[!UICONTROL Scrum]**: as equipes têm um backlog de trabalho que precisa ser feito. Quando a equipe está pronta para trabalhar em uma parte específica do trabalho, o trabalho é movido da lista de pendências para uma iteração. Para obter informações mais detalhadas sobre o gerenciamento de uma equipe Scrum, consulte [Scrum em uma equipe ágil](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** As equipes movem o trabalho na exibição Kanban entre status predeterminados. Os status padrão são: backlog, em andamento e concluído. Para obter informações mais detalhadas sobre o gerenciamento de uma equipe Kanban, consulte [Kanban em uma equipe ágil](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Plano] para criar uma nova Equipe Ágil; [!UICONTROL Trabalho] ou superior para converter uma equipe em uma Equipe Ágil</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber que tipo de plano ou licença você tem, entre em contato com o [!DNL Workfront] administrador.

## Decidir sobre uma metodologia ágil

Você pode usar uma metodologia ágil Scrum ou Kanban para sua equipe ágil. Cada metodologia oferece vários benefícios. A maneira como sua equipe ágil funciona determina a metodologia ágil que você escolhe usar.

As metodologias ágeis Scrum e Kanban em [!DNL Workfront] O permite mover histórias por um storyboard para indicar uma alteração de status e o progresso da história.

Metodologias ágeis de Scrum e Kanban em [!DNL Workfront] diferem das seguintes formas:

### Benefícios do uso do Kanban no [!DNL Workfront]

A variável [!DNL Kanban] metodologia ágil no [!DNL Workfront] O permite mover mais facilmente as histórias em um storyboard ágil, limitando a quantidade de trabalho em andamento. Não há datas de início e término ao usar o [!DNL Kanban] metodologia ágil.

A seguinte funcionalidade é compatível com essa metodologia:

* Exibir o backlog no [!DNL Kanban] storyboard ágil.\
   Para obter mais informações, consulte [Adicione o backlog à [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configurar itens no backlog para serem adicionados automaticamente ao [!UICONTROL Kanban] storyboard ágil quando outros itens são movidos para um status que é igual a Concluído.\
   Para obter mais informações, consulte a seção [Configurar matérias a serem adicionadas automaticamente a partir do backlog](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) no artigo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configure um limite de Trabalho em andamento (WIP) a ser exibido na [!UICONTROL Kanban] storyboard ágil.\
   Para obter mais informações, consulte [Gerenciar o limite de trabalho em andamento (WIP) no quadro Kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Benefícios do uso do Scrum no [!DNL Workfront]

A metodologia ágil de Scrum no [!DNL Workfront] permite adicionar um conjunto de histórias a uma iteração ágil e criar um storyboard para essa iteração. A iteração é baseada nas datas inicial e final definidas por você.

A seguinte funcionalidade é compatível com essa metodologia:

* Incluir problemas no [!UICONTROL Scrum] storyboard
* Incluir problemas na lista de pendências de uma equipe ágil
* Subtarefas podem ser exibidas na [!UICONTROL Scrum] storyboard
* Exibir um gráfico de burndown para ver o progresso em relação às histórias durante a iteração\
   Para obter mais informações, consulte [Visão geral do gráfico de burndown ágil](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Criar uma equipe ágil

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Equipes]**.
1. Clique em **[!UICONTROL Trocar equipes]** ícone ![Ícone Trocar equipe](assets/switch-team-icon.png)e, em seguida, clique em **[!UICONTROL Criar nova equipe]**.

   ![Selecione Criar nova equipe.](assets/create-new-team-350x198.png)

1. Especifique as seguintes informações sobre o [!UICONTROL Nova equipe] diálogo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nome da Equipe]</strong> </td> 
      <td>Digite um nome para a nova Equipe Agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Esta é uma Equipe Ágil]</strong> </td> 
      <td>Selecione esta opção para configurar o novo grupo para ser um grupo ágil.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Grupo]</strong> </td> 
      <td> <p>Comece a digitar o nome de um grupo para adicionar ao grupo e selecione o nome quando ele aparecer na lista suspensa.</p> <p>Observação: quando uma equipe é atribuída a um grupo ou subgrupo, os administradores desse grupo ou subgrupo podem gerenciar a equipe sem ser membros dele. Os administradores de grupo podem ir para a área [!UICONTROL Equipes] no [!UICONTROL Menu Principal] e clicar na seta [!UICONTROL Trocar Equipes] <img src="assets/switch-team-icon.png" alt="Ícone Trocar equipe"> para listar todas as equipes atribuídas aos grupos que eles gerenciam.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Membros da Equipe]</strong> </td> 
      <td>Comece a digitar o nome de um usuário para fazer parte da equipe e selecione o nome quando ele aparecer na lista suspensa.<br>Repita esse processo para adicionar vários usuários à equipe.<br>Como os usuários podem estar em mais de uma equipe, eles podem estar em equipes ágeis e não ágeis.</td> 
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

## Converter uma equipe existente em uma equipe ágil

É possível converter uma equipe existente em uma equipe ágil:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Equipes]**.
1. Clique em **[!UICONTROL Trocar equipe]** ícone ![Ícone Trocar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a equipe que você deseja converter em uma equipe ágil.
1. Clique em **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   Somente membros da equipe com um [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.\
   ![](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Agile]** , selecione **[!UICONTROL Esta é uma Equipe Agile]**.

1. No **[!UICONTROL Metodologia]** , selecione se a equipe usará uma **[!UICONTROL Scrum]** ou **[!UICONTROL Kanban]** metodologia ágil.

1. Clique em **Salvar alterações.**

   Para obter informações sobre como configurar uma Equipe Agile, consulte os seguintes artigos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
