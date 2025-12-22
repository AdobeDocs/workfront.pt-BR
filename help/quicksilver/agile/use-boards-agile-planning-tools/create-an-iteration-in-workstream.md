---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Criar uma iteração em um fluxo de trabalho
description: Uma iteração é uma quantidade definida de tempo reservado para concluir o trabalho. Algumas equipes Agile podem se referir a uma iteração como uma sprint.
author: Jenny
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 4%

---

# Criar uma iteração em um fluxo de trabalho

>[!IMPORTANT]
>
>Os fluxos de trabalho só estão disponíveis para um grupo específico de clientes.

Uma iteração é uma quantidade definida de tempo reservado para concluir o trabalho. Algumas equipes Agile podem se referir a uma iteração como uma sprint.

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
   <p>Colaborador ou superior</p> 
   <p>Solicitação ou superior</p>
   </td> 
  </tr>  
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma iteração em um fluxo de trabalho

{{step1-to-boards}}

1. Abra o fluxo de trabalho ao qual deseja adicionar a iteração. Para abrir um fluxo de trabalho, clique em [!UICONTROL **Exibir fluxo de trabalho**].
1. Crie uma iteração usando um destes métodos:

   * Na guia Lista de Cartão, na exibição de iteração, clique em [!UICONTROL **Criar iteração**].
   * Na guia Lista de Cartão, na exibição em lista, clique em [!UICONTROL **Criar iteração**].
   * Na guia Quadros, clique em [!UICONTROL **Adicionar quadro**] e selecione [!UICONTROL **Processo de Iteração**] como o modelo de quadro. Em seguida, abra o quadro de iteração e clique em [!UICONTROL **Configurar iterações**].

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

1. Para abrir um fluxo de trabalho, clique em [!UICONTROL **Exibir fluxo de trabalho**].
1. Abra a iteração usando um destes métodos:

   * Na guia Lista de Cartão, na exibição de iteração, clique no ícone [!UICONTROL **Detalhes da iteração**] ![Detalhes da iteração](assets/iteration-details-button.png).
   * No quadro de iteração, clique no ícone [!UICONTROL **Detalhes da iteração**] ![Detalhes da iteração](assets/iteration-details-button.png) na área de métricas na parte superior direita.

1. No painel [!UICONTROL Configuração de iteração], edite a iteração conforme necessário.
1. Para alterar o nome da iteração, expanda [!UICONTROL **Detalhes da iteração**].

   Depois que uma iteração é iniciada, você só pode alterar o nome da iteração e não as datas ou a duração da iteração.

<!--   

1. <span class="preview">To add goals to the iteration, expand [!UICONTROL **Goals**].</span>
1. <span class="preview">Click [!UICONTROL **Add goal**], and type the goal name.</span>

   <span class="preview">As goals are completed during the iteration, you can select the check box to mark them complete, or click the **Delete** icon ![Delete icon](assets/delete.png) to delete a goal. The metrics area on the top right of the iteration shows how many goals exist and how many have been completed.</span>

<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## Excluir uma iteração

1. Clique na guia [!UICONTROL **Lista de Cartão**] no fluxo de trabalho e abra a exibição de iteração.
1. Clique no ícone **Excluir** ![Excluir ícone](assets/delete.png) ao lado da iteração.
1. Clique em [!UICONTROL **Excluir iteração**] na mensagem de confirmação.
