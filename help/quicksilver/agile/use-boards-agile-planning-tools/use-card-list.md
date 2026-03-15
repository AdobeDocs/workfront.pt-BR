---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Usar a Lista de Cartões
description: É possível criar uma lista de cartões em um fluxo de trabalho e adicionar os cartões a iterações.
author: Courtney
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 9%

---

# Usar a lista de cartões

>[!IMPORTANT]
>
>Os fluxos de trabalho não estão disponíveis para todos os clientes.

É possível criar uma lista de cartões em um fluxo de trabalho e adicionar os cartões a iterações.

A lista de cartões pode funcionar como um acúmulo de trabalho para o fluxo de trabalho.

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

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar cartões à lista de cartões

{{step1-to-boards}}

1. Para abrir um fluxo de trabalho, clique em [!UICONTROL **Exibir fluxo de trabalho**].
1. Click the [!UICONTROL **Card List**] tab.
1. Click [!UICONTROL **Add card**].
1. In the [!UICONTROL **Create/Edit Card**] dialog, add the following information:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>The name of the card.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Description]</strong></td> 
      <td>Uma descrição do cartão.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimativa]</strong></td> 
      <td>O número estimado de horas para o cartão ser concluído. Esta é apenas uma entrada manual.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>Selecione um status para o cartão.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterations]</strong></td> 
      <td>Selecione uma iteração à qual atribuir o cartão.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Destinatários]</strong></td> 
      <td><p>Para atribuir o cartão, comece a digitar um nome no campo de pesquisa e selecione-o quando for exibido na lista. Você pode adicionar indivíduos e equipes e atribuir mais de uma pessoa ou equipe a um cartão.</p><p>Assignees must be members on the workstream or they will not appear in the selection list.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Clique em [!UICONTROL **Salvar**].
1. Continue adding cards until you have built the card list.

## Exibir cartões

Para exibir todos os cartões para o fluxo de trabalho em uma única lista, clique em [!UICONTROL **Exibição de lista**] na guia Lista de cartões.

Para exibir todos os cartões do fluxo de trabalho agrupados por iteração, clique em [!UICONTROL **Exibição de iteração**]. Unplanned cards are displayed in their own group.

To edit an existing card, select it in the list and click [!UICONTROL **Edit**].

To delete a card, select it in the list and click [!UICONTROL **Delete**].

### Filter cards

Cards can only be archived from the iteration board. When a card is archived, it is not displayed in the card list unless you filter to show archived cards. For information about archiving a card, see [Delete or archive a card from a board](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Acesse a lista de cartões para o fluxo de trabalho.
1. Clique em [!UICONTROL **Filtrar**] e selecione [!UICONTROL **Todos**], [!UICONTROL **Cartões ativos**] ou [!UICONTROL **Cartões arquivados**].

   Quando um filtro diferente do padrão é aplicado na lista de cartões, um indicador é exibido no ícone de filtro ![Filtro aplicado](assets/boards-filterapplied-30x30.png).

### Pesquisar na lista de cartões

1. Acesse a lista de cartões para o fluxo de trabalho.
1. Clique em [!UICONTROL **Pesquisar**] e digite um termo de pesquisa. Em seguida, pressione Enter.

   All cards that contain the search term are displayed.
Clique no X para limpar a pesquisa.

   ![Search for cards in a board](assets/boards-searchbox.png)

## Add cards to an iteration

>[!NOTE]
>
>You must create an iteration before you can add cards to it. For information, see [Create an iteration in a workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Access the card list for the workstream.
1. Select the [!UICONTROL **Iteration view**] to see which cards are assigned to an iteration and which are unplanned.
1. Select an unplanned card in the list and click [!UICONTROL **Edit**].
1. Select an iteration in the [!UICONTROL **Iterations**] field.
1. If you are using story points, enter a value in the [!UICONTROL **Estimation**] field.
1. Clique em [!UICONTROL **Salvar**].

   A placa é movida para a iteração e as métricas de iteração refletem o número de placas e pontos.

   Você também pode arrastar e soltar um cartão do grupo Cartões não planejados na iteração ou clicar em [!UICONTROL **Adicionar cartão**] para adicionar um novo cartão à iteração.

>[!TIP]
>
>Se você tiver criado um quadro de processo de iteração, todos os cartões não planejados na lista de cartões aparecerão na coluna [!UICONTROL Lista de pendências]. Quando uma placa é movida para outra coluna, ela se torna parte da iteração ativa. Os cartões adicionados à iteração na lista de cartões são adicionados a uma coluna com base em seu status.
