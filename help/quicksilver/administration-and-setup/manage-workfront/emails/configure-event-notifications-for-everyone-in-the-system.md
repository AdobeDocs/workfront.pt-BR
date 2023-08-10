---
title: Configurar notificações de eventos para todos no sistema
description: As notificações de eventos acionam emails para usuários quando ocorre um determinado evento. Como administrador do Adobe Workfront ou usuário com nível de acesso de Planejador, você pode configurar uma notificação de evento para todos os usuários no sistema. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.
author: Caroline, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: 207a8c8a642f3204a2d007789eb7ee8cd9379f1b
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Configurar notificações de eventos para todos no sistema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

As notificações de eventos acionam emails para usuários quando ocorre um determinado evento. Como administrador do Adobe Workfront ou usuário com nível de acesso de Planejador, você pode configurar uma notificação de evento para todos os usuários no sistema. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

Dependendo do evento que você ativar e o usuário manter ativado em seu próprio perfil, os usuários receberão notificações instantâneas, diárias ou por email instantâneas e diárias quando ocorrer um evento.

Primeiro, especifique quais notificações você deseja que todos os usuários recebam na área Configuração da sua instância do Workfront. Depois de ativar uma notificação na área Configuração, ela é exibida como ativada para cada usuário na página de perfil.

Depois que as notificações forem ativadas na área Configuração e aparecerem nas páginas de perfil dos usuários, os usuários individuais ou outro usuário com uma licença de Plano também poderão configurar as notificações ativadas em um perfil de usuário para controlar quais notificações esse usuário específico recebe e com que frequência. Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de eventos](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obter uma lista de todas as notificações de eventos que você pode ativar e desativar, consulte [Notificações de eventos disponíveis no Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para obter informações sobre como desbloquear uma notificação de evento para que administradores de grupos possam configurá-la para seus grupos, consulte [Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) e [Exibir e configurar notificações de eventos para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Planejador ou superior, com acesso administrativo a notificações de lembrete</p> <p>Para obter informações sobre como conceder acesso administrativo a um usuário do Plano, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Configurar notificações de eventos para todos os usuários

Você deve ativar notificações na área Configuração do Workfront antes que os usuários possam ativá-las ou desativá-las em seus perfis.

>[!TIP]
>
>Não é possível ativar notificações para o Workfront Goals na área Configuração. Os usuários podem ativar essas notificações somente em seus perfis. Os usuários com licenças de Plano podem ativá-las para outros usuários. Para obter informações sobre como ativar notificações do Workfront Goals para usuários, consulte [Notificações: Metas](../../../workfront-basics/using-notifications/notifications-goals.md).

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **E-mail** > **Notificação**.

   ![](assets/notifications-area-under-setup-emails.png)


1. Verifique se **Notificações de Eventos** está aberta.
1. Clique na chave à esquerda do nome do evento para ativá-lo ou desativá-lo.

   Para ver o status de notificação padrão de um evento, consulte [Notificações de eventos](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Opcional) Clique no nome de uma notificação de evento para personalizar a linha de assunto da notificação por email.

   Para obter mais informações sobre como personalizar as linhas de assunto das notificações por email, consulte [Personalizar assuntos de email para notificações de eventos](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Opcional) Se desejar desbloquear a configuração de uma notificação por email para que os administradores de grupo possam configurá-la separadamente para seus grupos, clique no botão ![](assets/lock-toggle-button.png) à direita da notificação para colocá-la na posição desbloqueada ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >Inicialmente, essa funcionalidade está disponível apenas para clientes no Cluster 4 como parte de uma implantação em fases. Logo depois disso, ela se tornará disponível para outros clusters. Este artigo será atualizado à medida que isso ocorrer.

   Para obter mais informações, consulte [Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
