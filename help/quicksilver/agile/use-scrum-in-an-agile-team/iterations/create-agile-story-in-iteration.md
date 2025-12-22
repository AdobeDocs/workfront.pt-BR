---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Criar uma história Agile em uma iteração
description: Este artigo descreve como criar uma nova história do Agile quando você já está na iteração.
author: Jenny
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 4%

---

# Criar uma história do Agile em uma iteração

Este artigo descreve como criar uma nova história do Agile quando você já está na iteração. Para obter informações sobre como criar uma história Agile a partir de uma tarefa, problema ou outra área de [!DNL Adobe Workfront], consulte [Adicionar histórias a uma iteração existente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

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

## Criar uma história do Agile em uma iteração

1. Vá para a iteração Agile onde deseja criar a história:

   {{step1-to-team}}

   1. (Opcional) Clique no ícone **[!UICONTROL Equipe do Switch]** ![Ícone da equipe do Switch](assets/switch-team-icon.png), em seguida, selecione uma nova equipe do Scrum no menu suspenso ou procure uma equipe na barra de pesquisa.

   1. No painel esquerdo, selecione **[!UICONTROL Iterações]**.
   1. Clique no nome da iteração específica em que deseja criar uma história.
   1. No painel esquerdo, selecione **[!UICONTROL Histórias]**.

1.  Clique em **[!UICONTROL Nova história]**.
1. Especifique as seguintes informações:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nome da História]</strong></td>
      <td>Digite um nome para a história.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Digite uma descrição para a história.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Pronto]</strong></td>
      <td>Selecione essa opção se a matéria estiver pronta para ser adicionada a uma iteração. Quando essa opção é selecionada, ela indica aos usuários quais histórias no backlog estão prontas para serem adicionadas a uma iteração.<br>Uma história pode ser adicionada a uma iteração independentemente de estar ou não marcada como <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimativa] (pontos)</strong></td>
      <td>Especifique a estimativa para a história. Se a sua equipe ágil estiver configurada para estimar histórias em pontos, por padrão, 1 ponto é igual a 8 horas. As estimativas são adicionadas como [!UICONTROL Horas planejadas] na história.<br>Por exemplo, se você estimar uma história como 3 pontos, o comportamento padrão é adicionar 24 horas planejadas à história.<br>Se uma história contiver subtarefas, lembre-se de que as estimativas combinadas para todas as subtarefas determinam a estimativa da história pai. Para obter mais informações, consulte <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Adicionar uma subtarefa a um texto existente no quadro [!UICONTROL Scrum]</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Projeto Pai]</strong></td>
      <td>Comece digitando o nome do projeto ao qual esta história será associada.<br>Por padrão, a cor da matéria é exibida como a mesma cor de outras matérias deste projeto.<br>O status do projeto deve ser definido como [!UICONTROL Atual]. Se o status do projeto for algo diferente de [!UICONTROL Atual], ele não será exibido no menu suspenso.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tarefa Pai]</strong></td>
      <td>Depois de escolher um projeto principal, você tem a opção de escolher uma tarefa principal. Quando você seleciona uma tarefa pai, a história é criada como uma subtarefa da tarefa pai no projeto selecionado.<br>Comece a digitar o nome da tarefa pai da matéria e clique nela quando ela aparecer na lista suspensa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Forms Personalizado]</strong></td>
      <td>Selecione qualquer formulário personalizado para adicionar à história.</td>
     </tr>
    </tbody>
   </table>

1. Clique em **[!UICONTROL Salvar história]**.
