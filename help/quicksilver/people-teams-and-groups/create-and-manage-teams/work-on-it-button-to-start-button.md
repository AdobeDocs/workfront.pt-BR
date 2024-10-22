---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Substitua o botão Trabalhar na tarefa por um botão Iniciar
description: A configuração padrão do Adobe Workfront inclui um botão Trabalhar na tarefa para tarefas e problemas que é exibido para itens aos quais você foi atribuído.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Substitua o botão [!UICONTROL Trabalhar nisto] por um botão [!UICONTROL Iniciar]

A configuração padrão de [!DNL Adobe Workfront] inclui um botão [!UICONTROL Trabalhar nisto] para tarefas e problemas que é exibido para itens aos quais você foi atribuído. Ao clicar em [!UICONTROL Trabalhar Nele] nos itens atribuídos a você, você sinaliza a outros usuários que recebeu o trabalho e reconhece que irá trabalhar nele. No entanto, o botão [!DNL Work On It] não atualiza o status da tarefa ou problema para indicar que o trabalho foi realmente iniciado.

Você pode substituir o botão [!DNL Work On It] por um botão [!UICONTROL Iniciar] para a equipe à qual pertence. Nesse caso, você clica no botão [!UICONTROL Iniciar] em vez de [!UICONTROL Trabalhar nisto], que atualiza automaticamente o status e a [!UICONTROL Data do Início Efetivo] do item de trabalho, sinalizando que você começou a trabalhar. Para obter informações sobre a configuração da equipe que pode afetar suas alterações no botão [!UICONTROL Trabalhar nisto], consulte a seção [Configurar o botão [!UICONTROL Iniciar]](#configure-the-uicontrol-start-button) neste artigo.

>[!IMPORTANT]
>
>Clicar no botão [!UICONTROL Iniciar] altera o status do item e a [!UICONTROL Data de Início Efetivo]. Se outra pessoa tiver começado a trabalhar em uma tarefa ou problema (que alterou o status para [!UICONTROL Em andamento] e preencheu a [!UICONTROL Data de Início Efetiva]), o botão do item será exibido como [!UICONTROL Trabalhar Nele] mesmo quando a equipe à qual você pertence tiver substituído o botão por um botão [!UICONTROL Iniciar].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar o botão [!UICONTROL Iniciar]

Se você tiver uma licença do [!UICONTROL Plano], poderá configurar o botão [!UICONTROL Iniciar] para uma equipe na janela de equipe [!UICONTROL Editar]. Veja a seguir como o botão funciona depois que ele é ativado para um grupo:

* **A equipe está atribuída a um item de trabalho**: se uma equipe estiver atribuída ao item de trabalho, os membros dessa equipe verão o botão [!UICONTROL Iniciar] e os status configurados para essa equipe.
* **O usuário pertence a uma Equipe Doméstica**: se nenhuma equipe estiver atribuída ao item de trabalho, mas o usuário estiver atribuído a uma Equipe Doméstica em seu perfil, o usuário verá o botão [!UICONTROL Iniciar] e os status configurados para essa equipe. Este é o cenário que recomendamos se você deseja que os usuários usem o botão [!UICONTROL Iniciar] com frequência.
* **O usuário está atribuído a um item de trabalho**: se não houver nenhuma equipe atribuída ao item de trabalho e nenhuma Equipe interna atribuída ao usuário, mas o usuário estiver atribuído ao item de trabalho, o usuário verá o botão [!UICONTROL Iniciar] e os status combinados configurados para todas as equipes às quais estão atribuídos.
* **O usuário não está atribuído a nenhuma equipe:** Se não houver nenhuma equipe atribuída ao item de trabalho e nenhuma equipe atribuída ao usuário, incluindo a Equipe Inicial, e o item estiver atribuído ao usuário, o usuário parecerá o botão [!UICONTROL Trabalhar Nele].

>[!NOTE]
>
>Este recurso não está disponível atualmente no
>
>* O aplicativo móvel [!DNL Workfront]
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] notificações por email
>

Para configurar o botão Iniciar:

{{step1-to-team}}

1. No menu suspenso **[!UICONTROL Equipes]**, selecione uma equipe.\
   ou\
   Clique em **[!UICONTROL Criar nova equipe]**.

1. Clique no ícone **[!UICONTROL Mais]** ![](assets/more-icon.png) e em **[!UICONTROL Editar]**.

1. Localize a seção do botão **[!UICONTROL Trabalhar nisto]** próxima à parte inferior da página [!UICONTROL Editar Equipes].
1. Marque a caixa de seleção **[!UICONTROL Alterar o botão Trabalhar na tarefa para um botão Iniciar para atualizar automaticamente o status de um item]**.
1. Selecione um ou mais status para cada tipo de item de trabalho. Se você selecionar mais de um status, um menu suspenso será exibido quando você clicar em [!UICONTROL Iniciar], onde você poderá escolher o status desejado.
1. Clique em **[!UICONTROL Salvar alterações]**. Os usuários agora veem o botão [!UICONTROL Iniciar Tarefa] ou [!UICONTROL Iniciar Problema] em vez do botão [!UICONTROL Trabalhar nisto] quando recebem um item de trabalho.

   >[!NOTE]
   >
   >Recomendamos configurar a equipe como a Equipe inicial do usuário para que o botão Iniciar apareça em todos os itens de trabalho atribuídos. Consulte [Associar usuários a uma Equipe Doméstica](#associate-users-with-a-home-team) abaixo.

## Associar usuários a uma Equipe interna

Para associar usuários a uma Equipe da Página Inicial:

{{step-1-to-users}}

1. Selecione o(s) usuário(s) que deseja associar a uma Equipe interna.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Na seção **[!UICONTROL Organização]**, selecione o campo **[!UICONTROL Equipe interna]**. Comece digitando o nome da equipe cujas configurações você deseja associar aos usuários. Clique no nome da equipe ao ser exibido na lista.

1. Clique em **[!UICONTROL Salvar alterações]**.\
   Os usuários selecionados agora estão associados a uma Equipe interna.

   Todas as configurações do grupo, incluindo os status associados ao botão [!UICONTROL Concluído], agora estão visíveis para esses usuários.

