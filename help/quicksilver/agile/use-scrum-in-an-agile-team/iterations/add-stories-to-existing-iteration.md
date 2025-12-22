---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Adicionar histórias a uma iteração existente
description: É possível adicionar histórias a uma iteração de várias maneiras.
author: Jenny
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 3%

---

# Adicionar histórias a uma iteração existente

Você pode adicionar histórias a uma iteração de qualquer uma das seguintes maneiras:

* Da lista de pendências após a criação da iteração, conforme descrito na seção [Mover histórias da lista de pendências para uma iteração ou quadro [!UICONTROL Kanban]](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) em [Gerenciar a lista de pendências Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Na página [!UICONTROL Detalhes] da tarefa ou problema individual
* De uma lista de tarefas ou problemas
* De um relatório
* De um painel

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p> 
   <p>Trabalho ou maior</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Gerenciar acesso ao projeto em que a história se encontra </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Entender como a adição de histórias afeta as datas da tarefa

Por padrão, quando você adiciona uma tarefa existente a uma iteração, a [!UICONTROL Data de início planejada] e a [!UICONTROL Data de conclusão planejada] da tarefa são definidas da seguinte maneira:

### [!UICONTROL Data de Início Planejada] da tarefa

* A tarefa usa a Data inicial da iteração quando:

   * O projeto não tem uma [!UICONTROL Data de Início Planejada] definida.
   * A [!UICONTROL Data de Início Planejada] do projeto é *antes* ou *em* da data de início da iteração.

* A tarefa usa a [!UICONTROL Data de Início Planejada] do projeto quando:

   * A [!UICONTROL Data de Início Planejada] do projeto é *após* a data de início da iteração.

### [!UICONTROL Data de Término Planejada] da tarefa

* A tarefa usa a Data final da iteração quando:

   * O projeto não tem uma [!UICONTROL Data de conclusão planejada] definida.
   * A [!UICONTROL Data de Início Planejada] do projeto é *antes ou na* a Data de Início da iteração ou a [!UICONTROL Data de Conclusão Planejada] do projeto é *antes ou na* a Data de Término da iteração.

* A tarefa usa a [!UICONTROL Data de Término Planejada] do projeto quando:

   * A [!UICONTROL Data de Início Planejada] do projeto é *após* a Data de Início da iteração e a [!UICONTROL Data de Conclusão Planejada] do projeto é *após* a Data de Término da iteração.

Você pode configurar equipes Scrum individuais para usar as datas do projeto por padrão, em vez das datas de iteração. Para obter informações, consulte a seção [Configurar como as datas são aplicadas ao adicionar itens de trabalho a uma iteração](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) no artigo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Adicionar uma história a uma iteração existente

É possível adicionar qualquer tarefa ou problema a qualquer iteração se você tiver acesso de Gerenciamento ao projeto. Lembre-se do seguinte ao mover uma tarefa ou problema para uma iteração:

* Se você adicionar várias equipes, a tarefa ou problema poderá ser exibido somente na iteração de uma equipe. Esta é a iteração que você escolhe na etapa 3 abaixo.
* Se a tarefa ou problema for atribuído a uma equipe Agile e movido para a iteração de outra equipe, a atribuição da equipe não será alterada.
* Se a tarefa ou problema não for atribuído a uma equipe, a tarefa ou problema será atribuído à equipe que possui a iteração.
* Não é possível adicionar tarefas pai à iteração. Se você adicionar qualquer tarefa filho, a tarefa pai aparecerá no quadro Scrum como uma raia.

>[!IMPORTANT]
>
>Depois que a tarefa é movida para a iteração, não é possível atualizar o [!UICONTROL Tipo de Duração] ou a [!UICONTROL Restrição de Tarefa]. [!UICONTROL Tipo de Duração] está definido como [!UICONTROL Simples] e [!UICONTROL Restrição de Tarefa] está definido como [!UICONTROL Datas Fixas] para manter a linha do tempo da tarefa consistente com a linha do tempo da iteração.

1. Abra a tarefa ou problema que deseja adicionar a uma iteração.
Ou
Vá para o projeto, relatório ou painel que contém a tarefa ou problema que deseja adicionar a uma iteração. Em seguida, selecione uma ou mais tarefas ou problemas.

1. Clique no ícone **[!UICONTROL Mais]** ![Mais](assets/more-icon.png) > **[!UICONTROL Adicionar à Iteração]**.
Não é possível atribuir tarefas ou problemas atribuídos a equipes não ágeis.

1. Na caixa **[!UICONTROL Adicionar a]**, comece digitando o nome da iteração e selecione-o quando ele aparecer na lista.

   >[!NOTE]
   >
   >Você pode mover uma história de uma iteração existente para uma nova iteração.

1. Clique em **[!UICONTROL Adicionar]**.
