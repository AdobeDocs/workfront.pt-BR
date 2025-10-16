---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Usar a lista de cartões
description: Você pode criar uma lista de cartões em um fluxo de trabalho e adicionar os cartões às iterações.
author: Lisa
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Usar a lista de cartões

>[!IMPORTANT]
>
>Os fluxos de trabalho não estão disponíveis para todos os clientes.

Você pode criar uma lista de cartões em um fluxo de trabalho e adicionar os cartões às iterações.

A lista de cartões pode funcionar como um backlog de trabalho para o workflow.

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

## Adicionar cartões à lista de cartões

{{step1-to-boards}}

1. Para abrir um fluxo de trabalho, clique em [!UICONTROL **Exibir fluxo de trabalho**].
1. Clique na guia [!UICONTROL **Lista de cartões**].
1. Clique em [!UICONTROL **Adicionar cartão**].
1. Na caixa de diálogo [!UICONTROL **Criar/Editar Cartão**], adicione as seguintes informações:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Nome]</strong></td> 
      <td>O nome do cartão.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Descrição]</strong></td> 
      <td>Uma descrição do cartão.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimativa]</strong></td> 
      <td>O número estimado de horas para a conclusão do cartão. Esta entrada é apenas manual.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>Selecione um status para o cartão.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterações]</strong></td> 
      <td>Selecione uma iteração à qual atribuir o cartão.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Atribuídos]</strong></td> 
      <td><p>Para atribuir o cartão, comece digitando um nome no campo de pesquisa e, em seguida, selecione-o quando ele for exibido na lista. Você pode adicionar indivíduos e equipes e atribuir mais de uma pessoa ou equipe a um cartão.</p><p>Os atribuídos devem ser membros no fluxo de trabalho ou não aparecerão na lista de seleção.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Clique em [!UICONTROL **Salvar**].
1. Continue adicionando cartões até criar a lista de cartões.

## Exibir cartões

Para exibir todos os cartões para o fluxo de trabalho em uma única lista, clique em [!UICONTROL **Exibição de lista**] na guia Lista de cartões.

Para exibir todos os cartões do fluxo de trabalho agrupados por iteração, clique em [!UICONTROL **Exibição de iteração**]. Os cartões não planejados são exibidos em seu próprio grupo.

Para editar um cartão existente, selecione-o na lista e clique em [!UICONTROL **Editar**].

Para excluir um cartão, selecione-o na lista e clique em [!UICONTROL **Excluir**].

### Filtrar cartões

Os cartões só podem ser arquivados do quadro de iteração. Quando um cartão é arquivado, ele não é exibido na lista de cartões, a menos que você filtre para mostrar cartões arquivados. Para obter informações sobre como arquivar um cartão, consulte [Excluir ou arquivar um cartão de um quadro](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Acesse a lista de cartões para o workflow.
1. Clique em [!UICONTROL **Filtro**] e selecione [!UICONTROL **Todos**], [!UICONTROL **Cartões ativos**] ou [!UICONTROL **Cartões arquivados**].

   Quando um filtro diferente do padrão é aplicado na lista de cartões, um indicador é exibido no ícone de filtro ![Filtro aplicado](assets/boards-filterapplied-30x30.png).

### Pesquisar na lista de cartões

1. Acesse a lista de cartões para o workflow.
1. Clique em [!UICONTROL **Pesquisar**] e digite um termo de pesquisa. Em seguida, pressione Enter.

   Todos os cartões que contêm o termo de pesquisa são exibidos.
Clique no X para limpar a pesquisa.

   ![Pesquisar cartões em um quadro](assets/boards-searchbox.png)

## Adicionar cartões a uma iteração

>[!NOTE]
>
>Você deve criar uma iteração antes de adicionar cartões a ela. Para obter informações, consulte [Criar uma iteração em um fluxo de trabalho](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Acesse a lista de cartões para o workflow.
1. Selecione a [!UICONTROL **Exibição de iteração**] para ver quais cartões estão atribuídos a uma iteração e quais não estão planejados.
1. Selecione um cartão não planejado na lista e clique em [!UICONTROL **Editar**].
1. Selecione uma iteração no campo [!UICONTROL **Iterações**].
1. Se você estiver usando pontos de história, insira um valor no campo [!UICONTROL **Estimativa**].
1. Clique em [!UICONTROL **Salvar**].

   O cartão é movido para a iteração e as métricas de iteração refletem o número de cartões e pontos.

   Você também pode arrastar e soltar um cartão do grupo Cartões não planejados na iteração ou clicar em [!UICONTROL **Adicionar cartão**] para adicionar um novo cartão à iteração.

>[!TIP]
>
>Se você criou um quadro de processo de iteração, todos os cartões não planejados na lista de cartões aparecerão na coluna [!UICONTROL Backlog]. Quando um cartão é movido para outra coluna, ele se torna parte da iteração ativa. Os cartões adicionados à iteração na lista de cartões são adicionados a uma coluna com base em seus status.
