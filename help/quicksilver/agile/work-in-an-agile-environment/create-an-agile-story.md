---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Crie uma história ágil
description: Você pode criar uma história Ágil com uma iteração de várias maneiras. Depois de criar uma matéria Ágil, é possível adicionar subtarefas à matéria.
author: Courtney
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 8%

---

# Crie um story ágil

Você pode criar uma história Ágil com uma iteração de várias maneiras. Depois de criar uma matéria Ágil, é possível adicionar subtarefas à matéria.

Quando você adiciona uma matéria ou subtarefa em uma iteração, o Tipo de Duração é definido como [!UICONTROL Simples] e a Restrição de Tarefa é definida como Datas Fixas, com as datas bloqueadas dentro da iteração. Não é possível modificar o Tipo de Duração ou a Restrição de Tarefa em uma iteração. Além disso, a duração da tarefa deve ser maior que 0 minutos.

Para obter informações sobre como gerenciar a história depois que ela é adicionada à iteração, consulte [Iterações](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

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
   <td> <p>Padrão</p> 
   <p>Trabalho ou maior</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Gerenciar o acesso ao projeto no qual a história está </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um story ágil em uma iteração

1. Vá para a iteração Ágil, onde deseja criar a matéria:

   {{step1-to-team}}

   1. (Opcional) Clique no ícone **[!UICONTROL Alternar equipe]** ![Ícone Alternar equipe](assets/switch-team-icon.png) e, em seguida, selecione uma nova equipe Scrum no menu suspenso ou pesquise uma equipe na barra de pesquisa.

   1. No painel esquerdo, selecione **[!UICONTROL Iterações]** para escolher uma iteração específica ou selecione **[!UICONTROL Iteração Atual]**.
   1. Clique no nome da iteração específica em que deseja criar uma matéria.

   ![Adicionar nova história à iteração](assets/iteration-stories-list.png)

1. Clique em **[!UICONTROL Nova História].**
1. Especifique as seguintes informações:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>Digite um nome para a matéria.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Digite uma descrição para a matéria.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>Selecione essa opção se a matéria estiver pronta para ser adicionada a uma iteração. Quando essa opção é selecionada, ela indica aos usuários quais matérias na lista de pendências estão prontas para serem adicionadas a uma iteração.<br>Uma história pode ser adicionada a uma iteração, estando ou não marcada como <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate] (pontos)</strong></td>
      <td>Especifique a estimativa da matéria. Se a sua equipe Ágil está configurada para estimar histórias em pontos, então por padrão 1 ponto é igual a 8 horas. As estimativas são adicionadas como [!UICONTROL Planned Hours] na matéria.<br>Por exemplo, se você estimar uma matéria como 3 pontos, o comportamento padrão é adicionar 24 [!UICONTROL Planned Hours] à matéria.<br>Se uma matéria contiver subtarefas, lembre-se de que as estimativas combinadas de todas as subtarefas determinam a estimativa da matéria pai. Para obter mais informações, consulte <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Adicionar matérias a uma iteração existente</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Projeto Pai]</strong></td>
      <td>Comece a digitar o nome do projeto ao qual esta matéria será associada.<br>Por padrão, a cor da matéria é exibida com a mesma cor das outras matérias deste projeto.<br>O status do projeto deve ser definido como [!UICONTROL Atual]. Se o status do projeto for algo além de [!UICONTROL Current], ele não será exibido no menu suspenso.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>Depois de escolher um projeto pai, você tem a opção de escolher uma tarefa pai. Quando você seleciona uma tarefa-pai, a matéria é criada como uma subtarefa da tarefa-pai no projeto selecionado.<br>Comece a digitar o nome da tarefa pai da matéria e clique nela quando ela aparecer na lista suspensa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Selecione qualquer formulário personalizado para adicionar à matéria.</td>
     </tr>
    </tbody>
   </table>

1. Clique em **[!UICONTROL Salvar matéria]**.

## Crie uma história ágil no acúmulo

Você pode criar uma história Ágil na lista de pendências Ágil, conforme descrito na seção [Criar novas histórias na lista de pendências](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) do artigo [[!UICONTROL Gerenciar] a lista de pendências Ágil](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Adicione uma tarefa ou ocorrência como uma história Ágil

É possível adicionar uma tarefa ou ocorrência existente como uma matéria a uma iteração. Para obter mais informações, consulte [Adicionar histórias a uma iteração existente](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) ou [Adicionar histórias e problemas do quadro [!UICONTROL Scrum]](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Criar subtarefas para uma matéria Ágil

Você pode criar uma subtarefa para uma matéria Ágil usando um dos seguintes métodos:

* Usando a guia **[!UICONTROL Subtarefas]**, conforme descrito em [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) em [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Diretamente do quadro de matérias, conforme descrito em [Criar uma iteração](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
