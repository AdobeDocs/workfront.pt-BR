---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Criar uma história ágil
description: Você pode criar uma história ágil em uma iteração de várias maneiras. Depois de criar uma matéria ágil, é possível adicionar subtarefas à matéria.
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 0%

---

# Criar uma história ágil

Você pode criar uma história ágil em uma iteração de várias maneiras. Depois de criar uma matéria ágil, é possível adicionar subtarefas à matéria.

Quando você adiciona uma história ou subtarefa em uma iteração, o Tipo de Duração é definido como [!UICONTROL Simples] e a Restrição de Tarefa é definida como Datas Fixas, com as datas bloqueadas dentro da iteração. Não é possível modificar o Tipo de Duração ou a Restrição de Tarefa em uma iteração. Além disso, a duração da tarefa deve ser superior a 0 minutos.

Para obter informações sobre como gerenciar a história depois de adicionada à iteração, consulte [Iterações](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

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
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Work] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Acesso [!UICONTROL Gerenciar] ao projeto em que a história está</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Criar uma história ágil em uma iteração

1. Vá para a iteração ágil na qual deseja criar a história:

   1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Equipes]**.

   1. (Opcional) Clique no ícone **[!UICONTROL Equipe do Switch]** ![Ícone da equipe do Switch](assets/switch-team-icon.png), em seguida, selecione uma nova equipe do Scrum no menu suspenso ou procure uma equipe na barra de pesquisa.

   1. No painel esquerdo, selecione **[!UICONTROL Iterações]** para escolher uma iteração específica, ou selecione **[!UICONTROL Iteração atual]**.
   1. Clique no nome da iteração específica em que deseja criar uma história.

   ![Adicionar nova história à iteração](assets/iteration-add-story.png)

1. Clique em **[!UICONTROL Nova história].**
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
      <td role="rowheader"><strong>[!UICONTROL Descrição]</strong></td>
      <td>Digite uma descrição para a história.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Pronto]</strong></td>
      <td>Selecione essa opção se a matéria estiver pronta para ser adicionada a uma iteração. Quando essa opção é selecionada, ela indica aos usuários quais histórias no backlog estão prontas para serem adicionadas a uma iteração.<br>Uma história pode ser adicionada a uma iteração independentemente de estar ou não marcada como <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimativa] (pontos)</strong></td>
      <td>Especifique a estimativa para a história. Se a sua equipe ágil estiver configurada para estimar histórias em pontos, por padrão, 1 ponto é igual a 8 horas. As estimativas são adicionadas como [!UICONTROL Horas planejadas] na história.<br>Por exemplo, se você estimar uma matéria como 3 pontos, o comportamento padrão é adicionar 24 [!UICONTROL Horas Planejadas] à matéria.<br>Se uma história contiver subtarefas, lembre-se de que as estimativas combinadas para todas as subtarefas determinam a estimativa da história pai. Para obter mais informações, consulte <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Adicionar histórias a uma iteração existente</a>.</td>
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

## Criar uma história ágil no backlog

Você pode criar uma história ágil a partir da lista de pendências ágil, conforme descrito na seção [Criar novas histórias na lista de pendências](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) do artigo [[!UICONTROL Gerenciar] a lista de pendências ágil](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Adicionar uma tarefa ou problema como uma história ágil

Você pode adicionar uma tarefa ou problema existente como uma história a uma iteração. Para obter mais informações, consulte [Adicionar histórias a uma iteração existente](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) ou [Adicionar histórias e problemas do quadro [!UICONTROL Scrum]](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Criar subtarefas para uma história ágil

É possível criar uma subtarefa para uma matéria ágil usando um dos seguintes métodos:

* Usando a guia **[!UICONTROL Subtarefas]**, conforme descrito em [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) em [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Diretamente do storyboard, conforme descrito em [Criar uma iteração](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
