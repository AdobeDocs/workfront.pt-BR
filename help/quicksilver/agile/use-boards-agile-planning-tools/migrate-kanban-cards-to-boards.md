---
content-type: reference
navigation-topic: boards
title: Migrar cartões Kanban da Equipe Ágil para quadros do Workfront
description: Você pode migrar seus itens de trabalho de um quadro Kanban da Equipe Ágil para um quadro Workfront novo ou existente.
author: Lisa
feature: Agile
exl-id: c40b6453-5869-437b-a1e0-f20dd833d2b8
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Migrar cartões Kanban da Equipe Ágil para quadros do Workfront

Você pode migrar seus itens de trabalho de um quadro Kanban da Equipe Ágil para um quadro Workfront novo ou existente. Quando você executa a migração, todos os cartões no quadro Kanban são copiados para o quadro Workfront. Você não tem permissão para escolher cartões específicos.

O posicionamento dos cartões no quadro do Workfront é baseado nas políticas de coluna. (Por exemplo, uma política poderia mover todos os cartões com status de &quot;Em andamento&quot; para uma coluna específica. Para obter mais informações sobre políticas de coluna, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Se não houver políticas ou os cartões não corresponderem às políticas, os cartões serão colocados na coluna mais à esquerda do quadro. Nesse momento, os cartões na coluna Backlog da placa herdada não são adicionados à placa Workfront.

Os cartões não são removidos do quadro Kanban da Equipe Ágil e as alterações de status do cartão serão sincronizadas com ambos os quadros. Você pode manter ambas as placas ativas até estar pronto para mudar para Workfront Boards.

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
   <td> <p>Qualquer Um</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td>
   <td> <p>[!UICONTROL Solicitação] ou superior</p> </td>
  </tr>
 </tbody>
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Migrar cartões Kanban para um novo quadro

{{step1-to-team}}

1. Acessar um quadro Kanban.
1. Clique em [!UICONTROL **Adicionar a painéis**] e selecione [!UICONTROL **Novo painel**].
1. No [!UICONTROL Adicionar ao novo quadro] digite um nome para o novo quadro (o nome do atual [!UICONTROL Kanban] automaticamente) e clique em [!UICONTROL **Adicionar**].

   ![Adicionar cartões Kanban ao novo quadro](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Opcional) Na mensagem de sucesso exibida, clique no link para abrir o novo quadro.

## Migrar cartões Kanban para um quadro existente

{{step1-to-team}}

1. Acessar um quadro Kanban.
1. Clique em [!UICONTROL **Adicionar a painéis**] e selecione [!UICONTROL **Quadro existente**].
1. No [!UICONTROL Adicionar a um quadro existente] , procure e selecione o quadro para o qual migrar os cartões. Em seguida, clique em [!UICONTROL **Adicionar**].

   ![Adicionar cartões Kanban ao quadro existente](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Opcional) Na mensagem de sucesso exibida, clique no link para abrir o quadro.
