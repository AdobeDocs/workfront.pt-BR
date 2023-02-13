---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Substitua o botão Trabalho nele por um botão Iniciar
description: A configuração padrão do Adobe Workfront inclui um botão Trabalhar nele para tarefas e problemas que são exibidos para itens aos quais você foi atribuído.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Substitua o [!UICONTROL Trabalhe Com Ele] com um botão [!UICONTROL Iniciar] botão

[!DNL Adobe Workfront]A configuração padrão do inclui um [!UICONTROL Trabalhe Com Ele] botão para tarefas e problemas que são exibidos para itens aos quais você foi atribuído. Ao clicar em [!UICONTROL Trabalhe Com Ele] em itens atribuídos a você, você sinaliza para outros usuários que recebeu o trabalho e reconhece que trabalhará nele. No entanto, a variável [!DNL Work On It] O botão não atualiza a tarefa ou emite o status para sinalizar que o trabalho foi realmente iniciado.

Você pode substituir a variável [!DNL Work On It] com um botão [!UICONTROL Iniciar] para um grupo ao qual você pertence. Nesse caso, clique no botão [!UICONTROL Iniciar] botão em vez de [!UICONTROL Trabalhe Com Ele], que atualiza automaticamente o status e a variável [!UICONTROL Data de início real] do item de trabalho, sinalizando que você começou a trabalhar. Para obter informações sobre a configuração de qual equipe pode afetar suas alterações no [!UICONTROL Trabalhe Com Ele] , consulte a seção [Configure o [!UICONTROL Iniciar] botão](#configure-the-uicontrol-start-button) neste artigo.

>[!IMPORTANT]
>
>Clicar no [!UICONTROL Iniciar] altera o status do item e [!UICONTROL Data de início real]. Se outra pessoa tiver começado a trabalhar em uma tarefa ou problema (que alterou o status para [!UICONTROL Em Andamento] e preencheu os [!UICONTROL Data de início real]), o botão do item é exibido como [!UICONTROL Trabalhe Com Ele] mesmo quando um grupo ao qual você pertence teve o botão substituído por um [!UICONTROL Iniciar] botão.

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
   <td> <p>Plano</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano ou tipo de licença você possui, entre em contato com seu [!DNL Workfront] administrador.

## Configure o [!UICONTROL Iniciar] botão

Se você tiver uma [!UICONTROL Plano] você pode configurar a [!UICONTROL Iniciar] para uma equipe no [!UICONTROL Editar] janela da equipe. Veja como o botão funciona após ser ativado para um grupo:

* **A equipe é atribuída a um item de trabalho**: Se uma equipe for atribuída ao item de trabalho, os membros dessa equipe visualizarão a variável [!UICONTROL Iniciar] e os status configurados para essa equipe.
* **O usuário pertence a uma Home Team**: Se nenhuma equipe for atribuída ao item de trabalho, mas o usuário for atribuído a uma Equipe Inicial em seu perfil, o usuário visualizará a variável [!UICONTROL Iniciar] e os status configurados para essa equipe. Este é o cenário que recomendamos se você deseja que os usuários usem a variável [!UICONTROL Iniciar] frequentemente.
* **O usuário é atribuído a um item de trabalho**: Se não houver equipe atribuída ao item de trabalho e nenhuma Equipe Inicial atribuída ao usuário, mas o usuário for atribuído ao item de trabalho, o usuário visualizará a [!UICONTROL Iniciar] e os status combinados configurados para que todas as equipes sejam atribuídas.
* **O usuário não está atribuído a nenhuma equipe:** Se não houver uma equipe atribuída ao item de trabalho e nenhuma equipe para o usuário, incluindo a Equipe Inicial, e o item for atribuído ao usuário, o usuário parece que [!UICONTROL Trabalhe Com Ele] botão.

>[!NOTE]
>
>Este recurso não está disponível no momento em
>
>* O [!DNL Workfront] aplicativo móvel
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] notificações por email
>


Para configurar o botão Start :

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Equipes]**.

1. No **[!UICONTROL Equipes]** selecione um grupo no menu suspenso.\
   ou\
   Clique em **[!UICONTROL Criar equipe]**.

1. Clique no botão **[!UICONTROL Mais]** ícone ![](assets/more-icon.png), depois clique em **[!UICONTROL Editar]**.

1. Encontre a **[!UICONTROL Trabalhe Com Ele]** seção do botão perto da parte inferior do [!UICONTROL Editar equipes] página.
1. Selecione o **[!UICONTROL Altere o botão Trabalhar nele para um botão Iniciar para atualizar automaticamente o status de um item]** caixa de seleção.
1. Selecione um ou mais status para cada tipo de item de trabalho. Se você selecionar mais de um status, um menu suspenso será exibido ao clicar em [!UICONTROL Iniciar] onde você pode escolher o status desejado.
1. Clique em **[!UICONTROL Salvar alterações]**. Os usuários agora veem um [!UICONTROL Iniciar tarefa] ou [!UICONTROL Problema inicial] em vez de [!UICONTROL Trabalhe Com Ele] quando um item de trabalho for atribuído a eles.

   >[!NOTE]
   >
   >Recomendamos configurar a equipe como Equipe inicial de um usuário para que o botão Iniciar apareça em todos os itens de trabalho atribuídos. Consulte [Associar usuários a uma Equipe Inicial](#associate-users-with-a-home-team) abaixo.

## Associar usuários a uma Equipe Inicial

Para associar usuários a uma Equipe inicial:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront].

1. Clique em **[!UICONTROL Usuários]** e, em seguida, selecione o(s) usuário(s) que deseja associar a uma Equipe Inicial.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. No **[!UICONTROL Organização]** selecione a **[!UICONTROL Equipe inicial]** campo. Comece a digitar o nome da equipe cujas configurações você deseja associar com os usuários. Clique no nome da equipe quando visualizá-lo na lista.

1. Clique em **[!UICONTROL Salvar alterações]**.\
   Os usuários selecionados agora estão associados a uma Equipe inicial.

   Todas as configurações do grupo, incluindo os status associados ao grupo [!UICONTROL Concluído] agora estão visíveis para esses usuários.

