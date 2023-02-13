---
content-type: overview;reference
navigation-topic: notifications
title: Notificações do Adobe Workfront
description: O Adobe Workfront envia notificações por email, notificações no aplicativo e notificações no seu dispositivo móvel.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1255'
ht-degree: 1%

---

# [!DNL Adobe Workfront] notificações

[!DNL Adobe Workfront] O envia notificações por email, notificações no aplicativo e notificações no seu dispositivo móvel.

## Notificações de email

[!DNL Workfront] O envia várias notificações por email para alertar os usuários sobre a atividade no Workfront e fornecer informações e links úteis.

>[!NOTE]
>
>Se quiser receber notificações por email do ambiente Sandbox, ative emails do seu perfil de usuário nesse ambiente.

Você pode receber as seguintes notificações por email de [!DNL Workfront]:

* [Notificações de evento](#event-notifications)
* [Notificações de resumo diário](#daily-digest-notifications)
* [Notificação de comentários postados](#notification-of-posted-comments)
* [Lembretes automáticos](#automatic-reminders)
* [Notificações de lembrete](#reminder-notifications)
* [Outras [!DNL Workfront] emails](#other-workfront-emails)

### Notificações de evento

As notificações de evento são predefinidas em [!DNL Workfront]. Normalmente, elas são acionadas por determinados eventos.

Depois que as notificações de evento forem ativadas pelo [!DNL Workfront] administrador ou administrador de grupo, você pode selecionar os que deseja receber editando seu [!UICONTROL Notificações] preferências no seu perfil de usuário. Você também pode escolher se deseja receber notificações conforme os eventos ocorrem ou se deseja receber eventos resumidos em um email de resumo diário.

Dependendo de como o [!DNL Workfront] o administrador configurou notificações de evento para seu [!DNL Workfront] (conforme descrito em [Configurar notificações de evento para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)), você pode ver apenas um subconjunto dessas notificações em suas configurações.

O status padrão mostra quais notificações (diárias, instantâneas ou ambas) são ativadas por padrão para novos usuários ao criar os novos usuários.

Para obter uma lista completa das notificações do evento e informações sobre como elas são ativadas e configuradas no nível do sistema, no nível do grupo ou no nível do usuário, consulte [Notificações de evento disponíveis em [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para obter informações sobre como escolher quais notificações de eventos você deseja receber, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>As notificações de eventos são as únicas notificações que podem ser configuradas para serem entregues em atualizações diárias de resumo.

### Notificações de resumo diário

Para obter uma lista completa de quais notificações por email foram ativadas para um delivery de email de resumo diário, bem como informações sobre todas as categorias para notificações por email, consulte [Notificações de evento](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] não envia notificações de resumo diário para o [!UICONTROL Diversos] e [!DNL Goals] categorias de eventos. Não é possível desativar as Notificações diárias para essas categorias.

Há várias coisas que devem ser levadas em conta ao receber notificações diárias de resumo:

* Cada [!UICONTROL notificações] na sua seção **[!UICONTROL Minhas configurações]** O painel gera seu próprio email de resumo diário. Você pode ter tantos emails diários de resumo todos os dias quanto configurações de notificação ativadas para emails de resumo diários.\
   Por exemplo, se você optou por receber um email de resumo diário para várias ações no **[!UICONTROL Informações sobre projetos I] Próprio,** você recebe uma notificação por email listando todos os eventos atendidos nessa área.

* As notificações em um email de resumo diário são agrupadas por vários critérios. Por exemplo, no caso de **[!UICONTROL Informações sobre projetos possuo]**, os eventos são agrupados pelo nome do projeto.

   Para o **[!UICONTROL Comunicação]** , as notificações são agrupadas pelo objeto em que a comunicação ocorreu.

* O email de resumo diário lista os eventos que ocorreram para as ações em uma área específica (como **Informações sobre os projetos que possuo**) nas 24 horas anteriores ao horário escolhido para a entrega.
* O fuso horário do horário selecionado para o delivery de resumo diário corresponde ao fuso horário, conforme configurado no navegador.
* Os emails de resumo diário têm o nome da seção na linha de assunto, bem como a data em que são entregues.
* Pelo menos um evento deve acionar uma notificação para que o resumo diário seja entregue. Os digests diários não são enviados se nenhum evento marcado para emails de resumo diários for atendido.

### Notificação de comentários postados

As notificações na [!UICONTROL Comunicação] alerte para os comentários que foram publicados na [!UICONTROL Atualizar] fluxo de um item específico.

Emails de resumo diários para o [!UICONTROL Comunicação] são selecionadas para todas as notificações disponíveis.

As informações são resumidas para o objeto em que a comunicação ocorreu e um número total de mensagens de comunicação é exibido para cada objeto.

Para obter mais informações sobre como configurar notificações por email, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obter instruções sobre como comentar sobre [!UICONTROL Comunicação] emails, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Para saber mais sobre [!UICONTROL Comunicação] emails, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obter mais informações sobre como ativar notificações de resumo diário, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Lembretes automáticos

Os lembretes automáticos são ativados pelo seu [!DNL Workfront] administrador para alertá-lo sobre tarefas e problemas que estão vencidos, atrasados ou próximos da data de conclusão planejada. Para notificações tardias, o email é enviado noturna até que a tarefa ou o problema seja concluído. Depois que o administrador configurá-los, você não poderá desativá-los. Além disso, não é possível alterar o conteúdo ou a linha de assunto de um email acionado por um lembrete automático.

Eles podem ser enviados para um ou mais dos seguintes:

* Os usuários atribuídos a uma tarefa ou problema
* O gerente imediato do usuário
* O gerente do gerente imediato

Os emails de lembrete automático são enviados pelo endereço de email de que sua [!DNL Workfront] administrador selecionado para lidar com emails de saída.

Dependendo do lembrete automático ativado, os seguintes tipos de informações estão disponíveis no email de lembrete automático:

* A data em que a tarefa ou o problema foi criado
* Nome da tarefa ou da emissão
* O nome do projeto em que a tarefa ou emissão reside
* Descrição da tarefa ou problema
* Uma lista de usuários atribuídos à tarefa ou ocorrência
* O nome do usuário que inseriu a tarefa ou o problema
* A prioridade da tarefa ou do problema
* Data em que a tarefa ou o problema ficou vencido

Para obter informações sobre como ativar lembretes automáticos, consulte [Configurar lembretes automáticos](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Notificações de lembrete

A [!DNL Workfront] administrador (ou um usuário com uma [!UICONTROL Planejador] nível de acesso e acesso administrativo às notificações de lembrete) pode criar notificações de lembrete sobre a aproximação dos prazos e anexá-las a projetos, tarefas, problemas e folhas de ponto. Para obter mais informações sobre como obter o acesso administrativo necessário, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!IMPORTANT]
>
>Se o prazo for alterado depois que um usuário receber uma notificação de lembrete para qualquer um dos objetos mencionados acima, o usuário não receberá outra notificação de lembrete.

As notificações do lembrete são enviadas pelo endereço de email de que a variável [!DNL Workfront] administrador selecionado para lidar com emails de saída.

Para obter informações sobre como configurar e ativar notificações de lembrete, consulte [Configurar notificações de lembrete](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

### Outras [!DNL Workfront] emails

Há outros emails que você pode receber [!DNL Workfront] que não podem ser configuradas. Os emails a seguir são enviados automaticamente por [!DNL Workfront] quando estas condições forem cumpridas:

* Restaurar um item: Quando a variável [!DNL Workfront] o administrador restaura um objeto do [!UICONTROL Reciclar] Bin, um email é enviado para o [!DNL Workfront] administrador.
* Falha ao restaurar: Quando a variável [!DNL Workfront] o administrador tenta restaurar um objeto da Lixeira e a restauração falha, um email é enviado para a [!DNL Workfront] administrador.

Os emails a seguir só podem ser configurados no nível do perfil do usuário. Eles não podem ser ativados ou desativados no nível do sistema:

* Conclusão da tarefa pessoal: quando uma tarefa pessoal atribuída a outra pessoa for concluída, você receberá um email.
* Comentário adicionado ao usuário: quando alguém comenta no seu perfil de usuário, você receberá um email.

## Notificações no aplicativo

Você pode receber notificações dentro do [!DNL Workfront] aplicação web, quando determinados eventos ocorrem.

Para obter mais informações sobre notificações no aplicativo, consulte [Exibir e gerenciar notificações no aplicativo](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Notificações por email no aplicativo de email móvel

Você pode receber [!DNL Workfront] notificações por email no aplicativo de email móvel, no dispositivo móvel.

Se você tiver a variável [!DNL Workfront] O aplicativo móvel instalado no seu telefone, tocar nos links no email os abrirá no [!DNL Workfront] Aplicativo móvel. Isso inclui tocar em qualquer um dos seguintes botões de ação:

* [!UICONTROL Trabalhar na tarefa]
* [!UICONTROL Comentário]
* [!UICONTROL Tomar uma decisão quanto à aprovação]
* [!UICONTROL Ver todas as notificações]
* [!UICONTROL Adicionar]
* [!UICONTROL Começar]
* [!UICONTROL Ver mais detalhes]

Para obter mais informações sobre o [!DNL Workfront] Aplicativo para dispositivos móveis, consulte [Use o [!DNL Adobe Workfront] aplicativo móvel](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
