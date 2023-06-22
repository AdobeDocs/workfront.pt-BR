---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Criar uma iteração em um fluxo de trabalho
description: Uma iteração é uma quantidade definida de tempo reservado para concluir o trabalho. Algumas equipes ágeis podem se referir a uma iteração como uma sprint.
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: 563e0f443ecef9ee99e9f9bfb5a0d579aa50cef4
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Criar uma iteração em um fluxo de trabalho

{{highlighted-preview}}

Uma iteração é uma quantidade definida de tempo reservado para concluir o trabalho. Algumas equipes ágeis podem se referir a uma iteração como uma sprint.

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

## Criar uma iteração em um fluxo de trabalho

{{step1-to-boards}}

1. Abra o fluxo de trabalho ao qual deseja adicionar a iteração. Para abrir um workflow, clique em [!UICONTROL **Exibir fluxo de trabalho**].
1. Crie uma iteração usando um destes métodos:

   * Na guia Lista de cartões, na visualização de iteração, clique em [!UICONTROL **Criar iteração**].
   * Na guia Lista de cartões, na exibição em lista, clique em [!UICONTROL **Criar iteração**].
   * Na guia Quadros, clique em [!UICONTROL **Adicionar quadro**] e selecione [!UICONTROL **Processo de iteração**] como o modelo do quadro. Em seguida, abra o quadro de iteração e clique em [!UICONTROL **Configurar iterações**].

1. Na caixa de diálogo Detalhes da iteração, adicione as seguintes informações:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Nome da Iteração]</strong></td> 
      <td>O nome da iteração, como "Sprint 1".</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Comprimento da iteração]</strong></td> 
      <td>A duração da iteração, em dias, semanas ou meses.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Data de início]</strong></td> 
      <td>A data em que a iteração começa. A data final é inserida automaticamente com base na duração da iteração.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em [!UICONTROL **Salvar**].

   A iteração agora aparece na visualização de iteração da lista de cartões e na área de métricas no quadro de iteração.

   Para adicionar cartões a uma iteração, consulte [Usar a lista de cartões](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## Editar uma iteração existente

1. Para abrir um workflow, clique em [!UICONTROL **Exibir fluxo de trabalho**].
1. Abra a iteração usando um destes métodos:

   * Na guia Lista de cartões, na visualização de iteração, clique no [!UICONTROL **Detalhes da iteração**] ícone ![Detalhes da iteração](assets/iteration-details-button.png).
   * No quadro de iteração, clique no botão [!UICONTROL **Detalhes da iteração**] ícone ![Detalhes da iteração](assets/iteration-details-button.png) na área métricas na parte superior direita.

1. No [!UICONTROL Configuração de iteração] edite a iteração conforme necessário.
1. Para alterar o nome da iteração, expanda [!UICONTROL **Detalhes da iteração**].

   Depois que uma iteração é iniciada, você só pode alterar o nome da iteração e não as datas ou a duração da iteração.

1. <span class="preview">Para adicionar metas à iteração, expanda [!UICONTROL **Metas**].</span>
1. <span class="preview">Clique em [!UICONTROL **Adicionar meta**] e digite o nome da meta.</span>

   <span class="preview">À medida que as metas são concluídas durante a iteração, você pode marcar a caixa de seleção para marcá-las como concluídas ou clicar no **Excluir** ícone ![Ícone Excluir](assets/delete.png) para excluir uma meta. A área de métricas na parte superior direita da iteração mostra quantas metas existem e quantas foram concluídas.</span>

<!--
<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## Excluir uma iteração

1. Clique em [!UICONTROL **Lista de cartões**] no fluxo de trabalho e abra a visualização de iteração.
1. Clique em **Excluir** ícone ![Ícone Excluir](assets/delete.png) ao lado da iteração.
1. Clique em [!UICONTROL **Excluir iteração**] na mensagem de confirmação.
