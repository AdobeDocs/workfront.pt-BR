---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Marcar outras pessoas em atualizações
description: Ao fornecer comentários de atualização em um objeto do Adobe Workfront, todos os usuários do projeto podem ver as informações enviadas. No entanto, pode haver momentos em que os usuários que não estão no projeto se beneficiem de visualizar essas informações. Em vez de incluir esses usuários no projeto, você pode marcá-los na atualização para compartilhá-los com eles. Os usuários marcados receberão uma notificação de evento.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: ba1d8d5a23da7e252e8c182a6bdb1cdd1e304eab
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Marcar outras pessoas em atualizações

<!--take "Beta" references out when we remove the beta-->

<!-- Drafted for commenting experience: 

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 
>
>You can access the new design for the following objects:
> * <span class="preview">Issues, when enabling the commenting Beta. </span>
> * Goals
>   The new commenting experience is the default for goals. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

-->
É possível marcar usuários ao fazer uma atualização em um objeto, caso deseje chamar a atenção para um objeto que, de outra forma, eles talvez não sigam.
Em vez de incluir esses usuários no objeto, atribuindo-os a ele ou fazendo com que eles se inscrevam nele, você pode marcá-los na atualização para compartilhá-los com eles. Os usuários marcados receberão uma notificação sobre a atualização inserida.

>[!NOTE]
>
>Uma notificação de evento deve estar ativada para que um usuário receba a notificação por email. Os administradores podem habilitar notificações para todo o sistema ou para um grupo de nível superior. Um usuário também pode ativar e desativar notificações de eventos individuais em seu próprio perfil de usuário. Para obter mais informações, consulte:
>
>* [Configurar notificações de evento para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [Exibir e configurar notificações de evento para um grupo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


Para obter informações sobre como adicionar atualizações a objetos Workfront, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Quando um problema é convertido em um projeto ou tarefa, as atualizações são copiadas para o novo projeto ou tarefa, mas os usuários marcados não são. Para continuar a conversa, você deve marcar os participantes novamente.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Pedido ou superior para questões e documentos; Revisar ou superior para todos os outros objetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Solicitante ou superior para problemas e documentos; Revisor ou superior para todos os outros objetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Exibir acesso ao objeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Marcar outras pessoas em atualizações

<!--
Tagging others in an update differs depending on which experience and which object you select.

### Tag others on updates in the current Updates section
-->

1. Comece a atualizar um item de trabalho, conforme descrito em [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. No **Notificar** , comece a digitar o nome do usuário ou da equipe que deseja incluir e clique no nome quando ele for exibido na lista suspensa.

   Ou

   Digite o símbolo @ no **Iniciar uma nova atualização** , comece a digitar o nome do usuário ou da equipe que deseja incluir na atualização e clique no nome quando ele for exibido na lista suspensa.

   >[!TIP]
   >
   >Para identificar o usuário correto quando há usuários com nomes semelhantes ou idênticos, observe o avatar, a função primária do usuário ou seu endereço de email. Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la à medida que você os marcar em uma atualização.

   ![](assets/tag-users-in-update.png)

1. (Opcional) Para tornar a atualização privada, habilite **Privado da minha empresa** no canto inferior direito da caixa de atualização. Isso torna a atualização visível apenas para os usuários em sua empresa.

   >[!NOTE]
   >
   >Os usuários marcados fora da empresa ainda podem receber uma notificação no aplicativo ou email, mesmo que não vejam os comentários privados na guia Atualizações . Recomendamos não adicionar tags a usuários externos em uma atualização se você não quiser compartilhar as informações com eles.

1. (Opcional) Para adicionar vários usuários e equipes, repita a etapa 2.

   >[!NOTE]
   >
   >Todos os usuários e membros da equipe listados no campo Notificar recebem uma notificação no aplicativo para a atualização e podem receber um email, dependendo da configuração de suas configurações de notificação por email. Os usuários que marcam um comentário ou resposta recebem uma notificação para esse comentário ou resposta e podem ver seu nome no campo Notificar para o restante do encadeamento, mas não recebem outra notificação, a menos que sejam marcados novamente. Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) e [Configurar notificações de evento para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Clique em **Atualizar**.\
   Os usuários incluídos na atualização recebem automaticamente permissão de Exibição para o objeto e podem visualizar e responder atualizações feitas no objeto.

   Você pode ver quem foi marcado em cada resposta na parte superior do thread de atualização. Esses usuários, juntamente com qualquer usuário inscrito no objeto, recebem uma notificação sempre que uma atualização ou resposta for feita no objeto.

   ![](assets/tagging-transparency-350x192.png)

   Para obter informações sobre a funcionalidade adicional que está disponível ao atualizar um item de trabalho, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--
<div class="preview">

### Tag others on updates in the commenting Beta experience

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Tag people or teams** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   <!- ********************* this doesn't seem to work in Beta - keep drafted for now: 
   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list. ************close draft

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. Users must be associated with at least one job role to view it as you tag them in an update.

   ![](assets/tag-others-unified-commenting.png)

      <!-******************* this might not be there for issues yet - keep drafted if not: 
      1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company.

         >[!NOTE]
         >
         >* This option displays only when the user is associated with a Company.
         >* Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them. - ************close draft 
      
1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the "Tag people or teams" field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in listed as a member of the thread for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Submit**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply under the text of the update, in the Members area. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.
1. (Optional) Cick the number of members included in the update to display a list of entities that the update you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)

   For information about the additional functionality that is available when updating a work item, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

-->