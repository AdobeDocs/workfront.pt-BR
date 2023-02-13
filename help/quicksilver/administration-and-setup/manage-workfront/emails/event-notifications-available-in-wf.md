---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Notificações de evento disponíveis no Adobe Workfront
description: As notificações de eventos são emails acionados por vários tipos de eventos em objetos, como projetos, tarefas e problemas, conforme explicado em Notificações de eventos.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '5070'
ht-degree: 26%

---

# Notificações de evento disponíveis no Adobe Workfront

As notificações de eventos são emails acionados por vários tipos de eventos em objetos, como projetos, tarefas e problemas, como explicado em [Notificações de evento](../../../workfront-basics/using-notifications/event-notifications.md).

Essas notificações podem ser configuradas no sistema e no nível do grupo:

* Para obter informações sobre como configurar notificações de eventos no nível do sistema, consulte [Configurar notificações de evento para todos no sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Para obter informações sobre como configurar notificações de eventos no nível do grupo, consulte [Exibir e configurar notificações de evento para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Os usuários individuais também podem ativar e desativar suas notificações de evento individual em seus perfis individuais. Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de evento](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

As tabelas a seguir listam todas as notificações de evento do Adobe Workfront, uma breve descrição do evento e se o evento está ativo ou inativo por padrão.

## Ação necessária

Consulte também [Notificações: Ação necessária](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de Objeto</th> 
   <th>Evento</th> 
   <th>Descrição</th> 
   <th>Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Usuário</p> </td> 
   <td> <p>Solicitação de acesso ao usuário</p> </td> 
   <td> <p>Alguém está solicitando acesso a mim.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> <p> </p> </td> 
   <td> <p>Adicionar solicitação de documento ao solicitante</p> </td> 
   <td> <p>Solicite-me que carregue documentos.</p> <p>A Solicitação de documento recebe uma notificação por email quando recebe uma solicitação para carregar um documento.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento pendendo aprovação dos aprovadores</p> </td> 
   <td> <p>Preciso aprovar um documento.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Atribuição de Problema para Problema Atribuído a</p> </td> 
   <td> <p>Quando a atribuição de um problema for alterada, enviar email para o novo usuário atribuído ao problema.</p> <p>O destinatário do problema recebe uma notificação por email somente se o status do projeto for Atual e o status do problema não for Fechado ou algo que seja igual a Fechado.</p> <p>Os usuários com uma licença de Revisão ou Solicitação não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema pendente de aprovação pelos aprovadores</p> </td> 
   <td> <p>Quando um problema está pendente de aprovação, enviar email para o aprovador.</p> <p>Os usuários que recebem uma notificação por email para esse evento dependem se a configuração "Aprovador não obrigatório para estar na equipe do projeto (para processos de aprovação que incluem uma função)" está ativada (conforme descrito em <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação global</a>). </p> <p>Se esta opção estiver ativada</strong>, uma notificação por email é enviada a todos os usuários no sistema com a Função de trabalho de "Aprovador".</p> <p>Se esta opção estiver desativada</strong>, somente os membros da equipe do projeto com a Função de trabalho de "Aprovador" recebem uma notificação por email.</p> <p>Uma notificação é enviada se o projeto estiver no status Planejamento ou Atual. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema pendente de aprovação do aprovador delegado</p> </td> 
   <td> <p>Preciso revisar uma aprovação de problema em que fui delegado.</p> <p>Quando alguém delega uma aprovação de edição a outro usuário, esse usuário é notificado. </p> <p>Uma notificação é enviada somente quando o projeto está no status Current .</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Projeto pendente de aprovação pelos aprovadores</p> </td> 
   <td> <p>Quando um projeto está pendente de aprovação, enviar email ao aprovador.</p> <p>Os usuários que recebem uma notificação por email para esse evento dependem se a configuração "Aprovador não obrigatório para estar na equipe do projeto (para processos de aprovação que incluem uma função de trabalho)" está ativada (conforme descrito em <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação global</a>).</p> <p>Se esta opção estiver ativada</strong>, uma notificação por email é enviada a todos os usuários no sistema com a Função de trabalho de "Aprovador".</p> <p>Se esta opção estiver desativada</strong>, somente os membros da equipe do projeto com a Função de trabalho de "Aprovador" recebem uma notificação por email.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>Projeto pendente de aprovação do aprovador delegado</td> 
   <td> <p>Preciso revisar um projeto, cuja aprovação foi delegada a mim.</p> </td> 
   <td> Ativo</td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Atribuição de Tarefa para o Recurso da Tarefa</p> </td> 
   <td> <p>Quando uma atribuição primária de uma tarefa for alterada, enviar email para o usuário mais recente atribuído.</p> <p>O Destinatário da Tarefa recebe uma notificação por e-mail se ele for o destinatário principal da tarefa, a menos que o destinatário seja o usuário que fez a atribuição.</p> <p>Uma notificação é enviada se o status do projeto for Current e a tarefa não estiver marcada como Complete.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Tarefa pendente de aprovação pelos aprovadores</p> </td> 
   <td> <p>Quando uma tarefa está pendente de aprovação, enviar email para o aprovador.</p> <p>Os usuários que recebem uma notificação por email para esse evento dependem se a configuração "Aprovador não obrigatório para estar na equipe do projeto (para processos de aprovação que incluem uma função)" está ativada (conforme descrito em <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação global</a>). </p> <p>Se esta opção estiver ativada</strong>, uma notificação por email é enviada a todos os usuários no sistema com a Função de trabalho de "Aprovador".</p> <p>Se esta opção estiver desativada</strong>, somente os membros da equipe do projeto com a Função de trabalho de "Aprovador" recebem uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual no momento da solicitação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Tarefa pendente de aprovação do aprovador delegado</p> </td> 
   <td> <p>Preciso revisar uma tarefa, cuja aprovação foi delegada a mim.</p> <p>Quando alguém delega uma aprovação de edição a outro usuário, esse usuário é notificado. </p> <p>Uma notificação é enviada somente se o status do projeto for Atual no momento da solicitação.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Planilha de horas</p> </td> 
   <td> <p>Planilha de horas reaberta para o usuário</p> </td> 
   <td> <p>Minha Planilha de horas foi reaberta.</p> <p>O Proprietário da folha de horas recebe uma notificação por email quando a folha de horas é reaberta, a menos que o usuário que reabriu a folha de horas também seja o proprietário da folha de horas.</p> <p>Uma notificação por email é enviada somente se o status da folha de horas for Open.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Planilha de horas</p> </td> 
   <td> <p>Rejeição de planilhasde horas para o usuário</p> </td> 
   <td> <p>Quando uma planilha de horas for rejeitada, enviar email para o usuário.</p> <p>O Proprietário da Folha de Horas recebe uma notificação por email quando a folha de horas é rejeitada, a menos que o usuário que rejeitou a folha de horas também seja o proprietário.</p> <p>Uma notificação por email é enviada somente se o status da folha de horas for Rejeitada.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Planilha de horas</p> </td> 
   <td> <p>Submissão de Planilha de horas para o aprovador</p> </td> 
   <td> <p>Quando uma planilha de horas for submetida, enviar email para o aprovador.</p> <p>O Aprovador da folha de horas recebe uma notificação por email quando uma folha de horas que precisa ser aprovada é enviada, a menos que o usuário que enviou a folha de horas também seja o Aprovador da folha de horas.</p> <p>Uma notificação é enviada somente se o status da folha de ponto for Submetida.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Atribuição</p> </td> 
   <td> <p>Requisição de item de trabalho para a equipe</p> </td> 
   <td> <p>Minha equipe recebeu uma nova requisição de trabalho.</p> <p>Os membros da equipe recebem uma notificação por email quando a equipe recebe uma nova solicitação de trabalho. (O usuário que enviou a solicitação não recebe uma notificação se for membro da equipe.)</p> <p>Uma notificação é enviada somente se o status do projeto for Atual no momento em que a Solicitação de trabalho for feita e o status da Solicitação de trabalho for Novo.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Atribuição</p> </td> 
   <td> <p>Requisição de Item de Trabalho para Atribuídos no Item de Trabalho</p> </td> 
   <td> <p>Quando um usuário recebe uma nova requisição de trabalho, envie email aos atribuídos.</p> <p>O destinatário do item de trabalho recebe uma notificação por email, a menos que o usuário que faz a solicitação também seja o destinatário. </p> <p>Uma notificação não é enviada se o status da tarefa for Complete ou se o status da emissão for Closed .</p> <p>Uma notificação é enviada somente se o status do projeto for Atual no momento da solicitação.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solicitações que fiz

Consulte também [Notificações: Solicitações que fiz](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de Objeto</th> 
   <th>Evento</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Alteração de status de aprovação de documento para o solicitante</p> </td> 
   <td> <p>Uma solicitação de aprovação de documento foi concluída.</p> <p>O Solicitante de documento recebe uma notificação por email quando a solicitação de aprovação de documento é concluída.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Concluir solicitação de documento para solicitante</p> </td> 
   <td> <p>Uma solicitação de carregamento de documento foi atendida.</p> <p>O Solicitante de documento recebe uma notificação por email quando uma solicitação para carregar um documento é atendida.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema: Adicionar para o originador do problema</p> </td> 
   <td> <p>Eu adiciono um problema a um projeto.</p> <p>O contato principal em um problema recebe uma notificação quando adiciona um problema em um projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>Atribuição de problema para o contato primário do problema</td> 
   <td> <p>Uma pessoa foi designada a um problema para o qual sou o contato primário.</p> <p>O contato principal em um problema recebe uma notificação quando o problema é atribuído a um usuário. </p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> Inativo</td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Término do Problema para originador do Problema</p> </td> 
   <td> <p>Quando um problema for concluído enviar email para o originador do problema.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Alteração de Status de Projeto para Cadastrado Por</p> </td> 
   <td> <p>Quando uma status de projeto for alterado, enviar email para o usuário que cadastrou o projeto.</p> <p>O usuário que criou o projeto recebe uma notificação por email quando o status do projeto é alterado.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Solicitação de Help Desk incluída para o originador do problema</p> </td> 
   <td> <p>Envio um pedido (confirmação).</p> <p>O Contato principal sobre o problema recebe uma notificação por email quando enviar um problema.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto estiver usando uma Exibição "Is Help Desk".</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Atribuição de uma solicitação do Help Desk para o originador do problema</p> </td> 
   <td> <p>Alguém está atribuído à minha solicitação.</p> <p>O contato principal do problema recebe uma notificação por email quando um usuário é atribuído ao problema, a menos que o contato principal e o usuário atribuído sejam o mesmo usuário.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto estiver usando uma Exibição "Is Help Desk".</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Solicitação de Help Desk fechada para originador do problema</p> </td> 
   <td> <p>Minha solicitação está fechada (confirmação).</p> <p>O contato principal do problema recebe uma notificação por email quando a solicitação é fechada.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto estiver usando uma Exibição "Is Help Desk".</p> <p>Se as notificações de "conclusão de emissão" estiverem ativadas, elas sempre serão acionadas em vez de "Solicitação fechada para Emitir contato principal". Se quiser que essa notificação seja acionada, desative as notificações de "conclusão de emissão".</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento incluído na solicitação de Help Desk para o originador do problema</p> </td> 
   <td> <p>Um documento foi alterado ou caregado sobre um problema para o qual sou o contato primário.</p> <p>O contato principal do problema recebe uma notificação por email quando um documento é carregado ou alterado no problema, a menos que o usuário que carregou ou alterou o documento também seja o contato principal.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto tiver a opção "Publicar como fila de solicitações de ajuda" ativada na guia Configuração da fila. &lt;!— DESENHADO EM FLARE: Para obter mais informações sobre como publicar um projeto como uma fila de solicitações de ajuda, consulte 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Visão geral da guia Detalhes da fila em um projeto</a>.

    —>&lt;/p> &lt;/td>
<td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Alteração de status na solicitação de Help Desk para o originador do problema</p> </td> 
   <td> <p>O status muda na minha solicitação.</p> <p>O contato principal do problema recebe uma notificação por email quando o status do problema muda, a menos que o usuário que alterou o status também seja o contato principal.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e o projeto estiver usando uma Exibição "Is Help Desk".</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
 </tbody> 
</table>

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
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Comentar no Documento para Proprietário do Documento</p> </td> 
   <td> <p>Foi adicionado um comentário ao seu documento.</p> <p>O proprietário de um documento no Workfront recebe uma notificação por email quando um comentário é postado no documento, a menos que o usuário que postou o comentário também seja o proprietário do documento.</p> <p>Qualquer usuário que esteja incluído diretamente no comentário também receberá uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual. </p> <p>O assunto do email de notificação instantânea é: <em>Comentar em &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> O objeto da notificação diária de resumo é:<em> Resumo da comunicação &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Ativo </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Nota adicionada à solicitação de Help Desk para originador do problema</p> </td> 
   <td> <p>Quando um comentário for postado em uma solicitação, envie um email para o contato principal da ocorrência.</p> <p>O contato principal de um problema recebe uma notificação por email quando um comentário é postado em uma solicitação, a menos que o usuário que postou o comentário também seja o contato principal para o problema.</p> <p>Qualquer usuário que esteja diretamente incluído no comentário também receberá uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário</p> </td> 
   <td>Atualização Direcionada ao Usuário</td> 
   <td> <p>Alguém tiver me incluído em uma atualização direcionada.</p> <p>Uma atualização direcionada ocorre quando um usuário inclui especificamente outro usuário em uma atualização, conforme descrito em <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Marcar outras pessoas em atualizações</a>.</p> <p>Nesse caso, o usuário que está incluído na atualização direcionada recebe uma notificação por email sobre a atualização.</p> <p>A notificação por email é enviada somente se o usuário tiver direitos de acesso ao objeto&lt;!&gt;— DESENHADO EM FLARE: e não é o mesmo usuário que insere a atualização

    -->. &lt;/p> &lt;p>Esta notificação de evento é ativada por padrão e não pode ser desativada.&lt;/p> &lt;/td>
<td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Equipe</p> </td> 
   <td> <p>Atualização Direcionada para Equipe</p> </td> 
   <td> <p>Alguém tiver incluído minha equipe em uma atualização direta.</p> <p>Uma atualização direcionada ocorre quando um usuário inclui especificamente outro usuário em uma atualização, conforme descrito em <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Marcar outras pessoas em atualizações</a>.</p> <p>Nesse caso, qualquer membro da equipe incluído na atualização direcionada recebe uma notificação por email sobre a atualização.</p> <p>A notificação por email é enviada apenas para usuários que têm direitos de acesso ao objeto da atualização.</p> <p>Se o usuário que está enviando a atualização direcionada for membro da equipe que está sendo incluída, o usuário que está enviando a atualização não receberá uma notificação por email.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Comentário de Item de Trabalho para os Participantes da Discussão</p> </td> 
   <td> <p>Quando alguém comentar em um item de trabalho, envie email para qualquer um que tiver comentado este item de trabalho.</p> <p>Os participantes no thread e os usuários incluídos em uma mensagem direta recebem uma notificação por email quando um usuário faz um comentário no thread.</p> <p>Os usuários devem ter acesso de Exibição para receber uma notificação.</p> <p>Os seguintes usuários não recebem uma notificação:</p> 
    <ul> 
     <li> <p>Equipes incluídas em uma mensagem direta</p> </li> 
     <li> <p>O proprietário da Nota</p> </li> 
     <li> <p>O Contato Principal</p> </li> 
    </ul> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Comentário no Item de Trabalho para os Atribuídos no Item de Trabalho</p> </td> 
   <td> <p>Quando alguém comentar no item de trabalho, envie email para os atribuídos.</p> <p>O destinatário do item de trabalho recebe uma notificação por email sempre que um usuário adiciona uma atualização a um item de trabalho, a menos que o usuário que adiciona a atualização também seja o destinatário.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Requisição de Trabalho responde para o Requisitante do Trabalho</p> </td> 
   <td> <p>Alguém responde ao meu pedido.</p> <p>Depois que um usuário envia uma solicitação e outro usuário responde a ela, o usuário que a enviou recebe uma notificação por email.</p> <p>Uma notificação por email não é enviada se:</p> 
    <ul> 
     <li> <p>O usuário que responde é o mesmo usuário que fez a solicitação</p> </li> 
     <li> <p>O usuário não tem acesso para visualizar a nota</p> </li> 
    </ul> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
 </tbody> 
</table>

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
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Usuário</p> </td> 
   <td> <p>Delegação de aprovação a outro usuário</p> </td> 
   <td> <p>Recebi a delegação de aprovador.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Mudança de status de aprovação de problema delegada</p> </td> 
   <td> <p>Uma solicitação de aprovação de problema foi concluída. </p> <p>Ao delegar uma aprovação de emissão a outra pessoa, você receberá uma notificação por email ao terminar essa aprovação (se ela aprovar ou rejeitar a aprovação de emissão). </p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Mudança de status de aprovação de projeto delegada</p> </td> 
   <td> <p>Uma solicitação de aprovação de projeto foi concluída.</p> <p>Ao delegar uma aprovação de projeto a outra pessoa, você receberá uma notificação por email ao concluir essa aprovação (se ela aprovar ou rejeitar a aprovação do projeto).</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Mudança de status de aprovação de tarefa delegada</p> </td> 
   <td> <p>Um status de aprovação de tarefa delegada é concluído.</p> <p>Quando você delega uma aprovação de tarefa a outra pessoa, você recebe uma notificação por e-mail quando ela terminar essa aprovação (se ela aprovar ou rejeitar a aprovação da tarefa).</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Cancelar aprovação de documento para o aprovador</p> </td> 
   <td> <p>Uma solicitação de aprovação de documento foi cancelada.</p> <p>O Aprovador de documento do documento recebe uma notificação por email quando a solicitação de aprovação do documento é cancelada.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Planilha de horas</p> </td> 
   <td> <p>Aprovação de Planilha de Horas para o Usuário</p> </td> 
   <td> <p>Quando uma planilha de horas for aceita e fechada, enviar email para o usuário.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informações sobre o trabalho que me foi atribuído

Consulte também [Notificações: Informações sobre o trabalho que me foi atribuído](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de Objeto</th> 
   <th>Evento</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Tarefa</td> 
   <td>Todas as predecessoras de Término da tarefa para as tarefas dependentes na equipe atribuída</td> 
   <td> <p>Todos os antecessores das tarefas da equipe estão concluídos.</p> <p>Os destinatários da tarefa (todos os membros da equipe) recebem uma notificação por e-mail.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td>Inativo</td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Todas as predecessoras de Término da tarefa para as tarefas dependentes</p> </td> 
   <td> <p>Quando todas as predecessoras forem concluídas enviar email para os usuários primariamente atribuídos de todas as tarefas dependentes.</p> <p>O destinatário da tarefa recebe uma notificação por email.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Decisão de aprovação da emissão atribuída ao</p> </td> 
   <td> <p>Quando um problema é aprovada ou rejeitada, envie email para o usuário atribuído.</p> <p>O destinatário de um problema recebe uma notificação por email quando uma decisão de aprovação é tomada (aprovada ou rejeitada).</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Decisão de aprovação para tarefa atribuída a</p> </td> 
   <td> <p>Quando uma aprovação de tarefa for realizada, enviar email para o usuário atribuído.</p> <p>O destinatário da tarefa recebe uma notificação por email quando a tarefa é aprovada ou rejeitada.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Término do Problema para Atribuído</p> </td> 
   <td> <p>Quando um problema for concluído enviar email para o usuário atribuído.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>A data de conclusão planejada do problema mudou</p> </td> 
   <td> <p>A data de conclusão de um problema atribuído a mim mudou.</p> <p>O destinatário do problema recebe uma notificação por email quando a Data de conclusão planejada muda, a menos que o usuário que alterou a Data de conclusão planejada também seja o destinatário.</p> <p>Uma notificação é enviada somente se o status do projeto for diferente de Planejamento.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Alteração do status de um problema para o problema atribuído a</p> </td> 
   <td> <p>O status de um dos meus itens de trabalho mudou.</p> <p>O destinatário do problema recebe uma notificação por email quando o status é alterado, a menos que o usuário que alterou o status também seja o destinatário.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento incluído na solicitação de Help Desk parO problema atribuída à</p> </td> 
   <td> <p>Documentos foram adicionados ou alterados na minha requisição.</p> <p>O destinatário do problema recebe uma notificação por email quando os documentos são carregados ou alterados em um problema adicionado.</p> <p>Uma notificação por email não é enviada se o usuário que inseriu o problema for o destinatário.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto tiver a opção "Publicar como fila de solicitações de ajuda" ativada na guia Configuração da fila.&lt;!— DESENHADO EM FLARE: Para obter mais informações sobre como publicar um projeto como uma fila de solicitações de ajuda, consulte 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Visão geral da guia Detalhes da fila em um projeto</a>.

    —>&lt;/p> &lt;/td>
<td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Término de Tarefa para Recurso da Tarefa</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para o usuário atribuído.</p> <p>O Destinatário da Tarefa recebe uma notificação por email quando a tarefa é concluída. As notificações não são enviadas quando uma tarefa pessoal é concluída.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença de Revisão ou Solicitante não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Término de Tarefa para Dependentes da Tarefa</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para os usuários atribuídos primariamente de todas as tarefas dependentes.</p> <p>O destinatário da tarefa recebe uma notificação por email quando um dos antecessores da tarefa for concluído.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>A data de conclusão planejada da tarefa mudou</p> </td> 
   <td> <p>A data de conclusão de uma tarefa atribuída a mim mudou.</p> <p>O Destinatário da Tarefa recebe uma notificação por email quando a Data de Conclusão Planejada da tarefa é alterada, a menos que o usuário que alterou a Data de Conclusão Planejada também seja o Destinatário da Tarefa.</p> <p>Uma notificação é enviada somente se o status do projeto for diferente de Planejamento.</p> <p>Nenhuma notificação é enviada sobre tarefas pessoais.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>O status de tarefa foi alterado para tarefa atribuída a</p> </td> 
   <td> <p>O status é alterado em uma tarefa para a qual fui atribuído.</p> <p>O Destinatário da Tarefa recebe uma notificação por email quando o status da tarefa é alterado, a menos que o usuário que alterou o status também seja o destinatário.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença Review não recebem uma notificação. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informações sobre projetos em que estou

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
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Alteração de status de projeto atual para a equipe do projeto</p> </td> 
   <td> <p>Quando uma status de projeto for alterada de ideia/aprovado/solicitado/em planejamento para atual, enviar email para a equipe.</p> <p>Os usuários do projeto recebem uma notificação por email quando o projeto se torna ativo.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento: Adicionar à equipe do projeto</p> </td> 
   <td> <p>Um documento é adicionado a um projeto no qual estou.</p> <p>Os usuários da equipe do projeto recebem uma notificação por email quando um documento é adicionado ao projeto, exceto para o usuário que adicionou o documento.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e o documento não for Privado. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema adicionado à equipe do projeto</p> </td> 
   <td> <p>Um problema é adicionado a um projeto no qual estou.</p> <p>Os usuários em um projeto recebem uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Término do Problema para a equipe do projeto</p> </td> 
   <td> <p>Quando um problema for concluído enviar email para a equipe.</p> <p>Qualquer usuário do projeto recebe uma notificação.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Término de etapa para a equipe do projeto</p> </td> 
   <td> <p>Uma tarefa de marco é concluída em um projeto no qual estou.</p> <p>Todos os usuários da Equipe do projeto recebem uma notificação quando uma tarefa de marco é concluída. </p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Término de Projeto para a equipe do projeto</p> </td> 
   <td> <p>Quando um projeto for concluído, enviar email para a equipe.</p> <p>Os usuários de uma equipe de projeto recebem uma notificação por email quando o status do projeto é Concluído.</p> <p>Dica: Se os projetos forem concluídos regularmente, ativar essa opção poderá criar muitos emails para usuários que têm um número limitado de tarefas em muitos projetos. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Alteração de status de projeto para a equipe do projeto</p> </td> 
   <td> <p>Quando uma status de projeto for alterado, enviar email para a equipe.</p> <p>Os usuários na Equipe do projeto recebem uma notificação por email quando o status do projeto é alterado. </p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário de Projeto</p> </td> 
   <td> <p>Usuário de Projeto adicionado para Usuário de Projeto</p> </td> 
   <td> <p>Quando um usuário for adicionado à equipe do projeto, enviar email para o usuário.</p> <p>O usuário que foi adicionado ao projeto recebe uma notificação por email quando é adicionado, a menos que o usuário tenha sido adicionado automaticamente ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Término de tarefa para a equipe do projeto</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para a equipe.</p> <p>Os membros da equipe do projeto recebem uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema não Atribuído adicionado à equipe do projeto</p> </td> 
   <td> <p>Um problema não atribuído é adicionado a um projeto no qual estou.</p> <p>Os usuários em um projeto recebem uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informações sobre os projetos que eu possuo

Consulte também [Notificações: Informações sobre os projetos que eu possuo](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de Objeto</th> 
   <th>Evento</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento: Adicionar para o proprietário do projeto</p> </td> 
   <td> <p>Um documento é adicionado a um projeto que eu possuo.</p> <p>O Proprietário do projeto recebe uma notificação por email quando um documento é adicionado ao projeto, a menos que o usuário que adicionou o documento também seja o Proprietário do projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e o documento não for Privado.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema: Adicionar para o proprietário do Projeto</p> </td> 
   <td> <p>Um problema é adicionado a um projeto que eu possuo.</p> <p>O Proprietário do projeto recebe uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Alteração da data de compromisso de um problema para o proprietário do projeto</p> </td> 
   <td> <p>Mudança da data de compromisso de um problema em um dos meus projetos.</p> <p>O Proprietário do projeto recebe uma notificação por email quando a Data da confirmação for alterada para um problema no projeto, a menos que o usuário que alterar a Data da confirmação seja o mesmo usuário que o Proprietário do projeto.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Término de Problema para Proprietário do Projeto</p> </td> 
   <td> <p>Quando um problema for concluído enviar email para o proprietário do projeto.</p> <p>O proprietário do projeto recebe uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Término de Etapa para proprietário de projeto</p> </td> 
   <td> <p>Uma tarefa de marco é concluída em um projeto que eu possuo.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Atribuição de proprietário de projeto para proprietário de projeto</p> </td> 
   <td> <p>Quando o proprietário do projeto mudar ou na criação do projeto, enviar email para o usuário recentemente atribuído.</p> <p>Quando um usuário é atribuído como proprietário de um projeto, ele recebe uma notificação por email.</p> <p>Se o proprietário do projeto for o mesmo usuário que fez a atribuição, uma notificação por email não será enviada</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Alteração de Progresso de Projeto para o Proprietário do Projeto</p> </td> 
   <td> <p>Quando um projeto for alterado de uma status positiva de progresso (no prazo) para uma status negativa de progresso (em atraso), enviar email para o proprietário do projeto.</p> <p>O proprietário do projeto recebe uma notificação por email quando o projeto estiver atrasado.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>A data de compromisso da tarefa para o proprietário do projeto mudou</p> </td> 
   <td> <p>A data de compromisso de uma tarefa em um dos meus projetos mudou.</p> <p>O Proprietário do projeto recebe uma notificação por email quando a Data da confirmação é alterada para uma tarefa no projeto, a menos que o usuário que alterou a Data da confirmação também seja o Proprietário do projeto.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Término de Tarefa para o Proprietário do Projeto</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para o proprietário do projeto.</p> <p>O proprietário do projeto recebe uma notificação. </p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Alteração de Progresso da Tarefa para o Proprietário do Projeto</p> </td> 
   <td> <p>Quando uma tarefa for alterada de uma status de progresso positivo (no prazo) para uma status de progresso negativo (em atraso), enviar email para o proprietário da tarefa.</p> <p>O Proprietário do projeto recebe uma notificação por email quando uma tarefa no projeto fica atrasada.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema não Atribuída Adicionada para o Proprietário do Projeto</p> </td> 
   <td> <p>Um problema não atribuído é adicionado a um projeto que eu possuo.</p> <p>O Proprietário do projeto recebe uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informações sobre projetos que patrocínio

Consulte também [Notificações: Informações sobre projetos que patrocínio](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de Objeto</th> 
   <th>Evento</th> 
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento adicionado para o patrocinador do projeto</p> </td> 
   <td> <p>Um documento é adicionado a um projeto que patrocino.</p> <p>O Patrocinador de projeto recebe uma notificação por email quando um documento é adicionado ao projeto, a menos que o documento seja adicionado pelo Patrocinador de projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o documento não for Privado.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema: Adicionar para o patrocinador do projeto</p> </td> 
   <td> <p>Um problema é adicionado a um projeto que patrocino.</p> <p>O Patrocinador de projeto recebe uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Término de Problema para Patrocinador do Projeto</p> </td> 
   <td> <p>Quando um problema for concluído enviar email para o patrocinador do projeto.</p> <p>O patrocinador do projeto recebe uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Término de etapa para patrocinador do projeto</p> </td> 
   <td> <p>Quando uma etapa for concluída, enviar email para o patrocinador de projeto.</p> <p>O Patrocinador de projeto recebe uma notificação por e-mail quando uma tarefa de marco é concluída em um projeto patrocinado por ele.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Alteração de Progresso do Projeto para o Patrocinador do Projeto</p> </td> 
   <td> <p>Quando um projeto for alterado de uma status de progresso positiva (no prazo) para uma status negativa de progresso (em atraso), enviar email para o patrocinador do projeto.</p> <p>O Patrocinador de projeto recebe uma notificação por email quando o projeto fica atrasado.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Atribuição de Patrocinador de Projeto para Patrocinador de Projeto</p> </td> 
   <td> <p>Quando o patrocinador do projeto mudar ou na criação do projeto, enviar email para o patrocinador recentemente atribuído.</p> <p>O patrocinador do projeto recebe uma notificação por email quando é definido como patrocinador de um projeto.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Término de Tarefa para o Patrocinador do Projeto</p> </td> 
   <td> <p>Quando uma tarefa for concluída, enviar email para o patrocinador do projeto.</p> <p>O patrocinador do projeto recebe uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Alteração no Progresso de Tarefa para o Patrocinador do Projeto</p> </td> 
   <td> <p>Quando uma tarefa for alterada de uma status de progresso positivo (no prazo) para uma status de progresso negativo (em atraso), enviar email para o patrocinador do projeto.</p> <p>O Patrocinador de projeto recebe uma notificação por email quando uma tarefa no projeto fica atrasada.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema não Atribuída adicionada para o Patrocinador do Projeto</p> </td> 
   <td> <p>Quando um problema não atribuída for adicionada enviar email para o patrocinador do projeto.</p> <p>O Patrocinador de projeto recebe uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
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
   <th>Descrição</th> 
   <th> Estado padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aviso</td> 
   <td> <p>A notificação foi adicionada</p> </td> 
   <td> <p>Uma mensagem foi enviada para o Centro de Notificações.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Cancelar solicitação de documento para o solicitante</p> </td> 
   <td> <p>Cancele uma solicitação de carregamento de documento de mim.</p> <p>A Solicitação de documento recebe uma notificação por email quando uma solicitação de documento é cancelada.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Notificação de erro</p> </td> 
   <td> <p>Foi encontrado um erro que necessita da sua atenção.</p> <p>Uma notificação por email é gerada depois que o Workfront tenta e falha ao se conectar a uma conta POP. Após 25 tentativas, o Workfront desativa a conexão com a conta POP para preservar os recursos e envia uma notificação. </p> <p>A notificação por email é enviada ao Proprietário do projeto, se o email POP estiver associado a uma fila de solicitações ou aos administradores do Workfront, se a conta POP estiver associada ao recurso "Email de entrada" na Configuração de email.
     <!--
      DRAFTED IN FLARE:
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      --></p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Atribuição de Problema para Proprietário do Recurso</p> </td> 
   <td> <p>Quando uma atribuição de problema for alterada, enviar email para o proprietário do recurso.</p> <p>O Gerenciador de destinatários da ocorrência recebe uma notificação por email quando uma alteração afeta um usuário que gerencia.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário</p> </td> 
   <td> <p>Novo Usuário para Usuário</p> </td> 
   <td> <p>Quando um novo usuário for criado no Workfront, enviar email para o usuário.</p> <p>Depois que o novo usuário é criado, ele recebe um convite por email, notificando-o de que uma conta do Workfront foi criada e solicitando que defina sua senha.</p> <p>Ao criar um novo usuário, os usuários podem selecionar a opção "Enviar um email de convite para essa pessoa" (conforme descrito em <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Adicionar usuários</a><span style="font-weight: 400;">). No entanto, quando a opção "Novo usuário para usuário" é ativada globalmente, todos os novos usuários recebem o convite por email independentemente da opção "Enviar um email de convite para essa pessoa" estar selecionada.</span></p> </td> 
   <td> Inativo </td> 
  </tr> 
  <tr> 
   <td> <p>Equipe</p> </td> 
   <td> <p>Objeto - Compartilhar com a Equipe</p> </td> 
   <td> <p>Alguém compartilhar um objeto com minha equipe.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário</p> </td> 
   <td> <p>Objeto - Compartilhar com o Usuário</p> </td> 
   <td> <p>Alguém compartilhar um objeto comigo.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário de Projeto</p> </td> 
   <td> <p>Adicionar Usuário no Projeto para Proprietário do Recurso</p> </td> 
   <td> <p>Quando um usuário for adicionado à equipe do projeto, enviar email para o proprietário do recurso.</p> <p>Um gerente recebe uma notificação por email quando um de seus relatórios diretos é adicionado a um projeto.</p> <p>Os usuários com uma licença Review não recebem uma notificação.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>Projeto adicionado ao portfólio ou programa</p> </td> 
   <td> <p>Alguém adicionar um projeto a um portfólio ou programa que possuo.</p> </td> 
   <td> <p>Ativo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa</p> </td> 
   <td> <p>Atribuição de Tarefa para o Proprietário do Recurso</p> </td> 
   <td> <p>Quando uma atribuição primária de uma tarefa for alterada, enviar email para o proprietário do recurso.</p> <p>O Gerenciador do Destinatário da Tarefa recebe uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> </td> 
   <td> <p>Inativo</p> </td> 
  </tr> 
  <tr> 
   <td> Projeto <br>Tarefa <br>Problema</td> 
   <td>Nova atualização para assinante </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Um e-mail é enviado quando uma atualização é feita em uma tarefa, problema ou projeto ao qual eu estou inscrito.</span> </p> </td> 
   <td>Ativo</td> 
  </tr> 
 </tbody> 
</table>

## Delegação

Consulte também [Notificações: Delegação](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Tipo de Objeto | Evento | Descrição | Estado padrão |
|------------------|---------------------------------------------|--------------------------------------------------------------|---------------|
| Tarefas e problemas | Delegação de tarefas e problemas à pessoa designada | Delego minhas tarefas e problemas (confirmação) | Ativo |
| Tarefas e problemas | Interromper delegação de tarefa e problemas à pessoa designada | Interrompo a delegação de minhas tarefas e problemas (confirmação) | Ativo |
| Tarefas e problemas | Delegação de tarefas e problemas à pessoa delegada | Alguém delega suas tarefas e problemas para mim | Ativo |
| Tarefas e problemas | Parar tarefas e emitir delegação para delegar | Alguém interrompe a delegação de suas tarefas e problemas para mim | Ativo |
