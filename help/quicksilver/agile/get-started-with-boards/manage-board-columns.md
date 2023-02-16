---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Gerenciar colunas do quadro
description: Um novo quadro contém três colunas por padrão. Você pode adicionar mais colunas, alterar a ordem das colunas, renomear colunas e excluir quaisquer colunas desnecessárias.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 3032fe730d57418d0680f2423ebb389cbe8bae1e
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 0%

---

# Gerenciar colunas do quadro

{{highlighted-preview}}

Um novo quadro contém três colunas por padrão. Você pode adicionar mais colunas, alterar a ordem das colunas, renomear colunas e excluir quaisquer colunas desnecessárias.

As configurações de coluna incluem políticas, que permitem definir opções para o que acontece com um cartão quando ele é movido para essa coluna.

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
   <td> <p>[!UICONTROL Solicitação] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Adicionar uma coluna a um quadro

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Quadros]**.
1. Acesse um quadro. Para obter mais informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em **[!UICONTROL Adicionar coluna]** à direita das colunas existentes.
1. Na nova coluna, digite um nome e clique em **[!UICONTROL Adicionar coluna]**.

   ![Adicionar nova coluna](assets/boards-add-column.png)

>[!TIP]
>
>Para adicionar uma coluna de entrada, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Reordenar colunas em um quadro

1. Acesse o quadro.
1. Arraste e solte as colunas na ordem correta. Certifique-se de selecionar a parte superior da coluna antes de arrastá-la para outro local.

   ![Arrastar e soltar coluna](assets/boards-dragdropcolumn.png)

## Renomear uma coluna de quadro

1. Acesse o quadro.
1. Clique no nome da coluna, digite o novo nome e pressione Enter.

   Ou

   Clique no botão **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) na coluna e selecione **[!UICONTROL Editar]**. Na área Configurações , digite o novo nome na **[!UICONTROL Nome da coluna]** e clique em **[!UICONTROL Fechar]**.

## Excluir uma coluna de quadro

1. Acesse o quadro.
1. Clique no botão **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) na coluna e selecione **[!UICONTROL Excluir]**.

   >[!NOTE]
   >
   >As colunas que contêm cartões, incluindo cartões arquivados, não podem ser excluídas. Se você tentar excluir uma coluna que contém cartões, é necessário escolher outra coluna para esses cartões.

## Exibir contagem de cartão

Você pode usar uma configuração para exibir o número de cartões em cada coluna.

Se você estiver usando o limite WIP em uma coluna, um contador de cartão separado não será adicionado. Para obter mais informações sobre limites WIP, consulte [Gerencie o [!UICONTROL Trabalho em Andamento] Limite (WIP) em um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Acesse o quadro.
1. Clique em **[!UICONTROL Configurar]** à direita do quadro para abrir o painel Configurar .
1. Expandir **[!UICONTROL Coluna]**.
1. Ligar **[!UICONTROL Exibir uma contagem de cartão de coluna]**.

   ![Ativar contador de cartão](assets/display-card-count.png)

   O contador de cartão aparece na parte superior de cada coluna.

1. Clique em **[!UICONTROL Ocultar configuração]** para fechar o [!UICONTROL Configurar] painel.

## Definir configurações e políticas da coluna

1. Acesse o quadro.
1. Clique no botão **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) na coluna e selecione **[!UICONTROL Editar]**.

   O [!UICONTROL Configurações] será exibida. O **[!UICONTROL Nome da coluna]** O permite saber para qual coluna você está definindo configurações.

1. Ative o **[!UICONTROL Atualizar valores de campo automaticamente]** política para alterar determinados valores de campo automaticamente quando um cartão for movido para essa coluna.

   ![Configurações e políticas da coluna](assets/boards-column-policies-enabled.png)

1. (Opcional) Defina um valor para o status do cartão:

   1. Selecione o **[!UICONTROL Status]** caixa de seleção.

   1. Selecione o status a ser aplicado a um cartão quando ele for movido para essa coluna.

      ![Status para colunas](assets/boards-column-status.png)

      As opções de tradução de status para cartões conectados também são exibidas. (A tradução de status não se aplica aos cartões ad hoc.) Essas opções determinam o status aplicado à tarefa ou ocorrência em [!DNL Workfront] quando uma placa conectada é movida para essa coluna.

   1. Para alterar as seleções de tradução de status padrão, clique no botão **[!UICONTROL Editar]** ícone ![Ícone Editar](assets/edit-icon-spectrum.png).
   1. <span class="preview">No ambiente de Visualização: Selecione um [!UICONTROL **Personalizado**] e um [!UICONTROL **Sistema**] status a ser aplicado ao cartão, para tarefas e problemas.</span>

      <span class="preview">Quando um cartão é movido para esta coluna, [!DNL Workfront] O primeiro tenta aplicar o status personalizado (por exemplo, Resolvido). Se o status personalizado não estiver disponível para esse cartão, a Workfront aplicará o status do sistema (por exemplo, Fechado).</span>

      <span class="preview">Além disso, se o status na tarefa ou problema conectado for alterado para o status personalizado ou do sistema definido na política de coluna, o cartão será movido automaticamente para a coluna .</span>

   1. No ambiente Produção: Selecione um status para tarefas e um status para problemas. Somente o padrão [!DNL Workfront] os status estão disponíveis, não os status personalizados.

      >[!NOTE]
      >
      >Se você usar status personalizados em [!DNL Workfront], na primeira vez que você mover um cartão conectado para essa coluna, será solicitado a escolher um status. Por exemplo, se o projeto conectado tiver vários tipos de status que correspondem a [!UICONTROL Concluído], você deve escolher em qual status usar [!DNL Workfront]. Você pode definir sua escolha como padrão, de modo que não precise fazer a seleção sempre que mover um cartão para a coluna.
      >Para obter mais informações sobre status, consulte [Visão geral dos status](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

1. (Opcional) Defina um valor para os destinatários do cartão:

   1. Selecione o **[!UICONTROL Destinatários]** caixa de seleção.
   1. Selecione uma ação.

      * **[!UICONTROL Adicionar destinatários]:** Os destinatários selecionados são adicionados à lista existente de destinatários em um cartão quando movidos para essa coluna.
      * **[!UICONTROL Substituir destinatários]:** Os destinatários que você seleciona substituem todos os outros destinatários e se tornam os únicos destinatários de um cartão quando ele é movido para essa coluna.
   1. Selecione os destinatários na lista suspensa. Somente os membros no quadro estão disponíveis para escolha. Para obter mais informações, consulte [Adicionar ou remover membros de um quadro](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

      ![Destinatários da coluna](assets/boards-column-assignees.png)


1. (Opcional) Defina um valor para as tags de cartão:

   1. Selecione o **[!UICONTROL Cartões]** caixa de seleção.
   1. Selecione uma ação.

      * **[!UICONTROL Adicionar tags]:** As tags selecionadas são adicionadas à lista existente de tags em um cartão quando movidas para essa coluna.
      * **[!UICONTROL Substituir tags]:** As tags selecionadas substituem todas as outras tags e se tornam as únicas em um cartão quando são movidas para essa coluna.
   1. Selecione as tags na lista suspensa. Somente as tags já criadas no [!UICONTROL Gerenciador de tags] estão disponíveis para escolha. Para obter informações sobre como adicionar novas tags, consulte [Adicionar tags](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Tags da coluna](assets/boards-column-tags.png)


1. Ative o **[!UICONTROL Limite de trabalho em andamento]** política para limitar o número de cartões que podem ser adicionados à coluna. Em seguida, digite o número do limite na variável **[!UICONTROL Definir limite]** campo.

   ![Limite WIP para coluna](assets/boards-wip-limit-in-column.png)

   Para obter mais informações, consulte [Gerenciar o limite de Trabalho em Andamento (WIP) em um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Clique em **[!UICONTROL Fechar]** para sair da área Configurações e exibir a coluna e seus cartões.
