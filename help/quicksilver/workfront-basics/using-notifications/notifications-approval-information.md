---
content-type: reference
navigation-topic: notifications
title: '"Notificações: Informações de aprovação'''
description: As notificações a seguir alertam sobre as atividades de aprovação que ocorrem em um item de trabalho com o qual você está envolvido. Para obter informações sobre como configurar quais notificações você recebe, consulte Ativar ou desativar suas próprias notificações de evento.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 6%

---

# Notificações: Informações de aprovação

As notificações a seguir alertam sobre as atividades de aprovação que ocorrem em um item de trabalho com o qual você está envolvido. Para obter informações sobre como configurar quais notificações você recebe, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Uma solicitação de aprovação de problema foi concluída</strong> </p> <p>Uma aprovação de problema que você delegou a outro usuário foi aprovada ou rejeitada por esse usuário.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Emitir aprovação/rejeição feita em seu nome por] &lt;user name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo das informações de aprovação] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do problema<br>Nome do projeto<br>Número de referência da emissão<br>Nome do usuário que aprovou/rejeitou o problema em seu nome<br>Decisão de aprovação<br>Status do problema<br>Nome do usuário que solicitou a aprovação<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Número de referência do projeto<br>*Nome do projeto<br>*Número total de aprovações de emissão delegadas<br>*Nome da ocorrência<br>*Nome do Aprovador<br>*Data do resumo diário<br><br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de aprovação de projeto foi concluída</strong> </p> <p>Uma aprovação de projeto que você delegou a outro usuário foi aprovada ou rejeitada por esse usuário.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Aprovação/rejeição de projeto feita em seu nome por] &lt;user name=""&gt;</em></p> <p><em>O objeto da notificação diária de resumo é: [!UICONTROL Resumo das informações de aprovação] &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> Nome do projeto<br>[!UICONTROL Portfolio Name]<br>[!UICONTROL Número de referência do projeto]<br>Nome do usuário que aprovou/rejeitou o projeto em seu nome<br>[!UICONTROL Decisão de aprovação]<br>[!UICONTROL Status do projeto]<br>Nome do usuário que solicitou a aprovação<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Número de referência do projeto<br>*Nome do projeto<br>*Nome do Aprovador<br>[!UICONTROL *Data da compilação diária]<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de aprovação de tarefa foi concluída</strong> </p> <p>Uma aprovação de tarefa que você delegou a outro usuário foi aprovada ou rejeitada por esse usuário.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Tarefa Aprovação/Rejeição feita em seu nome por] &lt;user name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo das informações de aprovação] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que aprovou/rejeitou a tarefa em seu nome<br>Decisão de aprovação<br>Status da tarefa<br>Nome do usuário que solicitou a aprovação<br><strong>Veja mais detalhes</strong> botão<br>*Número de referência do projeto<br>*Nome do projeto<br>*Número total de aprovações de tarefas delegadas<br>*Nome da tarefa<br>*Nome do Aprovador<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de aprovação de documento foi cancelada</strong> </p> <p>O Aprovador de documento do documento recebe uma notificação por email quando a solicitação de aprovação do documento é cancelada.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;user name=""&gt; [!UICONTROL cancelou a solicitação de aprovação de documento]</em></p> <p> <p>Observação: Não é possível configurar essa notificação para um email de resumo diário.</p> </p> </td> 
   <td> Nome do usuário que cancelou a solicitação de aprovação<br>[!UICONTROL Nome do documento] </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Recebi a delegação de aprovador</strong> </p> <p>Se alguém tiver delegado uma aprovação a você, você receberá uma notificação por email. </p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Delegado] &lt;object type=""&gt; [!UICONTROL Aprovação - Revisar] &lt;object name=""&gt;</em></p> <p> <p>Observação: Não é possível configurar essa notificação para um email de resumo diário.</p> </p> </td> 
   <td> <p>[!UICONTROL Nome do objeto]<br>[!UICONTROL Nome do objeto pai]<br>[!UICONTROL Número de referência do objeto]<br>Nome do usuário que enviou o objeto para aprovação<br>Nome do usuário em nome do qual você está aprovando o objeto<br>Status do objeto<br>Data e hora em que a aprovação foi solicitada<br>Prioridade do objeto<br>Nome da etapa de aprovação<br>[!UICONTROL Data de conclusão planejada] do objeto<br><strong>[!UICONTROL Tornar decisão de aprovação]</strong> botão</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma planilha de horas for aceita e fechada, enviar email para o usuário</strong> </p> <p>Quando a folha de horas é aprovada, você recebe uma notificação por email.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Folha de Horas Aprovada]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>Observação: Não é possível configurar essa notificação para um email de resumo diário.</p> </p> </td> 
   <td> Nome do usuário que aprovou sua Folha de Horas<br>Data e hora em que a Folha de Horas foi aprovada<br>Status da Folha de Horas ([!UICONTROL Aprovado])<br>Data inicial e Data final da folha de horas<br>Total de horas registradas na Folha de Horas<br>Horas extras registradas na Folha de Horas </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
