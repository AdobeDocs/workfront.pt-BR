---
content-type: reference
navigation-topic: notifications
title: "Notificações: informações sobre aprovação"
description: As notificações a seguir alertam sobre as atividades de aprovação que ocorrem em um item de trabalho com o qual você está envolvido. Para obter informações sobre como configurar as notificações recebidas, consulte Modificar suas próprias notificações por email.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 6%

---

# Notificações: Informações de aprovação

As notificações a seguir alertam sobre as atividades de aprovação que ocorrem em um item de trabalho com o qual você está envolvido. Para obter informações sobre como configurar as notificações recebidas, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Uma solicitação de aprovação de problema foi concluída</strong> </p> <p>Uma aprovação de problema que você delegou a outro usuário foi aprovada ou rejeitada por esse usuário.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Aprovação de Problema/ Rejeição Feita em Seu Nome por] &lt;user name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo das Informações de Aprovação] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do problema<br>Nome do projeto<br>Número de referência da edição<br>Nome do usuário que aprovou/rejeitou o problema em seu nome<br>Decisão de aprovação<br>Status do Problema<br>Nome do usuário que solicitou a aprovação<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Número de Referência do Projeto<br>*Nome do projeto<br>*Número total de aprovações delegadas de problemas<br>*Nome do problema<br>*Nome do aprovador<br>*Data do resumo diário<br><br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de aprovação de projeto foi concluída</strong> </p> <p>Uma aprovação de projeto delegada a outro usuário foi aprovada ou rejeitada por esse usuário.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Aprovação/Rejeição de Projeto Feita em Seu Nome por] &lt;user name=""&gt;</em></p> <p><em>O assunto da notificação de resumo diário é: [!UICONTROL Resumo das Informações de Aprovação] &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> Nome do projeto<br>[!UICONTROL Nome do Portfolio]<br>[!UICONTROL Número de Referência de Projeto]<br>Nome do usuário que aprovou/rejeitou o projeto em seu nome<br>[!UICONTROL Decisão de Aprovação]<br>[!UICONTROL Status do Projeto]<br>Nome do usuário que solicitou a aprovação<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Número de Referência do Projeto<br>*Nome do projeto<br>*Nome do aprovador<br>[!UICONTROL *Data do resumo diário]<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de aprovação de tarefa foi concluída</strong> </p> <p>Uma aprovação de tarefa delegada a outro usuário foi aprovada ou rejeitada por esse usuário.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Aprovação de Tarefa/ Rejeição Feita em Seu Nome por] &lt;user name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo das Informações de Aprovação] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que aprovou/rejeitou a tarefa em seu nome<br>Decisão de aprovação<br>Status da tarefa<br>Nome do usuário que solicitou a aprovação<br><strong>Ver mais detalhes</strong> botão<br>*Número de Referência do Projeto<br>*Nome do projeto<br>*Número total de aprovações delegadas de tarefas<br>*Nome da tarefa<br>*Nome do aprovador<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de aprovação de documento foi cancelada</strong> </p> <p>O Aprovador de documentos do documento recebe uma notificação por email quando a solicitação de aprovação de documento é cancelada.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;user name=""&gt; [!UICONTROL cancelou a solicitação de aprovação de documento]</em></p> <p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </p> </td> 
   <td> Nome do usuário que cancelou a solicitação de aprovação<br>[!UICONTROL Nome do Documento] </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Recebi a delegação de aprovador</strong> </p> <p>Se alguém delegar uma aprovação a você, você receberá uma notificação por email. </p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Delegado] &lt;object type=""&gt; [!UICONTROL Aprovação - Favor Revisar] &lt;object name=""&gt;</em></p> <p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </p> </td> 
   <td> <p>[!UICONTROL Nome do Objeto]<br>[!UICONTROL Nome do Objeto Pai]<br>[!UICONTROL Número de Referência de Objeto]<br>Nome do usuário que enviou o objeto para aprovação<br>Nome do usuário em nome do qual você está aprovando o objeto<br>Status do objeto<br>Data e hora em que a aprovação foi solicitada<br>Prioridade do objeto<br>Nome da etapa de aprovação<br>[!UICONTROL Data de Término Planejada] do Objeto<br><strong>[!UICONTROL Tomar Decisão de Aprovação]</strong> botão</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma planilha de horas for aceita e fechada, enviar email para o usuário</strong> </p> <p>Quando sua planilha de horas é aprovada, você recebe uma notificação por email.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Planilha de Horas aprovada]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </p> </td> 
   <td> Nome do usuário que aprovou sua Planilha de Horas<br>Data e hora em que a folha de horas foi aprovada<br>Status da Planilha de Horas ([!UICONTROL Aprovado])<br>Data inicial e data final da folha de horas<br>Total de horas registradas na Planilha de Horas<br>Horas extras registradas na planilha de horas </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
