---
content-type: reference
navigation-topic: notifications
title: "Notificações: informações sobre os projetos que eu patrocino"
description: As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você está patrocinando.
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 6%

---

# Notificações: Informações sobre projetos que eu patrociono

As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você está patrocinando.

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
   <td> <p><strong>Quando um documento for adicionado, enviar email para o patrocinador do projeto.</strong> </p> <p>O Patrocinador do projeto recebe uma notificação por email quando um documento é adicionado ao projeto.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual] e se o documento não for [!UICONTROL Privado].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Documento adicionado a] &lt;project name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo dos Projetos que Você Patrocina] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Documento<br>Nome do usuário que adicionou o documento<br>Nome do documento<br>Adicionado na data<br>Detalhes do documento (formato, tamanho, número da versão)<br>Miniatura do documento<br><strong>[!UICONTROL Visualizar]</strong> e <strong>[!UICONTROL Baixar]</strong> botões<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de documentos adicionados<br>*Nome do documento<br>*Nome do usuário que adicionou o documento<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma etapa for concluída, enviar email para o patrocinador de projeto</strong> </p> <p>O Patrocinador do projeto recebe uma notificação por email quando uma tarefa de etapa é concluída em um projeto que ele ou ela patrocina.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;task name=""&gt; em &lt;project name=""&gt;</em></p> <p>Observação: se a tarefa for alterada para um status igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".<br></p> <p>O assunto da notificação de resumo diário é:<em> Resumo dos projetos que você patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Novo Status de Tarefa<br>Data e hora em que a tarefa foi concluída<br>Status da tarefa anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão <br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um projeto for alterado de uma status de progresso positiva (no prazo) para uma status negativa de progresso (em atraso), enviar email para o patrocinador do projeto</strong> </p> <p>O Patrocinador do projeto recebe uma notificação por email quando o projeto atrasa o agendamento. "Um projeto está atrasado no agendamento quando o Status de Progresso é "[!UICONTROL Em Risco]" ou "[!UICONTROL Com Problemas]"."</p> <p>Os usuários com uma licença de [!UICONTROL Review] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de Progresso de Projeto]: &lt;project name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é: <em>[!UICONTROL Resumo dos Projetos que Você Patrocina] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Status de Progresso do Projeto<br>Projeto [!UICONTROL Data de Início Planejada]<br>Projeto [!UICONTROL Data de Término Planejada]<br>Projeto [!UICONTROL Data de Início Projetada]<br>Projeto [!UICONTROL Data de Término Projetada]<br>Porcentagem Concluída do Projeto<br>Status do projeto<br>Proprietário do Projeto<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Status de progresso do projeto<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma tarefa for concluída, enviar email para o patrocinador do projeto</strong> </p> <p>O patrocinador do projeto recebe uma notificação por email.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;task name=""&gt; em &lt;project name=""&gt;</em></p> <p> <p>Observação: se a tarefa for alterada para um status igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".</p> </p> <p>O assunto da notificação de resumo diário é:<em> Resumo dos projetos que você patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Status da tarefa<br>Data e hora em que o status da tarefa foi alterado<br>Status da tarefa anterior<br><strong>Ver mais detalhes</strong> botão<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma tarefa for alterada de uma status de progresso positivo (no prazo) para uma status de progresso negativo (em atraso), enviar email para o patrocinador do projeto</strong> </p> <p>O Patrocinador do projeto recebe uma notificação por email quando uma tarefa do projeto atrasa o cronograma. "Uma tarefa está atrasada quando o Status do Progresso é "[!UICONTROL em Risco]", "[!UICONTROL Atrasado]" ou "[!UICONTROL Atrasado]"."</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de Progresso de Tarefa]: &lt;task name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo dos Projetos que Você Patrocina] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Status de progresso da nova tarefa<br>Tarefa [!UICONTROL Data de Início Planejada]<br>Tarefa [!UICONTROL Data de conclusão planejada]<br>Tarefa [!UICONTROL Data de Início Projetada]<br>Tarefa [!UICONTROL Data de Término Projetada]<br>Percentual Concluído da Tarefa<br>Status da tarefa<br>Atribuído a nome<br>Cadastrado por nome<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas atrasadas<br>*Nome da tarefa<br>*Nome do usuário que entrou na tarefa<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for adicionada enviar email para o patrocinador do projeto.</strong> </p> <p>O patrocinador do projeto recebe uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Problema adicionado a] &lt;project name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é: <em>[!UICONTROL Resumo dos Projetos que Você Patrocina] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de referência da edição<br>Nome do usuário que adicionou o problema<br>Nome do problema<br>Tipo de Problema<br>Data inserida<br>Prioridade do problema<br>Atribuído a nome <br>Status do Problema<br>Contato Primário<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados ao projeto<br>*Nome do problema<br>*Nome do usuário atribuído ao problema<br>*Data do resumo diário<br><br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for concluído enviar email para o patrocinador do projeto</strong> </p> <p>O patrocinador do projeto recebe uma notificação por email.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;issue name=""&gt; em &lt;project name=""&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> Resumo dos projetos que você patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do problema<br>Nome do projeto<br>Número de referência da edição<br>Nome do usuário que concluiu o problema<br>Status do Problema<br>Data e hora em que o problema foi concluído<br>Status do problema anterior<br><strong>Ver mais detalhes</strong> botão<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de problemas concluídos<br>*Nome do problema<br>*Nome do usuário atribuído ao problema<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema não atribuída for adicionada enviar email para o patrocinador do projeto</strong> </p> <p>O Patrocinador do projeto recebe uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Quem deve ser atribuído a este novo problema no] &lt;project name=""&gt;?</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo dos Projetos que Você Patrocina] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de referência da edição<br>Nome do usuário que adicionou o problema<br>Nome do problema<br>Tipo de Problema<br>Data inserida<br>Prioridade do problema<br>Atribuído a nome (vazio)<br>Status do Problema<br>Contato Primário<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados<br>*Nome do problema<br>*Nome do usuário que adicionou o problema<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando o patrocinador do projeto mudar ou na criação do projeto, enviar email para o patrocinador recentemente atribuído</strong> </p> <p>O patrocinador do projeto recebe uma notificação por email quando é definido como patrocinador de um projeto.<br></p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Patrocinador do Projeto]: &lt;project name=""&gt;</em></p> <p>O texto a seguir está incluído no corpo do email de notificação:</p> <p><em>[!UICONTROL Olá] &lt;your name=""&gt;,</em> </p> <p><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" sponsor=""&gt; [!UICONTROL tornou você o patrocinador de] &lt;project name=""&gt;. [!UICONTROL Como Patrocinador do Projeto, você poderá receber notificações de email adicionais sobre as atividades do projeto ou envolver-se na aprovação de trabalho relacionado ao projeto. Aproveite.]</em> </p> <p>O assunto da notificação de resumo diário é: <em>Resumo dos projetos que você patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Data de Término Planejada do Projeto<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Data do resumo diário</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
