---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Criar uma equipe Agile
description: O Adobe Workfront permite que equipes ágeis concluam o trabalho de forma incremental e organizada.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 1%

---

# Criar uma equipe ágil

<!--Audited: 01/2024-->

O [!DNL Adobe Workfront] permite que equipes ágeis concluam o trabalho de forma incremental e organizada.

Qualquer usuário na organização pode ver a equipe ágil e visualizar todos os componentes ágeis da equipe, incluindo a lista de pendências, as iterações, o storyboard e as histórias individuais. No entanto, somente membros da equipe com acesso de [!UICONTROL Edição] ao trabalho podem fazer alterações no trabalho atribuído à equipe.

O [!DNL Workfront] oferece suporte às seguintes metodologias ágeis:

* **[!UICONTROL Scrum]**: as equipes têm uma lista de pendências de trabalho que precisa ser feito. Quando a equipe está pronta para trabalhar em uma parte específica do trabalho, o trabalho é movido da lista de pendências para uma iteração. Para obter informações mais detalhadas sobre o gerenciamento de uma equipe Scrum, consulte [Scrum em uma equipe ágil](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** as equipes movem o trabalho na exibição Kanban entre status predeterminados. Os status padrão são: backlog, em andamento e concluído. Para obter informações mais detalhadas sobre o gerenciamento de uma equipe Kanban, consulte [Kanban em uma equipe ágil](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: Padrão</p>
   Atual: 
   <ul><li><p>[!UICONTROL Plano] para criar uma nova Equipe Ágil</p></li> 
   <li><p>[!UICONTROL Trabalho] ou superior para converter um grupo em um grupo ágil</p></li></ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Decidir sobre uma metodologia ágil

Você pode usar uma metodologia ágil Scrum ou Kanban para sua equipe ágil. Cada metodologia oferece vários benefícios. A maneira como sua equipe ágil funciona determina a metodologia ágil que você escolhe usar.

As metodologias ágeis de Scrum e Kanban em [!DNL Workfront] permitem mover histórias por um storyboard para indicar uma alteração de status e o progresso da história.

As metodologias ágeis de Scrum e Kanban em [!DNL Workfront] diferem das seguintes maneiras:

### Benefícios do uso do Kanban em [!DNL Workfront]

A metodologia ágil [!DNL Kanban] no [!DNL Workfront] permite mover mais facilmente as histórias por um storyboard ágil, limitando a quantidade de trabalho em andamento. Não há datas de início e término ao usar a metodologia ágil [!DNL Kanban].

A seguinte funcionalidade é compatível com essa metodologia:

* Exibir o backlog no storyboard ágil [!DNL Kanban].
Para obter mais informações, consulte [Adicionar o backlog ao quadro [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configure os itens na lista de pendências a serem adicionados automaticamente ao [!UICONTROL Kanban] storyboard ágil quando outros itens forem movidos para um status que equivale a Concluído.
Para obter mais informações, consulte a seção [Configurar histórias que serão adicionadas automaticamente da lista de pendências](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) no artigo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configure um limite de Trabalho em andamento (WIP) a ser exibido no storyboard ágil [!UICONTROL Kanban].
Para obter mais informações, consulte [Gerenciar o limite de trabalhos em andamento (WIP) no quadro Kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Benefícios do uso do Scrum em [!DNL Workfront]

A metodologia ágil de Scrum no [!DNL Workfront] permite que você adicione um conjunto de histórias a uma iteração ágil e crie um storyboard para essa iteração. A iteração é baseada nas datas inicial e final definidas por você.

A seguinte funcionalidade é compatível com essa metodologia:

* Incluir problemas no storyboard [!UICONTROL Scrum]
* Incluir problemas na lista de pendências de uma equipe ágil
* Subtarefas podem ser exibidas no storyboard [!UICONTROL Scrum]
* Exibir um gráfico de burndown para ver o progresso em relação às histórias durante a iteração
Para obter mais informações, consulte [Visão geral do gráfico de burndown ágil](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Criar uma equipe ágil

{{step1-to-team}}

1. Clique no ícone **[!UICONTROL Alternar equipes]** ![Ícone Alternar equipe](assets/switch-team-icon.png) e clique em **[!UICONTROL Criar nova equipe]**.

   ![Selecione Criar nova equipe.](assets/create-new-team-350x198.png)

   A caixa Nova equipe é exibida.

1. Especifique as seguintes informações:

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
      <td>Comece a digitar o nome de um usuário para fazer parte da equipe e selecione o nome quando ele aparecer na lista suspensa.<br>Repita esse processo para adicionar vários usuários à equipe.<br>Como os usuários podem pertencer a mais de uma equipe, eles podem pertencer a equipes ágeis e não ágeis.</td> 
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

{{step1-to-team}}

1. Clique no ícone **[!UICONTROL Equipe de comutação]** ![Ícone Equipe de comutação](assets/switch-team-icon.png) e selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a equipe que você deseja converter em uma equipe ágil.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com uma licença [!UICONTROL Padrão], [!UICONTROL Plano] ou [!UICONTROL Trabalho] podem ver esta opção.
   ![](assets/edit-team-settings-350x205.png)

1. Na seção **[!UICONTROL Agile]**, selecione **[!UICONTROL Equipe Agile]**.

1. Na seção **[!UICONTROL Metodologia]**, selecione se a equipe usará uma metodologia ágil de **[!UICONTROL Scrum]** ou **[!UICONTROL Kanban]**.

1. Clique em **Salvar alterações**.

   A equipe é salva como uma equipe Agile. Você pode configurar a nova equipe como um Scrum ou uma equipe Kanban ao editá-la.

   Para obter mais informações, consulte os seguintes artigos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
