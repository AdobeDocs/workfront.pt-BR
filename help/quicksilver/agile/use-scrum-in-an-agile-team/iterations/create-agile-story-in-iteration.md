---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Criar uma história ágil em uma iteração
description: Este artigo descreve como criar uma nova história ágil quando você já estiver na iteração.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Criar uma história ágil em uma iteração

Este artigo descreve como criar uma nova história ágil quando você já estiver na iteração. Para obter informações sobre como criar uma história ágil a partir de uma tarefa, edição ou outra área de [!DNL Adobe Workfront], consulte [Adicionar histórias a uma iteração existente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

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
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Acesso do [!UICONTROL Gerenciar] ao projeto no qual a história está</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Criar uma história ágil em uma iteração

1. Vá para a iteração ágil onde deseja criar a história:

   1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront, em seguida, clique em **[!UICONTROL Equipes]**.

   1. (Opcional) Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png)e, em seguida, selecione uma nova equipe de Soma no menu suspenso ou procure por uma equipe na barra de pesquisa.

   1. No painel esquerdo, selecione **[!UICONTROL Iterações]**.
   1. Clique no nome da iteração específica onde deseja criar uma história.
   1. No painel esquerdo, selecione **[!UICONTROL Histórias]**.

1.  Clique em **[!UICONTROL Nova história].**
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
      <td>Especifique a estimativa para a história. Se sua equipe ágil estiver configurada para estimar histórias em pontos, então por padrão 1 ponto é igual a 8 horas. As estimativas são adicionadas como [!UICONTROL Horas planejadas] na história.<br>Por exemplo, se você estimar uma história como 3 pontos, o comportamento padrão é adicionar 24 Horas Planejadas à história.<br>Se uma história contiver subtarefas, lembre-se de que as estimativas combinadas para todas as subtarefas determinam a estimativa da história pai. Para obter mais informações, consulte <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Adicionar uma subtarefa a uma história existente no quadro [!UICONTROL Scrum]</a>.</td>
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
