---
content-type: overview
navigation-topic: notifications
title: Notificações de eventos
description: As notificações de eventos são emails acionados por vários tipos de eventos em objetos, como projetos, tarefas ou problemas. Eles são enviados quando algo ocorre no projeto que outros precisam saber. Dependendo do evento, os usuários recebem notificações instantâneas, diárias ou por email instantâneas e diárias sobre ele.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Notificações de eventos

As notificações de eventos são emails acionados por vários tipos de eventos em objetos, como projetos, tarefas ou problemas. Eles são enviados quando algo ocorre no projeto que outros precisam saber. Dependendo do evento, os usuários recebem notificações instantâneas, diárias ou por email instantâneas e diárias sobre ele.

>[!NOTE]
>
>As notificações de eventos são um dos vários tipos de [!DNL Adobe Workfront] notificações. Para obter informações sobre todos os tipos de notificação [!DNL Workfront], consulte [[!DNL Adobe Workfront] notificações](../../workfront-basics/using-notifications/wf-notifications.md).

## Configurar notificações de eventos

Os emails de notificação de eventos podem ser configurados nos seguintes níveis listados abaixo. A configuração de uma notificação de evento consiste em ativá-la ou desativá-la.

* **Nível do sistema**: um administrador [!DNL Workfront] pode ativar e desativar notificações de eventos no nível do sistema, conforme explicado em [Configurar notificações de eventos para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Todos os grupos herdam notificações do sistema por padrão, mas os administradores de grupos podem alterar algumas configurações no nível do grupo, se permitido pelo administrador [!DNL Workfront], conforme explicado no próximo item de marcador abaixo.

* **Nível do grupo**: um administrador de grupo pode configurar uma notificação de evento para grupos que gerenciam depois que um administrador [!DNL Workfront] desbloqueia esta habilidade para grupos. Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo é verdadeiro para administradores [!DNL Workfront] (para qualquer grupo). Para obter mais informações, consulte [Exibir e configurar notificações de eventos para um grupo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >Inicialmente, essa funcionalidade está disponível apenas para clientes no Cluster 4 como parte de uma implantação em fases. Logo depois disso, ela se tornará disponível para outros clusters. Este artigo será atualizado à medida que isso ocorrer.

* **Nível de usuário**: todas as notificações de eventos ativadas em todo o sistema estão listadas na seção [!UICONTROL Notificações] de cada usuário em seus perfis individuais. Os usuários podem ativar e desativar as notificações de eventos individuais lá.

  [!DNL Workfront] administradores e usuários com acesso para editar outros usuários também podem ativar e desativar notificações no perfil de usuários individuais.

  Para obter mais informações, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >As notificações de nível de usuário também incluem [!DNL Workfront Goals] notificações. No entanto, o administrador [!DNL Workfront] ou o administrador de grupo não pode configurar notificações para [!DNL Workfront Goals]. Cada usuário deve configurar suas próprias [!DNL Workfront Goals] notificações em seu perfil. Se você tiver acesso para editar usuários, também poderá modificar essas notificações para outras pessoas. Para habilitar [!DNL Workfront Goals] notificações para seu perfil ou para outros usuários aos quais você tem acesso para editar, consulte [Notificações: Metas](../../workfront-basics/using-notifications/notifications-goals.md).

  Para obter mais informações sobre quais notificações o administrador do [!DNL Workfront] pode configurar, consulte [Configurar notificações de eventos para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] estão disponíveis somente na nova experiência [!DNL Adobe Workfront].

## Conteúdo da notificação de eventos

Um email de notificação de evento contém informações sobre o evento que ocorreu e contém um link para [!DNL Workfront] onde você pode ver o evento no sistema. Para obter mais informações sobre como receber notificações por email, consulte [[!DNL Adobe Workfront] notificações](../../workfront-basics/using-notifications/wf-notifications.md).

Um administrador do [!DNL Workfront] não pode alterar o conteúdo das notificações por email, pois elas são configuradas por [!DNL Workfront]. No entanto, eles podem alterar as linhas de assunto dos emails de notificações de eventos. Para obter mais informações, consulte [Personalizar assuntos de email para notificações de eventos](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Para obter uma lista de todas as [!DNL Workfront] notificações de eventos, juntamente com uma breve descrição de cada evento, e se ele está ativo ou inativo por padrão, consulte [Notificações de eventos disponíveis em [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
