---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Gerenciar [!DNL Adobe Workfront] notificações em [!DNL Microsoft] Equipes
description: Você pode receber notificações de [!DNL Adobe Workfront] sobre itens que você precisa aprovar, atribuições que você recebeu ou comentários e alterações nos itens aos quais você está associado.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 1f2655c0e88a5cc918501e2a0ef830758111ded8
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 0%

---

# Gerenciar [!DNL Adobe Workfront] notificações em [!DNL Microsoft Teams]

>[!NOTE]
>
>Atualmente, o Adobe Workfront para integração do Microsoft Teams é compatível apenas com a experiência clássica do Microsoft Teams.

Você pode receber notificações de [!DNL Adobe Workfront] sobre itens que você precisa aprovar, atribuições que você recebeu ou comentários e alterações nos itens aos quais você está associado.

Essas notificações contêm [!DNL Workfront] ações que você pode realizar no [!DNL Microsoft Teams] sem sair do [!DNL Microsoft Teams] para realizá-los.

>[!NOTE]
>
>[!DNL Microsoft Teams] não oferece mais suporte [!DNL Internet Explorer]. Para usar o [!DNL Adobe Workfront for Microsoft Teams integration], você deve usar um navegador da Web diferente do [!DNL Internet Explorer].


## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Trabalho], [!UICONTROL Plano]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Pré-requisitos para Recebimento [!DNL Workfront] Notificações em [!DNL Microsoft Teams]

Você pode receber [!DNL Workfront] notificações em [!DNL Microsoft Teams] se as seguintes condições forem atendidas:

* Um proprietário de equipe instalou e configurou o [!DNL Workfront for Microsoft Teams] para a sua equipe.
* Você está conectado [!DNL Workfront] de [!DNL Microsoft Teams].
* Você ativou as notificações instantâneas no [!DNL Workfront]. Para obter informações sobre como ativar notificações instantâneas, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obter informações sobre a instalação [!DNL Workfront for Microsoft Teams] e fazendo logon no [!DNL Workfront from Microsoft Teams], consulte [Instalar [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Gerenciamento [!DNL Workfront] Notificações em [!DNL Microsoft Teams]

Quando a variável [!DNL Workfront for Microsoft Teams] estiver instalado, um [!DNL Workfront] o canal de chat é criado em [!DNL Microsoft Teams] para cada membro dessa equipe. Quando uma determinada ação é executada no [!DNL Workfront], é possível definir as configurações para [!DNL Workfront for Microsoft Teams] para receber notificações sobre essa ação no [!DNL Workfront] canal de chat de [!DNL Microsoft Teams].

Considere o seguinte ao trabalhar com o [!DNL Workfront] notificações de [!DNL Microsoft Teams]:

* Você não pode receber todos, mas apenas um número selecionado de [!DNL Workfront] notificações em [!DNL Microsoft Teams].
* Todas as notificações recebidas do [!DNL Workfront] aparecem no [!DNL Workfront] canal de chat do bot.

  Para obter informações sobre como instalar o [!DNL Workfront] canal de bot, consulte a [Efetuando logon no [!DNL Workfront] de [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) seção em [Instalando [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) artigo.

* Pode haver um atraso de até 5 minutos entre o momento em que uma atualização é feita na [!DNL Workfront] e quando você receber a notificação sobre ele no [!DNL Microsoft Teams].
* Para cada [!DNL Microsoft Teams] você também receberá uma notificação por email.

Para gerenciar o [!DNL Workfront] notificações que você pode receber no [!DNL Microsoft Teams]:

1. Clique em **[!UICONTROL Mais adicionados]** (três pontos) ícone de aplicativos na barra de navegação esquerda no [!DNL Microsoft Teams].

1. Clique em [!DNL Workfront] na lista exibida.
1. Selecione o **[!UICONTROL Configurações]** guia.

   ![](assets/ms-teams-settings-tab-350x552.png)

1. Desative qualquer uma das notificações que você não deseja receber. Você pode ativar ou desativar grupos de notificações, como notificações de informações ou de aprovação, ou gerenciar notificações individualmente.

   Todas as notificações são ativadas por padrão.

   As configurações de notificação para [!DNL Workfront for Microsoft] As equipes são salvas automaticamente.

   >[!NOTE]
   >
   >Não é possível adicionar mais notificações às que estão disponíveis por padrão.

## Respondendo a [!DNL Workfront] Notificações e solicitações de aprovação em [!DNL Microsoft Teams]

1. Efetue logon no [!DNL Workfront] de [!DNL Microsoft Teams].\
   Para obter informações sobre como fazer logon no [!DNL Workfront], consulte [Instalar [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Vá para a **[!UICONTROL Bate-papo]** e clique na guia **[!DNL Workfront]** canal de bot.\
   Este canal é para o seu chat pessoal com a [!DNL Workfront] bot. Todos [!DNL Workfront] as notificações são exibidas aqui.
1. Dependendo do tipo de notificação recebida, vá para a seção relevante:

   * [Notificações de aprovação](#approval-notifications-approval-notifications)
   * [Notificações de atribuição](#assignment-notifications-assignment-notifications)
   * [Notificações de comentários](#comment-notifications-comment-notifications)
   * [Atualizar notificações](#update-notifications-update-notifications)
   * [Notificações de alteração de data](#date-change-notifications-date-change-notifications)

### Notificações de aprovação {#approval-notifications}

Você recebe notificações de aprovação quando é solicitado a aprovar um objeto, como uma tarefa, uma folha de horas ou uma prova. No entanto, você ainda pode comentar na notificação. Na notificação de aprovação, é possível executar as seguintes ações:

* **[!UICONTROL Aprovar]**: Clique em para aprovar o item.
* **[!UICONTROL Alterar]**: clique em para aprovar o item com alterações.
* **[!UICONTROL Rejeitar]**: Clique para rejeitar o item.
* **[!UICONTROL Comentário]**: Clique em para fazer um comentário. Seu comentário também aparece em [!DNL Workfront] como uma atualização do objeto sobre o qual a notificação é feita.
* **[!UICONTROL Ir para prova]**: clique em para abrir a prova. Você pode tomar uma decisão diretamente na prova. Para obter mais informações, consulte [Tomar uma decisão sobre uma prova no visualizador de provas](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>Depois de tomar uma decisão de aprovação, você não poderá alterá-la da notificação.

#### Ações disponíveis em notificações de aprovação específicas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificação</th> 
   <th>[!UICONTROL Aprovar]</th> 
   <th>[!UICONTROL Rejeitar]</th> 
   <th> <p>[!UICONTROL Alterar]</p> </th> 
   <th> <p>[!UICONTROL Ir para Prova] </p> </th> 
   <th>[!UICONTROL Comentário]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Você precisa aprovar um projeto</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Você precisa aprovar uma tarefa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Você precisa aprovar um problema</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Você precisa aprovar um documento</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Você precisa aprovar o acesso a um objeto</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Você precisa aprovar uma planilha de horas</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguém deseja que você aprove esta prova</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sua planilha de horas foi rejeitada</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sua Planilha de Horas foi reaberta</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uma solicitação de aprovação de documento que você solicitou foi aprovada</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uma solicitação de aprovação de documento que você solicitou foi aprovada com alterações</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uma solicitação de aprovação de documento que você solicitou foi rejeitada</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sua planilha de horas foi aprovada</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Notificações de atribuição {#assignment-notifications}

Você recebe notificações de atribuição quando você ou uma equipe da qual você faz parte está atribuída a uma tarefa ou problema no Workfront. Na notificação de atribuição, você pode executar as seguintes ações:

* **[!UICONTROL Trabalhar nisso]**: selecione para confirmar o trabalho no item. Uma notificação é exibida brevemente para confirmar que um novo item foi adicionado à sua lista de trabalho.
* **[!UICONTROL Exibir em[!DNL Workfront]]**: selecione para exibir o problema ou a tarefa atribuída na Workfront, o que abre uma nova guia.
* **[!UICONTROL Início]**: Clique para iniciar o trabalho no item. Uma notificação é exibida brevemente para confirmar que um novo item foi adicionado à sua lista de trabalho.
* **[!UICONTROL Comentário]**: clique para fazer um comentário no item. Seu comentário também aparece no fluxo de atualização do item no Workfront.
* **[!UICONTROL Status]**: Clique em e selecione o novo status para o item de trabalho no menu suspenso.

#### Ações disponíveis em notificações de atribuições específicas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificação</th> 
   <th>[!UICONTROL Iniciar]</th> 
   <th>[!UICONTROL Comentário]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Você está atribuído a uma tarefa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Você está atribuído a um problema</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uma equipe atribuída a você recebe uma solicitação de trabalho para uma tarefa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uma equipe à qual você está atribuído recebe uma solicitação de trabalho para um problema</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
 </tbody> 
</table>

### Notificações de comentários {#comment-notifications}

Você recebe uma notificação de comunicação quando alguém comenta em um item ao qual você está associado ou o inclui em uma atualização. Na notificação de comunicação, você pode executar as seguintes ações:

* **Reply**: Clique para responder ao comentário ou [!UICONTROL atualizar]. Sua resposta também aparece na sequência de atualização em que o comentário aparece no Workfront.
* **[!UICONTROL Exibir no Workfront]**: selecione para exibir o comentário e o item no Workfront, que é aberto em uma nova guia.
* **[!UICONTROL Status]**: Clique em e selecione um novo status para o item de trabalho sobre o qual o comentário ou atualização é.

#### Ações disponíveis em notificações de comunicação específicas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificação</th> 
   <th>[!UICONTROL Responder]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Um comentário é postado na sua solicitação</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uma resposta é postada em sua solicitação de trabalho</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando alguém comentar em um item de trabalho, envie email para qualquer um que tiver comentado este item de trabalho</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguém comentou um dos seus itens de trabalho</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando alguém comentar em uma planilha de horas aprovada, envie email para os atribuídos</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Um comentário é adicionado na página do perfil do usuário ou ao editar vários usuários em massa</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Um comentário é adicionado em uma de suas atualizações</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Um comentário é adicionado em sua folha de horas</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Atualizar notificações {#update-notifications}

Você recebe uma notificação de informações quando há uma atualização de um item ao qual você está associado, mas não é necessário realizar nenhuma ação no item. A partir da notificação de informações, você pode executar as seguintes ações:

* **[!UICONTROL Responder]**: Clique para responder à [!UICONTROL atualizar]. Sua resposta também aparece no fluxo de atualização do item no Workfront.
* **Exibir no Workfront**: selecione para exibir o comentário e o item no Workfront, que é aberto em uma nova guia.
* **[!UICONTROL Status]**: Clique em e selecione o novo status para o item no menu suspenso.

#### Ações disponíveis em notificações de informações específicas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificação</th> 
   <th>[!UICONTROL Responder]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Foi feita uma atualização em uma tarefa, problema ou projeto que você assina</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguém tiver incluído você em uma atualização direcionada</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguém tiver incluído sua equipe em uma [!UICONTROL atualização direcionada]</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
 </tbody> 
</table>

### Notificações de alteração de data {#date-change-notifications}

Você recebe uma notificação de alteração de data quando a data muda em um item de trabalho ao qual você está atribuído. Na notificação de alteração de data, você pode executar as seguintes ações.

* **[!UICONTROL Comentário]**: clique para fazer um comentário no item. Seu comentário também aparece no fluxo de atualização do item no Workfront.
* **[!UICONTROL Status]**: Clique em e selecione o novo status para o item de trabalho no menu suspenso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificação</th> 
   <th> <p>[!UICONTROL Comentário]</p> </th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">A data de conclusão de uma tarefa atribuída a você mudou</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
 </tbody> 
</table>
