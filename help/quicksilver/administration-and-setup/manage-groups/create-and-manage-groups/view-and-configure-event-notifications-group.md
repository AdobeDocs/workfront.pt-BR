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
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

# Exibir e configurar notificações de eventos para um grupo

Como administrador de grupo, você pode exibir as notificações de eventos ativadas para um grupo gerenciado.

Além disso, se um administrador do Adobe Workfront desbloquear uma notificação de evento, você poderá configurá-la para um grupo de nível superior gerenciado por você. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.

Um administrador do Workfront também pode fazer isso para qualquer grupo.

Configurar uma notificação de evento para um grupo afeta os usuários para os quais esse grupo, ou um de seus subgrupos, é seu Grupo padrão. Em seus perfis de usuário, esses usuários veem as notificações de evento ativadas para seu Grupo inicial, em vez das notificações de evento ativadas em todo o sistema.

Para obter informações sobre como um administrador do Workfront desbloqueia uma notificação de evento, consulte [Desbloquear ou bloquear a configuração de notificações de evento para todos os grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Para obter informações sobre a configuração de notificação padrão de um evento, consulte [Tipos de notificação de evento](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir e configurar as notificações de eventos de um grupo

>[!TIP]
>
>Se você for um administrador do Workfront e já estiver na página Notificações por email (Configurar > Email > Notificações), faça o seguinte e pule para a etapa 6: Excluir **Notificações de eventos do sistema** na caixa acima da lista, começar a digitar o nome do grupo na caixa e, em seguida, clicar nele quando ele aparecer.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo de nível superior.
1. No menu esquerdo, clique em **Notificações de eventos**.

   Na lista exibida, a coluna **Ativo** à esquerda mostra quais notificações estão ativas (azul) e inativas (cinza) para o grupo.

1. Para ativar ou desativar uma notificação de evento desbloqueada: Clique no botão na coluna <strong>Ativo</strong> para ativar <img src="assets/email-notification-enabled-unlocked.png"> ou desativar <img src="assets/email-notification-disabled-unlocked.png"> ele.

   >[!INFO]
   >
   >**Exemplo:** você pode configurar as duas principais notificações de eventos de grupos de marketing mostradas abaixo que foram desbloqueadas para grupos.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Se um botão na coluna <strong>Ativo</strong> estiver cinza e esmaecido <img src="assets/email-notification-disabled-locked.png">, a notificação de eventos está desativada para todos os usuários e os administradores de grupos não podem ativá-la ou editar sua linha de assunto do email
   >* Se um botão na coluna <strong>Ativo</strong> estiver cinza e não esmaecido <img src="assets/email-notification-disabled-unlocked.png">, a notificação de eventos é <strong>desativada para todos os usuários e</strong> administradores de grupos podem ativá-la para seus grupos.
   >* Se um botão na coluna <strong>Ativo</strong> estiver azul e esmaecido <img src="assets/email-notification-enabled-locked.png">, a notificação de eventos é ativada para todos os usuários e os administradores de grupos não podem desativá-la ou editar a linha de assunto do email para seus grupos.
   >* Se um botão na coluna <strong>Ativo</strong> estiver azul e não esmaecido <img src="assets/email-notification-enabled-unlocked.png">, a notificação de eventos é <strong>ativada para todos os usuários e</strong> administradores de grupos podem desativá-la para seus grupos.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

