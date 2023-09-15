---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Receber [!DNL Adobe Workfront] notificações em [!DNL Slack]
description: Receber [!DNL Adobe Workfront] notificações em [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 6%

---

# Receber [!DNL Adobe Workfront] notificações em [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Depois de instalar o [!DNL Adobe Workfront for Slack], você pode receber [!DNL Workfront] notificações em [!DNL Slack].\
Para obter informações sobre a instalação [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Você pode ativar um número selecionado de [!UICONTROL notificações] que aparecem na bolha de notificações no [!DNL Workfront] interface, que também deverá ser entregue em [!DNL Slack].

As notificações por email funcionam independentemente das [!DNL Workfront] notificações de interface. Você ou seu [!DNL Workfront] o administrador pode desativar notificações por email, enquanto notificações por interface não podem ser desativadas no [!DNL Workfront].\
No entanto, você pode desativar [!DNL Workfront] notificações que você pode receber no [!DNL Slack], se quiser se concentrar nessas notificações somente dentro do [!DNL Workfront] interface.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plano]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.\

## Pré-requisitos

Antes de receber [!DNL Workfront] notificações em [!DNL Slack], você deve

* Configurar [!DNL Workfront for Slack]\
   Para obter instruções sobre como configurar o [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configurar [!DNL Workfront] notificações para [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Condicional) Após [!DNL Workfront] foi adicionado ao seu [!DNL Slack] instância, fazer logon no [!DNL Workfront] de [!DNL Slack].\
   Para obter informações sobre como fazer logon no [!DNL Workfront] de [!DNL Slack], consulte [Access [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Em qualquer canal, comece digitando um dos seguintes comandos no campo de mensagem:

   `/workfront settings`

   Ou

   `/wf settings`

1. Todas as notificações são ativadas, por padrão.\
   Desative qualquer uma das seguintes notificações:

   * [!UICONTROL Quando uma tarefa ou problema for alterado, enviar email para o usuário recentemente atribuído]
   * [!UICONTROL Minha equipe foi atribuída a uma nova tarefa ou problema]
   * [!UICONTROL Recebo uma nova solicitação de aprovação ou de acesso]
   * [!UICONTROL Alguém me inclui em uma atualização direcionada]
   * [!UICONTROL Quando alguém comentar em um item de trabalho, envie email para qualquer um que tiver comentado este item de trabalho]
   * [!UICONTROL Foi feita uma atualização em uma tarefa, problema ou projeto que eu assino]
   * [!UICONTROL Quando alguém comentar no item de trabalho, envie email para os atribuídos]
   * [!UICONTROL Quando alguém comentar na minha solicitação de ajuda, envie email para o usuário atribuído]

   As alterações feitas na variável [!UICONTROL notificações] as opções entrarão em vigor imediatamente.\
   As notificações ativadas são entregues no [!DNL Workfront] [!DNL Slack] canal. Quando você desativar as notificações aqui, elas só serão desativadas para [!DNL Slack], e não para o [!DNL Workfront] interface. Você continua a recebê-los no [!DNL Workfront] bolha de notificações na parte superior direita da interface.

## Gerenciar [!DNL Workfront] notificações de [!DNL Slack]

Você pode receber e responder a [!DNL Workfront] notificações de [!DNL Slack].

Você pode desativar notificações por email para notificações ativadas no [!DNL Slack], para garantir que você não receba notificações duplicadas.\
Para obter informações sobre como configurar as notificações por email, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Ativando ou desativando [!DNL Workfront] notificações em [!DNL Slack] não afeta as notificações que você recebe dentro do [!DNL Workfront] interface.\
Notificações dentro do [!DNL Workfront] não é possível desabilitar a interface.

Para gerenciar o seu [!DNL Workfront] notificações para [!DNL Slack]:

1. Efetue logon no [!UICONTROL Slack].
1. Efetue logon no [!DNL Workfront] de [!DNL Slack].\
   Para obter informações sobre como fazer logon no [!DNL Workfront] de [!DNL Slack], consulte a seção &quot;Logon no [!DNL Workfront] de [!DNL Slack]seção &quot; em [Access [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Verifique se [!DNL Workfront] notificações para [!DNL Slack] são ativados.\
   Para obter mais informações sobre qual [!DNL Workfront] as notificações podem ser configuradas para também serem enviadas para [!DNL Slack], consulte [Configurar [!DNL Workfront] notificações para [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Vá para a **[!DNL Workfront]** canal para encontrar seu [!DNL Workfront] notificações.
1. (Condicional e opcional) Execute um dos seguintes procedimentos:

   * Clique em **[!UICONTROL Trabalhar nisso]** para aceitar trabalhar em uma tarefa.

   * (Condicional e opcional) Clique em **[!UICONTROL Responder em[!DNL Workfront]]** para responder a um comentário, digite sua resposta e clique em **[!UICONTROL Responder]**.

   * (Condicional e opcional) Clique em **[!UICONTROL Aprovar]** ou **[!UICONTROL Rejeitar]** para aprovar ou rejeitar tarefas, problemas ou projetos que estejam pendentes de aprovação.

   * (Condicional e opcional) Clique em **[!UICONTROL Aprovar]**, **[!UICONTROL Alterações]** ou **[!UICONTROL Rejeitar]**, para aprovar, aprovar com alterações ou rejeitar um documento.

     Você também pode passar o mouse sobre a miniatura do documento e clicar no ícone de lupa para exibir uma visualização maior do documento, antes de aprová-lo.\
      Somente o Slack aprovado [tipos de arquivo](https://api.slack.com/types/file) pode ser visualizado.

   * (Condicional e opcional) Clique em **[!UICONTROL Conceder]** ou **[!UICONTROL Ignorar]** para conceder ou ignorar a solicitação de mais acesso de outro usuário.\

     Você receberá uma confirmação de que sua ação foi concluída em [!DNL Workfront], para cada decisão tomada nas notificações.
