---
content-type: reference
navigation-topic: notifications
title: 'Notificações: Comunicação'
description: As notificações a seguir alertam você sobre a comunicação, como um comentário atualizado, que acontece em um item de trabalho com o qual você está envolvido. Para obter informações sobre como configurar as notificações recebidas, consulte Modificar suas próprias notificações por email.
author: Courtney
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 0%

---

# Notificações: Comunicação

As notificações a seguir alertam você sobre a comunicação, como um comentário atualizado, que acontece em um item de trabalho com o qual você está envolvido. Para obter informações sobre como configurar as notificações recebidas, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Essas notificações alertam você sobre todos os comentários que foram publicados em um item específico. Por esse motivo, você deve selecionar ou desmarcar todas as notificações ao mesmo tempo para serem entregues em um email de resumo diário. Se você quiser ser notificado sobre determinados comentários somente quando ocorrerem, poderá especificar as notificações individuais para entrega instantânea.

Consulte também [Notificações de eventos](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificação</th> 
   <th> <p>Campos incluídos </p> <p> *Somente campos de resumo diários</p> </th> 
   <th>Status padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Alguém me inclui em uma atualização direcionada</strong> </p> <p>Uma atualização direcionada é quando um usuário inclui especificamente outro usuário em uma atualização, conforme descrito em <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Marcar outros usuários em] atualizações</a>.</p> <p>Nesse caso, o usuário incluído na atualização direcionada recebe uma notificação por email sobre a atualização.</p> <p>A notificação por email é enviada somente se o usuário tiver direitos de acesso ao objeto.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;Nome do usuário que o incluiu na atualização&gt; [!UICONTROL deseja que você saiba]</em></p> <p>O assunto da notificação de resumo diário é: <em>[!UICONTROL Resumo da Comunicação] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Objeto onde a atualização foi feita<br>Nome do Objeto Pai<br>Número de Referência do Objeto<br>Nomes de todos os usuários e equipes incluídos na atualização direcionada<br>Data e Hora em que a atualização foi feita<br>Texto da atualização direcionada<br><strong>[!UICONTROL Comentário]</strong> botão<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada objeto<br>*<strong>[!UICONTROL Ver Todas as Notificações]</strong> botão<br>*Data do resumo diário<br></td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém respondeu à minha solicitação</strong> </p> <p>Depois que um usuário envia uma solicitação de trabalho e outro usuário responde a ela, o usuário que enviou a solicitação recebe uma notificação por email.</p> <p>Uma notificação por e-mail não será enviada se:</p> 
    <ul> 
     <li> <p>O usuário que responde é o mesmo usuário que fez a solicitação</p> </li> 
     <li> <p>O usuário não tem acesso para ver a nota</p> </li> 
    </ul><strong>O assunto do email de notificação instantânea é: <em>[!UICONTROL Comentário sobre] &lt;Nome da Solicitação&gt; em &lt;Nome do Projeto&gt; (ref# &lt;Número de Referência da Solicitação&gt;)</em></strong> O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Comunicação] &lt;Data do resumo diário&gt;</em></td> 
   <td> Nome da Solicitação<br>Nome do projeto<br>Número de Referência<br>Nome do usuário que respondeu à sua Solicitação<br>Data e Hora em que o comentário foi feito<br>Texto do comentário feito na sua Solicitação<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada solicitação<br>*<strong>[!UICONTROL Ver Todas as Notificações]</strong> botão<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um comentário foi postado em minha solicitação</strong> </p> <p>O contato principal de um problema recebe uma notificação por email quando um comentário é postado em uma solicitação do [!UICONTROL Help Desk], a menos que o usuário que postou o comentário também seja o contato principal do problema.</p> <p>Todos os usuários incluídos diretamente no comentário também recebem uma notificação por email.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Comentário sobre] &lt;Nome da Solicitação&gt; em &lt;Nome do Projeto&gt; (ref# &lt;Número de Referência da Solicitação&gt;)</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Comunicação] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome da Solicitação<br>Nome do projeto<br>Número de Referência<br>Nome do usuário que respondeu à sua Solicitação<br>Data e Hora em que o comentário foi feito<br>Texto do comentário feito na sua Solicitação<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada solicitação<br>*Nome do Projeto<br>*<strong>[!UICONTROL Ver Todas as Notificações]</strong>*Data do resumo diário<br><br></td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um comentário foi adicionado ao meu documento</strong> </p> <p>O proprietário de um documento no [!DNL Adobe Workfront] recebe uma notificação por email quando um comentário é postado no documento, a menos que o usuário que postou o comentário também seja o proprietário do documento.</p> <p>Todos os usuários incluídos diretamente no comentário também recebem uma notificação por email.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual]. </p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Comentário sobre] &lt;Nome da Solicitação&gt; em &lt;Nome do Projeto&gt; (ref# &lt;Número de Referência da Solicitação&gt;)</em></p> <p> O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Comunicação] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td>Nome do Documento<br>Nome do Projeto, Tarefa ou Problema<br>Número de Referência<br>Nome do usuário que respondeu à sua Solicitação<br>Data e Hora em que o comentário foi feito<br>Texto do comentário feito no documento</td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando alguém comentar em um thread, eu estarei</strong> </p> <p>Os participantes da thread e os usuários incluídos em uma mensagem direta recebem uma notificação por email quando um usuário faz um comentário na thread.</p> <p>Os usuários devem ter acesso à [!UICONTROL View] para receber uma notificação.</p> <p>Os seguintes usuários não recebem uma notificação:</p> 
    <ul> 
     <li>Equipes incluídas em uma mensagem direta</li> 
     <li>O proprietário da Nota</li> 
     <li>O contato primário</li> 
    </ul> <p><strong>O assunto do email de notificação instantânea é: <em>[!UICONTROL RE: Comentar em] &lt;Nome do Objeto&gt;&lt;Tipo de Objeto&gt; em &lt;Nome do Projeto&gt;(ref# &lt;Número de Referência do Objeto&gt;</em>)</strong> </p> <p><strong> O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Comunicação] &lt;Data do resumo diário&gt;</em></strong> </p> </td> 
   <td> Nome do Objeto<br>Nome do Objeto Pai<br>Nome do usuário que comentou o thread<br>Texto do comentário feito no thread<br>Data e Hora em que o comentário foi feito<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada objeto<br>*Nome do Projeto<br>*<strong>[!UICONTROL Ver Todas as Notificações]</strong> botão<br>*Data do resumo diário </td> 
   <td><strong>[!UICONTROL Diário]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém comentou um dos meus itens de trabalho</strong> </p> <p>O destinatário do item de trabalho recebe uma notificação por email sempre que um usuário adiciona uma atualização a um item de trabalho, a menos que o usuário que adiciona a atualização também seja o destinatário. </p> <p>Quando um comentário for postado em uma solicitação, envie um email para o contato principal do problema.</p> <p>O contato principal de um problema recebe uma notificação por email quando um comentário é postado em uma solicitação, a menos que o usuário que postou o comentário também seja o contato principal do problema.</p> <p>Todos os usuários incluídos diretamente no comentário também recebem uma notificação por email.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Comentário sobre] &lt;Nome do Item de Trabalho&gt; em &lt;Nome do Projeto (ref# &lt;Número de Referência do Item de Trabalho&gt;)</em></p> <p> O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Comunicação] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Item de Trabalho<br>Nome do Projeto<br>Número de Referência do Item de Trabalho<br>Nome do usuário que comentou o Item de Trabalho<br>Texto do comentário feito no Item de Trabalho<br>Data e Hora em que o comentário foi feito<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada objeto<br>*Nome do Projeto<br>*<strong>[!UICONTROL Ver Todas as Notificações]</strong>*Data do resumo diário<br> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém tiver incluído minha equipe em uma atualização direta</strong> </p> <p>Uma atualização direcionada é quando um usuário inclui especificamente outro usuário em uma atualização, conforme descrito em <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Marcar outros usuários em atualizações</a>.</p> <p>Nesse caso, qualquer membro da equipe incluída na atualização direcionada receberá uma notificação por email sobre a atualização.</p> <p>A notificação por email é enviada somente para usuários que têm direitos de acesso ao objeto.</p> <p>Se o usuário que envia a atualização direcionada for um membro da equipe que está sendo incluída, o usuário que envia a atualização não receberá uma notificação por email.</p> <p>O assunto do email de notificação instantânea é: [!UICONTROL Comentário sobre] &lt;Nome do objeto&gt; em &lt;Nome do objeto pai&gt; (ref# &lt;Número de referência do objeto&gt;)</p> <p> O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Comunicação] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> <p>Nome do Objeto<br>Nome do Objeto Pai<br>Número de Referência do Objeto<br>Nome do usuário que fez a atualização direcionada<br>Nome de todas as equipes e usuários incluídos na atualização direcionada<br>Data e Hora em que a atualização direcionada foi feita<br>Texto da atualização direcionada<br><strong>[!UICONTROL Comentário]</strong> botão<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada objeto<br>*Nome do Projeto<br>*<strong>[!UICONTROL Ver Todas as Notificações]</strong> botão<br>*Data do resumo diário </p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando o comentário for adicionado ao usuário</strong> </p> <p>Você pode fazer um comentário sobre um usuário na guia [!UICONTROL Atualizações] do objeto do usuário. Você também pode fazer um comentário em um usuário quando estiver editando as configurações do usuário. O usuário contra o qual o comentário é feito recebe um email para notificá-lo desse comentário. </p> <p>Você deve ter permissões para pelo menos [!UICONTROL Exibir] o usuário para inserir uma atualização na guia [!UICONTROL Atualizações] do usuário. Você deve ter permissões de [!UICONTROL Editar] no usuário para editar as configurações do usuário. </p> <p>Para obter mais informações sobre como fazer comentários sobre usuários na guia Atualizações, consulte <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Trabalho de atualização</a>.</p> <p>Para obter mais informações sobre como inserir um comentário em um usuário ao editar as configurações do usuário, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurar minhas configurações</a>.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;Nome de Usuário&gt; [!UICONTROL deseja que você saiba]</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Comunicação] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Seu Nome de Usuário<br>Nome do usuário que adicionou o comentário<br>Texto do comentário<br>Data e Hora em que o comentário foi feito<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada objeto<br>*<strong>[!UICONTROL Ver Todas as Notificações]</strong> botão<br>*Data do resumo diário </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
