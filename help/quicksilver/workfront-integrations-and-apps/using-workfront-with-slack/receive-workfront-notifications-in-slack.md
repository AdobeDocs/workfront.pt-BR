---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Receber [!DNL Adobe Workfront] notificações em [!DNL Slack]
description: Receber [!DNL Adobe Workfront] notificações em [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

# Receber [!DNL Adobe Workfront] notificações em [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Após instalar o [!DNL Adobe Workfront for Slack], você poderá receber [!DNL Workfront] notificações em [!DNL Slack].\
Para obter informações sobre como instalar o [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Você pode habilitar um número selecionado de [!UICONTROL notificações] que aparecem na bolha de notificações na interface [!DNL Workfront], para também serem entregues em [!DNL Slack].

As notificações por email funcionam independentemente das notificações da interface [!DNL Workfront]. Você ou o administrador do [!DNL Workfront] pode desabilitar notificações por email, enquanto notificações por interface não podem ser desabilitadas no [!DNL Workfront].\
No entanto, você pode desabilitar [!DNL Workfront] notificações que poderá receber em [!DNL Slack], se quiser se concentrar nessas notificações somente dentro da interface [!DNL Workfront].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Qualquer</p>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de receber [!DNL Workfront] notificações em [!DNL Slack], você deve

* Configurar [!DNL Workfront for Slack]\
   Para obter instruções sobre como configurar o [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configurar notificações de [!DNL Workfront] para [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Condicional) Depois que [!DNL Workfront] for adicionado à sua instância do [!DNL Slack], faça logon no [!DNL Workfront] em [!DNL Slack].\
   Para obter informações sobre como fazer logon no [!DNL Workfront] a partir de [!DNL Slack], consulte [Acesso [!DNL Adobe Workfront] a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Em qualquer canal, comece digitando um dos seguintes comandos no campo de mensagem:

   `/workfront settings`

   Ou

   `/wf settings`

1. Todas as notificações são ativadas, por padrão.\
   Desative qualquer uma das seguintes notificações:

   * [!UICONTROL Estou atribuído a uma nova tarefa ou problema]
   * [!UICONTROL Minha equipe foi atribuída a uma nova tarefa ou problema]
   * [!UICONTROL Recebi uma nova solicitação de aprovação ou acesso]
   * [!UICONTROL Alguém me inclui em uma atualização direcionada]
   * [!UICONTROL Quando alguém comentar em um thread, eu estarei]
   * [!UICONTROL Foi feita uma atualização em uma tarefa, problema ou projeto que eu assino]
   * [!UICONTROL Alguém comentou um dos meus itens de trabalho]
   * [!UICONTROL Alguém comentou minha solicitação de ajuda]

   As alterações feitas nas opções [!UICONTROL notificações] entrarão em vigor imediatamente.\
   As notificações habilitadas são entregues no canal [!DNL Workfront] [!DNL Slack]. Quando você desabilita as notificações aqui, elas são desabilitadas apenas para [!DNL Slack], e não para a interface [!DNL Workfront]. Você continua a recebê-las na bolha de notificações [!DNL Workfront] na parte superior direita da interface.

## Gerenciar [!DNL Workfront] notificações de [!DNL Slack]

Você pode receber e responder a [!DNL Workfront] notificações de [!DNL Slack].

Você pode desabilitar notificações por email para notificações habilitadas no [!DNL Slack], para garantir que você não receba notificações duplicadas.\
Para obter informações sobre como configurar suas notificações por email, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Habilitar ou desabilitar notificações [!DNL Workfront] em [!DNL Slack] não afeta as notificações que você recebe dentro da interface [!DNL Workfront].\
Não é possível desabilitar notificações dentro da interface [!DNL Workfront].

Para gerenciar suas notificações do [!DNL Workfront] para [!DNL Slack]:

1. Faça logon no [!UICONTROL Slack].
1. Faça logon em [!DNL Workfront] a partir de [!DNL Slack].\
   Para obter informações sobre como fazer logon no [!DNL Workfront] a partir de [!DNL Slack], consulte a seção &quot;Fazendo logon no [!DNL Workfront] a partir de [!DNL Slack]&quot; no [Acesso [!DNL Adobe Workfront] a partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Verifique se as notificações de [!DNL Workfront] para [!DNL Slack] estão habilitadas.\
   Para obter mais informações sobre quais [!DNL Workfront] notificações podem ser configuradas para também serem enviadas para [!DNL Slack], consulte [Configurar [!DNL Workfront] notificações para [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Vá para o canal **[!DNL Workfront]** para encontrar suas notificações do [!DNL Workfront].
1. (Condicional e opcional) Execute um dos seguintes procedimentos:

   * Clique em **[!UICONTROL Trabalhar nisto]** para aceitar trabalhar em uma tarefa.

   * (Condicional e opcional) Clique em **[!UICONTROL Responder em[!DNL Workfront]]** para responder a um comentário, digite sua resposta e clique em **[!UICONTROL Responder]**.

   * (Condicional e opcional) Clique em **[!UICONTROL Aprovar]** ou **[!UICONTROL Rejeitar]** para aprovar ou rejeitar uma tarefa, problema ou projeto que esteja com sua aprovação pendente.

   * (Condicional e opcional) Clique em **[!UICONTROL Aprovar]**, **[!UICONTROL Alterações]** ou **[!UICONTROL Rejeitar]** para aprovar, aprovar com alterações ou rejeitar um documento.

     Você também pode passar o mouse sobre a miniatura do documento e clicar no ícone de lupa para exibir uma visualização maior do documento, antes de aprová-lo.\
      Somente os [tipos de arquivos](https://api.slack.com/types/file) aprovados do Slack podem ser visualizados.

   * (Condicional e opcional) Clique em **[!UICONTROL Conceder]** ou **[!UICONTROL Ignorar]** para conceder ou ignorar a solicitação de mais acesso de outro usuário.\

     Você receberá uma confirmação de que sua ação foi concluída em [!DNL Workfront] para cada decisão que você tomar em suas notificações.
