---
user-type: administrator
product-area: system-administration;user-management
keywords: exibir,grupo,evento,notificações,configurar,ativar,desativar
navigation-topic: create-and-manage-groups
title: Exibir e configurar notificações de evento para um grupo
description: Como administrador de grupo, você pode exibir as notificações de eventos ativadas para um grupo que você gerencia. Além disso, se um administrador do Adobe Workfront desbloquear uma notificação de evento, você poderá configurá-la para um grupo de nível superior que você gerencia. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: 306d6493ff0413d5814f4aed8ab44fb897f3568d
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Exibir e configurar notificações de evento para um grupo

Como administrador de grupo, você pode exibir as notificações de eventos ativadas para um grupo que você gerencia.

Além disso, se um administrador do Adobe Workfront desbloquear uma notificação de evento, você poderá configurá-la para um grupo de nível superior que você gerencia. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.

Um administrador do Workfront também pode fazer isso para qualquer grupo.

A configuração de uma notificação de evento para um grupo afeta os usuários para os quais esse grupo, ou um de seus subgrupos, é o Grupo doméstico. Em seus perfis de usuário, esses usuários visualizam as notificações de eventos ativadas para seu Grupo doméstico, em vez das notificações de eventos ativadas em todo o sistema.

Para obter informações sobre como um administrador do Workfront desbloqueia uma notificação de evento, consulte [Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Para obter informações sobre a configuração de notificação padrão para um evento, consulte [Notificações de evento disponíveis no Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plano Workfront</a>*</td> 
   <td> <p>Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Licença Adobe Workfront</a>*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Exibir e configurar notificações de evento de um grupo

1. (Condicional e opcional) Se você for um administrador do Workfront e já estiver na página Notificações por email (Configurar > Email > Notificações), poderá fazer o seguinte e, em seguida, pular para a etapa 6: Excluir **Notificações de evento do sistema** na caixa acima da lista, comece a digitar o nome do grupo na caixa e, em seguida, clique nele quando for exibido.
1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo de nível superior.
1. No menu esquerdo, clique em **Notificações de evento**.

   Na lista que é exibida, a variável **Ativo** à esquerda, mostra quais notificações estão ativas (azul) e inativas (cinza) para o grupo.

1. Para ativar ou desativar uma notificação de evento desbloqueado: Clique no botão no <strong>Ativo</strong> coluna para ativar <img src="assets/email-notification-enabled-unlocked.png"> ou desativar <img src="assets/email-notification-disabled-unlocked.png"> sim.

   >[!INFO]
   >
   >**Exemplo:** Você pode configurar as duas principais notificações de evento do grupo de marketing mostradas abaixo que foram desbloqueadas para grupos.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Se um botão no <strong>Ativo</strong> é cinza e esmaecida <img src="assets/email-notification-disabled-locked.png">, a notificação de evento é desativada para todos os usuários e os administradores de grupo não podem ativá-la ou editar sua linha de assunto do email
   >* Se um botão no <strong>Ativo</strong> é cinza e não está esmaecida <img src="assets/email-notification-disabled-unlocked.png">, a notificação de evento é <strong>desativado para todos os usuários e</strong> os administradores de grupo podem ativá-la para seus grupos.
   >* Se um botão no <strong>Ativo</strong> é azul e esmaecida <img src="assets/email-notification-enabled-locked.png">, a notificação de evento é ativada para todos os usuários e os administradores de grupo não podem desativá-la ou editar sua linha de assunto de email para seus grupos.
   >* Se um botão no <strong>Ativo</strong> é azul e não está esmaecida <img src="assets/email-notification-enabled-unlocked.png">, a notificação de evento é <strong>ativada para todos os usuários e</strong> os administradores de grupo podem desativá-la para seus grupos.


<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

