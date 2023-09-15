---
content-type: reference
navigation-topic: notifications
title: "Notificações: solicitações que fiz"
description: As notificações a seguir informam sobre solicitações feitas no Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 7%

---

# Notificações: Solicitações que fiz

As notificações a seguir informam sobre solicitações feitas no [!DNL Adobe Workfront].

Para obter informações sobre como configurar as notificações recebidas, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte também [Notificações de eventos](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Solicitações que eu fiz</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de aprovação de documento foi concluída</strong> </p> <p>O usuário que solicitou uma aprovação para um documento recebe uma notificação por email quando a solicitação de aprovação de documento é concluída.</p> <p>O assunto do email de notificação instantânea é:<em> &lt;approver name=""&gt; tem &lt;approval decision="" uicontrol="" approved="" uicontrol="" approved="" with="" changes="" uicontrol="" rejected=""&gt; neste documento.</em></p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </td> 
   <td> Nome do documento<br>Nome do aprovador </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um documento foi alterado ou caregado sobre um problema para o qual sou o contato primário</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando um documento é carregado ou alterado no problema, a menos que o usuário que carregou ou alterou o documento também seja o contato principal.</p> <p>Uma notificação só será enviada se o projeto estiver configurado como uma [!UICONTROL Fila de Solicitações de Ajuda] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma Fila de Solicitações]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>Documento adicionado a &lt;issue name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é: <em>Resumo de suas solicitações &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do objeto no qual o documento foi carregado<br>Nome do objeto pai<br>Número de Referência do Documento<br>Nome do usuário que carregou o documento<br>Nome do documento<br>Adicionado na data<br>Detalhes do documento (formato, tamanho, número da versão)<br>Miniatura do documento<br><strong>[!UICONTROL Visualizar]</strong> e <strong>[!UICONTROL Baixar]</strong> botões<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de documentos carregados<br>*Nome do documento<br>*Nome do objeto pai<br>*Nome do usuário que adicionou o documento<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de carregamento de documento foi atendida</strong> </p> <p>O Solicitante de documentos recebe uma notificação por email quando uma solicitação de upload de documento é atendida.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Sua solicitação de documento de] &lt;user name=""&gt; foi cumprido</em></p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </td> 
   <td> <p>Nome do usuário que carregou o documento<br>Nome do objeto no qual o documento foi carregado<br>Nome do documento<br><br></p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma tarefa pessoal que eu atribuí a outra pessoa foi concluída</strong> </p> <p>Uma notificação é enviada ao usuário que atribuiu uma tarefa ad-hoc a outra pessoa quando essa tarefa for concluída. </p> <p>Para obter mais informações sobre tarefas ad hoc, consulte <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Criar itens de trabalho da área [!UICONTROL Home]</a>.</p> <p>O assunto do email de notificação instantânea é: <em>Conclusão da tarefa: &lt;task name=""&gt;</em></p> <p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </p> </td> 
   <td> Nome da tarefa<br>Nome do projeto padrão (Projeto pessoal do usuário que recebeu a tarefa pessoal)<br>Número de Referência da Tarefa<br>Nome do proprietário da tarefa<br>Novo Status de Tarefa<br>Data e hora em que a tarefa foi concluída<br>Status da tarefa anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br><br><br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for concluído enviar email para o originador do problema</strong> </p> <p>O contato principal sobre um problema recebe uma notificação quando o problema é concluído.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Conclusão de Problema]: &lt;issue name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> Resumo de suas solicitações &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> Nome do problema<br>Nome do projeto<br>Número de referência da edição<br>Nome do usuário que concluiu o problema<br>Novo Status<br>Data e hora em que o problema foi concluído<br>Status do problema anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão <br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de problemas concluídos<br>*Nome do problema<br>*Nome do usuário que concluiu o problema<br>*Data do resumo diário </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for adicionada enviar email para o originador do problema.</strong> </p> <p>O contato principal em um problema recebe uma notificação quando adiciona um problema em um projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Problema enviado]: &lt;issue name=""&gt; em &lt;project name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> Resumo de suas solicitações &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de referência da edição<br>Seu nome<br>Nome do problema<br>Data inserida<br>Prioridade do problema<br>Status do Problema<br>Atribuído a nome<br>Contato Primário<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados<br>*Nome do problema<br>*Data do resumo diário </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma solicitação de Help Desk é incluída, enviar email para o originador do problema.</strong> </p> <p>O contato principal sobre o problema recebe uma notificação por email quando envia um problema.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual] e se o projeto estiver configurado como uma [!UICONTROL Fila de Solicitações de Ajuda] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma Fila de Solicitações]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>[!Solicitação de UICONTROL Enviada]: &lt;request name=""&gt; em &lt;project request="" queue="" name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> Resumo de suas solicitações &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do projeto (nome da fila de solicitações)<br>Nome do Portfolio<br>Número de referência da edição<br>Nome do problema<br>Data inserida<br>Prioridade do problema<br>Status do Problema<br>Atribuído a nome<br>Contato Primário<br>*Número de Referência do Projeto<br>*Nome do projeto<br>*Número total de solicitações enviadas<br>*Nome da solicitação<br>*Prioridade de solicitação<br>*Data do resumo diário</p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma solicitação de Help Desk é fechada, enviar email para o originador do problema.</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando a solicitação é fechada.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual e se o projeto estiver configurado como uma [!UICONTROL Fila de Solicitações de Ajuda] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a>).</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Sua solicitação foi fechada]:"&lt;request name=""&gt;"</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo de suas Solicitações] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da solicitação<br>Nome do projeto<br>Número de Referência da Solicitação<br>Nome do usuário que fechou a solicitação<br>Status do Problema<br>Data e hora em que a solicitação foi fechada<br>Status da solicitação anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Número de Referência do Projeto<br>*Nome do projeto<br>*Número total de solicitações fechadas<br>*Nome da solicitação<br>*Nome do usuário que encerrou a solicitação<br>*Data do resumo diário </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma solicitação de Help Desk é atribuída, enviar email para o originador do problema.</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando um usuário é atribuído ao problema, a menos que o contato principal e o usuário atribuído sejam o mesmo usuário.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual e se o projeto estiver configurado como uma [!UICONTROL Fila de Solicitações de Ajuda] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma Fila de Solicitações]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL foi atribuído à sua solicitação]: "&lt;request name=""&gt;"</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo de suas Solicitações] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do problema<br>Nome do projeto<br>Número de referência da edição<br>Nome da solicitação<br>Tipo de solicitação<br>Data inserida<br>Prioridade do problema<br>Contato Primário<br>Data de Término Planejada<br>Status do Problema<br><strong>Ver mais detalhes</strong> botão <br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de solicitações atribuídas<br>*Nome da solicitação<br>*Atribuído a nome<br>*Data do resumo diário</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma status de projeto for alterado, enviar email para o usuário que cadastrou o projeto</strong> </p> <p>O usuário que criou o projeto recebe uma notificação por email quando o status do projeto é alterado.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de Status de Projeto]: &lt;project name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo de suas Solicitações] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que alterou o status<br>Novo Status<br>Data e hora em que o status do projeto foi alterado<br>Status do projeto anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Novo status do projeto<br>*Nome do usuário que alterou o status do projeto<br>*Data do resumo diário</p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando a status é alterado em uma solicitação de Help Desk, enviar email ao originador do problema.</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando o status do problema é alterado, a menos que o usuário que alterou o status também seja o contato principal.</p> <p>Uma notificação só será enviada se o status do projeto for Atual e o projeto estiver configurado como uma [!UICONTROL Fila de Solicitações de Ajuda] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma Fila de Solicitações]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>&lt;request name=""&gt; é &lt;new status=""&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> Resumo de suas solicitações &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da solicitação<br>Nome do projeto<br>Número de Referência da Solicitação<br>Nome do usuário que alterou o Status da Solicitação<br>Novo Status<br>Data e hora em que o status da solicitação foi alterado<br>Status da solicitação anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de solicitações cujo status foi alterado<br>*Nome da solicitação<br>*Status da solicitação anterior<br>*Novo status de solicitação<br>*Nome do usuário que alterou o status<br>*Data do resumo diário<br></td> 
   <td> <p><strong>Diariamente</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
