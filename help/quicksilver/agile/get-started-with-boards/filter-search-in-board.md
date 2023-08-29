---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Filtrar e pesquisar em um quadro
description: Você pode filtrar um quadro para exibir apenas determinados cartões.
author: Lisa
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: 44ced4ec8af150bc373699389bd63d150cc387f6
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# Filtrar e pesquisar em um quadro

Você pode filtrar um quadro para exibir:

* Cartões atribuídos a determinadas pessoas
* Cartões com determinadas tags
* Cartões com um status específico
* Cartões com vencimento em um determinado período de tempo
* Cartões arquivados
* Cartões conectados a um projeto específico

A classificação do quadro classifica todos os cartões nas colunas. Não é possível classificar uma única coluna, e a coluna de backlog ou de entrada não é classificada.

A pesquisa também ajuda a localizar um cartão específico no quadro.

Quando os filtros são aplicados, um indicador é exibido no quadro ![Filtro aplicado ao quadro](assets/boards-filterapplied-30x30.png). Clique em **[!UICONTROL Limpar tudo]** para remover todos os filtros do quadro, e clique no ícone recolher para fechar o painel filtro.

![Painel Filtro](assets/boards-all-filters-collapsed-0823.png)

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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

## Filtrar um quadro por responsáveis

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Quadros]**.
1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em [!UICONTROL **Filtro**], expanda a [!UICONTROL Membros] e selecione a pessoa ou as pessoas cujos cartões você deseja ver. Também é possível exibir cartões não atribuídos.

   ![Filtrar por membro](assets/boards-filter-by-assignees-0822.png)

## Filtrar um quadro por tags

1. Acesse o quadro.
1. Clique em [!UICONTROL **Filtro**], expanda a [!UICONTROL Tags] e selecione as tags que deseja ver.

   ![Filtrar por tag](assets/boards-filter-by-tags-0822.png)

## Filtrar um quadro por status

1. Acesse o quadro.
1. Clique em [!UICONTROL **Filtro**], expanda a [!UICONTROL Status] e selecione os tipos de status que deseja ver.

   Também é possível ocultar cartões concluídos.

   ![Filtrar por status](assets/boards-filter-by-status-0822.png)

## Filtrar um quadro pela data de vencimento

1. Acesse o quadro.
1. Clique em [!UICONTROL **Filtro**], expanda a [!UICONTROL Prazo] e selecione as opções de data que deseja ver.

   Somente cartões nos intervalos de datas selecionados são exibidos.

   ![Filtrar por data de vencimento](assets/boards-filter-by-due-date-0822.png)

## Filtrar um quadro para mostrar cartões arquivados

Por padrão, somente os cartões ativos são exibidos em um quadro. Você pode filtrar o quadro para exibir também todos os cartões arquivados.

1. Acesse o quadro.
1. Clique em [!UICONTROL **Filtro**], expanda a [!UICONTROL Cartões arquivados] e selecione **[!UICONTROL Cartões arquivados]** para exibir cartões arquivados.

   O filtro mostra o número de cartões arquivados.

   ![Filtrar cartões arquivados](assets/boards-filter-by-archived-cards_0822.png)

1. Selecionar **[!UICONTROL Cartões arquivados]** novamente para desmarcar a opção e exibir somente cartões ativos.

## Filtrar um quadro por conexão

1. Acesse o quadro.
1. Clique em [!UICONTROL **Filtro**], expanda a [!UICONTROL Conexão] e selecione o [!DNL Workfront] projetos para os cartões conectados que você deseja ver.

   Você também pode exibir cartões que não estão conectados a um projeto.

   ![Filtrar por conexão](assets/boards-filter-by-connection.png)

## Classificar em um quadro

Quando você seleciona uma opção para classificar por, todas as colunas são classificadas. Não é possível classificar uma única coluna, e a coluna de backlog ou de entrada não é classificada.

1. Acesse o quadro.
1. Clique em [!UICONTROL **Classificar por**] e selecione [!UICONTROL **Nome**], [!UICONTROL **Prazo**], [!UICONTROL **Estimativa**], [!UICONTROL **Status**] ou [!UICONTROL **Conexão**].

   A conexão (nome do projeto) se aplica somente a cartões conectados e as outras opções classificarão os cartões conectados e ad hoc nas colunas.

   A opção &quot;ordem do usuário&quot; retorna os cartões na ordem em que foram definidos manualmente, antes de qualquer outra opção de classificação ser aplicada. Essa é a classificação padrão das colunas.

1. Selecionar [!UICONTROL **Ordem inversa**] para classificar as colunas na ordem inversa da opção de classificação.

   A seta no ícone de classificação indica se as colunas são classificadas em ordem crescente ou decrescente.

   Quando uma classificação diferente do padrão é aplicada, um indicador é exibido no ícone de classificação ![Classificação aplicada](assets/sort-applied-boards.png).

   ![Classificar por colunas em um quadro](assets/sort-by-columns-in-board.png)

## Pesquisar em um quadro

1. Acesse o quadro.
1. Clique em [!UICONTROL **Pesquisar**] e digite um termo de pesquisa. Em seguida, pressione Enter.

   Todos os cartões que contêm o termo de pesquisa são exibidos.

   Clique no X para limpar a pesquisa.

   ![Pesquisar cartões em um quadro](assets/boards-searchbox.png)
