---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Gerenciar colunas do quadro
description: Um novo quadro contém três colunas por padrão. Você pode adicionar mais colunas, alterar a ordem das colunas, renomear colunas e excluir colunas desnecessárias. Você também pode definir políticas de coluna.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 040dd446ff2b347dabf8a139feb17fd1a7d50e4e
workflow-type: tm+mt
source-wordcount: '1149'
ht-degree: 0%

---

# Gerenciar colunas do quadro

<!-- Audited: 05/2024 -->

Um novo quadro contém três colunas por padrão. Você pode adicionar mais colunas, alterar a ordem das colunas, renomear colunas e excluir colunas desnecessárias.

As configurações de coluna incluem políticas, que permitem definir opções para o que acontece a um cartão quando ele é movido para essa coluna.

Para obter informações sobre como classificar os cartões em colunas, consulte [Filtrar e pesquisar em um quadro](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: Colaborador ou superior </p>
        <p>ou</p> 
        <p>Atual: [!UICONTROL Request] ou superior </p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Adicionar uma coluna a um quadro

{{step1-to-boards}}

1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
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

## Renomear uma coluna do quadro

1. Acesse o quadro.
1. Clique no nome da coluna, digite o novo nome e pressione Enter.

   Ou

   Clique em **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) na coluna e selecione **[!UICONTROL Editar]**. Na área Configurações, digite o novo nome no campo **[!UICONTROL Nome da coluna]** e clique em **[!UICONTROL Fechar]**.

## Excluir uma coluna de quadro

Quando você exclui uma coluna de um quadro, ela não pode ser recuperada.

1. Acesse o quadro.
1. Clique em **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) na coluna e selecione **[!UICONTROL Excluir]**.

   >[!NOTE]
   >
   >As colunas que contêm cartões, incluindo cartões arquivados, não podem ser excluídas. Se você tentar excluir uma coluna que contém cartões, deverá escolher outra coluna para esses cartões.

## Exibir contagem de cartões

Você pode usar uma definição de configuração para exibir o número de cartões em cada coluna.

Se você estiver usando o limite de WIP em uma coluna, não será adicionado um contador de placa separado. Para obter mais informações sobre limites WIP, consulte [Gerenciar o [!UICONTROL Trabalho em progresso] Limite (WIP) em um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Acesse o quadro.
1. Clique em **[!UICONTROL Configurar]** à direita da placa para abrir o painel Configurar.
1. Expandir **[!UICONTROL Coluna]**.
1. Ativar **[!UICONTROL Exibir uma contagem de cartão de coluna]**.

   ![Ativar contador de cartões](assets/display-card-count.png)

   O contador de cartão é exibido na parte superior de cada coluna.

1. Clique em **[!UICONTROL Ocultar configuração]** para fechar o [!UICONTROL Configurar] painel.

## Definir configurações e políticas de coluna

As políticas de coluna incluem a atualização automática dos valores de campo e a configuração de um limite de trabalho em andamento.

A política de atualização do status funciona automaticamente para o cartão e a coluna:

* Quando um cartão é movido para uma coluna com uma política, o status do cartão é atualizado para o status definido na política. Isso se aplica a placas ad hoc e conectadas.
* Quando um status ad hoc ou cartão conectado é atualizado no cartão para corresponder ao status da coluna na política ou um status de cartão conectado é atualizado em outro lugar no Workfront, o cartão é movido automaticamente para essa coluna. Além disso, se um status personalizado em um cartão corresponder ao status do sistema atribuído à coluna, o cartão é movido para essa coluna.

Um cartão permanecerá em uma coluna em que é colocado se o status do cartão não corresponder a nenhum status definido em nenhuma política de coluna existente.

>[!NOTE]
>
>Os painéis dinâmicos sempre colocam cartões na coluna que corresponde ao status, independentemente das políticas de coluna estarem ativadas ou desativadas. Os cartões retornarão às colunas atribuídas quando você atualizar o quadro.
> 
>Além disso, para todos os tipos de quadro, se você mover um cartão de uma coluna para outra coluna com o mesmo status, o cartão retornará à coluna original quando você atualizar o quadro.

1. Acesse o quadro.
1. Clique em **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) na coluna e selecione **[!UICONTROL Editar]**.

   A variável [!UICONTROL Configurações] é exibida. A variável **[!UICONTROL Nome da coluna]** informa para qual coluna você está definindo configurações.

1. Ativar o **[!UICONTROL Atualizar valores de campo automaticamente]** política para alterar determinados valores de campo automaticamente quando um cartão for movido para essa coluna.

   ![Configurações e políticas de coluna](assets/boards-column-policies-enabled.png)

1. (Opcional) Defina um valor para o status do cartão:

   1. Selecione o **[!UICONTROL Status]** caixa de seleção

   1. Selecione o status a ser aplicado a um cartão quando ele for movido para essa coluna.

      ![Status das colunas](assets/boards-column-status.png)

      As opções de conversão de status para cartões conectados também são exibidas. (A tradução de status não se aplica a cartões ad hoc.) Essas opções determinam o status personalizado aplicado à tarefa ou problema no [!DNL Workfront] quando um cartão conectado é movido para essa coluna.

   1. Selecione um [!UICONTROL **Personalizado**] Status a ser aplicado ao cartão para tarefas e problemas.

      Quando um cartão é movido para essa coluna, [!DNL Workfront] O primeiro tenta aplicar o status personalizado (por exemplo, Resolvido). Se o status personalizado selecionado não estiver disponível para essa placa, você será solicitado a escolher outro status que corresponda ao status do sistema (da etapa b acima). Para obter mais informações sobre status, consulte [Visão geral dos status](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      Além disso, se o status na tarefa ou problema conectado for alterado para o status personalizado ou do sistema definido na política de coluna, o cartão será movido automaticamente para a coluna.

1. (Opcional) Defina um valor para os atribuídos do cartão:

   1. Selecione o **[!UICONTROL Responsáveis]** caixa de seleção
   1. Selecione uma ação.

      * **[!UICONTROL Adicionar responsáveis]:** Os atribuídos selecionados são adicionados à lista existente de atribuídos em um cartão quando ele é movido para essa coluna.
      * **[!UICONTROL Substituir responsáveis]:** Os atribuídos selecionados substituem todos os outros atribuídos e se tornam os únicos atribuídos em um cartão quando ele é movido para essa coluna.

   1. Clique em [!UICONTROL **Adicionar atribuição**] e procure um usuário. Selecione os atribuídos nos resultados da pesquisa. Todos os usuários e equipes do Workfront estão disponíveis para escolha.

      ![Responsáveis pela coluna](assets/boards-column-assignees.png)

1. (Opcional) Defina um valor para as tags do cartão:

   1. Selecione o **[!UICONTROL Cartões]** caixa de seleção
   1. Selecione uma ação.

      * **[!UICONTROL Adicionar em tags]:** As tags selecionadas são adicionadas à lista existente de tags em um cartão quando ele é movido para essa coluna.
      * **[!UICONTROL Substituir tags]:** As tags selecionadas substituem todas as outras tags e se tornam as únicas tags em um cartão quando ele é movido para essa coluna.

   1. Selecione as tags na lista suspensa. Somente as tags já criadas na [!UICONTROL Gerenciador de tags] estão disponíveis para escolha. Para obter informações sobre como adicionar novas tags, consulte [Adicionar tags](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Tags para a coluna](assets/boards-column-tags.png)

1. Ativar o **[!UICONTROL Limite de trabalho em andamento]** política para limitar o número de cartões que podem ser adicionados à coluna. Em seguida, digite o número do limite na caixa **[!UICONTROL Definir limite]** campo.

   ![Limite de WIP para a coluna](assets/boards-wip-limit-in-column.png)

   Para obter mais informações, consulte [Gerenciar o limite Trabalho em curso (WIP) em um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Clique em **[!UICONTROL Fechar]** para sair da área Configurações e visualizar a coluna e seus cartões.
