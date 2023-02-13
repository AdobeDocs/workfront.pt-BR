---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Criar uma história ágil
description: Você pode criar uma história ágil em uma iteração de várias maneiras. Depois de criar uma história ágil, você pode adicionar subtarefas à história.
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Criar uma história ágil

Você pode criar uma história ágil em uma iteração de várias maneiras. Depois de criar uma história ágil, você pode adicionar subtarefas à história.

Quando você adiciona uma história ou subtarefa em uma iteração, o Tipo de duração é definido como [!UICONTROL Simples] e a Restrição de tarefa é definida como Datas fixas, com as datas bloqueadas dentro da iteração. Não é possível modificar o Tipo de duração ou a Restrição de tarefa em uma iteração. Além disso, a duração da tarefa deve ser superior a 0 minutos.

Para obter informações sobre como gerenciar a história depois que ela for adicionada à iteração, consulte [Iterações](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

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
   <td> <p>[!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Acesso do [!UICONTROL Gerenciar] ao projeto no qual a história está</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Criar uma história ágil em uma iteração

1. Vá para a iteração ágil onde deseja criar a história:

   1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Equipes]**.

   1. (Opcional) Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png)e, em seguida, selecione uma nova equipe de Soma no menu suspenso ou procure por uma equipe na barra de pesquisa.

   1. No painel esquerdo, selecione **[!UICONTROL Iterações]** para escolher uma iteração específica, ou selecione **[!UICONTROL Iteração atual]**.
   1. Clique no nome da iteração específica onde deseja criar uma história.

   ![Adicionar nova história à iteração](assets/iteration-add-story.png)

1. Clique em **[!UICONTROL Nova história].**
1. Especifique as seguintes informações:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nome da história]</strong></td>
      <td>Digite um nome para a história.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Descrição]</strong></td>
      <td>Digite uma descrição para a história.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Pronto]</strong></td>
      <td>Selecione essa opção se a história estiver pronta para ser adicionada a uma iteração. Quando essa opção é selecionada, ela indica aos usuários quais histórias no backlog estão prontas para serem adicionadas a uma iteração.<br>Uma história pode ser adicionada a uma iteração, seja marcada ou não <strong>[!UICONTROL Pronto].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimativa] (pontos)</strong></td>
      <td>Especifique a estimativa para a história. Se sua equipe ágil estiver configurada para estimar histórias em pontos, então por padrão 1 ponto é igual a 8 horas. As estimativas são adicionadas como [!UICONTROL Horas planejadas] na história.<br>Por exemplo, se você estimar uma história como 3 pontos, o comportamento padrão é adicionar 24 [!UICONTROL Horas planejadas] à história.<br>Se uma história contiver subtarefas, lembre-se de que as estimativas combinadas para todas as subtarefas determinam a estimativa da história pai. Para obter mais informações, consulte <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Adicionar histórias a uma iteração existente</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Projeto pai]</strong></td>
      <td>Comece digitando o nome do projeto ao qual essa história será associada.<br>Por padrão, a cor da história é exibida com a mesma cor de outras histórias desse projeto.<br>O status do projeto deve ser definido como [!UICONTROL Atual]. Se o status do projeto for qualquer coisa menos [!UICONTROL Atual], ele não será exibido no menu suspenso.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tarefa pai]</strong></td>
      <td>Depois de escolher um projeto pai, você tem a opção de escolher uma tarefa pai. Ao selecionar uma tarefa pai, a história é criada como uma subtarefa da tarefa pai no projeto selecionado.<br>Comece digitando o nome da tarefa pai da história e clique nele quando ela for exibida na lista suspensa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Forms personalizado]</strong></td>
      <td>Selecione quaisquer formulários personalizados para adicionar à história.</td>
     </tr>
    </tbody>
   </table>

1. Clique em **[!UICONTROL Salvar história]**.

## Criar uma história ágil no backlog

Você pode criar uma história ágil no backlog ágil, conforme descrito na seção [Criar novas histórias no backlog](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) no artigo [[!UICONTROL Gerenciar] o backlog ágil](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Adicionar uma tarefa ou um problema como uma história ágil

Você pode adicionar uma tarefa ou edição existente como uma história a uma iteração. Para obter mais informações, consulte [Adicionar histórias a uma iteração existente](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) ou [Adicionar histórias e problemas do [!UICONTROL Scrum] quadro](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Criar subtarefas em uma história ágil

Você pode criar uma subtarefa para uma história ágil usando um dos seguintes métodos:

* Ao usar a variável **[!UICONTROL Subtarefas]** conforme descrito em [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) em [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Diretamente do quadro de história, conforme descrito em [Criar uma iteração](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
