---
content-type: reference
navigation-topic: notifications
title: 'Notificações: Informações sobre o trabalho atribuído a mim'
description: As notificações a seguir alertam sobre atividades que ocorrem em um item de trabalho atribuído a você.
author: Courtney
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 1%

---

# Notificações: Informações sobre o trabalho atribuído a mim

As notificações a seguir alertam sobre atividades que ocorrem em um item de trabalho atribuído a você.

Para obter informações sobre como configurar as notificações recebidas, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Um predecessor de uma tarefa atribuída à minha equipe foi concluído</strong> </p> <p>A equipe atribuída recebe uma notificação por email quando uma predecessora de uma de suas tarefas é concluída. </p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>Concluído: &lt;Nome da Tarefa&gt;</em></p> <p> O assunto da notificação do resumo diário é: <em> [!UICONTROL Resumo do Trabalho Atribuído a Você] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome da Tarefa Predecessora<br>Projeto da Tarefa Predecessora<br>Número de Referência da Tarefa Predecessora<br>Nome do usuário que concluiu a tarefa predecessora<br>Status da tarefa predecessora<br>Data e Hora de conclusão da predecessora<br>Status Anterior da tarefa predecessora<br><strong>Botão Mais Detalhes</strong><br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de predecessores concluídos<br>*Nome da Tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário </p> </td> 
   <td><strong>Diariamente</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Quando uma tarefa for concluída, enviar email para os usuários atribuídos primariamente de todas as tarefas dependentes</strong> </p> <p>O destinatário da tarefa recebe uma notificação por email quando um predecessor de uma de suas tarefas é concluído. </p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;Nome da Tarefa&gt;</em></p> <p> O assunto da notificação do resumo diário é: <em> [!UICONTROL Resumo do Trabalho Atribuído a Você] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome da Tarefa Predecessora<br>Projeto da Tarefa Predecessora<br>Número de Referência da Tarefa Predecessora<br>Nome do usuário que concluiu a tarefa predecessora<br>Status da tarefa predecessora<br>Data e Hora de conclusão da predecessora<br>Status Anterior da tarefa predecessora<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de predecessores concluídos<br>*Nome da Tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário </p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>Uma tarefa que concluí foi aprovada ou rejeitada</strong> </p> <p>O destinatário da tarefa recebe uma notificação por e-mail quando a tarefa é aprovada ou rejeitada.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;Nome da Tarefa&gt; em &lt;Nome do Projeto&gt;</em></p> <p> O assunto da notificação do resumo diário é: <em> [!UICONTROL Resumo do Trabalho Atribuído a Você] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concedeu a aprovação<br>Novo Status da Tarefa<br>Data e Hora em que a tarefa foi aprovada ou rejeitada<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas aprovadas ou rejeitadas<br>*Nome da Tarefa<br>*Nome do usuário que aprovou ou rejeitou a tarefa<br>*Decisão de Aprovação ([!UICONTROL Approved]/ [!UICONTROL Rejeitado])<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Uma tarefa à qual estou atribuído foi concluída</strong> </p> <p>O Destinatário da tarefa recebe uma notificação por e-mail quando a tarefa é concluída.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;Nome da Tarefa&gt; em &lt;Nome do projeto&gt;</em></p> <p> <p>Observação: se a tarefa for alterada para um status que equivale a [!UICONTROL Concluído], o assunto do email ainda exibirá "Concluído".</p> </p> <p> O assunto da notificação do resumo diário é: <em> [!UICONTROL Resumo do Trabalho Atribuído a Você] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome da Tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Data e Hora de conclusão da tarefa<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas<br>*Nome da Tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Todos os predecessores de uma tarefa atribuída à minha equipe foram concluídos</strong> </p> <p>A equipe atribuída recebe uma notificação por email quando uma predecessora de uma de suas tarefas é marcada como concluída.</p> <p>Os usuários com uma licença de Revisão ou Solicitante não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>Tarefa Concluída: &lt;Nome&gt;</em></p> <p> O assunto da notificação do resumo diário é: <em> Resumo do trabalho atribuído a você &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome da Tarefa<br>Projeto da Tarefa<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa predecessora<br>Status da tarefa predecessora<br>Data e Hora de conclusão da predecessora<br>Status Anterior da tarefa predecessora<br><strong>Botão Ver Mais Detalhes</strong><br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas<br>*Nome da Tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário </td>
   <td><strong>Instantâneo</strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Todas as predecessoras de minhas tarefas foram concluídas</strong> </p> <p>O destinatário da tarefa recebe uma notificação por email para cada predecessora que foi concluída.</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;Nome da Tarefa&gt;</em><br></p> <p> O assunto da notificação do resumo diário é: <em> [!UICONTROL Resumo do Trabalho Atribuído a Você] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome da Tarefa<br>Projeto da Tarefa<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa predecessora<br>Status da tarefa predecessora<br>Data e Hora de conclusão da predecessora<br>Status Anterior da tarefa predecessora<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas<br>*Nome da Tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Um problema que resolvi foi aprovado ou rejeitado</strong> </p> <p>O destinatário de um problema recebe uma notificação por email quando uma decisão de aprovação é tomada (aprovada ou rejeitada).</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>Problema Pendente de Aprovação: &lt;Data de Início Planejada&gt; &lt;Número de Referência do Problema&gt; - &lt;Nome do Problema&gt; em &lt;Nome do Projeto&gt;</em></p> <p> O assunto da notificação do resumo diário é: <em> Resumo do trabalho atribuído a você &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nome do usuário que aprovou ou rejeitou o problema<br>Decisão de Aprovação (Aprovada ou Rejeitada)<br>Status do Problema<br>Nome do usuário que solicitou a aprovação<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas aprovados ou rejeitados<br>*Nome do Problema<br>*Nome do usuário que aprovou ou rejeitou o problema<br>*Decisão de Aprovação (Aprovada ou ou Rejected)<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Um problema ao qual estou atribuído foi concluído</strong> </p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>Concluído: &lt;Nome do Problema&gt; em &lt;Nome do Projeto&gt;</em></p> <p><em> O assunto da notificação do resumo diário é: Resumo do trabalho atribuído a você &lt;Data do resumo diário&gt; </em> </p> </td> 
   <td> Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nome do usuário que concluiu o problema<br>Novo Status do Problema<br>Data e Hora de conclusão do problema<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas concluídos<br>*Nome do Problema<br>*Nome do usuário que concluiu o problema<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Documentos foram carregados ou alterados nas solicitações às quais estou atribuído</strong> </p> <p>O destinatário da ocorrência recebe uma notificação por email quando os documentos são carregados ou os detalhes do documento são alterados em uma ocorrência que ele adicionou.</p> <p>Uma notificação por email não é enviada se o usuário que acionou o problema for o destinatário do problema.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] e se o projeto estiver configurado como uma Fila de Solicitações de Ajuda (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma Fila de Solicitações</a>).</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Documento adicionado a] &lt;Nome da Solicitação&gt;</em></p> <p> O assunto da notificação do resumo diário é: <em> [!UICONTROL Resumo do Trabalho Atribuído a Você] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome da Solicitação<br>Nome do Projeto (Nome da Fila de Solicitações)<br>Número de Referência do Documento <br>Nome do usuário que carregou o documento<br>Nome do Documento <br>Adicionado na Data<br>Detalhes do Documento (formato, tamanho, número da Versão)<br>Miniatura do Documento<br><strong>[!UICONTROL Visualização]</strong> e <strong>[!UICONTROL Download]</strong> botões<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de documentos carregados ou alterados<br>*Documento Nome<br>*Nome do Objeto<br>*Nome do usuário que carregou o documento<br>*Data do resumo diário</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A data de conclusão de uma tarefa atribuída a mim mudou</strong> </p> <p>O Destinatário da tarefa recebe uma notificação por e-mail quando a [!UICONTROL Data de conclusão planejada] da tarefa é alterada, a menos que o usuário que alterou a Data de conclusão planejada também seja o Destinatário da tarefa.</p> <p>Uma notificação só será enviada se o status do projeto for diferente de [!UICONTROL Planning].</p> <p>Nenhuma notificação é enviada sobre tarefas pessoais.</p> <p> Os usuários com uma licença de Revisão ou Solicitante não recebem uma notificação. </p> <p> O assunto do email de notificação instantânea é: <em>[!UICONTROL A Data de Conclusão foi alterada.]</em></p> <p> O assunto da notificação do resumo diário é: <em> [!UICONTROL Resumo do Trabalho Atribuído a Você] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Nova Data de Vencimento ([!UICONTROL Data de Conclusão Planejada])<br>Data e Hora em que a Data de Conclusão foi alterada<br>Nome do usuário que alterou a Data de Conclusão Planejada<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas em que a Data de Conclusão Planejada (Data de Conclusão Planejada) foi alterada<br>*Nome da Tarefa<br>*Nova Data de Conclusão Planejada<br>*Nome do usuário que alterou a Data de Conclusão diária<br>*Data de resumo diária </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A data de conclusão de um problema atribuído a mim</strong> mudou </p> <p>O destinatário do problema recebe uma notificação por email quando a [!UICONTROL Data de conclusão planejada] é alterada, a menos que o usuário que alterou a [!UICONTROL Data de conclusão planejada] também seja o destinatário.</p> <p>Uma notificação só será enviada se o status do projeto for diferente de [!UICONTROL Planning].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Data de Conclusão foi alterada]</em></p> <p> </p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo do Trabalho Atribuído a Você] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> <p>Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nova Data de Vencimento ([!UICONTROL Data de Conclusão Planejada])<br>Data e Hora em que a data de vencimento foi alterada<br>Nome do usuário que alterou a data de vencimento<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas em que a Data de Vencimento ([!UICONTROL Data de Conclusão Planejada]) foi alterada<br>*Nome do Problema<br>*Nova [!UICONTROL Data de Conclusão Planejada]<br>*Nome do usuário alterou a Data de Vencimento<br>*Data do resumo diário<br></p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>O status é alterado em uma tarefa para a qual estou atribuído</strong> <p>O Destinatário da tarefa recebe uma notificação por e-mail quando o status da tarefa é alterado, a menos que o usuário que alterou o status também seja o destinatário.</p> <p>Observação: esta notificação não é enviada quando o status da tarefa é alterado para concluído. Uma notificação separada é usada para tarefas concluídas. Consulte <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Uma tarefa à qual estou atribuído foi concluída</a>, acima.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;Nome da Tarefa&gt; de &lt;Nome do Projeto&gt; é &lt;Novo Status&gt;</em></p> <p> </p> <p> O assunto da notificação do resumo diário é: <em> [!UICONTROL Resumo do Trabalho Atribuído a Você] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Nome do usuário que alterou o status<br>Novo Status<br>Data e Hora em que o status foi alterado<br>Status de Visualização<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas em que o Status foi alterado<br>*Nome da Tarefa<br>*Status da Tarefa Anterior<br>*Novo Status da Tarefa<br>*Nome do usuário que alterou o Status<br>*Data resumo diário<br></td> 
   <td><strong>[!UICONTROL Diário]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>O status é alterado em um dos meus itens de trabalho</strong> </p> <p>Você recebe uma notificação por email quando o status é alterado em um problema para o qual você está atribuído, a menos que você mesmo altere o status. </p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;Nome do Problema&gt; de &lt;Nome do Projeto&gt; é &lt;Novo Status&gt;</em></p> <p> O assunto da notificação do resumo diário é: <em> [!UICONTROL Resumo do Trabalho Atribuído a Você] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nome do usuário que alterou o status<br>Novo Status<br>Data e Hora em que o status foi alterado<br>Status do Problema Anterior<br><strong>Ver Mais Detalhes</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas em que o Status foi alterado<br>*Nome da Tarefa<br>*Status do Problema Anterior<br>*Novo Status de Problema<br>*Nome do usuário que alterou o Status<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
 </tbody> 
</table>
