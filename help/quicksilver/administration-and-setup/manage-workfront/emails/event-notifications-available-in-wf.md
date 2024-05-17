---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Tipos de notificação de eventos
description: As notificações de eventos são emails acionados por vários tipos de eventos em objetos, como projetos, tarefas e problemas. Este artigo lista e descreve os tipos disponíveis de notificações de eventos.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '5201'
ht-degree: 7%

---

# Tipos de notificação de eventos

<!-- Audited: 1/2024 -->

As notificações de eventos são emails acionados por vários tipos de eventos em objetos, como projetos, tarefas e problemas, conforme explicado em [Notificações de eventos](../../../workfront-basics/using-notifications/event-notifications.md).

Essas notificações podem ser configuradas no nível do sistema e do grupo:

* Para obter informações sobre como configurar notificações de eventos no nível do sistema, consulte [Configurar notificações de eventos para todos no sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Para obter informações sobre como configurar notificações de eventos no nível do grupo, consulte [Exibir e configurar notificações de eventos para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Os usuários individuais também podem ativar e desativar as notificações de eventos individuais em seus perfis individuais. Para obter mais informações, consulte [Modificar suas próprias notificações por email](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <th>Tipo de Objeto</th> 
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
   <td> <p>Alguém solicitou acesso a mim.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> <p> </p> </td> 
   <td> <p>Adicionar solicitação de documento</p> </td> 
   <td> <p>Usuário ao qual o documento é solicitado</p> </td> 
   <td> <p>Alguém solicitou que eu carregue documento(s).</p> <p>O Solicitante de documentos recebe uma notificação por email quando recebe uma solicitação para carregar um documento.</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento com aprovação pendente</p> </td> 
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
   <td> <p>Preciso aprovar um problema.</p> <p>A definição de quais usuários receberão uma notificação por email para esse evento dependerá se a configuração "Aprovador não precisa pertencer à equipe do projeto (para processos de aprovação que incluam uma função)" está ativada (conforme descrito em <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação global</a>). </p> <p>Se esta opção estiver habilitada</strong>, uma notificação por email será enviada a todos os usuários no sistema com a Função de trabalho "Aprovador".</p> <p>Se essa opção estiver desativada</strong>, somente os membros da equipe do projeto com a Função de trabalho "Aprovador" receberão uma notificação por email.</p> <p>Uma notificação é enviada se o projeto estiver no status Planejamento ou Atual. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problemas Pendentes de Aprovação</p> </td> 
   <td> <p>Aprovador delegado</p> </td> 
   <td> <p>Preciso revisar um problema, cuja aprovação foi delegada a mim.</p> <p>Quando alguém delega uma aprovação de problema a outro usuário, esse usuário é notificado. </p> <p>Uma notificação é enviada somente quando o projeto está no status Atual.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Projeto Pendente de Aprovação</p> </td> 
   <td> <p>Aprovadores</p> </td> 
   <td> <p>Preciso aprovar um projeto.</p> <p>A definição de quais usuários recebem uma notificação por email sobre esse evento dependerá se a configuração "Não é necessário que o aprovador esteja na equipe do projeto (para processos de aprovação que incluem uma função no trabalho)" está ativada (conforme descrito em <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação global</a>).</p> <p>Se esta opção estiver habilitada</strong>, uma notificação por email será enviada a todos os usuários no sistema com a Função de trabalho "Aprovador".</p> <p>Se essa opção estiver desativada</strong>, somente os membros da equipe do projeto com a Função de trabalho "Aprovador" receberão uma notificação por email.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>Projeto Pendente de Aprovação</td> 
   <td>Aprovador delegado</td> 
   <td> <p>Preciso revisar um projeto, cuja aprovação foi delegada a mim.</p> </td> 
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
   <td> <p>Preciso aprovar uma tarefa.</p> <p>A definição de quais usuários receberão uma notificação por email para esse evento dependerá se a configuração "Aprovador não precisa pertencer à equipe do projeto (para processos de aprovação que incluam uma função)" está ativada (conforme descrito em <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação global</a>). </p> <p>Se esta opção estiver habilitada</strong>, uma notificação por email será enviada a todos os usuários no sistema com a Função de trabalho "Aprovador".</p> <p>Se essa opção estiver desativada</strong>, somente os membros da equipe do projeto com a Função de trabalho "Aprovador" receberão uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual no momento da solicitação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Pendência de Aprovação de Tarefa</p> </td> 
   <td> <p>Aprovador delegado</p> </td> 
   <td> <p>Preciso revisar uma tarefa, cuja aprovação foi delegada a mim.</p> <p>Quando alguém delega uma aprovação de problema a outro usuário, esse usuário é notificado. </p> <p>Uma notificação é enviada somente se o status do projeto for Atual no momento da solicitação.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Planilha de horas</p> </td> 
   <td> <p>Planilha de horas reaberta</p> </td> 
   <td> <p>Usuário ao qual a folha de horas pertence</p> </td> 
   <td> <p>Minha planilha de horas foi reaberta.</p> <p>O Proprietário da folha de horas recebe uma notificação por email quando a folha de horas é reaberta, a menos que o usuário que a reabriu também seja o proprietário da folha de horas.</p> <p>Uma notificação por email é enviada somente se o status da folha de horas for Aberto.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Planilha de horas</p> </td> 
   <td> <p>Rejeição de Planilha de Horas</p> </td> 
   <td> <p>Usuário ao qual a folha de horas pertence</p> </td> 
   <td> <p>Minha planilha de horas foi rejeitada.</p> <p>O Proprietário da folha de horas recebe uma notificação por email quando a folha de horas é rejeitada, a menos que o usuário que a rejeitou também seja o proprietário.</p> <p>Uma notificação por e-mail será enviada somente se o status da folha de horas for Rejeitada.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Planilha de horas</p> </td> 
   <td> <p>Envio de Planilha de Horas</p> </td> 
   <td> <p>Aprovador</p> </td> 
   <td> <p>Eu preciso aprovar uma planilha de horas.</p> <p>O Aprovador de Planilha de Horas recebe uma notificação por e-mail quando uma planilha de horas que ele precisa aprovar é enviada, a menos que o usuário que enviou a planilha de horas também seja o Aprovador de Planilha de Horas.</p> <p>Uma notificação é enviada somente se o status da folha de horas for Enviado.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Atribuição</p> </td> 
   <td> <p>Solicitação de item de trabalho</p> </td> 
   <td> <p>Membros da equipe para a qual o item é solicitado</p> </td> 
   <td> <p>Minha equipe recebe uma nova solicitação de trabalho.</p> <p>Os membros da equipe recebem uma notificação por e-mail quando a equipe recebe uma nova solicitação de trabalho. (O usuário que enviou a solicitação não recebe uma notificação se for membro da equipe.)</p> <p>Uma notificação é enviada somente se o status do projeto for Atual no momento em que a Solicitação de trabalho é feita e o status da Solicitação de trabalho for Novo.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Atribuição</p> </td> 
   <td> <p>Solicitação de item de trabalho</p> </td> 
   <td> <p>Usuário para o qual o item de trabalho é solicitado</p> </td> 
   <td> <p>Eu recebo uma nova requisição de trabalho.</p> <p>O destinatário do item de trabalho recebe uma notificação por email, a menos que o usuário que faz a solicitação também seja o destinatário. </p> <p>Uma notificação não será enviada se o status da tarefa for Concluído ou se o status do problema for Fechado.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual no momento da solicitação.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solicitações que eu fiz

Consulte também [Notificações: Solicitações que fiz](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de Objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Mudança de status de aprovação de documento</p> </td> 
   <td> <p>Solicitante</p> </td> 
   <td> <p>Uma solicitação de aprovação de documento foi concluída.</p> <p>O Solicitante de documentos recebe uma notificação por email quando a solicitação de aprovação de documentos é concluída.</p> </td> 
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
   <td>Atribuição de problema</td> 
   <td>Originador do problema</td> 
   <td> <p>Uma pessoa foi designada a um problema para o qual sou o contato primário.</p> <p>O contato principal em um problema recebe uma notificação quando o problema é atribuído a um usuário. </p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> Inativo</td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Conclusão do problema</p> </td> 
   <td> <p>Originador do problema</p> </td> 
   <td> <p>Um problema para o qual sou o contato principal foi concluído.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Alteração do status do projeto</p> </td> 
   <td> <p>Usuário que criou o projeto (Cadastrado por)</p> </td> 
   <td> <p>O status muda em um projeto que criei.</p> <p>O usuário que criou o projeto recebe uma notificação por email quando o status do projeto é alterado.</p> </td> 
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
   <td> <p>Originador do problema</p> </td> 
   <td> <p>Quando uma solicitação de Help Desk é atribuída, enviar email ao originador do problema.</p> <p>O contato principal do problema recebe uma notificação por email quando um usuário é atribuído ao problema, a menos que o contato principal e o usuário atribuído sejam o mesmo usuário.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto estiver usando uma Visualização "Is Help Desk".</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Solicitação fechada</p> </td> 
   <td> <p>Originador do problema</p> </td> 
   <td> <p>Minha solicitação foi fechada (confirmação).</p> <p>O contato principal do problema recebe uma notificação por email quando a solicitação é fechada.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto estiver usando uma Visualização "Is Help Desk".</p> <p>Se as notificações de "conclusão do problema" estiverem ativadas, elas sempre serão acionadas em vez de "Solicitação fechada para o contato principal do problema". Se quiser que essa notificação seja acionada, desative as notificações de "conclusão de problemas".</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Adicionar Documento de Solicitação</p> </td> 
   <td> <p>Originador do problema</p> </td> 
   <td> <p>Um documento foi alterado ou carregado sobre um problema para o qual sou o contato principal.</p> <p>O contato principal do problema recebe uma notificação por email quando um documento é carregado ou alterado no problema, a menos que o usuário que carregou ou alterou o documento também seja o contato principal.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual e se o projeto tiver a opção "Publicar como Fila de solicitação de ajuda" ativada na guia Configuração da fila.</p> </td> 
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
   <th>Tipo de Objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Comentar no documento</p> </td> 
   <td> <p>Proprietário do Documento</p> </td> 
   <td> <p>Um comentário é adicionado ao meu documento.</p> <p>O proprietário de um documento no Workfront recebe uma notificação por email quando um comentário é postado no documento, a menos que o usuário que postou o comentário também seja o proprietário do documento.</p> <p>Todos os usuários incluídos diretamente no comentário também recebem uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual. </p> <p>O assunto do email de notificação instantânea é: <em>Comentar em &lt;request name=""&gt; em &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> O assunto da notificação de resumo diário é:<em> Resumo das comunicações &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Adicionar Nota de Solicitação</p> </td> 
   <td> <p>Originador do problema</p> </td> 
   <td> <p>Quando um comentário for postado em uma solicitação, envie um email para o contato principal do problema.</p> <p>O contato principal de um problema recebe uma notificação por email quando um comentário é postado em uma solicitação, a menos que o usuário que postou o comentário também seja o contato principal do problema.</p> <p>Todos os usuários incluídos diretamente no comentário também recebem uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
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
   <td> <p>Atualização direcionada</p> </td> 
   <td> <p>Membros da equipe</p> </td> 
   <td> <p>Alguém tiver incluído minha equipe em uma atualização direta.</p> <p>Uma atualização direcionada é quando um usuário inclui especificamente outro usuário em uma atualização, conforme descrito em <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Marcar outros usuários em atualizações</a>.</p> <p>Nesse caso, qualquer membro da equipe incluído na atualização direcionada receberá uma notificação por email sobre a atualização.</p> <p>A notificação por email é enviada somente para usuários que têm direitos de acesso ao objeto da atualização.</p> <p>Se o usuário que envia a atualização direcionada for um membro da equipe que está sendo incluída, o usuário que envia a atualização não receberá uma notificação por email.</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Comentário do Item de Trabalho</p> </td> 
   <td> <p>Participantes da thread</p> </td> 
   <td> <p>Quando alguém comentar em um item de trabalho, envie email para qualquer um que tiver comentado este item de trabalho.</p> <p>Os participantes da thread e os usuários incluídos em uma mensagem direta recebem uma notificação por email quando um usuário faz um comentário na thread.</p> <p>Os usuários devem ter acesso de Visualização para receber uma notificação.</p> <p>Os seguintes usuários não recebem uma notificação:</p> 
    <ul> 
     <li> <p>Equipes incluídas em uma mensagem direta</p> </li> 
     <li> <p>O proprietário da Nota</p> </li> 
     <li> <p>O contato primário</p> </li> 
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
   <th>Tipo de Objeto</th> 
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
   <td> <p>Recebi a delegação de aprovador.</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
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
   <td> <p>Uma solicitação de aprovação de documento foi cancelada.</p> <p>O Aprovador de documentos do documento recebe uma notificação por email quando a solicitação de aprovação de documento é cancelada.</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Planilha de horas</p> </td> 
   <td> <p>Aprovação de Planilha de Horas</p> </td> 
   <td> <p>Usuário ao qual a folha de horas pertence</p> </td> 
   <td> <p>Minha planilha de horas foi aprovada.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informações sobre o trabalho atribuído a mim

Consulte também [Notificações: Informações sobre o trabalho atribuído a mim](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de Objeto</th> 
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
   <td> <p>Todas as predecessoras de minhas tarefas foram concluídas.</p> <p>O destinatário da tarefa recebe uma notificação por email.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Decisão de aprovação</p> </td> 
   <td> <p>Usuário ao qual o problema está atribuído</p> </td> 
   <td> <p>Quando um problema é aprovada ou rejeitada, envie email para o usuário atribuído.</p> <p>O destinatário de um problema recebe uma notificação por email quando uma decisão de aprovação é tomada (aprovada ou rejeitada).</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Decisão de aprovação</p> </td> 
   <td> <p>Usuário ao qual a tarefa está atribuída</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para o usuário atribuído</p> <p>O destinatário da tarefa recebe uma notificação por e-mail quando a tarefa é aprovada ou rejeitada.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Conclusão do problema</p> </td> 
   <td> <p>Usuário ao qual o problema está atribuído</p> </td> 
   <td> <p>Quando um problema for concluído enviar email para o usuário atribuído.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>A data de conclusão planejada do problema mudou</p> </td> 
   <td> <p>Usuário ao qual o problema está atribuído</p> </td> 
   <td> <p>A data de conclusão de um problema atribuído a mim mudou.</p> <p>O destinatário do problema recebe uma notificação por email quando a Data de conclusão planejada é alterada, a menos que o usuário que alterou a Data de conclusão planejada também seja o destinatário.</p> <p>Uma notificação é enviada somente se o status do projeto for algo diferente de Planejamento.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Alteração do status do problema</p> </td> 
   <td> <p>Usuário ao qual o problema está atribuído</p> </td> 
   <td> <p>O status de um dos meus itens de trabalho mudou.</p> <p>O destinatário do problema recebe uma notificação por email quando o status é alterado, a menos que o usuário que alterou o status também seja o destinatário.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Ativo (somente diariamente)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Adicionar Documento de Solicitação</p> </td> 
   <td> <p>Usuário ao qual o problema está atribuído</p> </td> 
   <td> <p>Documentos foram carregados ou alterados na minha requisição.</p> <p>O destinatário do problema recebe uma notificação por email quando os documentos são carregados ou alterados em um problema adicionado.</p> <p>Uma notificação por e-mail não é enviada se o usuário que inseriu o problema for o destinatário do problema.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual e se o projeto tiver a opção "Publicar como Fila de solicitação de ajuda" ativada na guia Configuração da fila.</p> </td> 
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
   <td> <p>A data de conclusão de uma tarefa atribuída a mim mudou.</p> <p>O Destinatário da tarefa recebe uma notificação por e-mail quando a Data de conclusão planejada da tarefa é alterada, a menos que o usuário que alterou a Data de conclusão planejada também seja o Destinatário da tarefa.</p> <p>Uma notificação é enviada somente se o status do projeto for algo diferente de Planejamento.</p> <p>Nenhuma notificação é enviada sobre tarefas pessoais.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Mudança do status da tarefa</p> </td> 
   <td> <p>Usuário ao qual a tarefa está atribuída</p> </td> 
   <td> <p>O status muda em uma tarefa para a qual fui atribuído.</p> <p>O Destinatário da tarefa recebe uma notificação por e-mail quando o status da tarefa é alterado, a menos que o usuário que alterou o status também seja o destinatário.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## Informações sobre projetos em que estou trabalhando

Consulte também [Notificações: Informações sobre projetos em que estou](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de Objeto</th> 
   <th>Evento</th> 
   <th>Destinatário</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Status atual do projeto</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando uma status de projeto for alterada de ideia/aprovado/solicitado/em planejamento para atual, enviar email para a equipe.</p> <p>Os usuários no projeto recebem uma notificação por email quando o projeto se torna ativo.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Adicionar documento</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando um documento for adicionado enviar email para a equipe.</p> <p>Os usuários na equipe do projeto recebem uma notificação por email quando um documento é adicionado ao projeto, exceto para o usuário que adicionou o documento.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e o documento não for Privado. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema adicionado</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando um problema for adicionada enviar email para a equipe.</p> <p>Os usuários em um projeto recebem uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
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
   <td> <p>Quando um projeto for concluído, enviar email para a equipe.</p> <p>Os usuários de uma equipe de projeto recebem uma notificação por email quando o status do projeto é Concluído.</p> <p>Dica: se os projetos forem concluídos regularmente, habilitar essa opção pode criar muitos emails para usuários que têm um número limitado de tarefas em muitos projetos. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Alteração do status do projeto</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando uma status de projeto for alterado, enviar email para a equipe.</p> <p>Os usuários na equipe do projeto recebem uma notificação por email quando o status do projeto é alterado. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário de Projeto</p> </td> 
   <td> <p>Adição de Usuário de Projeto</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando um usuário for adicionado à equipe, enviar email para o usuário.</p> <p>O usuário que foi adicionado ao projeto recebe uma notificação por email quando é adicionado, a menos que o usuário tenha sido adicionado automaticamente ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Conclusão da tarefa</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para a equipe.</p> <p>Os membros da equipe do projeto recebem uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema não Atribuído adicionado</p> </td> 
   <td> <p>Membros da equipe do projeto</p> </td> 
   <td> <p>Quando um problema não atribuída for adicionada enviar email para a equipe.</p> <p>Os usuários em um projeto recebem uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informações sobre projetos dos quais sou proprietário

Consulte também [Notificações: informações sobre os projetos que possuo](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de Objeto</th> 
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
   <td> <p>Quando um documento for adicionado enviar email para a equipe.</p> <p>O Proprietário do projeto recebe uma notificação por email quando um documento é adicionado ao projeto, a menos que o usuário que adicionou o documento também seja o Proprietário do projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e o documento não for Privado.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
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
   <td> <p>Quando um problema for concluído enviar email para a equipe.</p> <p>O proprietário do projeto recebe uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Término de etapa</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>Quando uma etapa for concluída, enviar email para o proprietário do projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Atribuição do proprietário do projeto</p> </td> 
   <td> <p>Proprietário do projeto</p> </td> 
   <td> <p>Quando o proprietário do projeto mudar ou na criação do projeto, enviar email para o usuário recentemente atribuído</p> <p>Quando um usuário é atribuído como o proprietário de um projeto, ele recebe uma notificação por email.</p> <p>Se o proprietário do projeto for o mesmo usuário que fez a atribuição, uma notificação por email não será enviada</p> </td> 
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
   <td> <p>Conclusão da tarefa</p> </td> 
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
   <th>Tipo de Objeto</th> 
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
   <td> <p>Quando um documento for adicionado enviar email para o patrocinador do projeto.</p> <p>O Patrocinador do projeto recebe uma notificação por email quando um documento é adicionado ao projeto, a menos que o documento seja adicionado pelo Patrocinador do projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o documento não for Privado.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema adicionado</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>Quando um problema for adicionada enviar email para o patrocinador do projeto.</p> <p>O patrocinador do projeto recebe uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Conclusão do problema</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>Quando um problema for concluído enviar email para o patrocinador do projeto.</p> <p>O patrocinador do projeto recebe uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
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
   <td> <p>Quando um projeto for alterado de uma status positiva de progresso (no prazo) para uma status negativa de progresso (em atraso), enviar email para o patrocinador do projeto.</p> <p>O Patrocinador do projeto recebe uma notificação por email quando o projeto atrasa o agendamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Atribuição do Patrocinador do Projeto</p> </td> 
   <td> <p>Patrocinador do Projeto</p> </td> 
   <td> <p>Quando um patrocinador de projeto mudar ou na criação do projeto, enviar email para o patrocinador do projeto.</p> <p>O patrocinador do projeto recebe uma notificação por email quando é definido como patrocinador de um projeto.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Conclusão da tarefa</p> </td> 
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
   <td> <p>Quando um problema não atribuída for adicionada enviar email para o patrocinador do projeto.</p> <p>O Patrocinador do projeto recebe uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informações diversas

Consulte também [Notificações: Informações diversas](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de Objeto</th> 
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
   <td> <p>Foi encontrado um erro que requer sua atenção.</p> <p>Uma notificação por email é gerada depois que o Workfront tenta e falha ao se conectar a uma conta POP. Após 25 tentativas, o Workfront desativa a conexão com a conta POP para preservar os recursos e envia uma notificação. </p> <p>A notificação por email é enviada ao Proprietário do projeto, se o email POP estiver associado a uma fila de solicitações, ou aos administradores do Workfront, se a conta POP estiver associada ao recurso "Email de entrada" na Configuração de email.
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
   <td> <p>Quando um novo usuário for criado no Workfront, envie um email para o usuário.</p> <p>Depois que o novo usuário é criado, ele recebe um convite por email, notificando-o de que uma conta do Workfront foi criada e solicitando que defina sua senha.</p> <p>Ao criar um novo usuário, os usuários podem selecionar a opção "Enviar um email de convite para essa pessoa" (conforme descrito em <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Adicionar usuários</a><span style="font-weight: 400;">). No entanto, quando a opção "Novo usuário para usuário" está habilitada globalmente, todos os novos usuários recebem o convite por email independentemente da opção "Enviar um email de convite para essa pessoa" estar selecionada.</span></p> </td> 
   <td> Inativo </td> 
  </tr> 
  <tr> 
   <td> <p>Equipe</p> </td> 
   <td> <p>Compartilhamento de objeto</p> </td> 
   <td> <p>Membros da equipe com os quais o objeto foi compartilhado</p> </td> 
   <td> <p>Alguém compartilhar um objeto com minha equipe.</p> </td> 
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
   <td> <p>Usuário de Projeto</p> </td> 
   <td> <p>Adição de Usuário de Projeto</p> </td> 
   <td> <p>Proprietário do recurso</p> </td> 
   <td> <p>Quando um usuário for adicionado à equipe do projeto, enviar email para o usuário.</p> <p>Um gerente recebe uma notificação por email quando um de seus subordinados diretos é adicionado a um projeto.</p> <p>Os usuários com uma licença Light ou Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Projeto adicionado ao portfólio ou programa</p> </td> 
   <td> <p>Proprietário do Portfolio ou programa</p> </td> 
   <td> <p>Alguém adicionar um projeto a um portfólio ou programa que possuo.</p> </td> 
   <td> <p>Ativo (apenas instantâneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Atribuição de tarefa</p> </td> 
   <td> <p>Proprietário do recurso</p> </td> 
   <td> <p>Quando uma atribuição de tarefa for alterada, enviar email para o proprietário do recurso.</p> <p>O gerente do destinatário da tarefa recebe uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> Projeto <br>Tarefa <br>Problema</td> 
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

| Tipo de Objeto | Evento | Destinatário | Descrição | Estado padrão |
|------------------|--------------------------------------------|-----------|--------------------------------------------------------------|-----------------------|
| Tarefas e problemas | Delegação de tarefas e problemas | Atribuidor | Delego minhas tarefas e problemas (confirmação) | Ativo (apenas instantâneo) |
| Tarefas e problemas | Interromper delegação de tarefas e problemas | Atribuidor | Interrompo a delegação de minhas tarefas e problemas (confirmação) | Ativo (apenas instantâneo) |
| Tarefas e problemas | Delegação de tarefas e problemas | Pessoa delegada | Alguém delega suas tarefas e problemas para mim | Ativo (apenas instantâneo) |
| Tarefas e problemas | Interromper delegação de tarefas e problemas | Pessoa delegada | Alguém interrompe a delegação de suas tarefas e problemas para mim | Ativo (apenas instantâneo) |
