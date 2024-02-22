---
user-type: administrator
product-area: system-administration;user-management
keywords: exibir,grupo,evento,notificações,configurar,ativar,desativar
navigation-topic: create-and-manage-groups
title: Exibir e configurar notificações de eventos para um grupo
description: Como administrador de grupo, você pode exibir as notificações de eventos ativadas para um grupo gerenciado. Além disso, se um administrador do Adobe Workfront desbloquear uma notificação de evento, você poderá configurá-la para um grupo de nível superior gerenciado por você. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Exibir e configurar notificações de eventos para um grupo

Como administrador de grupo, você pode exibir as notificações de eventos ativadas para um grupo gerenciado.

Além disso, se um administrador do Adobe Workfront desbloquear uma notificação de evento, você poderá configurá-la para um grupo de nível superior gerenciado por você. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.

Um administrador do Workfront também pode fazer isso para qualquer grupo.

Configurar uma notificação de evento para um grupo afeta os usuários para os quais esse grupo, ou um de seus subgrupos, é seu Grupo padrão. Em seus perfis de usuário, esses usuários veem as notificações de evento ativadas para seu Grupo inicial, em vez das notificações de evento ativadas em todo o sistema.

Para obter informações sobre como um administrador do Workfront desbloqueia uma notificação de evento, consulte [Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Para obter informações sobre a configuração de notificação padrão de um evento, consulte [Tipos de notificação de eventos](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir o tipo de plano ou licença que possui, entre em contato com o administrador do Workfront.

## Exibir e configurar as notificações de eventos de um grupo

1. (Condicional e opcional) Se você for um administrador do Workfront e já estiver na página Notificações por email (Configurar > Email > Notificações), poderá fazer o seguinte e pular para a etapa 6: Excluir **Notificações de Eventos do Sistema** na caixa acima da lista, comece digitando o nome do grupo na caixa e, em seguida, clique nele quando ele for exibido.
1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo de nível superior.
1. No menu esquerdo, clique em **Notificações de eventos**.

   Na lista exibida, a variável **Ativo** A coluna à esquerda mostra quais notificações estão ativas (azul) e inativas (cinza) para o grupo.

1. Para ativar ou desativar uma notificação de evento desbloqueada: clique no botão na <strong>Ativo</strong> coluna a ser ativada <img src="assets/email-notification-enabled-unlocked.png"> ou desativar <img src="assets/email-notification-disabled-unlocked.png"> o mesmo.

   >[!INFO]
   >
   >**Exemplo:** Você pode configurar as duas principais notificações de eventos de grupos de marketing mostradas abaixo que foram desbloqueadas para grupos.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Se um botão no <strong>Ativo</strong> a coluna está cinza e esmaecida <img src="assets/email-notification-disabled-locked.png">, a notificação de eventos é desativada para todos os usuários e os administradores de grupos não podem ativá-la ou editar sua linha de assunto do email
   >* Se um botão no <strong>Ativo</strong> a coluna está cinza e não esmaecida <img src="assets/email-notification-disabled-unlocked.png">, a notificação de evento é <strong>desativado para todos os usuários e</strong> administradores de grupos podem ativá-la para seus grupos.
   >* Se um botão no <strong>Ativo</strong> a coluna está azul e esmaecida <img src="assets/email-notification-enabled-locked.png">, a notificação de eventos é ativada para todos os usuários e os administradores de grupos não podem desativá-la ou editar a linha de assunto do email para seus grupos.
   >* Se um botão no <strong>Ativo</strong> a coluna é azul e não esmaecida <img src="assets/email-notification-enabled-unlocked.png">, a notificação de evento é <strong>ativado para todos os usuários e</strong> os administradores de grupo podem desativá-la para seus grupos.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

