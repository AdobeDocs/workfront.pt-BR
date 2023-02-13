---
content-type: reference
navigation-topic: notifications
title: "Notificações: Pedidos que fiz"
description: As notificações a seguir informam sobre solicitações que você fez no Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 6%

---

# Notificações: Solicitações que fiz

As notificações a seguir informam sobre as solicitações feitas em [!DNL Adobe Workfront].

Para obter informações sobre como configurar quais notificações você recebe, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte também [Notificações de evento](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Solicitações que eu fiz</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de aprovação de documento foi concluída</strong> </p> <p>O usuário que solicitou uma aprovação em um documento recebe uma notificação por email quando a solicitação de aprovação do documento é concluída.</p> <p>O assunto do email de notificação instantânea é:<em> &lt;approver name=""&gt; has &lt;approval decision="" uicontrol="" approved="" uicontrol="" approved="" with="" changes="" uicontrol="" rejected=""&gt; este documento.</em></p> <p>Observação: Não é possível configurar essa notificação para um email de resumo diário.</p> </td> 
   <td> Nome do documento<br>Nome do Aprovador </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um documento foi alterado ou caregado sobre um problema para o qual sou o contato primário</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando um documento é carregado ou alterado no problema, a menos que o usuário que carregou ou alterou o documento também seja o contato principal.</p> <p>Uma notificação é enviada somente se o projeto estiver configurado como uma [!UICONTROL Help Request Queue] (Fila de solicitação de ajuda) (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma fila de solicitações]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>Documento adicionado a &lt;issue name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é: <em>Resumo de suas solicitações &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do objeto no qual o documento foi carregado<br>Nome do objeto pai<br>Número de referência do documento<br>Nome do usuário que carregou o documento<br>Nome do documento<br>Adição Na Data<br>Detalhes do documento (formato, tamanho, número da versão)<br>Miniatura do documento<br><strong>[!UICONTROL Preview]</strong> e <strong>[!UICONTROL Download]</strong> botões<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de documentos carregados<br>*Nome do documento<br>*Nome do objeto pai<br>*Nome do usuário que adicionou o documento<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de carregamento de documento foi atendida</strong> </p> <p>O Solicitante de documento recebe uma notificação por email quando uma solicitação de carregamento de documento é atendida.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Sua solicitação de documento do] &lt;user name=""&gt; foi cumprido</em></p> <p>Observação: Não é possível configurar essa notificação para um email de resumo diário.</p> </td> 
   <td> <p>Nome do usuário que carregou o documento<br>Nome do objeto no qual o documento foi carregado<br>Nome do documento<br><br></p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma tarefa pessoal que eu atribuí a outra pessoa foi concluída</strong> </p> <p>Uma notificação é enviada ao usuário que atribuiu uma tarefa ad-hoc a outra pessoa quando essa tarefa é concluída. </p> <p>Para obter mais informações sobre tarefas ad hoc, consulte <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Criar itens de trabalho na área [!UICONTROL Início]</a>.</p> <p>O assunto do email de notificação instantânea é: <em>Conclusão da tarefa: &lt;task name=""&gt;</em></p> <p> <p>Observação: Não é possível configurar essa notificação para um email de resumo diário.</p> </p> </td> 
   <td> Nome da tarefa<br>Nome do Projeto Padrão (Projeto Pessoal do usuário que recebeu a tarefa pessoal)<br>Número de Referência da Tarefa<br>Nome do Proprietário da Tarefa<br>Novo Status da Tarefa<br>Data e hora em que a tarefa foi concluída<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br><br><br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for concluído enviar email para o originador do problema</strong> </p> <p>O contato principal em um problema recebe uma notificação quando o problema é concluído.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Conclusão do problema]: &lt;issue name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é:<em> Resumo de suas solicitações &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> Nome do problema<br>Nome do projeto<br>Número de referência da emissão<br>Nome do usuário que concluiu o problema<br>Novo status<br>Data e hora em que o problema foi concluído<br>Status do problema anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão <br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas concluídos<br>*Nome da ocorrência<br>*Nome do usuário que concluiu o problema<br>*Data da compilação diária </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for adicionada enviar email para o originador do problema.</strong> </p> <p>O contato principal em um problema recebe uma notificação quando ele adiciona um problema em um projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Problema enviado]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é:<em> Resumo de suas solicitações &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de referência da emissão<br>Seu nome<br>Nome do problema<br>Data Inserida<br>Prioridade do problema<br>Status do problema<br>Atribuído ao nome<br>Contato Principal<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas adicionados<br>*Nome da ocorrência<br>*Data da compilação diária </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma solicitação de Help Desk é incluída, enviar email para o originador do problema.</strong> </p> <p>O Contato Principal sobre o problema recebe uma notificação por email quando ele envia um problema.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] e se o projeto estiver configurado como uma [!UICONTROL Help Request Queue] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma fila de solicitações]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Solicitação enviada]: &lt;request name=""&gt; on &lt;project request="" queue="" name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é:<em> Resumo de suas solicitações &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do projeto (Nome da fila de solicitações)<br>Nome do Portfolio<br>Número de referência da emissão<br>Nome do problema<br>Data Inserida<br>Prioridade do problema<br>Status do problema<br>Atribuído ao nome<br>Contato Principal<br>*Número de referência do projeto<br>*Nome do projeto<br>*Número total de solicitações enviadas<br>*Nome da solicitação<br>*Prioridade da solicitação<br>*Data da compilação diária</p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma solicitação de Help Desk é fechada, enviar email para o originador do problema.</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando a solicitação é fechada.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto estiver configurado como uma [!UICONTROL Help Request Queue] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a>).</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Sua solicitação foi fechada]:"&lt;request name=""&gt;"</em></p> <p>O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo de suas solicitações] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da solicitação<br>Nome do projeto<br>Número de Referência da Solicitação<br>Nome do usuário que fechou a Solicitação<br>Status do problema<br>Data e Hora em que a Solicitação foi fechada<br>Status da solicitação anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Número de referência do projeto<br>*Nome do projeto<br>*Número total de solicitações fechadas<br>*Nome da solicitação<br>*Nome do usuário que fechou a solicitação<br>*Data da compilação diária </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma solicitação de Help Desk é atribuída, enviar email para o originador do problema.</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando um usuário é atribuído ao problema, a menos que o contato principal e o usuário atribuído sejam o mesmo usuário.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e se o projeto estiver configurado como uma [!UICONTROL Help Request Queue] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma fila de solicitações]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL foi atribuído à sua solicitação]: "&lt;request name=""&gt;"</em></p> <p>O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo de suas solicitações] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do problema<br>Nome do projeto<br>Número de referência da emissão<br>Nome da solicitação<br>Tipo de solicitação<br>Data Inserida<br>Prioridade do problema<br>Contato Principal<br>Data de Conclusão Planejada<br>Status do problema<br><strong>Veja mais detalhes</strong> botão <br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de solicitações atribuídas<br>*Nome da solicitação<br>*Atribuído ao nome<br>*Data da compilação diária</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma status de projeto for alterado, enviar email para o usuário que cadastrou o projeto</strong> </p> <p>O usuário que criou o projeto recebe uma notificação por email quando o status do projeto é alterado.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de status do projeto]: &lt;project name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo de suas solicitações] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que alterou o status<br>Novo status<br>Data e Hora em que o Status do Projeto foi alterado<br>Status do projeto anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Novo Status do Projeto<br>*Nome do usuário que alterou o status do projeto<br>*Data da compilação diária</p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando a status é alterado em uma solicitação de Help Desk, enviar email ao originador do problema.</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando o status do problema muda, a menos que o usuário que alterou o status também seja o contato principal.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual e o projeto estiver configurado como uma [!UICONTROL Help Request Queue] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma fila de solicitações]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>&lt;request name=""&gt; é &lt;new status=""&gt;</em></p> <p>O objeto da notificação diária de resumo é:<em> Resumo de suas solicitações &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da solicitação<br>Nome do projeto<br>Número de Referência da Solicitação<br>Nome do usuário que alterou o Status da Solicitação<br>Novo status<br>Data e Hora em que o Status da Solicitação foi alterado<br>Status da solicitação anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de solicitações cujo status foi alterado<br>*Nome da solicitação<br>*Status da solicitação anterior<br>*Novo status de solicitação<br>*Nome do usuário que alterou o status<br>*Data do resumo diário<br></td> 
   <td> <p><strong>Diariamente</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
