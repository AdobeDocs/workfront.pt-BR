---
content-type: overview;reference
navigation-topic: notifications
title: Visão geral das notificações
description: O Adobe Workfront envia notificações por email, notificações no aplicativo e notificações em seu dispositivo móvel.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 1%

---

# Visão geral das notificações

<!--Audited: 12/2023-->

O [!DNL Adobe Workfront] envia notificações por email, notificações no aplicativo e notificações no seu dispositivo móvel.

## Notificações de email

O [!DNL Workfront] envia notificações por email para alertar os usuários sobre atividades no Workfront e fornecer informações e links úteis.

Para alterar as preferências das suas notificações por email, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Se você quiser receber notificações por email do ambiente de sandbox, ative os emails do seu perfil de usuário nesse ambiente.

Você pode receber as seguintes notificações por email de [!DNL Workfront]:

* [Notificações de eventos](#event-notifications)
* [Notificações de resumo diárias](#daily-digest-notifications)
* [Notificação de comentários publicados](#notification-of-posted-comments)
* [Lembretes automáticos](#automatic-reminders)
* [Notificações de lembrete](#reminder-notifications)
* [Notificações de painéis](#boards-notifications)
* [Outros [!DNL Workfront] emails](#other-workfront-emails)

### Notificações de eventos

As notificações de eventos geralmente são acionadas por determinados eventos predefinidos, como ter uma tarefa atribuída a você ou obter uma resposta sobre um comentário feito por você.

Depois que as notificações de eventos forem ativadas no sistema [!DNL Workfront] pelo administrador ou administrador de grupo [!DNL Workfront], você poderá selecionar quais deseja receber editando suas preferências de [!UICONTROL Notificações] no perfil do usuário. Você também pode escolher se deseja receber notificações conforme os eventos ocorrem ou se deseja receber eventos resumidos em um email de resumo diário.

Você poderá ver apenas um subconjunto dessas notificações nas suas configurações, dependendo de como o administrador do [!DNL Workfront] configurou as notificações de evento para o seu sistema [!DNL Workfront]. Para obter mais informações, consulte [Configurar notificações de eventos para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

O status padrão mostra quais notificações (diárias, instantâneas ou ambas) são ativadas por padrão para novos usuários quando você cria os novos usuários.

Para obter uma lista completa das notificações de eventos e informações sobre como elas são habilitadas e configuradas no nível do sistema, do grupo ou do usuário, consulte [Notificações de eventos disponíveis em [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para obter informações sobre como escolher quais notificações de evento você deseja receber, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>As notificações de eventos são as únicas notificações que podem ser configuradas para serem entregues em atualizações de resumo diárias.

### Notificações de resumo diárias

Uma notificação de resumo diário é um email que contém todas as notificações de um determinado tipo recebidas nas 24 horas anteriores ao email.

Para obter uma lista completa de quais notificações por email foram habilitadas para uma entrega diária por email de resumo, bem como informações sobre todas as categorias de notificações por email, consulte [Notificações de eventos](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL O Workfront] não envia notificações de Resumo diário para as categorias [!UICONTROL Diversos] e [!DNL Goals] de eventos. Não é possível desativar as notificações Diárias para essas categorias.

Há vários fatores que devem ser levados em conta ao receber notificações de resumo diárias:

* Cada seção de [!UICONTROL notificações] do painel **[!UICONTROL Minhas configurações]** gera seu próprio email de resumo diário. Você pode ter quantos emails de resumo diário todos os dias quanto as configurações de notificação que estão ativadas para emails de resumo diário.\
   Por exemplo, se você optou por receber um email de resumo diário para várias ações no **[!UICONTROL Informações sobre Projetos dos quais sou proprietário]**, você receberá uma notificação por email listando todos os eventos atendidos nesta área.

* As notificações em um email de resumo diário são agrupadas por vários critérios. Por exemplo, no caso de **[!UICONTROL Informações sobre Projetos dos quais sou proprietário]**, os eventos são agrupados pelo nome do projeto.

  Para a categoria **[!UICONTROL Comunicação]**, as notificações são agrupadas pelo objeto onde a comunicação aconteceu.

  >[!NOTE]
  >
  >Na categoria Comunicação, é possível selecionar notificações individuais somente para entrega instantânea. Para que as notificações sejam entregues em um resumo diário, selecione todas elas.

* O email de resumo diário lista eventos que ocorreram para as ações em uma área específica (como **Informações sobre projetos que possuo**) nas 24 horas anteriores ao horário escolhido para a entrega.
* O fuso horário do horário selecionado para o delivery de resumo diário corresponde ao seu fuso horário, conforme configurado no navegador.
* Os emails de resumo diário têm o nome da seção na linha de assunto, bem como a data em que são entregues.
* Pelo menos um evento deve acionar uma notificação para que o resumo diário seja entregue. Os resumos diários não são enviados se nenhum evento marcado para emails de resumo diários for atendido.

### Notificação de comentários publicados

As notificações na categoria [!UICONTROL Comunicação] alertam você sobre comentários que foram postados no fluxo [!UICONTROL Atualização] de um item específico.

Os emails de resumo diários da categoria [!UICONTROL Comunicação] são selecionados para todas as notificações disponíveis.

As informações são resumidas para o objeto em que a comunicação aconteceu, e um número total de mensagens de comunicação é exibido para cada objeto.

Para responder ao comentário ou visualizá-lo no Workfront:

1. Clique no botão **[!UICONTROL Comentário]** no email.

   A área [!UICONTROL Atualizações] do objeto é aberta, com o comentário específico destacado em azul.

   Uma caixa de resposta está aberta e pode ser usada para responder ao comentário.

Para obter mais informações sobre como configurar notificações por email, incluindo como habilitar notificações de resumo diárias, consulte [Exibir e modificar suas configurações de notificação por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) em [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Lembretes automáticos

Os lembretes automáticos são habilitados pelo administrador do [!DNL Workfront] para alertá-lo sobre tarefas e problemas que estão atrasados ou próximos da data planejada de conclusão. Para notificações de atraso, o email é enviado à noite até que a tarefa ou o problema seja concluído. Depois que o administrador configurar, não será possível desabilitá-los. Além disso, não é possível alterar o conteúdo ou a linha de assunto de um email acionado por um lembrete automático.

Eles podem ser enviados para um ou mais dos itens a seguir:

* Os usuários atribuídos a uma tarefa ou problema
* O gerente imediato do usuário
* O gerente do gerente imediato

Emails de lembrete automáticos são enviados pelo endereço de email que o administrador do [!DNL Workfront] selecionou para tratar de emails enviados.

Dependendo do lembrete automático ativado, os seguintes tipos de informações estão disponíveis no email de lembrete automático:

* A data em que a tarefa ou problema foi criado
* Nome da tarefa ou problema
* O nome do projeto onde a tarefa ou problema reside
* Descrição da tarefa ou problema
* Uma lista de usuários atribuídos à tarefa ou problema
* O nome do usuário que inseriu a tarefa ou problema
* A prioridade da tarefa ou problema
* Data em que a tarefa ou o problema venceu

Para obter informações sobre como habilitar lembretes automáticos, consulte [Configurar lembretes automáticos](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Notificações de lembrete

Um administrador do [!DNL Workfront] (ou um usuário com nível de acesso de [!UICONTROL Planejador] e acesso administrativo a notificações de lembrete) pode criar notificações de lembrete sobre prazos de entrega iminentes e associá-las manualmente a projetos, tarefas, problemas e planilhas de horas.

>[!IMPORTANT]
>
>Se o prazo mudar depois que um usuário receber uma notificação de lembrete para qualquer um dos objetos mencionados acima, o usuário não receberá outra notificação de lembrete.

Notificações de lembrete são enviadas pelo endereço de email que o administrador do [!DNL Workfront] selecionou para tratar de emails de saída.

Para obter informações sobre como configurar e habilitar notificações de lembrete, consulte [Configurar notificações de lembrete](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

Para obter informações sobre como obter o acesso administrativo necessário, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### Notificações de painéis

[!DNL Adobe Workfront] [!UICONTROL Quadros] envia um email quando você é adicionado a um quadro e quando um cartão é atribuído a você. Você pode selecionar quais emails deseja receber nas preferências de Quadros.

Para obter mais informações, consulte [Notificações e preferências de email dos painéis](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Outros emails [!DNL Workfront]

Há outros emails que você pode receber de [!DNL Workfront] que não podem ser configurados.

Os emails a seguir são enviados automaticamente por [!DNL Workfront] quando estas condições são atendidas:

* Restaurar um item: Quando o administrador do [!DNL Workfront] restaura um objeto da Lixeira [!UICONTROL 2}, um email é enviado ao administrador do [!DNL Workfront].]
* Falha ao restaurar: Quando o administrador do [!DNL Workfront] tenta restaurar um objeto da Lixeira e a restauração falha, um email é enviado ao administrador do [!DNL Workfront].

Os emails a seguir podem ser configurados somente no nível do perfil do usuário. Eles não podem ser ativados ou desativados no nível do sistema:

* Conclusão da tarefa pessoal: quando uma tarefa pessoal atribuída a outra pessoa for concluída, você receberá um email.
* Comentário adicionado ao usuário: quando alguém comentar no seu perfil de usuário, você receberá um email.

## Notificações no aplicativo

Você pode receber notificações no aplicativo Web [!DNL Workfront] quando determinados eventos ocorrerem.

Para obter mais informações sobre notificações no aplicativo, consulte [Exibir e gerenciar notificações no aplicativo](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Notificações por email no aplicativo de email para dispositivos móveis

Você pode receber notificações por email de [!DNL Workfront] no seu aplicativo de email para dispositivos móveis.

Se você tiver o Aplicativo Móvel [!DNL Workfront] instalado no seu telefone, tocar nos links no email os abrirá no Aplicativo Móvel [!DNL Workfront]. Isso inclui tocar em qualquer um dos seguintes botões de ação:

* [!UICONTROL Trabalhar Nele]
* [!UICONTROL Comentário]
* [!UICONTROL Tomar uma decisão quanto à aprovação]
* [!UICONTROL Ver Todas as Notificações]
* [!UICONTROL Adicionar]
* [!UICONTROL Introdução]
* [!UICONTROL Ver Mais Detalhes]

Para obter mais informações sobre o Aplicativo Móvel [!DNL Workfront], consulte [Usar o [!DNL Adobe Workfront] aplicativo móvel](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
