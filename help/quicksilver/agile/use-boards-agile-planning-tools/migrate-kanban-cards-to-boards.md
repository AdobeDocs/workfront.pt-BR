---
content-type: reference
navigation-topic: boards
title: Migrar cartões Kanban da Equipe Agile para painéis do Workfront
description: Você pode migrar seus itens de trabalho de um quadro Kanban da Equipe Agile para um quadro Workfront novo ou existente.
author: Courtney
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/RXk7PYF6JsdF71pRVwEA-Wk23h-UqbgLPXSyNR7VX5Y
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 360
ht-degree: 11%

---

# Migrar cartões Kanban da equipe ágil para o Workfront Boards

Você pode migrar seus itens de trabalho de um quadro Kanban da Equipe Agile para um quadro Workfront novo ou existente. Quando você executa a migração, todos os cartões no quadro Kanban são copiados para o quadro Workfront. Você não tem permissão para escolher cartões específicos.

O posicionamento dos cartões no quadro do Workfront é baseado nas políticas de coluna. (Por exemplo, uma política poderia mover todos os cartões com status de &quot;Em andamento&quot; para uma coluna específica. Para obter mais informações sobre políticas de coluna, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Se não houver políticas ou os cartões não corresponderem às políticas, os cartões serão colocados na coluna mais à esquerda do quadro. Nesse momento, os cartões na coluna Backlog da placa herdada não são adicionados à placa Workfront.

Os cartões não são removidos do quadro Kanban da equipe Agile e as alterações de status do cartão serão sincronizadas com ambos os quadros. Você pode manter ambas as placas ativas até estar pronto para mudar para Workfront Boards.

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
   <td> 
   <p>Colaborador ou posterior</p> 
   <p>Solicitação ou posterior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Migrar cartões Kanban para um novo quadro

{{step1-to-team}}

1. Acessar um quadro Kanban.
1. Clique em [!UICONTROL **Adicionar aos Quadros**] e selecione [!UICONTROL **Novo Quadro**].
1. Na caixa de diálogo [!UICONTROL Adicionar ao novo painel], digite um nome para o novo painel (o nome do atual painel [!UICONTROL Kanban] é exibido automaticamente) e clique em [!UICONTROL **Adicionar**].

   ![Adicionar cartões Kanban ao novo quadro](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Opcional) Na mensagem de sucesso exibida, clique no link para abrir o novo quadro.

## Migrar cartões Kanban para um quadro existente

{{step1-to-team}}

1. Acessar um quadro Kanban.
1. Clique em [!UICONTROL **Adicionar aos Quadros**] e selecione [!UICONTROL **Quadro Existente**].
1. Na caixa de diálogo [!UICONTROL Adicionar ao quadro existente], procure e selecione o quadro para o qual migrar os cartões. Em seguida, clique em [!UICONTROL **Adicionar**].

   ![Adicionar cartões Kanban ao quadro existente](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Opcional) Na mensagem de sucesso exibida, clique no link para abrir o quadro.
