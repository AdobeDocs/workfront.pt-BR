---
content-type: reference
navigation-topic: notifications
title: "Notificações: Informações sobre o trabalho que me é atribuído"
description: As notificações a seguir alertam sobre atividades que ocorrem em um item de trabalho atribuído a você.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 39ba9e93a8597d4354472a19b1ac1c5f530f4398
workflow-type: tm+mt
source-wordcount: '2092'
ht-degree: 6%

---

# Notificações: Informações sobre o trabalho que me foi atribuído

As notificações a seguir alertam sobre atividades que ocorrem em um item de trabalho atribuído a você.

Para obter informações sobre como configurar quais notificações você recebe, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte também [Notificações de evento](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificação</th> 
   <th> <p>Campos incluídos </p> <p> *Somente campos de resumo diário</p> </th> 
   <th>Status padrão</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>Um predecessor de uma tarefa atribuída à minha equipe foi concluído</strong> </p> <p>A equipe atribuída recebe uma notificação por email quando um antecessor de uma de suas tarefas é concluído. </p> <p>Os usuários com uma licença do [!UICONTROL Review] ou Re[!UICONTROL Requestor]questor não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>Concluído: &lt;task name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo do trabalho atribuído a você] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome da tarefa do antecessor<br>Projeto de Tarefa Antecessora<br>Número de Referência da Tarefa Antecessora<br>Nome do usuário que concluiu a tarefa antecessora<br>Status da tarefa antecessora<br>Data e hora em que o antecessor foi concluído<br>Status anterior da tarefa antecessora<br><strong>Veja mais detalhes</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de predecessores concluídos<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data da compilação diária </p> </td> 
   <td><strong>Diariamente</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Quando uma tarefa for concluída, enviar email para os usuários atribuídos primariamente de todas as tarefas dependentes</strong> </p> <p>O destinatário da tarefa recebe uma notificação por email quando um antecessor de uma de suas tarefas é concluído. </p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL concluído]: &lt;task name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo do trabalho atribuído a você] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome da tarefa do antecessor<br>Projeto de Tarefa Antecessora<br>Número de Referência da Tarefa Antecessora<br>Nome do usuário que concluiu a tarefa antecessora<br>Status da tarefa antecessora<br>Data e hora em que o antecessor foi concluído<br>Status anterior da tarefa antecessora<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de predecessores concluídos<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data da compilação diária </p> </td> 
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
   <td> <p><strong>Quando uma aprovação de tarefa for realizada, enviar email para o usuário atribuído</strong> </p> <p>O destinatário da tarefa recebe uma notificação por email quando a tarefa é aprovada ou rejeitada.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL concluído]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo do trabalho atribuído a você] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concedeu a aprovação<br>Novo Status da Tarefa<br>Data e hora em que a tarefa foi aprovada ou rejeitada<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas aprovadas ou rejeitadas<br>*Nome da tarefa<br>*Nome do usuário que aprovou ou rejeitou a tarefa<br>*Decisão De Aprovação ([!UICONTROL Aprovado]/ [!UICONTROL Rejeitado])<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Quando uma tarefa for concluída, enviar email para o usuário atribuído</strong> </p> <p>O Destinatário da Tarefa recebe uma notificação por email quando a tarefa é concluída.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL concluído]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>Observação: Se a tarefa for alterada para um status que seja igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "Concluído".</p> </p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo do trabalho atribuído a você] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Data e hora em que a tarefa foi concluída<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas concluídas<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Todos os predecessores de uma tarefa atribuída à minha equipe foram concluídos</strong> </p> <p>A equipe atribuída recebe uma notificação por email quando um antecessor de uma de suas tarefas é marcado como concluído.</p> <p>Os usuários com uma licença de Revisão ou Solicitante não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>Tarefa concluída: &lt;name&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> Resumo do trabalho atribuído a você &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome da tarefa<br>Projeto de tarefa<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa antecessora<br>Status da tarefa antecessora<br>Data e hora em que o antecessor foi concluído<br>Status anterior da tarefa antecessora<br><strong>Veja mais detalhes</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas concluídas<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data da compilação diária </td>
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
   <td> <p><strong>Quando todas as predecessoras forem concluídas enviar email para os usuários primariamente atribuídos de todas as tarefas dependentes</strong> </p> <p>O destinatário da tarefa recebe uma notificação por email para cada antecessor concluído.</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL concluído]: &lt;task name=""&gt;</em><br></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo do trabalho atribuído a você] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome da tarefa<br>Projeto de tarefa<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa antecessora<br>Status da tarefa antecessora<br>Data e hora em que o antecessor foi concluído<br>Status anterior da tarefa antecessora<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas concluídas<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data da compilação diária </td> 
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
   <td> <p><strong>Quando um problema é aprovada ou rejeitada, envie email para o usuário atribuído</strong> </p> <p>O destinatário de um problema recebe uma notificação por email quando uma decisão de aprovação é tomada (aprovada ou rejeitada).</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>Emissão de Aprovação Pendente: &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; em &lt;project name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> Resumo do trabalho atribuído a você &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome do problema<br>Nome do projeto<br>Número de referência da emissão<br>Nome do usuário que aprovou ou rejeitou o problema<br>Decisão de aprovação (aprovada ou rejeitada)<br>Status do problema<br>Nome do usuário que solicitou a aprovação<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas aprovados ou rejeitados<br>*Nome da ocorrência<br>*Nome do usuário que aprovou ou rejeitou o problema<br>*Decisão de aprovação (aprovada ou rejeitada)<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Quando um problema for concluído enviar email para o usuário atribuído</strong> </p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>Concluído: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p><em> O objeto da notificação diária de resumo é: Resumo do trabalho atribuído a você &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> Nome do problema<br>Nome do projeto<br>Número de referência da emissão<br>Nome do usuário que concluiu o problema<br>Status da nova ocorrência<br>Data e hora em que o problema foi concluído<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas concluídos<br>*Nome da ocorrência<br>*Nome do usuário que concluiu o problema<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Documentos foram adicionados ou alterados na minha requisição</strong> </p> <p>O destinatário do problema recebe uma notificação por email quando os documentos são carregados ou os detalhes do documento são alterados em um problema adicionado.</p> <p>Uma notificação por email não é enviada se o usuário que acionou o problema for o destinatário do problema.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] e se o projeto estiver configurado como uma Fila de solicitação de ajuda (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a>).</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Documento adicionado ao] &lt;request name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo do trabalho atribuído a você] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome da solicitação<br>Nome do projeto (Nome da fila de solicitações)<br>Número de referência do documento <br>Nome do usuário que carregou o documento<br>Nome do documento <br>Adição Na Data<br>Detalhes do documento (formato, tamanho, número da versão)<br>Miniatura do documento<br><strong>[!UICONTROL Preview]</strong> e <strong>[!UICONTROL Download]</strong> botões<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de documentos carregados ou alterados<br>*Nome do documento<br>*Nome do objeto<br>*Nome do usuário que carregou o documento<br>*Data da compilação diária</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A data de conclusão de uma tarefa atribuída a mim mudou</strong> </p> <p>O Destinatário da Tarefa recebe uma notificação por email quando a [!UICONTROL Data de Conclusão Planejada] da tarefa é alterada, a menos que o usuário que alterou a Data de Conclusão Planejada também seja o Destinatário da Tarefa.</p> <p>Uma notificação é enviada somente se o status do projeto for diferente do [!UICONTROL Planning].</p> <p>Nenhuma notificação é enviada sobre tarefas pessoais.</p> <p> Os usuários com uma licença de Revisão ou Solicitante não recebem uma notificação. </p> <p> O assunto do email de notificação instantânea é: <em>[!UICONTROL Data de vencimento foi alterada.]</em></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo do trabalho atribuído a você] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nova Data de Vencimento ([!UICONTROL Data de Conclusão Planejada])<br>Data e Hora em que a Data de Vencimento foi alterada<br>O nome do usuário que alterou a Data de Vencimento<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas em que a Data de Vencimento (Data de Conclusão Planejada) foi alterada<br>*Nome da tarefa<br>*Nova Data de Conclusão Planejada<br>*Nome do usuário que alterou a Data de Vencimento<br>*Data da compilação diária </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A data de conclusão de um problema atribuído a mim mudou</strong> </p> <p>O destinatário do problema recebe uma notificação por email quando a [!UICONTROL Data de conclusão planejada] é alterada, a menos que o usuário que alterou a [!UICONTROL Data de conclusão planejada] também seja o destinatário.</p> <p>Uma notificação é enviada somente se o status do projeto for diferente do [!UICONTROL Planning].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Data de vencimento foi alterada]</em></p> <p> </p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo do trabalho atribuído a você] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do problema<br>Nome do projeto<br>Número de referência da emissão<br>Nova Data de Vencimento ([!UICONTROL Data de Conclusão Planejada])<br>Data e Hora em que a data de vencimento foi alterada<br>Nome do usuário que alterou a data de vencimento<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas em que a Data de Vencimento ([!UICONTROL Data de Conclusão Planejada]) foi alterada<br>*Nome da ocorrência<br>*Nova [!UICONTROL Data de conclusão planejada]<br>*Nome do usuário que alterou a Data de Vencimento<br>*Data do resumo diário<br></p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>O status é alterado em uma tarefa para a qual fui atribuído</strong> <p>O Destinatário da Tarefa recebe uma notificação por email quando o status da tarefa é alterado, a menos que o usuário que alterou o status também seja o destinatário.</p> <p>Observação: Esta notificação não é enviada quando o status da tarefa é alterado para concluído. Uma notificação separada é usada para tarefas concluídas. Consulte <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Uma tarefa à qual estou atribuído está concluída</a>, acima.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;task name=""&gt; from &lt;project name=""&gt; é &lt;new status=""&gt;</em></p> <p> </p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo do trabalho atribuído a você] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que alterou o status<br>Novo status<br>Data e hora em que o status foi alterado<br>Status da visualização<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas em que o Status foi alterado<br>*Nome da tarefa<br>*Status da tarefa anterior<br>*Novo Status da Tarefa<br>*Nome do usuário que alterou o Status<br>*Data do resumo diário<br></td> 
   <td><strong>[!UICONTROL diariamente]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>O status de um dos meus itens de trabalho mudou</strong> </p> <p>Você recebe uma notificação por email quando o status é alterado em um problema ao qual está atribuído, a menos que você mesmo altere o status. </p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;issue name=""&gt; from &lt;project name=""&gt; é &lt;new status=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo do trabalho atribuído a você] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome do problema<br>Nome do projeto<br>Número de referência da emissão<br>Nome do usuário que alterou o status<br>Novo status<br>Data e hora em que o status foi alterado<br>Status do problema anterior<br><strong>Veja mais detalhes</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas em que o Status foi alterado<br>*Nome da tarefa<br>*Status do problema anterior<br>*Status da nova ocorrência<br>*Nome do usuário que alterou o Status<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
 </tbody> 
</table>
