---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Adicionar uma coluna de entrada a um quadro
description: Opcionalmente, é possível adicionar uma coluna de entrada ao quadro que automaticamente extrai tarefas e problemas como cartões conectados quando adicionados no Workfront, com base nos filtros definidos.
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: a4ccd48956fedbafc04ce19198592efdad49e5a3
workflow-type: tm+mt
source-wordcount: '975'
ht-degree: 0%

---

# Adicionar uma coluna de entrada a um quadro

Opcionalmente, é possível adicionar uma coluna de entrada ao quadro que automaticamente inclui tarefas e problemas como cartões conectados quando adicionados em [!DNL Workfront], com base nos filtros definidos por você. A coluna de entrada pode servir como uma coluna de backlog para uma equipe Kanban, um local de entrada para uma equipe de suporte ver os problemas à medida que são adicionados a uma fila de solicitações ou qualquer outro propósito necessário.

Somente uma coluna de entrada é permitida em um quadro e sempre aparece como a coluna mais à esquerda.

A coluna de entrada não está disponível em uma placa dinâmica.

A coluna de entrada não está disponível em placas que fazem parte de um fluxo de trabalho. Em vez disso, você pode configurar uma coluna de backlog para obter cartões da lista de cartões. Para obter informações sobre como adicionar uma coluna de backlog a um quadro em um workflow, consulte [Configurar o backlog em uma placa de workflow](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-backlog-workstream-board.md).

A coluna de entrada é limitada a 300 tarefas e 300 problemas. Elas são classificadas pela prioridade definida nos itens. Para obter informações sobre a prioridade, consulte [Atualizar prioridade da tarefa](/help/quicksilver/manage-work/tasks/task-information/task-priority.md) e [Atualizar prioridade do problema](/help/quicksilver/manage-work/issues/issue-information/update-issue-priority.md).

Para obter mais informações sobre colunas, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Para obter informações sobre placas conectadas, consulte [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

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
   <td> <p>[!DNL Request] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Criar uma coluna de entrada usando filtros simples

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **[!UICONTROL Quadros]**.
1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em **[!UICONTROL Configurar]** à direita da placa para abrir o painel Configurar.
1. Expandir **[!UICONTROL Quadro]**.
1. Ativar **[!UICONTROL Entrada dinâmica de itens no quadro]**.

   ![Opções de filtro simples da coluna de entrada](assets/intake-column-simple-filters.png)

   A coluna de entrada é adicionada à esquerda do quadro. Permanece em branco até que você aplique filtros a ele.

1. (Opcional) Procure por e selecione [!DNL Workfront] [!UICONTROL **Projetos**].
1. (Opcional) Procurar e selecionar usuário ou equipe [!UICONTROL **Atribuições**].
1. Selecionar [!UICONTROL **Incluir trabalho concluído**] para exibir tarefas e problemas com status Concluído na coluna entrada.

   >[!NOTE]
   >
   >Se esta opção não estiver selecionada, quando os cartões em outros status estiverem marcados como concluídos, eles &quot;cairão&quot; do quadro e não serão mais exibidos.

1. Clique em [!UICONTROL **Aplicar**].

   Todos os objetos aparecem na coluna de entrada do quadro como cartões conectados.

   ![Coluna de entrada](assets/intake-column-added3.png)

## Criar uma coluna de entrada usando filtros avançados

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **[!UICONTROL Quadros]**.
1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em **[!UICONTROL Configurar]** à direita da placa para abrir o painel Configurar.
1. Expandir **[!UICONTROL Quadro]**.
1. Ativar **[!UICONTROL Entrada dinâmica de itens no quadro]**.

   A coluna de entrada é adicionada à esquerda do quadro. Permanece em branco até que você aplique filtros a ele.

1. Clique em [!UICONTROL **Usar filtros avançados**].
1. Clique em **[!UICONTROL Adicionar fontes de filtro]** e selecione **[!UICONTROL Tarefas]** ou **[!UICONTROL Problemas]**.

   ![Opções de filtro avançado da coluna de entrada](assets/intake-column-advanced-filters1.png)

   >[!NOTE]
   >
   >Você pode filtrar a coluna de entrada para incluir tarefas e problemas, mas deve configurar os filtros separadamente para cada tipo de objeto.
   >
   >Além disso, os filtros salvos e os filtros padrão do sistema estão disponíveis para seleção.

1. No painel de filtro, clique em **[!UICONTROL Novo filtro]** para começar.

   ![Clique em Novo filtro](assets/intake-filter-dialog5.png)

1. Crie seu filtro e clique em **[!UICONTROL Salvar como novo]**.

   ![Construtor de filtros](assets/intake-filter-dialog6.png)

   Este exemplo mostra um filtro para tarefas de um projeto específico que estão no status de [!UICONTROL Novo] ou [!UICONTROL Em andamento], e são atribuídos a mim.

   Para obter detalhes sobre como criar um filtro, consulte a seção &quot;Criar ou editar um filtro no construtor padrão&quot; no artigo [Criar ou editar filtros no [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. Nomeie o filtro e clique em **[!UICONTROL Salvar]**.

   ![Digite um nome para o filtro](assets/intake-filter-dialog7.png)

   Dar ao filtro um nome exclusivo permite pesquisá-lo posteriormente.

1. O filtro é exibido na lista de filtros salvos e é aplicado automaticamente à coluna de entrada. Clique no X na parte superior do painel de filtro para fechá-lo.

   ![Filtro salvo](assets/intake-filter-dialog8.png)

1. (Opcional) Para compartilhar o filtro com outras pessoas, passe o mouse sobre o filtro salvo, clique no link **[!UICONTROL Mais]** menu ![Ícone do menu Mais](assets/more-icon-spectrum.png)e selecione **[!UICONTROL Compartilhar]**. Escolha os usuários ou equipes com os quais compartilhar na caixa Compartilhamento de filtro. Para obter mais informações, consulte [Compartilhar um filtro, uma exibição ou um agrupamento](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. (Opcional) Para incluir tarefas e problemas na coluna de entrada, clique em **[!UICONTROL Filtrar fontes]** e selecione o outro objeto para criar outro filtro.
1. Quando terminar de adicionar filtros, analise a coluna entrada para verificar se as tarefas e problemas corretos foram exibidos.

   ![Coluna de entrada](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >É possível atualizar os filtros a qualquer momento, abrindo o painel Configurar e clicando em **[!UICONTROL Filtrar fontes]** e selecionando **[!UICONTROL Tarefas]** ou **[!UICONTROL Problemas]**.

## Usar a coluna de entrada

Os cartões na coluna de entrada não são editáveis até que você os mova para outras colunas do quadro. Você pode clicar no cartão para abri-lo em uma exibição somente leitura ou clicar em ![Abrir tarefa ou problema](assets/boards-launch-icon.png) para abrir a tarefa ou o problema em uma nova guia do navegador.


Você pode reordenar manualmente os itens na coluna de entrada.

Os ícones na parte superior direita da coluna de entrada mostram quantos cartões estão atualmente na coluna e quantos filtros são aplicados.

1. (Opcional) Para procurar um item na coluna de entrada, clique em ![Ícone de pesquisa](assets/search-icon.png) na coluna.
1. (Opcional) Para mover um cartão da coluna de entrada para outra coluna, arraste e solte o cartão na posição em que deseja que ele seja exibido.

   Ou

   Clique em **[!UICONTROL Mais]** menu ![Ícone do menu Mais](assets/more-icon-spectrum.png) no cartão e selecione **[!UICONTROL Mover]**. Em seguida, no **[!UICONTROL Mover item]** , escolha outra coluna e selecione **[!UICONTROL Mover]**.

1. (Opcional) Para excluir a coluna de entrada, clique no botão **[!UICONTROL Mais]** menu ![Ícone do menu Mais](assets/more-icon-spectrum.png) e selecione **[!UICONTROL Excluir]**.
