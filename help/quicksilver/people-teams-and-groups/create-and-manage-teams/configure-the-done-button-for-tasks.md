---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurar o botão Concluído para tarefas
description: O botão Concluído pode definir automaticamente o status de uma tarefa ou problema. Por padrão, o Adobe Workfront marca uma tarefa como Concluída quando um destinatário clica em Concluído em seu item de trabalho.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 62db557f6347004836fac1ea37e55d557dcc6b87
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# Configure o [!UICONTROL Concluído] botão para tarefas

A variável [!UICONTROL Concluído] pode definir automaticamente o status de uma tarefa ou problema. Por padrão, [!UICONTROL Adobe Workfront] marca uma tarefa como [!UICONTROL Concluído] quando um destinatário clica em Concluído em seu item de trabalho.

## Visão geral

Os usuários com determinadas permissões podem configurar o [!UICONTROL Concluído] para refletir determinados status no sistema. Há duas maneiras diferentes de [!UICONTROL Concluído] botão funciona para tarefas em [!UICONTROL Workfront]:

* Se o usuário tiver uma Equipe inicial atribuída, uma equipe [!DNL Workfront] administrador ou um usuário com uma [!UICONTROL Plano] a licença pode configurar o [!UICONTROL Concluído] para refletir determinados status para os membros da equipe. Consulte [Configure o [!UICONTROL Concluído] botão para uma Equipe](#configure-the-uicontrol-done-button-for-a-team) neste artigo.
* Se o usuário não tiver uma [!UICONTROL Equipe interna], mas eles têm [!UICONTROL Outras equipes] em seu perfil, o Workfront procura a configuração da variável [!UICONTROL Concluído] em qualquer equipe associada ao usuário. A seleção é aleatória e o status associado a qualquer uma das equipes é usado para a tarefa.
* Se o usuário não tiver uma Equipe interna atribuída, a variável [!UICONTROL Concluído] para tarefas está vinculado a um status concluído. Não há opções de configuração disponíveis neste cenário. A variável [!UICONTROL Concluído] automaticamente assume esse status como padrão.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] plano*</strong></p></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] licença*</strong></p></td> 
   <td> <p>[!UICONTROL Plano] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber que tipo de plano ou licença você tem, entre em contato com o [!DNL Workfront] administrador.

## Configure o [!UICONTROL Concluído] botão para uma Equipe

Você pode alterar qual status é aplicado ao item de trabalho com o [!UICONTROL Concluído] botão. Você também pode definir vários status e permitir que o usuário escolha qual status é apropriado.

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **[!UICONTROL Equipes]**.

1. Clique em **[!UICONTROL Trocar equipe]** , selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.
1. Clique em **[!UICONTROL Mais]** e clique em **[!UICONTROL Editar]**.
1. Localize o **[!UICONTROL Botão Concluído]** na parte inferior do **[!UICONTROL Configurações da equipe]** página.

1. Selecione um ou mais status para cada tipo de item de trabalho.

   >[!NOTE]
   >
   >Considere o seguinte ao selecionar status para tarefas ou problemas:
   >
   >* Quando você seleciona um status para cada tipo de item de trabalho, o status da tarefa ou do problema é definido para esse status quando um usuário clica em [!UICONTROL Concluído] em seu item. Se você definir vários status para cada tipo de item de trabalho, um menu suspenso será adicionado à [!UICONTROL Concluído] e o usuário deve escolher um status para alterar o status no item de trabalho.
   >* Você pode associar somente os status de nível de sistema com o [!UICONTROL Concluído] botão. Você não pode associar status específicos de Grupo a status de item de trabalho.
   >* Quando um usuário atribuído ao item coloca o item no status associado à [!UICONTROL Concluído] , o item é exibido como [!UICONTROL Concluído] para esse usuário, independentemente de o status selecionado ser um [!UICONTROL Concluído] ou [!UICONTROL Fechado] ou um estado de trabalho.
   >   
   >   
   >  Por exemplo, associar a variável [!UICONTROL Concluído] botão com [!UICONTROL Em andamento] causa a exibição do item de trabalho como [!UICONTROL Concluído] para o usuário que altera o status de [!UICONTROL Novo] para [!UICONTROL Em andamento].
   >   
   >* Os tipos de problemas são personalizáveis e podem ter nomes diferentes dos listados abaixo em seu ambiente.\
   >  A seguir estão as tarefas padrão e os tipos de problemas:
   >     
   >   * [!UICONTROL Tarefas]
   >   * [!UICONTROL Problema]
   >   * [!UICONTROL Solicitar]
   >   * [!UICONTROL Pedido de alteração]
   >   * [!UICONTROL Registro de Defeito]

   Se a tarefa ou o problema for atribuído a vários usuários, você verá um &quot;[!UICONTROL Pronto com minha parte]&quot; no menu suspenso, além dos vários status escolhidos para sua equipe.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Associar usuários a uma Equipe interna

Para fazer as alterações no [!UICONTROL Concluído] funcionalidade de botão visível para os usuários, você pode tornar a equipe cujas configurações você alterou a Equipe inicial dos usuários.

Para associar usuários a uma Equipe da Página Inicial:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront].

1. Clique em **[!UICONTROL Usuários]**, em seguida, selecione o(s) usuário(s) que deseja associar a uma Equipe interna.
1. Clique em **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. No **[!UICONTROL Organização]** , selecione a **[!UICONTROL Equipe interna]** campo. Comece digitando o nome da equipe cujas configurações você deseja associar aos usuários. Clique no nome da equipe ao ser exibido na lista.

1. Clique em **[!UICONTROL Salvar alterações]**.\
   Os usuários selecionados agora estão associados a uma Equipe interna.
Quaisquer configurações do grupo, incluindo os status associados à [!UICONTROL Concluído] agora estão visíveis para esses usuários.
