---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Excluir ou arquivar um cartão de um quadro
description: Ao excluir um cartão de um quadro, ele é permanentemente excluído e não pode ser restaurado. O arquivamento de um cartão o envia para o arquivo e você pode restaurá-lo para o quadro posteriormente.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 46099e6ceba4310453743c023823e8952f5ce553
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# Excluir ou arquivar um cartão de um quadro

Ao excluir um cartão ad hoc de um quadro, ele é permanentemente excluído e não pode ser restaurado. Os cartões conectados podem ser adicionados manualmente de volta a um quadro após serem excluídos.

Se você excluir um cartão conectado de um quadro dinâmico, ele reaparecerá quando você atualizar o quadro porque esse tipo de quadro extrai todas as tarefas e problemas de um projeto específico. Para excluir o cartão, você deve excluir a tarefa ou problema conectado do projeto Workfront.

Quando você exclui um cartão conectado de qualquer outro tipo de placa que tenha uma coluna de entrada, o cartão reaparecerá na coluna de entrada quando você atualizar o quadro se a tarefa ou problema conectado ainda não estiver marcado como concluído. Para obter mais informações sobre colunas de entrada, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

O arquivamento de um cartão o envia para o arquivo e você pode restaurá-lo para o quadro posteriormente.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Solicitação] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Excluir um cartão de um quadro

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Quadros]**.
1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) no cartão e selecione **[!UICONTROL Excluir]**.
1. Clique em **[!UICONTROL Excluir]** na mensagem de confirmação.

## Arquivar um cartão de um quadro

1. Acesse o quadro.
1. Clique em **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) no cartão e selecione **[!UICONTROL Arquivar]**.

   Cartões arquivados ficam ocultos no quadro, a menos que você aplique um filtro para exibi-los. Para obter mais informações, consulte [Filtrar um quadro para mostrar cartões arquivados](#filter-a-board-to-show-archived-cards) neste artigo.

   Um [!UICONTROL Arquivar] ícone ![Arquivar](assets/archive-icon-spectrum-25x20.png) é exibido em cartões arquivados. Você não pode editar um cartão arquivado, mas pode excluí-lo ou movê-lo para outra coluna.

1. Para restaurar um cartão arquivado, clique no link **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) no cartão e selecione **[!UICONTROL Restaurar]**.

## Filtrar um quadro para mostrar cartões arquivados {#filter-a-board-to-show-archived-cards}

Por padrão, somente os cartões ativos são exibidos em um quadro. Você pode filtrar o quadro para exibir também todos os cartões arquivados.

1. Acesse o quadro.
1. Clique em [!UICONTROL **Configurar**] à direita da placa para abrir o painel Configurar.
1. Expandir [!UICONTROL **Cartões**].
1. Ativar [!UICONTROL **Exibir cartões arquivados no quadro**].
1. Clique em [!UICONTROL **Filtro**], expanda a [!UICONTROL Cartões arquivados] e selecione **[!UICONTROL Cartões arquivados]** para exibir cartões arquivados.

   O filtro mostra o número de cartões arquivados.

   ![Filtrar cartões arquivados](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >A variável [!UICONTROL Cartões arquivados] A seção não está disponível no filtro se você não ativou a configuração para exibir cartões arquivados. Para obter mais informações, consulte [Personalizar quais campos são exibidos em um cartão](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Selecionar **[!UICONTROL Cartões arquivados]** novamente para desmarcar a opção e exibir somente cartões ativos.
