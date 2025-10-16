---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Excluir ou arquivar um cartão de um quadro
description: Ao excluir um cartão de um quadro, ele é permanentemente excluído e não pode ser restaurado. O arquivamento de um cartão o envia para o arquivo e você pode restaurá-lo para o quadro posteriormente.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Excluir ou arquivar um cartão de um quadro

Ao excluir um cartão ad hoc de um quadro, ele é permanentemente excluído e não pode ser restaurado. Os cartões conectados podem ser adicionados manualmente de volta a um quadro após serem excluídos.

Se você excluir um cartão conectado de um quadro dinâmico, ele reaparecerá quando você atualizar o quadro porque esse tipo de quadro extrai todas as tarefas e problemas de um projeto específico. Para excluir o cartão, você deve excluir a tarefa ou problema conectado do projeto Workfront.

Quando você exclui um cartão conectado de qualquer outro tipo de placa que tenha uma coluna de entrada, o cartão reaparecerá na coluna de entrada quando você atualizar o quadro se a tarefa ou problema conectado ainda não estiver marcado como concluído. Para obter mais informações sobre colunas de entrada, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

O arquivamento de um cartão o envia para o arquivo e você pode restaurá-lo para o quadro posteriormente.

Cartões arquivados não são sincronizados com tarefas e problemas do Workfront. Se você restaurar um cartão, ele será sincronizado novamente.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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

## Excluir um cartão de um quadro

{{step1-to-boards}}

1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique no menu **[!UICONTROL Mais]** ![Mais menus](assets/more-icon-spectrum.png) no cartão e selecione **[!UICONTROL Excluir]**.
1. Clique em **[!UICONTROL Excluir]** na mensagem de confirmação.

## Arquivar um cartão de um quadro

1. Acesse o quadro.
1. Clique no menu **[!UICONTROL Mais]** ![Mais menu](assets/more-icon-spectrum.png) no cartão e selecione **[!UICONTROL Arquivar]**.

   Cartões arquivados ficam ocultos no quadro, a menos que você aplique um filtro para exibi-los. Para obter mais informações, consulte [Filtrar um quadro para mostrar cartões arquivados](#filter-a-board-to-show-archived-cards) neste artigo.

   Um ícone [!UICONTROL Arquivar] ![Arquivar](assets/archive-icon-spectrum-25x20.png) aparece em cartões arquivados. Você não pode editar um cartão arquivado, mas pode excluí-lo ou movê-lo para outra coluna.

1. Para restaurar um cartão arquivado, clique no menu **[!UICONTROL Mais]** ![Mais menu](assets/more-icon-spectrum.png) no cartão e selecione **[!UICONTROL Restaurar]**.

## Filtrar um quadro para mostrar cartões arquivados

Por padrão, somente os cartões ativos são exibidos em um quadro. Você pode filtrar o quadro para exibir também todos os cartões arquivados.

1. Acesse o quadro.
1. Clique em [!UICONTROL **Configurar**] à direita do quadro para abrir o painel Configurar.
1. Expanda [!UICONTROL **Cartões**].
1. Ative [!UICONTROL **Exibir cartões arquivados no quadro**].
1. Clique em [!UICONTROL **Filtro**], expanda a seção [!UICONTROL Cartões Arquivados] e selecione **[!UICONTROL Cartões arquivados]** para exibir todos os cartões arquivados.

   O filtro mostra o número de cartões arquivados.

   ![Filtrar cartões arquivados](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >A seção [!UICONTROL Cartões Arquivados] não estará disponível no filtro se você não tiver ativado a definição de configuração para exibir cartões arquivados. Para obter mais informações, consulte [Personalizar quais campos são exibidos em um cartão](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Selecione **[!UICONTROL Cartões arquivados]** novamente para limpar a opção e exibir apenas cartões ativos.
