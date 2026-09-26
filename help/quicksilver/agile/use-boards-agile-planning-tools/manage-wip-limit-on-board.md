---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Gerenciar o limite do Trabalho em curso (WIP) em um quadro
description: Você pode configurar um limite de Trabalho em andamento (WIP) para cada coluna de um quadro.
author: Courtney
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/jOCQTCkNgEZfE8O4-KyKVjEluncwWx0vh5NdrKHC9vg'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 14%
---
# Gerenciar o limite de [!UICONTROL Trabalho em andamento] (WIP) em um quadro

Você pode configurar um limite de [!UICONTROL Trabalho em andamento] (WIP) para cada coluna de um quadro.

O limite WIP é simplesmente uma advertência visual e não o impede de ter mais itens em cada coluna do que o limite definido.

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

## Definir o limite de WIP em uma coluna

{{step1-to-boards}}

1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Localize a coluna à qual deseja adicionar o limite de WIP.

   Para adicionar uma nova coluna, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

1. Clique no menu **[!UICONTROL Mais]** na coluna e selecione **[!UICONTROL Editar]** para abrir a área Configurações.
1. Em [!UICONTROL Políticas de Coluna], habilite a política de limite **de**[!UICONTROL  Trabalho em andamento] para limitar o número de cartões que podem ser adicionados à coluna.
1. Digite o número de limite no campo **[!UICONTROL Definir limite]**.

   ![Limite de WIP para a coluna](assets/boards-wip-limit-in-column.png)

   O número de cartões e o limite são exibidos na parte superior da coluna. Se a coluna contiver mais cartões do que o limite, o contador ficará vermelho.

   ![Contador de limite de WIP](assets/boards-wip-limit-counter.png)

1. Clique em **[!UICONTROL Fechar]** para sair da área [!UICONTROL Configurações] e exibir a coluna e seus cartões.
