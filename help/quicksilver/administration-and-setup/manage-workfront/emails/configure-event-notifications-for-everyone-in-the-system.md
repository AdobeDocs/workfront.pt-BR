---
title: Configurar notificações de evento para todos no sistema
description: As notificações de eventos acionam emails para os usuários quando um determinado evento ocorre. Como administrador do Adobe Workfront ou usuário com nível de acesso do Planejador, você pode configurar uma notificação de evento para todos os usuários no sistema. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.
author: Caroline, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Configurar notificações de evento para todos no sistema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

As notificações de eventos acionam emails para os usuários quando um determinado evento ocorre. Como administrador do Adobe Workfront ou usuário com nível de acesso do Planejador, você pode configurar uma notificação de evento para todos os usuários no sistema. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

Dependendo do evento que você ativar e o usuário continuar ativado em seu próprio perfil, os usuários recebem notificações instantâneas, diárias ou instantâneas e diárias de email quando um evento ocorre.

Primeiro, especifique quais notificações você deseja que todos os usuários recebam na área Configuração da sua instância do Workfront. Depois de ativar uma notificação na área Configuração, ela é exibida como ativada para cada usuário na página do perfil.

Depois que as notificações são ativadas na área Configuração e aparecem nas páginas de perfil dos usuários, os usuários individuais ou outros usuários com uma licença de Plano também podem configurar as notificações ativadas em um perfil de usuário para controlar quais notificações um usuário específico recebe e com que frequência. Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de evento](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obter uma lista de todas as notificações de eventos que podem ser ativadas e desativadas, consulte [Notificações de evento disponíveis no Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para obter informações sobre como desbloquear uma notificação de evento para que os administradores de grupo possam configurá-la para seus grupos, consulte [Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) e [Exibir e configurar notificações de evento para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Planejador ou superior, com acesso administrativo às notificações de lembrete</p> <p>Para obter informações sobre como conceder acesso administrativo a um Usuário do Plano, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Configurar notificações de evento para todos os usuários

Você deve ativar as notificações na área Configuração do Workfront antes que os usuários possam ativá-las ou desativá-las em seus perfis.

>[!TIP]
>
>Não é possível ativar notificações para Objetivos do Workfront na área Configuração. Os usuários podem ativar essas notificações somente em seus perfis. Os usuários com licenças de Plano podem ativá-las para outros usuários. Para obter informações sobre como ativar notificações de Metas do Workfront para usuários, consulte [Notificações: Metas](../../../workfront-basics/using-notifications/notifications-goals.md).

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Email** > **Notificações**.

1. Certifique-se de que o **Notificações de evento** está aberta.
1. Clique no botão à esquerda do nome do evento para ativá-lo ou desativá-lo.

   Para ver o status de notificação padrão de um evento, consulte [Notificações de evento](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Opcional) Clique no nome de uma notificação de evento para personalizar a linha de assunto da notificação de email.

   Para obter mais informações sobre como personalizar as linhas de assunto das notificações por email, consulte [Personalizar assuntos de email para notificações de eventos](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Opcional) Se desejar desbloquear a configuração de uma notificação por email para que os administradores de grupo possam configurá-la separadamente para seus grupos, clique no botão ![](assets/lock-toggle-button.png) à direita da notificação para alterá-la para a posição desbloqueada ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >Essa funcionalidade está disponível inicialmente apenas para clientes no Cluster 4 como parte de uma implantação em fases. Estará disponível para outros clusters em breve. Este artigo será atualizado à medida que isso ocorrer.

   Para obter mais informações, consulte [Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
