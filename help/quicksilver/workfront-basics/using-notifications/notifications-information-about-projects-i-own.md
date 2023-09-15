---
content-type: reference
navigation-topic: notifications
title: "Notificações: informações sobre os projetos que possuo"
description: As notificações a seguir alertam você sobre atividades que ocorrem em um projeto que você possui. Para obter informações sobre como configurar as notificações recebidas, consulte Modificar suas próprias notificações por email.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 6%

---

# Notificações: informações sobre os projetos que possuo

As notificações a seguir alertam você sobre atividades que ocorrem em um projeto que você possui. Para obter informações sobre como configurar as notificações recebidas, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Quando um documento for adicionado, enviar email para o proprietário do projeto.</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando um documento é adicionado ao projeto, a menos que o usuário que adicionou o documento também seja o Proprietário do projeto.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual] e o documento não for Privado.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Documento adicionado a] &lt;project name=""&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que adicionou o documento<br>Nome do documento<br>Adicionado na data<br>Detalhes do documento (formato, tamanho, número da versão)<br><strong>[!UICONTROL Visualizar]</strong> e <strong>[!UICONTROL Baixar]</strong> botões<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de documentos adicionados<br>*Nome do documento<br>*Nome do usuário que adicionou o documento<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma etapa for concluída, enviar email para o proprietário do projeto.</strong> </p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;task name=""&gt; em &lt;project name=""&gt;</em></p> <p>Observação: se a tarefa for alterada para um status igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".</p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Novo Status de Tarefa<br>Data e hora em que a tarefa foi concluída<br>Status da tarefa anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um projeto for alterado de uma status positiva de progresso (no prazo) para uma status negativa de progresso (em atraso), enviar email para o proprietário do projeto</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando o projeto está atrasado. Um projeto está atrasado no agendamento quando o Status de Progresso é "[!UICONTROL em Risco]", "[!UICONTROL Atrasado]" ou "[!UICONTROL Atrasado]".</p> <p>A prática recomendada é manter essa notificação ativa. </p> <p>Os usuários com uma licença de [!UICONTROL Review] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de Progresso de Projeto]: &lt;project name=""&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Status de Progresso do Projeto<br>Projeto [!UICONTROL Data de Início Planejada]<br>Projeto [!UICONTROL Data de Término Planejada]<br>Projeto [!UICONTROL Data de Início Projetada]<br>Projeto [!UICONTROL Data de Término Projetada]<br>Porcentagem Concluída do Projeto<br>Status do projeto<br>Proprietário do Projeto<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Status de progresso do projeto<br>*Data do resumo diário<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for adicionada enviar email para o proprietário do projeto.</strong> </p> <p>O proprietário do projeto recebe uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Problema adicionado a] &lt;project name=""&gt;</em></p> <p> </p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de referência da edição<br>Nome do usuário que adicionou o problema<br>Nome do problema<br>Tipo de Problema<br>Data inserida<br>Prioridade do problema<br>Atribuído a nome <br>Status do Problema<br>Contato Primário<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados ao projeto<br>*Nome do problema<br>*Nome do usuário que adicionou o problema<br>*Data do resumo diário</p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma tarefa for concluída, enviar email para o proprietário do projeto</strong> </p> <p>O Proprietário do projeto recebe uma notificação quando uma tarefa é concluída em seu projeto.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;task name=""&gt; em &lt;project name=""&gt;</em></p> <p> <p>Observação: se a tarefa for alterada para um status igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".</p> </p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa <br>Status da tarefa<br>Data e hora em que a tarefa foi concluída<br>Status da tarefa anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas <br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma tarefa for alterada de uma status de progresso positivo (no prazo) para uma status de progresso negativo (em atraso), enviar email para o proprietário da tarefa</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando uma tarefa no projeto atrasa o agendamento. "Uma tarefa está atrasada quando o Status do Progresso é "[!UICONTROL em Risco]", "[!UICONTROL Atrasado]" ou "[!UICONTROL Atrasado]"."</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de Progresso de Tarefa]: &lt;task name=""&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Status de progresso da nova tarefa<br>Tarefa [!UICONTROL Data de Início Planejada]<br>Tarefa [!UICONTROL Data de conclusão planejada]<br>Tarefa [!UICONTROL Data de Início Projetada]<br>Tarefa [!UICONTROL Data de Término Projetada]<br>Percentual Concluído da Tarefa<br>Status da tarefa<br>Atribuído a nome<br>Cadastrado por nome<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas atrasadas<br>*Nome da tarefa<br>*Atribuído a nome<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for concluído enviar email para o proprietário do projeto</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando um problema é concluído em seu projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>Os usuários com uma licença de [!UICONTROL Review] não recebem uma notificação. </p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;issue name=""&gt; em &lt;project name=""&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome do problema<br>Nome do projeto<br>Número de referência da edição<br>Nome do usuário que concluiu o problema<br>Status do Problema<br>Data e hora em que o problema foi concluído<br>Status do problema anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão <br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de problemas concluídos<br>*Nome do problema<br>*Nome do usuário atribuído ao problema<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema atribuída for adicionada enviar email para o proprietário do projeto.</strong> </p> <p>O proprietário do projeto recebe uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Quem deve ser atribuído a este novo problema no] &lt;project name=""&gt;?</em></p> <p> </p> <p> O assunto da notificação de resumo diário é: <em> Resumo dos projetos que você possui &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de referência da edição<br>Nome do usuário que adicionou o problema<br>Nome do problema<br>Tipo de Problema<br>Data inserida<br>Prioridade do problema<br>Atribuído a nome (vazio)<br>Status do Problema<br>Contato Primário<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados<br>*Nome do problema<br>*Nome do usuário que adicionou o problema<br>*Data do resumo diário<br></p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando o proprietário do projeto mudar ou na criação do projeto, enviar email para o usuário recentemente atribuído</strong> </p> <p>Quando um usuário é atribuído como o proprietário de um projeto, ele recebe uma notificação por email.</p> <p>Se o proprietário do projeto for o mesmo usuário que fez a atribuição, uma notificação por email não será enviada.</p> <p>Os usuários com uma licença de [!UICONTROL Review] não recebem uma notificação.</p> <p>Ligar este recurso porque eles estão sendo atribuídos a algo. </p> <p> Atribuir algo, compartilhar algo, obter acesso a algo.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Você agora é o proprietário do projeto] &lt;project name=""&gt;</em></p> <p>O texto a seguir está incluído no corpo do email de notificação:<em><br></em></p> <p><em>[!UICONTROL Olá] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL tornou você o proprietário de] &lt;project name=""&gt;. [!UICONTROL Como Proprietário do Projeto, você poderá receber notificações de email adicionais sobre as atividades do projeto, ter de aprovar horas para o projeto ou envolver-se na aprovação de trabalho relacionado ao projeto. É todo seu.]</em> </p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Data de conclusão do projeto<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Data do resumo diário</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A data de compromisso de uma tarefa em um dos meus projetos mudou</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando a Data de confirmação é alterada para uma tarefa no projeto, a menos que o usuário que alterou a Data de confirmação também seja o Proprietário do projeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Confirmar data para] &lt;task name=""&gt; [!UICONTROL agora é] &lt;new commit="" date=""&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> Resumo dos projetos que você possui &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que alterou a Data de confirmação<br>Nova data de compromisso<br>Tarefa [!UICONTROL Data de conclusão planejada]<br>Informações sobre como a Linha do tempo do projeto é afetada por essa alteração<br>Atribuído a nome<br>Cadastrado por nome<br>Proprietário do Projeto<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas cuja Data de confirmação foi alterada<br>*Nome da tarefa<br>*Data do resumo diário<br></p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e [!UICONTROL Diariamente]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mudança da data de compromisso de um problema em um dos meus projetos</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando a Data de confirmação é alterada para um problema no projeto, a menos que o usuário que altera a Data de confirmação seja o mesmo usuário que o Proprietário do projeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Confirmar data para] &lt;issue name=""&gt; [!UICONTROL agora é] &lt;new commit="" date=""&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome do problema<br>Nome do projeto<br>Número de referência da edição<br>Nome do usuário que alterou a Data de confirmação<br>Nova data de compromisso<br>Data de Término Planejada do Problema<br>Atribuído a nome<br>Cadastrado por nome<br>Proprietário do Projeto<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do projeto<br>*Número de Referência do Projeto<br>*Número total de problemas cuja data de confirmação foi alterada<br>*Nome do problema<br>*Data do resumo diário<br></p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e [!UICONTROL Diariamente]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
