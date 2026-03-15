---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Gerenciar colunas do painel
description: Um novo painel contém três colunas por padrão. É possível adicionar mais colunas, alterar a ordem das colunas, renomear colunas e excluir colunas desnecessárias. Você também pode definir políticas de coluna.
author: Courtney
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '1081'
ht-degree: 4%

---

# Gerenciar colunas do quadro

<!-- Audited: 05/2024 -->

Um novo painel contém três colunas por padrão. É possível adicionar mais colunas, alterar a ordem das colunas, renomear colunas e excluir colunas desnecessárias.

As configurações de coluna incluem políticas, que permitem definir opções para o que acontece a um cartão quando ele é movido para essa coluna.

Para obter informações sobre como classificar os cartões em colunas, consulte [Filtrar e pesquisar em um painel](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar uma coluna a um painel

{{step1-to-boards}}

1. Acessar um painel. Para obter mais informações, consulte [Criar ou editar um painel](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em **[!UICONTROL Adicionar Coluna]** à direita das colunas existentes.
1. Na nova coluna, digite um nome e clique em **[!UICONTROL Adicionar Coluna]**.

   ![Adicionar nova coluna](assets/boards-add-column.png)

>[!TIP]
>
>Para adicionar uma coluna de entrada, consulte [Adicionar uma coluna de entrada a um painel](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Reordenar colunas em um painel

1. Acesse o painel.
1. Arraste e solte as colunas na ordem correta. Certifique-se de selecionar a parte superior da coluna antes de arrastá-la para outro local.

   ![Arrastar e soltar coluna](assets/boards-dragdropcolumn.png)

## Renomear uma coluna de quadro

1. Acesse o painel.
1. Clique no nome da coluna, digite o novo nome e pressione Enter.

   Ou

   Clique no menu **[!UICONTROL Mais]** ![Mais menus](assets/more-icon-spectrum.png) na coluna e selecione **[!UICONTROL Editar]**. Na área Configurações, digite o novo nome no campo **[!UICONTROL Nome da coluna]** e clique em **[!UICONTROL Fechar]**.

## Excluir uma coluna do quadro

Quando você exclui uma coluna de um painel, ela não pode ser recuperada.

1. Acesse o painel.
1. Clique no menu **[!UICONTROL Mais]** ![Mais menus](assets/more-icon-spectrum.png) na coluna e selecione **[!UICONTROL Excluir]**.

   >[!NOTE]
   >
   >As colunas que contêm cartões, incluindo cartões arquivados, não podem ser excluídas. Se você tentar excluir uma coluna que contém cartões, deverá escolher outra coluna para esses cartões.

## Exibir contagem de cartões

Você pode usar uma definição de configuração para exibir o número de cartões em cada coluna.

Se você estiver usando o limite de WIP em uma coluna, um contador de placa separado não será adicionado. Para obter mais informações sobre limites WIP, consulte [Gerenciar o limite de [!UICONTROL Trabalho em andamento] (WIP) em um painel](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Acesse o painel.
1. Clique em **[!UICONTROL Configurar]** à direita do painel para abrir o painel Configurar.
1. Expanda a **[!UICONTROL Coluna]**.
1. Ative **[!UICONTROL Exibir uma contagem de cartões de coluna]**.

   ![Ativar contador de cartões](assets/display-card-count.png)

   O contador do cartão aparece na parte superior de cada coluna.

1. Clique em **[!UICONTROL Ocultar configuração]** para fechar o painel [!UICONTROL Configurar].

## Definir configurações e políticas de coluna

As políticas de coluna incluem a atualização automática de valores de campo e a definição de um limite de trabalho em andamento.

A política para atualizar o status funciona automaticamente para o cartão e para a coluna:

* Quando um cartão é movido para uma coluna com uma política, seu status é atualizado para o status definido na política. Isso se aplica a placas ad hoc e conectadas.
* Quando o status de um cartão ad hoc ou conectado é atualizado no cartão para corresponder ao status da coluna na política ou um status de cartão conectado é atualizado em outro local no Workfront, o cartão é movido automaticamente para essa coluna. Além disso, se um status personalizado em um cartão corresponder ao status de sistema atribuído à coluna, o cartão será movido para essa coluna.

Um cartão permanecerá em uma coluna onde é colocado se o status do cartão não corresponder a nenhum status definido em quaisquer políticas de coluna existentes.

1. Acesse o painel.
1. Clique no menu **[!UICONTROL Mais]** ![Mais menus](assets/more-icon-spectrum.png) na coluna e selecione **[!UICONTROL Editar]**.

   A área [!UICONTROL Configurações] é exibida. O **[!UICONTROL Nome da coluna]** permite saber para qual coluna você está definindo configurações.

1. Habilite a política **[!UICONTROL Atualizar valores de campo automaticamente]** para alterar certos valores de campo automaticamente quando um cartão for movido para esta coluna.

   ![Configurações e políticas de coluna](assets/boards-column-policies-enabled.png)

1. (Opcional) Defina um valor para o status do cartão:

   1. Marque a caixa de seleção **[!UICONTROL Status]**.

   1. Selecione o status a ser aplicado a um cartão quando ele for movido para esta coluna.

      ![Status para colunas](assets/boards-column-status.png)

      As opções de conversão de status para cartões conectados também são exibidas. (A conversão de status não se aplica a cartões ad hoc.) Essas opções determinam o status personalizado aplicado à tarefa ou ocorrência em [!DNL Workfront] quando um cartão conectado é movido para esta coluna.

   1. Selecione um status [!UICONTROL **Personalizado**] para aplicar ao cartão para tarefas e problemas.

      Quando um cartão é movido para esta coluna, [!DNL Workfront] tenta primeiro aplicar o status personalizado (por exemplo, Resolvido). Se o status personalizado selecionado não estiver disponível para esse cartão, você será solicitado a escolher outro status que corresponda ao status do sistema (da etapa b acima). Para obter mais informações sobre status, consulte [Visão geral sobre status](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      Além disso, se o status na tarefa ou ocorrência conectada for alterado para o status personalizado ou do sistema definido na política de coluna, o cartão será automaticamente movido para a coluna.

1. (Opcional) Defina um valor para os destinatários do cartão:

   1. Marque a caixa de seleção **[!UICONTROL Atribuídos]**.
   1. Selecione uma ação.

      * **[!UICONTROL Adicionar destinatários]:** os destinatários selecionados são adicionados à lista existente de destinatários em um cartão quando ele é movido para esta coluna.
      * **[!UICONTROL Substituir destinatários]:** os destinatários selecionados substituem todos os outros destinatários e se tornam os únicos destinatários em um cartão quando ele é movido para esta coluna.

   1. Clique em [!UICONTROL **Adicionar Atribuição**] e procure um usuário. Selecione os destinatários nos resultados da pesquisa. Todos os usuários e equipes do Workfront estão disponíveis para escolha.

      ![Destinatários da coluna](assets/boards-column-assignees.png)

1. (Opcional) Defina um valor para as tags de cartão:

   1. Marque a caixa de seleção **[!UICONTROL Cartões]**.
   1. Selecione uma ação.

      * **[!UICONTROL Adicionar em marcas]:** As marcas selecionadas são adicionadas à lista existente de marcas em um cartão quando ele é movido para esta coluna.
      * **[!UICONTROL Substituir marcas]:** As marcas selecionadas substituem todas as outras marcas e se tornam as únicas marcas em um cartão quando ele é movido para esta coluna.

   1. Selecione as tags na lista suspensa. Somente as marcas já criadas no [!UICONTROL Gerenciador de Marcas] estão disponíveis para escolha. Para obter informações sobre como adicionar novas marcas, consulte [Adicionar marcas](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Marcas para coluna](assets/boards-column-tags.png)

1. Habilite a política de **[!UICONTROL Limite de trabalho em andamento]** para limitar o número de cartões que podem ser adicionados à coluna. Em seguida, digite o número do limite no campo **[!UICONTROL Definir limite]**.

   ![Limite de WIP para a coluna](assets/boards-wip-limit-in-column.png)

   Para obter mais informações, consulte [Gerenciar o limite de Trabalho em Andamento (WIP) em uma placa](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Clique em **[!UICONTROL Fechar]** para sair da área Configurações e exibir a coluna e seus cartões.
