---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Tipos de Notificação de Eventos
description: As notificações de eventos são emails acionados por vários tipos de eventos em objetos, como projetos, tarefas e problemas. Este artigo lista e descreve os tipos disponíveis de notificações de eventos.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '5237'
ht-degree: 7%

---

# Tipos de notificação de evento

<!-- Audited: 1/2024 -->

As notificações de eventos são emails acionados por vários tipos de eventos em objetos, como projetos, tarefas e problemas, conforme explicado em [Notificações de eventos](../../../workfront-basics/using-notifications/event-notifications.md).

Essas notificações podem ser configuradas no nível do sistema e do grupo:

* Para obter informações sobre como configurar notificações de eventos no nível do sistema, consulte [Configurar notificações de eventos para todos no sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Para obter informações sobre como configurar notificações de evento no nível do grupo, consulte [Exibir e configurar notificações de evento para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Usuários individuais também podem ativar e desativar notificações de evento individuais em seus perfis individuais. Para obter mais informações, consulte [Modificar suas próprias notificações por email](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

As tabelas a seguir listam todas as notificações de eventos do Adobe Workfront, uma breve descrição do evento e se o evento está ativo ou inativo por padrão.

>[!NOTE]
>
>As notificações com um valor &quot;Ativo&quot; na coluna Estado padrão estão ativas para notificações instantâneas e diárias por padrão, a menos que observado de outra forma.

## Ação necessária

Consulte também [Notificações: ação necessária](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th>Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Usuário</p> </td> 
   <td> <p>Solicitação de Acesso</p> </td> 
   <td> <p>Usuário</p> </td> 
   <td> <p>Someone requests access from me.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> <p> </p> </td> 
   <td> <p>Document Request Add</p> </td> 
   <td> <p>Usuário ao qual o documento é solicitado</p> </td> 
   <td> <p>Alguém solicitou que eu carregue documento(s).</p> <p>O Solicitante de documentos recebe uma notificação por email quando recebe uma solicitação para carregar um documento.</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Document pending approval</p> </td> 
   <td> <p>Aprovadores</p> </td> 
   <td> <p>Preciso aprovar um documento.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Atribuição de problema</p> </td> 
   <td> <p>Usuário ao qual o problema está atribuído</p> </td> 
   <td> <p>Quando um problema for atribuída, enviar email para o usuário atribuído.</p> <p>O destinatário da ocorrência recebe uma notificação por email somente se o status do projeto for Atual e o status da ocorrência não for Fechado ou algo que equivale a Fechado.</p> <p>Os usuários com uma licença Light, Contributor, Review ou Request não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problemas Pendentes de Aprovação</p> </td> 
   <td> <p>Aprovadores</p> </td> 
   <td> <p>Preciso aprovar um problema.</p> <p>A definição de quais usuários receberão uma notificação por email para este evento dependerá se a configuração "Aprovador não precisa estar na equipe do projeto (para processos de aprovação que incluem uma função)" está habilitada (conforme descrito em <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação globais</a>). </p> <p>Se esta opção estiver habilitada</strong>, uma notificação por email será enviada a todos os usuários no sistema com a Função de Trabalho "Aprovador".</p> <p>Se esta opção estiver desabilitada</strong>, somente membros da equipe do projeto com a Função de Trabalho "Aprovador" receberão uma notificação por email.</p> <p>Uma notificação é enviada se o projeto estiver no status Planejamento ou Atual. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problemas Pendentes de Aprovação</p> </td> 
   <td> <p>Aprovador delegado</p> </td> 
   <td> <p>Preciso revisar uma aprovação de ocorrência que foi delegada.</p> <p>When someone delegates an issue approval to another user, that user is notified. </p> <p>A notification is sent only when the project is in the Current status.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Projeto Pendente de Aprovação</p> </td> 
   <td> <p>Aprovadores</p> </td> 
   <td> <p>Preciso aprovar um projeto.</p> <p>A definição de quais usuários receberão uma notificação por email para este evento dependerá se a configuração "Aprovador não precisa estar na equipe do projeto (para processos de aprovação que incluem uma função de trabalho)" está habilitada (conforme descrito em <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação globais</a>).</p> <p>Se esta opção estiver habilitada</strong>, uma notificação por email será enviada a todos os usuários no sistema com a Função de Trabalho "Aprovador".</p> <p>Se esta opção estiver desabilitada</strong>, somente membros da equipe do projeto com a Função de Trabalho "Aprovador" receberão uma notificação por email.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>Projeto Pendente de Aprovação</td> 
   <td>Aprovador delegado</td> 
   <td> <p>Preciso revisar uma aprovação de projeto à qual fui delegado.</p> </td> 
   <td> Ativo</td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Atribuição de tarefa</p> </td> 
   <td> <p>Usuário ao qual a tarefa está atribuída</p> </td> 
   <td> <p>Quando uma atribuição primária de uma tarefa for alterada, enviar email para o usuário mais recente atribuído.</p> <p>O Destinatário da tarefa receberá uma notificação por e-mail se for o principal destinatário da tarefa, a menos que o destinatário seja o usuário que fez a atribuição.</p> <p>Uma notificação será enviada se o status do projeto for Atual e a tarefa não estiver marcada como Concluída.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Pendência de Aprovação de Tarefa</p> </td> 
   <td> <p>Aprovadores</p> </td> 
   <td> <p>Preciso aprovar uma tarefa.</p> <p>Which users receive an email notification for this event depends on whether the "Approver not required to be on the project team (for approval processes that include a role)" setting is enabled (as described in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configure global approval settings</a>). </p> <p>If this option is enabled</strong>, an email notification is sent to all users in the system with the "Approver" Job Role.</p> <p>If this option is disabled</strong>, only project team members with the "Approver" Job Role receive an email notification.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual no momento da solicitação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Pendência de Aprovação de Tarefa</p> </td> 
   <td> <p>Aprovador delegado</p> </td> 
   <td> <p>I need to review a task approval I've been delegated.</p> <p>When someone delegates an issue approval to another user, that user is notified. </p> <p>A notification is sent only if the project status is Current at the time of the request.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Folha de horas</p> </td> 
   <td> <p>Planilha de horas reaberta</p> </td> 
   <td> <p>Usuário ao qual a folha de horas pertence</p> </td> 
   <td> <p>Minha planilha de horas foi reaberta.</p> <p>O Proprietário da folha de horas recebe uma notificação por email quando a folha de horas é reaberta, a menos que o usuário que a reabriu também seja o proprietário da folha de horas.</p> <p>Uma notificação por email é enviada somente se o status da folha de horas for Aberto.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Folha de horas</p> </td> 
   <td> <p>Timesheet Rejection</p> </td> 
   <td> <p>Usuário ao qual o quadro de horários pertence</p> </td> 
   <td> <p>Minha folha de ponto foi rejeitada.</p> <p>O Proprietário da folha de horas recebe uma notificação por email quando a folha de horas é rejeitada, a menos que o usuário que a rejeitou também seja o proprietário.</p> <p>Uma notificação por e-mail será enviada somente se o status da folha de horas for Rejeitada.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Folha de horas</p> </td> 
   <td> <p>Envio de Quadro de Horários</p> </td> 
   <td> <p>Aprovador</p> </td> 
   <td> <p>Preciso aprovar um quadro de horários.</p> <p>The Timesheet Approver receives an email notification when a timesheet that they need to approve is submitted, unless the user who submitted the timesheet is also the Timesheet Approver.</p> <p>A notification is sent only if the status of the timesheet is Submitted.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Atribuição</p> </td> 
   <td> <p>Solicitação de Item de Trabalho</p> </td> 
   <td> <p>Membros da equipe para a qual o item é solicitado</p> </td> 
   <td> <p>Minha equipe recebe uma nova solicitação de trabalho.</p> <p>Os membros da equipe recebem uma notificação por e-mail quando a equipe recebe uma nova solicitação de trabalho. (O usuário que enviou a solicitação não recebe uma notificação se for membro da equipe.)</p> <p>Uma notificação é enviada somente se o status do projeto for Atual no momento em que a Solicitação de trabalho é feita e o status da Solicitação de trabalho for Novo.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Atribuição</p> </td> 
   <td> <p>Solicitação de Item de Trabalho</p> </td> 
   <td> <p>Usuário para o qual o item de trabalho é solicitado</p> </td> 
   <td> <p>Recebo uma nova solicitação de trabalho.</p> <p>O destinatário do item de trabalho recebe uma notificação por email, a menos que o usuário que está fazendo a solicitação também seja o destinatário. </p> <p>Uma notificação não será enviada se o status da tarefa for Concluído ou se o status da ocorrência for Fechado.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual no momento da solicitação.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solicitações que eu fiz

Consulte também [Notificações: solicitações que fiz](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Document Approval Status Change</p> </td> 
   <td> <p>Solicitante</p> </td> 
   <td> <p>A document approval request is completed.</p> <p>O Solicitante de documentos recebe uma notificação por email quando a solicitação de aprovação de documentos é concluída.</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Solicitação de Documento Concluída</p> </td> 
   <td> <p>Solicitante</p> </td> 
   <td> <p>Uma solicitação de carregamento de documento foi atendida.</p> <p>O Solicitante de documentos recebe uma notificação por email quando uma solicitação para carregar um documento é atendida.</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema adicionado</p> </td> 
   <td> <p>Originador do problema</p> </td> 
   <td> <p>Eu adiciono um problema a um projeto.</p> <p>O contato principal em um problema recebe uma notificação quando adiciona um problema em um projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>Issue Assignment</td> 
   <td>Issue Primary Contact</td> 
   <td> <p>Someone is assigned to an issue for which I'm the primary contact.</p> <p>O contato principal em uma ocorrência recebe uma notificação quando a ocorrência é atribuída a um usuário. </p> <p>Uma notificação será enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> Inativo</td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Conclusão do problema</p> </td> 
   <td> <p>Contato Principal do Problema</p> </td> 
   <td> <p>Uma ocorrência para a qual eu sou o contato principal foi concluída.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Alteração de Status do Projeto</p> </td> 
   <td> <p>User that created project (Entered By)</p> </td> 
   <td> <p>The status changes on a project I created.</p> <p>The user who created the project receives an email notification when the project status changes.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Adicionar solicitação</p> </td> 
   <td> <p>Originador do problema</p> </td> 
   <td> <p>Eu envio uma solicitação (confirmação).</p> <p>O contato principal sobre o problema recebe uma notificação por email quando envia um problema.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto estiver usando uma Visualização "Is Help Desk".</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Solicitar atribuição</p> </td> 
   <td> <p>Contato Principal do Problema</p> </td> 
   <td> <p>Alguém foi atribuído à minha solicitação.</p> <p>O contato principal da ocorrência recebe uma notificação por email quando um usuário é atribuído à ocorrência, a menos que o contato principal e o usuário atribuído sejam o mesmo usuário.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto estiver usando uma Visualização "Is Help Desk".</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Solicitação fechada</p> </td> 
   <td> <p>Originador do problema</p> </td> 
   <td> <p>Minha solicitação foi fechada (confirmação).</p> <p>O contato principal do problema recebe uma notificação por email quando a solicitação é fechada.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto estiver usando uma Visualização "Is Help Desk".</p> <p>If the notifications for "issue completion" are enabled, they will always trigger instead of the "Request closed to Issue Primary Contact." If you want this notification to trigger, you must deactivate the "issue completion" notifications.</p> </td> 
   <td> <p>Active (Instant only)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Request Document Add</p> </td> 
   <td> <p>Contato Principal do Problema</p> </td> 
   <td> <p>A document is changed or uploaded on an issue for which I am the primary contact.</p> <p>The issue's primary contact receives an email notification when a document is uploaded or changed on the issue, unless the user who uploaded or changed the document is also the primary contact.</p> <p>A notification is sent only if the project status is Current and if the project has the "Publish as Help Request Queue" enabled on the Queue Setup tab.</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Solicitar mudança de status</p> </td> 
   <td> <p>Originador do problema</p> </td> 
   <td> <p>O status muda conforme minha solicitação.</p> <p>O contato principal do problema recebe uma notificação por email quando o status do problema é alterado, a menos que o usuário que alterou o status também seja o contato principal.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e o projeto estiver usando uma Visualização "Is Help Desk".</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE:
       For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.-->

## Comunicação

Consulte também [Notificações: Comunicação](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th> Default state</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Comment on Document</p> </td> 
   <td> <p>Proprietário do Documento</p> </td> 
   <td> <p>Um comentário é adicionado ao meu documento.</p> <p>O proprietário de um documento no Workfront recebe uma notificação por email quando um comentário é postado no documento, a menos que o usuário que postou o comentário também seja o proprietário do documento.</p> <p>Todos os usuários incluídos diretamente no comentário também recebem uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual. </p> <p>O assunto do email de notificação instantânea é: <em>Comentário em &lt;Nome da Solicitação&gt; em &lt;Nome do Projeto&gt; (ref# &lt;Número de Referência da Solicitação&gt;)</em></p> <p> O assunto da notificação de resumo diário é:<em> Resumo da Comunicação &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Request Note Add</p> </td> 
   <td> <p>Contato Principal do Problema</p> </td> 
   <td> <p>When a comment is posted on a request, email the issue primary contact.</p> <p>The primary contact for an issue receives an email notification when a comment is posted on a request, unless the user who posted the comment is also the primary contact for the issue.</p> <p>Any users who are directly included on the comment also receive an email notification.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário</p> </td> 
   <td>Atualização direcionada</td> 
   <td>Usuário</td> 
   <td> <p>Alguém tiver me incluído em uma atualização direta.</p> <p>Uma atualização direcionada é quando um usuário inclui especificamente outro usuário em uma atualização, conforme descrito em <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Marcar outros usuários em atualizações</a>.</p> <p>Nesse caso, o usuário incluído na atualização direcionada recebe uma notificação por email sobre a atualização.</p> <p>A notificação por email é enviada somente se o usuário tiver direitos de acesso ao objeto e se ele a mantiver ativada em seu perfil.  </p> <p>Essa notificação de eventos é ativada por padrão e não pode ser desativada.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Equipe</p> </td> 
   <td> <p>Directed Update</p> </td> 
   <td> <p>Membros da equipe</p> </td> 
   <td> <p>Alguém tiver incluído minha equipe em uma atualização direta.</p> <p>A directed update is when a user specifically includes another user in an update, as described in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p> <p>In this case, any member of the team that is included in the directed update receives an email notification about the update.</p> <p>The email notification is sent only to users who have access rights to the object of the update.</p> <p>If the user sending the directed update is a member of the team being included, the user sending the update does not receive an email notification.</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Work Item Comment</p> </td> 
   <td> <p>Thread Participants</p> </td> 
   <td> <p>Someone comments on a thread I'm in.</p> <p>Participants in the thread and users who are included in a direct message receive an email notification when a user makes a comment in the thread.</p> <p>Users must have View access to receive a notification.</p> <p>The following users do not receive a notification:</p> 
    <ul> 
     <li> <p>Teams that are included in a direct message</p> </li> 
     <li> <p>The owner of the Note</p> </li> 
     <li> <p>The Primary Contact</p> </li> 
    </ul> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Comentário do Item de Trabalho</p> </td> 
   <td> <p>Destinatário do item de trabalho</p> </td> 
   <td> <p>Quando alguém comentar em um dos meus itens de trabalho, envie email para os atribuídos.</p> <p>O destinatário do item de trabalho recebe uma notificação por email sempre que um usuário adiciona uma atualização a um item de trabalho, a menos que o usuário que adiciona a atualização também seja o destinatário.</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Resposta à requisição de trabalho</p> </td> 
   <td> <p> Solicitante do trabalho</p> </td> 
   <td> <p>Alguém responde ao meu pedido.</p> <p>Depois que um usuário envia uma solicitação e outro usuário responde, o usuário que enviou a solicitação recebe uma notificação por email.</p> <p>Uma notificação por e-mail não será enviada se:</p> 
    <ul> 
     <li> <p>O usuário que responde é o mesmo usuário que fez a solicitação</p> </li> 
     <li> <p>O usuário não tem acesso para ver a nota</p> </li> 
    </ul> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## Informações de aprovação

Consulte também [Notificações: Informações de aprovação](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Usuário</p> </td> 
   <td> <p>Delegação de aprovações</p> </td> 
   <td> <p>Usuário</p> </td> 
   <td> <p>I'm delegated as an approver.</p> </td> 
   <td> <p>Active (Instant only)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Mudança de status de aprovação de problema delegada</p> </td> 
   <td> <p>Usuário que delegou a aprovação</p> </td> 
   <td> <p>Uma solicitação de aprovação de problema foi concluída. </p> <p>Quando você delega uma aprovação de problema a outra pessoa, você recebe uma notificação por email quando ela conclui essa aprovação (se ela aprova ou rejeita a aprovação do problema). </p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Mudança de status de aprovação de projeto delegada</p> </td> 
   <td> <p>Usuário que delegou a aprovação</p> </td> 
   <td> <p>Uma solicitação de aprovação de projeto foi concluída.</p> <p>Quando você delega uma aprovação de projeto a outra pessoa, você recebe uma notificação por email quando ela conclui essa aprovação (se ela aprova ou rejeita a aprovação do projeto).</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Mudança de status de aprovação de tarefa delegada</p> </td> 
   <td> <p>Usuário que delegou a aprovação</p> </td> 
   <td> <p>Um status de aprovação de tarefa foi concluído.</p> <p>Quando você delega uma aprovação de tarefa a outra pessoa, você recebe uma notificação por email quando ela conclui essa aprovação (se ela aprova ou rejeita a aprovação da tarefa).</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Cancelar aprovação de documento para o aprovador</p> </td> 
   <td> <p>Usuário que delegou a aprovação</p> </td> 
   <td> <p>A document approval request is canceled.</p> <p>The Document Approver of the document receives an email notification when the document approval request is canceled.</p> </td> 
   <td> <p>Active (Instant only)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Folha de horas</p> </td> 
   <td> <p>Timesheet Approval</p> </td> 
   <td> <p>User that timesheet belongs to</p> </td> 
   <td> <p>My timesheet is approved.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Information about work assigned to me

See also [Notifications: Information about work assigned to me](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Tarefa</td> 
   <td>Conclusão de todas as tarefas predecessoras</td> 
   <td>Membros da equipe atribuídos a tarefas dependentes</td> 
   <td> <p>Todos os predecessores das tarefas da equipe são concluídos.</p> <p>Os atribuídos à tarefa (todos os membros da equipe) recebem uma notificação por email.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td>Inativo</td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Conclusão de todas as tarefas predecessoras</p> </td> 
   <td> <p>Usuário atribuído a tarefas dependentes</p> </td> 
   <td> <p>All predecessors of my tasks are completed.</p> <p>The task assignee receives an email notification.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Decisão de aprovação</p> </td> 
   <td> <p>Usuário ao qual a ocorrência está atribuída</p> </td> 
   <td> <p>Um problema que resolvo é aprovado ou rejeitado.</p> <p>O destinatário de uma ocorrência recebe uma notificação por email quando uma decisão de aprovação é tomada (aprovada ou rejeitada).</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Decisão de aprovação</p> </td> 
   <td> <p>Usuário ao qual a tarefa está atribuída</p> </td> 
   <td> <p>Uma tarefa concluída é aprovada ou rejeitada.</p> <p>O destinatário da tarefa recebe uma notificação por e-mail quando a tarefa é aprovada ou rejeitada.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Issue Completion</p> </td> 
   <td> <p>Usuário ao qual o problema está atribuído</p> </td> 
   <td> <p>Quando um problema for concluído enviar email para o usuário atribuído.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>A data de conclusão planejada do problema mudou</p> </td> 
   <td> <p>Usuário ao qual o problema está atribuído</p> </td> 
   <td> <p>A data de conclusão de um problema atribuído a mim mudou.</p> <p>O destinatário do problema recebe uma notificação por email quando a Data de conclusão planejada é alterada, a menos que o usuário que alterou a Data de conclusão planejada também seja o destinatário.</p> <p>A notification is sent only if the project status is anything other than Planning.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Issue Status Change</p> </td> 
   <td> <p>Usuário ao qual o problema está atribuído</p> </td> 
   <td> <p>The status changes on one of my work items.</p> <p>The assignee of the issue receives an email notification when the status changes, unless the user who changed the status is also the assignee.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Request Document Add</p> </td> 
   <td> <p>Usuário ao qual a ocorrência está atribuída</p> </td> 
   <td> <p>Documents are uploaded or changed on requests I'm assigned to.</p> <p>The issue assignee receives an email notification when documents are uploaded or changed on an issue they added.</p> <p>An email notification is not sent if the user who entered the issue is the issue assignee.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual e se o projeto tiver a opção "Publicar como Fila de solicitação de ajuda" ativada na guia Configuração da fila.</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Conclusão da tarefa</p> </td> 
   <td> <p>Usuário ao qual a tarefa está atribuída</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para o usuário atribuído</p> <p>O Destinatário da tarefa recebe uma notificação por e-mail quando a tarefa é concluída. As notificações não são enviadas quando uma tarefa pessoal é concluída.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença Light, Contributor, Review ou Requestor não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Conclusão da tarefa</p> </td> 
   <td> <p>Usuário atribuído à tarefa dependente</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para os usuários atribuídos primariamente de todas as tarefas dependentes</p> <p>O destinatário da tarefa recebe uma notificação por e-mail quando um de seus predecessores tiver sido concluído.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>A data de conclusão planejada da tarefa mudou</p> </td> 
   <td> <p>Usuário ao qual a tarefa está atribuída</p> </td> 
   <td> <p>A data de vencimento é alterada em uma tarefa à qual estou atribuído.</p> <p>O Designado da Tarefa recebe uma notificação por e-mail quando a Data de Conclusão Planejada da tarefa é alterada, a menos que o usuário que alterou a Data de Conclusão Planejada também seja o Designado da Tarefa.</p> <p>Uma notificação será enviada somente se o status do projeto for algo diferente de Planejamento.</p> <p>Nenhuma notificação é enviada sobre tarefas pessoais.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Mudança do status da tarefa</p> </td> 
   <td> <p>Usuário ao qual a tarefa está atribuída</p> </td> 
   <td> <p>O status muda em uma tarefa à qual estou atribuído.</p> <p>O Destinatário da tarefa recebe uma notificação por e-mail quando o status da tarefa é alterado, a menos que o usuário que alterou o status também seja o destinatário.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## Information about projects I&#39;m on

Consulte também [Notificações: Informações sobre projetos em que estou](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th> Default state</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Current Project Status</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando uma status de projeto for alterada de ideia/aprovado/solicitado/em planejamento para atual, enviar email para a equipe.</p> <p>Users on the project receive an email notification when the project becomes active.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Document Add</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>A document is added to a project I'm on.</p> <p>Users on the project team receive an email notification when a document is added to the project, except for the user who added the document.</p> <p>A notification is sent only if the project status is Current and the document is not Private. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema Adicionar</p> </td> 
   <td> <p>Membros da equipe de projeto</p> </td> 
   <td> <p>An issue is added to a project I'm on.</p> <p>Users in a project receive an email notification when an issue is added to the project.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Conclusão do problema</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando um problema for concluído enviar email para a equipe.</p> <p>Qualquer usuário no projeto recebe uma notificação.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Término de etapa</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando uma etapa for concluída, enviar email para a equipe.</p> <p>Todos os usuários da Equipe do projeto recebem uma notificação quando uma tarefa de etapa é concluída. </p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Conclusão do projeto</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando um projeto for concluído, enviar email para a equipe.</p> <p>Os usuários de uma equipe de projeto recebem uma notificação por email quando o status do projeto é Concluído.</p> <p>Dica: se os projetos forem concluídos regularmente, ativar essa opção pode criar muitos emails para usuários com um número limitado de tarefas em muitos projetos. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Alteração de Status do Projeto</p> </td> 
   <td> <p>Membros da equipe de projeto</p> </td> 
   <td> <p>Quando uma status de projeto for alterado, enviar email para a equipe.</p> <p>Os usuários na equipe do projeto recebem uma notificação por email quando o status do projeto é alterado. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
     <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Status Atual do Projeto</p> </td> 
   <td> <p>Membros da equipe atribuída</p> </td> 
   <td> <p>Um projeto em que minha equipe se torna ativa.</p> <p>Os membros de uma equipe atribuída do Workfront recebem uma notificação por email quando o projeto atribuído para eles se tornarem ativos.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário de projeto</p> </td> 
   <td> <p>Adição de Usuário de Projeto</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando um usuário for adicionado à equipe, enviar email para o usuário.</p> <p>O usuário que foi adicionado ao projeto recebe uma notificação por email quando é adicionado, a menos que o usuário tenha sido adicionado automaticamente ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Task Completion</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para a equipe.</p> <p>Members of the project team receive an email notification.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Unassigned Issue Added</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando um problema não atribuída for adicionada enviar email para a equipe.</p> <p>Os usuários em um projeto recebem uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informações sobre projetos dos quais sou proprietário

See also [Notifications: Information about projects I own](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Adicionar documento</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>A document is added to a project I own.</p> <p>The Project Owner receives an email notification when a document is added to the project, unless the user who added the document is also the Project Owner.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e o documento não for Privado.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema adicionado</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>Quando um problema for adicionada enviar email para o proprietário do projeto.</p> <p>O proprietário do projeto recebe uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Mudança da data de compromisso do problema</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>Mudança da data de compromisso de um problema em um dos meus projetos.</p> <p>O Proprietário do projeto recebe uma notificação por email quando a Data de confirmação é alterada para um problema no projeto, a menos que o usuário que altera a Data de confirmação seja o mesmo usuário que o Proprietário do projeto.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Conclusão do problema</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>Quando um problema for concluído enviar email para a equipe.</p> <p>O proprietário do projeto recebe uma notificação por email.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Conclusão de Tarefas de Marco</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>Quando uma etapa for concluída, enviar email para o proprietário do projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Atribuição do Proprietário do Projeto</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>Quando o proprietário do projeto mudar ou na criação do projeto, enviar email para o usuário recentemente atribuído</p> <p>Quando um usuário é atribuído como proprietário de um projeto, ele recebe uma notificação por email.</p> <p>Se o proprietário do projeto for o mesmo usuário que fez a atribuição, uma notificação por email não será enviada</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Alteração de Progresso do Projeto</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>Quando um projeto for alterado de uma status positiva de progresso (no prazo) para uma status negativa de progresso (em atraso), enviar email para o proprietário do projeto.</p> <p>O proprietário do projeto recebe uma notificação por email quando o projeto está atrasado.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Mudança da data de compromisso da tarefa</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>A data de compromisso de uma tarefa em um dos meus projetos mudou.</p> <p>O Proprietário do projeto recebe uma notificação por email quando a Data de confirmação é alterada para uma tarefa no projeto, a menos que o usuário que alterou a Data de confirmação também seja o Proprietário do projeto.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Conclusão de tarefas</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para o proprietário do projeto.</p> <p>O proprietário do projeto recebe uma notificação. </p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Alteração do Progresso da Tarefa</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>Quando uma tarefa for alterada de uma status de progresso positivo (no prazo) para uma status de progresso negativo (em atraso), enviar email para o proprietário da tarefa.</p> <p>O Proprietário do projeto recebe uma notificação por email quando uma tarefa no projeto atrasa o agendamento.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Adicionar Problema Não Atribuída</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>Quando um problema não atribuída for adicionada enviar email para o proprietário do projeto.</p> <p>O proprietário do projeto recebe uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informações sobre projetos que eu patrociono

Consulte também [Notificações: Informações sobre projetos que eu patrociono](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Adicionar documento</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>Um documento é adicionado a um projeto que eu patrociono.</p> <p>The Project Sponsor receives an email notification when a document is added to the project, unless the document is added by the Project Sponsor.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual e se o documento não for Privado.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema Adicionar</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>Quando um problema for adicionada enviar email para o patrocinador do projeto.</p> <p>O patrocinador do projeto recebe uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Conclusão do Problema</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>Uma ocorrência foi concluída em um projeto que eu patrocinei.</p> <p>O patrocinador do projeto recebe uma notificação por email.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Término de etapa</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>Quando uma etapa for concluída, enviar email para o patrocinador do projeto.</p> <p>O Patrocinador do projeto recebe uma notificação por email quando uma tarefa de etapa é concluída em um projeto que ele patrocina.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Alteração de Progresso do Projeto</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>A project I sponsor gets behind.</p> <p>The Project Sponsor receives an email notification when the project gets behind schedule.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Atribuição do Patrocinador do Projeto</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>Quando um patrocinador de projeto mudar ou na criação do projeto, enviar email para o patrocinador do projeto.</p> <p>The project sponsor receives an email notification when they are set as the sponsor of a project.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Conclusão de tarefas</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para o patrocinador do projeto.</p> <p>O patrocinador do projeto recebe uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Alteração do Progresso da Tarefa</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>Quando uma tarefa for alterada de uma status de progresso positivo (no prazo) para uma status de progresso negativo (em atraso), enviar email para o patrocinador do projeto.</p> <p>O Patrocinador do projeto recebe uma notificação por email quando uma tarefa do projeto atrasa o cronograma.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Adicionar Problema Não Atribuída</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>Quando um problema não atribuída for adicionada enviar email para o patrocinador do projeto.</p> <p>O Patrocinador do projeto recebe uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informações diversas

Consulte também [Notificações: informações diversas](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aviso</td> 
   <td> <p>A notificação foi adicionada</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Uma mensagem será enviada para o Centro de Notificações.</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Cancelar solicitação de documento</p> </td> 
   <td> <p>Usuário ao qual o documento é solicitado</p> </td> 
   <td> <p>Cancele uma solicitação de carregamento de documento minha.</p> <p>O Solicitante de documentos recebe uma notificação por email quando uma solicitação de documento é cancelada.</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Notificação de erro</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Foi encontrado um erro que precisa de sua atenção.</p> <p>Uma notificação por email é gerada depois que o Workfront tenta e falha ao se conectar a uma conta POP. Após 25 tentativas, o Workfront desativa a conexão com a conta POP para preservar os recursos e envia uma notificação. </p> <p>A notificação por email é enviada ao Proprietário do projeto, se o email POP estiver associado a uma fila de solicitações, ou aos administradores do Workfront, se a conta POP estiver associada ao recurso "Email de entrada" na Configuração de email.
   </p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Atribuição de problema</p> </td> 
   <td> <p>Proprietário do recurso</p> </td> 
   <td> <p>Quando uma atribuição de problema for alterada, enviar email para o proprietário do recurso.</p> <p>O Gerente do destinatário da ocorrência recebe uma notificação por email quando uma alteração afeta um usuário que ele gerencia.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário</p> </td> 
   <td> <p>Novo Usuário</p> </td> 
   <td> <p>Usuário</p> </td> 
   <td> <p>When a new user is created in Workfront, email the user.</p> <p>Depois que o novo usuário é criado, ele recebe um convite por email, notificando-o de que uma conta do Workfront foi criada e solicitando que defina sua senha.</p> <p>Ao criar um novo usuário, os usuários podem selecionar a opção "Enviar um email de convite para essa pessoa" (conforme descrito em <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Adicionar usuários</a><span style="font-weight: 400;">). No entanto, quando a opção "Novo Usuário para Usuário" está habilitada globalmente, todos os novos usuários recebem o convite por email independentemente da opção "Enviar um email de convite para essa pessoa" estar selecionada.</span></p> </td> 
   <td> Inativo </td> 
  </tr> 
  <tr> 
   <td> <p>Equipe</p> </td> 
   <td> <p>Object Share</p> </td> 
   <td> <p>Members of team that object was shared with</p> </td> 
   <td> <p>Someone shares an object with my team.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário</p> </td> 
   <td> <p>Compartilhamento de objeto</p> </td> 
   <td> <p>Usuário com quem o objeto foi compartilhado</p> </td> 
   <td> <p>Alguém compartilhar um objeto comigo.</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário de projeto</p> </td> 
   <td> <p>Adição de Usuário de Projeto</p> </td> 
   <td> <p>Proprietário do recurso</p> </td> 
   <td> <p>Quando um usuário for adicionado à equipe do projeto, enviar email para o usuário.</p> <p>A manager receives an email notification when one of his or her direct reports is added to a project.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Projeto adicionado ao portfólio ou programa</p> </td> 
   <td> <p>Portfolio ou Proprietário do Programa</p> </td> 
   <td> <p>Alguém adicionar um projeto a um portfólio ou programa que possuo.</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Atribuição de Tarefa</p> </td> 
   <td> <p>Proprietário do Recurso</p> </td> 
   <td> <p>Uma alteração de atribuição de tarefa afeta um de meus funcionários.</p> <p>The Task Assignee's Manager receives an email notification.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> Problema <br>da Tarefa <br>do Projeto</td> 
   <td>Nova atualização</td> 
   <td>Assinante </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Um email é enviado quando uma atualização é feita em uma tarefa, problema ou projeto que eu assino.</span> </p> </td> 
   <td>Ativo (apenas instantâneo)</td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from Error notification above: 
      
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      -->

## Delegação

Consulte também [Notificações: Delegação](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Tipo de objeto | Evento | Destinatário | Descrição | Estado padrão |
|------------------|--------------------------------------------|-----------|--------------------------------------------------------------|-----------------------|
| Tarefas e problemas | Delegação de tarefa e saída | Atribuidor | Delego minhas tarefas e problemas (confirmação) | Ativo (apenas instantâneo) |
| Tarefas e problemas | Interromper delegação de tarefas e problemas | Atribuidor | Interrompo a delegação de minhas tarefas e problemas (confirmação) | Ativo (apenas instantâneo) |
| Tarefas e problemas | Delegação de tarefas e problemas | Pessoa delegada | Alguém delega suas tarefas e problemas para mim | Ativo (apenas instantâneo) |
| Tarefas e problemas | Stop tasks and issue delegation | Pessoa delegada | Alguém interrompe a delegação de suas tarefas e problemas para mim | Active (Instant only) |
