---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurar o Botão Concluído para Tarefas
description: O botão Concluído pode definir automaticamente o status de uma tarefa ou ocorrência. Por padrão, o Adobe Workfront marca uma tarefa como Concluída quando um destinatário clica em Concluído em seu item de trabalho.
author: Courtney
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 6%

---

# Configurar o botão [!UICONTROL Concluído] para tarefas

O botão [!UICONTROL Concluído] pode definir automaticamente o status de uma tarefa ou problema. Por padrão, o [!UICONTROL Adobe Workfront] marca uma tarefa como [!UICONTROL Concluída] quando um destinatário clica em Marcar como concluído em seu item de trabalho.

>[!NOTE]
>
>O botão Concluído é exibido como Marcar como concluído em todas as áreas do Workfront.

## Visão geral

Os usuários com determinadas permissões podem configurar o botão [!UICONTROL Concluído] para associá-lo a determinados status no sistema. Há duas maneiras diferentes de o botão [!UICONTROL Concluído] funcionar para tarefas no [!UICONTROL Workfront]:

* Se o usuário tiver uma Equipe Inicial atribuída, um administrador do [!DNL Workfront] ou um usuário com uma licença do [!UICONTROL Plano] poderá configurar o botão [!UICONTROL Concluído] para refletir determinados status para os membros da equipe. Consulte [Configurar o botão [!UICONTROL Concluído] para uma equipe](#configure-the-uicontrol-done-button-for-a-team) neste artigo.
* Se o usuário não tiver uma [!UICONTROL Equipe Inicial], mas tiver [!UICONTROL Outras Equipes] em seu perfil, o Workfront procurará a configuração do botão [!UICONTROL Concluído] em qualquer uma das equipes associadas ao usuário. A seleção é aleatória e o status associado a qualquer uma das equipes é usado para a tarefa.
* Se o usuário não tiver uma Equipe Inicial atribuída, o botão [!UICONTROL Concluído] das tarefas estará vinculado a um status concluído. Não há opções de configuração disponíveis neste cenário. O botão [!UICONTROL Concluído] automaticamente usa este status como padrão.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Pacote do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Padrão</p>
   <p>Plano</p></td>
  </tr>  
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar o botão [!UICONTROL Concluído] para uma equipe

Você pode alterar o status aplicado ao item de trabalho com o botão [!UICONTROL Concluído]. Você também pode definir vários status e permitir que o usuário escolha qual status é apropriado.

{{step1-to-team}}

1. Clique no ícone **[!UICONTROL Alternar equipe]** e, em seguida, selecione uma nova equipe no menu suspenso ou pesquise uma equipe na barra de pesquisa.
1. Clique no menu **[!UICONTROL Mais]** e clique em **[!UICONTROL Editar]**.
1. Localize a seção **[!UICONTROL Botão Concluído]** na parte inferior da página **[!UICONTROL Configurações de Equipe]**.

1. Selecione um status ou mais de um status para cada tipo de item de trabalho.

   >[!NOTE]
   >
   >Considere o seguinte ao selecionar status para tarefas ou ocorrências:
   >
   >* Quando você seleciona um status para cada tipo de item de trabalho, o status da tarefa ou da ocorrência é definido para esse status quando um usuário clica em [!UICONTROL Concluído] no item. Se você definir vários status para cada tipo de item de trabalho, um menu suspenso será adicionado ao botão [!UICONTROL Concluído] e o usuário deverá escolher um status para alterar o status do item de trabalho.
   >* Você pode associar apenas status de sistema ao botão [!UICONTROL Concluído]. Não é possível associar status específicos de Grupo a status de item de trabalho.
   >* Quando um usuário atribuído ao item coloca o item no status associado ao botão [!UICONTROL Concluído], o item é exibido como [!UICONTROL Concluído] para esse usuário, independentemente do status selecionado ser [!UICONTROL Concluído] ou [!UICONTROL Fechado] ou um status de trabalho.
   >   
   >   
   >  Por exemplo, associar o botão [!UICONTROL Concluído] a [!UICONTROL Em andamento] faz com que o item de trabalho seja exibido como [!UICONTROL Concluído] para o usuário que altera o status de [!UICONTROL Novo] para [!UICONTROL Em andamento].
   >   
   >* Os tipos de problema são personalizáveis e podem ter nomes diferentes dos listados abaixo em seu ambiente.\
   >  Veja a seguir as tarefas e os tipos de ocorrência padrão:
   >     
   >   * [!UICONTROL Tarefas]
   >   * [!UICONTROL Problema]
   >   * [!UICONTROL Solicitar]
   >   * [!UICONTROL Pedido de alteração]
   >   * [!UICONTROL Relatório de erro]

   Se a tarefa ou ocorrência for atribuída a vários usuários, você verá a opção “[!UICONTROL Concluído com minha parte]” no menu suspenso, além dos vários status escolhidos para sua equipe.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Associar usuários a uma equipe da página inicial

Para que as alterações na funcionalidade do botão [!UICONTROL Concluído] fiquem visíveis para os usuários, você pode tornar a equipe cujas configurações alterou a Equipe Inicial dos usuários.

Para associar usuários a uma equipe da página inicial:

1. Clique no ícone **[!UICONTROL do]** Menu Principal![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront].

1. Clique em **[!UICONTROL Usuários]** e, em seguida, selecione o(s) usuário(s) que deseja associar a uma Equipe Inicial.
1. Clique no menu **[!UICONTROL Mais]** e clique em **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Na seção **[!UICONTROL Organização]**, selecione o campo **[!UICONTROL Equipe Inicial]**. Comece a digitar o nome da equipe cujas configurações você deseja associar aos usuários. Clique no nome da equipe quando ela aparecer na lista.

1. Clique em **[!UICONTROL Salvar alterações]**.\
   Os usuários selecionados agora estão associados a uma Equipe Inicial.
Todas as configurações da equipe, incluindo os status associados ao botão [!UICONTROL Concluído], agora estão visíveis para esses usuários.
