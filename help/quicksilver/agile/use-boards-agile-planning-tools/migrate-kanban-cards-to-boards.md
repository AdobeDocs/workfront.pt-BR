---
content-type: reference
navigation-topic: boards
title: Migrar cartões Kanban da Equipe Agile para painéis do Workfront
description: Você pode migrar seus itens de trabalho de um quadro Kanban da Equipe Ágil para um quadro Workfront novo ou existente.
author: Lisa
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Migrar cartões Kanban da Equipe Ágil para quadros do Workfront

Você pode migrar seus itens de trabalho de um quadro Kanban da Equipe Ágil para um quadro Workfront novo ou existente. Quando você executa a migração, todos os cartões no quadro Kanban são copiados para o quadro Workfront. Você não tem permissão para escolher cartões específicos.

O posicionamento dos cartões no quadro do Workfront é baseado nas políticas de coluna. (Por exemplo, uma política poderia mover todos os cartões com status de &quot;Em andamento&quot; para uma coluna específica. Para obter mais informações sobre políticas de coluna, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Se não houver políticas ou os cartões não corresponderem às políticas, os cartões serão colocados na coluna mais à esquerda do quadro. Nesse momento, os cartões na coluna Backlog da placa herdada não são adicionados à placa Workfront.

Os cartões não são removidos do quadro Kanban da Equipe Ágil e as alterações de status do cartão serão sincronizadas com ambos os quadros. Você pode manter ambas as placas ativas até estar pronto para mudar para Workfront Boards.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> 
   <p>Novo: [!UICONTROL Contributor] ou superior</p> 
   <p>ou</p>
   <p>Atual: [!UICONTROL Request] ou superior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
