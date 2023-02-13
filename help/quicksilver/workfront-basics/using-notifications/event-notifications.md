---
content-type: overview
navigation-topic: notifications
title: Notificações de evento
description: As notificações de eventos são emails acionados por vários tipos de eventos em objetos, como projetos, tarefas ou problemas. Elas são enviadas quando ocorre algo no projeto que outros precisam saber. Dependendo do evento, os usuários recebem notificações instantâneas, diárias ou instantâneas e diárias por email sobre ele.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Notificações de evento

As notificações de eventos são emails acionados por vários tipos de eventos em objetos, como projetos, tarefas ou problemas. Elas são enviadas quando ocorre algo no projeto que outros precisam saber. Dependendo do evento, os usuários recebem notificações instantâneas, diárias ou instantâneas e diárias por email sobre ele.

>[!NOTE]
>
>As notificações de eventos são um dos vários tipos de [!DNL Adobe Workfront] notificações. Para obter informações sobre todos [!DNL Workfront] tipos de notificação, consulte [[!DNL Adobe Workfront] notificações](../../workfront-basics/using-notifications/wf-notifications.md).

## Configurar notificações de evento

Os emails de notificação de evento podem ser configurados nos seguintes níveis listados abaixo. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.

* **Nível do sistema**: A [!DNL Workfront] o administrador pode ativar e desativar as notificações de eventos no nível do sistema, conforme explicado em [Configurar notificações de evento para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Todos os grupos herdam notificações do sistema por padrão, mas os administradores de grupo podem alterar algumas configurações no nível do grupo, se permitido pelo [!DNL Workfront] administrador, conforme explicado no próximo item de marcador abaixo.

* **Nível do grupo**: Um administrador de grupo pode configurar uma notificação de evento para grupos que gerenciam após um [!DNL Workfront] O administrador desbloqueia essa capacidade para grupos. Se houver algum grupo acima do grupo que você gerencia, os administradores também poderão fazer isso para o seu grupo. O mesmo se aplica a [!DNL Workfront] administradores (para qualquer grupo). Para obter mais informações, consulte [Exibir e configurar notificações de evento para um grupo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

   >[!NOTE]
   >
   >Essa funcionalidade está disponível inicialmente apenas para clientes no Cluster 4 como parte de uma implantação em fases. Estará disponível para outros clusters em breve. Este artigo será atualizado à medida que isso ocorrer.

* **Nível do usuário**: Todas as notificações de eventos ativadas em todo o sistema são listadas em cada [!UICONTROL Notificações] em seu perfil individual. Os usuários podem ativar e desativar suas notificações de evento individual lá.

   [!DNL Workfront] administradores e usuários com acesso para editar outros usuários também podem ativar e desativar notificações no perfil de usuários individuais.

   Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

   >[!NOTE]
   >
   >As notificações no nível do usuário também incluem [!DNL Workfront Goals] notificações. No entanto, a variável [!DNL Workfront] o administrador ou o administrador do grupo não pode configurar notificações para [!DNL Workfront Goals]. Cada uso deve configurar seus próprios [!DNL Workfront Goals] notificações em seus perfis. Se você tiver acesso para editar usuários, também poderá modificar essas notificações para outros. Para ativar [!DNL Workfront Goals] notificações para seu perfil ou para outros usuários que você tem acesso para editar, consulte [Notificações: Metas](../../workfront-basics/using-notifications/notifications-goals.md).

   Para obter mais informações sobre quais notificações a variável [!DNL Workfront] administrador pode configurar, consulte [Configurar notificações de evento para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] estão disponíveis somente em [!DNL Adobe Workfront] experiência.

## Conteúdo de notificação de evento

Um email de notificação de evento contém informações sobre o evento que ocorreu e contém um link para [!DNL Workfront] onde você pode ver o evento no sistema. Para obter mais informações sobre o recebimento de notificações por email, consulte [[!DNL Adobe Workfront] notificações](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] o administrador não pode alterar o conteúdo das notificações por email, pois elas são configuradas por [!DNL Workfront]. No entanto, eles podem alterar as linhas de assunto dos emails de notificações de eventos. Para obter mais informações, consulte [Personalizar assuntos de email para notificações de eventos](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Para uma lista, todas as [!DNL Workfront] notificações de eventos, juntamente com uma breve descrição de cada evento e se ele está ativo ou inativo por padrão, consulte [Notificações de evento disponíveis em [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
