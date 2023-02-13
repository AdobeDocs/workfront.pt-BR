---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurar o botão Concluído para tarefas
description: O botão Concluído pode definir automaticamente o status de uma tarefa ou problema. Por padrão, o Adobe Workfront marca uma tarefa como Concluída quando um destinatário clica em Concluído em seu item de trabalho.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 1%

---

# Configure o [!UICONTROL Concluído] botão para tarefas

O [!UICONTROL Concluído] pode definir automaticamente o status de uma tarefa ou de um problema. Por padrão, [!UICONTROL Adobe Workfront] marca uma tarefa como [!UICONTROL Concluído] quando um destinatário clicar em Concluído em seu item de trabalho.

## Visão geral

Os usuários com certas permissões podem configurar o [!UICONTROL Concluído] para refletir determinados status no sistema. Há duas maneiras diferentes de [!UICONTROL Concluído] funciona para tarefas em [!UICONTROL Workfront]:

* Se o usuário tiver uma Equipe Inicial atribuída, um [!DNL Workfront] administrador ou um usuário com uma [!UICONTROL Plano] licença pode configurar o [!UICONTROL Concluído] para refletir determinados status para os membros da equipe. Consulte [Configure o [!UICONTROL Concluído] botão para uma equipe](#configure-the-uicontrol-done-button-for-a-team) neste artigo.
* Se o usuário não tiver uma Equipe Inicial atribuída, a variável [!UICONTROL Concluído] botão para tarefas está vinculado a um status completo. Não há opções de configuração disponíveis neste cenário. O [!UICONTROL Concluído] assume automaticamente esse status como padrão.

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
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano ou tipo de licença você possui, entre em contato com seu [!DNL Workfront] administrador.

## Configure o [!UICONTROL Concluído] botão para uma equipe

Você pode alterar qual status é aplicado ao item de trabalho com a variável [!UICONTROL Concluído] botão. Você também pode definir vários status e permitir que o usuário escolha qual status é apropriado.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Equipes]**.

1. Clique no botão **[!UICONTROL Alterar equipe]** em seguida, selecione uma nova equipe no menu suspenso ou pesquise por uma equipe na barra de pesquisa.
1. Clique no botão **[!UICONTROL Mais]** , em seguida, clique em **[!UICONTROL Editar]**.
1. Encontre a **[!UICONTROL Botão Concluído]** na parte inferior do **[!UICONTROL Configurações do grupo]** página.

1. Selecione um status ou mais de um para cada tipo de item de trabalho.

   >[!NOTE]
   >
   >Considere o seguinte ao selecionar os status para tarefas ou problemas:
   >
   >* Quando você seleciona um status para cada tipo de item de trabalho, o status da tarefa ou da emissão é definido para esse status quando um usuário clica em [!UICONTROL Concluído] no seu item. Se você definir vários status para cada tipo de item de trabalho, um menu suspenso será adicionado à variável [!UICONTROL Concluído] e o usuário deve escolher um status para alterar o status no item de trabalho.
   >* Você pode associar somente status de nível de sistema à variável [!UICONTROL Concluído] botão. Não é possível associar status específicos do grupo a status de item de trabalho.
   >* Quando um usuário atribuído ao item coloca o item no status associado ao [!UICONTROL Concluído] botão, o item é exibido como [!UICONTROL Concluído] para esse usuário, independentemente de o status selecionado ser um [!UICONTROL Concluído] ou [!UICONTROL Fechado] status ou status de trabalho.

   >   
   >   
   >  Por exemplo, associar a variável [!UICONTROL Concluído] botão com [!UICONTROL Em Andamento] faz com que o item de trabalho seja exibido como [!UICONTROL Concluído] para o usuário que altera o status de [!UICONTROL Novo] para [!UICONTROL Em andamento].
   >   
   >* Os tipos de problemas são personalizáveis e podem ter nomes diferentes dos listados abaixo no seu ambiente.\
      >  A seguir estão as tarefas padrão e os tipos de problema:
      >     
      >   * [!UICONTROL Tarefas]
      >   * [!UICONTROL Problema]
      >   * [!UICONTROL Solicitar]
      >   * [!UICONTROL Pedido de alteração]
      >   * [!UICONTROL Registro de Defeito]


   Se a tarefa ou o problema for atribuído a vários usuários, você verá um &quot;[!UICONTROL Feito com a minha parte]&quot; no menu suspenso, além dos vários status escolhidos para sua equipe.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Associar usuários a uma Equipe Inicial

Para fazer as alterações no [!UICONTROL Concluído] Para tornar a funcionalidade do botão visível para os usuários, é possível tornar a equipe cujas configurações você alterou a Home Team dos usuários.

Para associar usuários a uma Equipe inicial:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront].

1. Clique em **[!UICONTROL Usuários]** e, em seguida, selecione o(s) usuário(s) que deseja associar a uma Equipe Inicial.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. No **[!UICONTROL Organização]** selecione a **[!UICONTROL Equipe inicial]** campo. Comece a digitar o nome da equipe cujas configurações você deseja associar com os usuários. Clique no nome da equipe quando visualizá-lo na lista.

1. Clique em **[!UICONTROL Salvar alterações]**.\
   Os usuários selecionados agora estão associados a uma Equipe inicial.
Todas as configurações do grupo, incluindo os status associados ao grupo [!UICONTROL Concluído] agora estão visíveis para esses usuários.
