---
content-type: reference
navigation-topic: notifications
title: 'Notificações: Informações sobre projetos que eu patrociono'
description: As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você está patrocinando.
author: Courtney
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 0%

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
   <td> <p><strong>Um documento foi adicionado ao patrocinador do projeto</strong> </p> <p>O Patrocinador do projeto recebe uma notificação por email quando um documento é adicionado ao projeto.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual] e se o documento não for [!UICONTROL Privado].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Documento adicionado a] &lt;Nome do Projeto&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo dos Projetos que Você Patrocinou] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Documento<br>Nome do usuário que adicionou o documento<br>Nome do Documento<br>Adicionado na Data<br>Detalhes do Documento (formato, tamanho, Número da Versão)<br>Miniatura do Documento<br><strong>[!UICONTROL Visualização]</strong> e <strong>[!UICONTROL Download]</strong> botões<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de documentos adicionados<br>*Nome do Documento<br>*Nome do usuário que adicionou o documento<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma tarefa de etapa foi concluída em um projeto que estou patrocinando</strong> </p> <p>O Patrocinador do projeto recebe uma notificação por email quando uma tarefa de etapa é concluída em um projeto que ele ou ela patrocina.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;Nome da Tarefa&gt; em &lt;Nome do Projeto&gt;</em></p> <p>Observação: se a tarefa for alterada para um status igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".<br></p> <p>O assunto da notificação de resumo diário é:<em> Resumo dos projetos que você patrocina &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Novo Status da Tarefa<br>Data e Hora de conclusão da tarefa<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão <br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas<br>*Nome da Tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um projeto for alterado de uma status positiva de progresso (no prazo) para uma status negativa de progresso (em atraso)</strong>, enviar email para o patrocinador do projeto </p> <p>O Patrocinador do projeto recebe uma notificação por email quando o projeto atrasa o agendamento. "Um projeto está atrasado no agendamento quando o Status de Progresso é "[!UICONTROL Em Risco]" ou "[!UICONTROL Com Problemas]"."</p> <p>Os usuários com uma licença de [!UICONTROL Review] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de Progresso do Projeto]: &lt;Nome do Projeto&gt;</em></p> <p>O assunto da notificação de resumo diário é: <em>[!UICONTROL Resumo dos Projetos que Você Patrocinou] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Status de Progresso do Projeto<br>Data de Início Planejada do Projeto [!UICONTROL]<br>Data de Término Planejada do Projeto [!UICONTROL]<br>Projeto [!UICONTROL Data de Início Projetada]<br>Projeto [!UICONTROL Data de Término Projetada]<br>Percentual de Término do Projeto<br>Status do Projeto<br>Proprietário do Projeto<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Status de Progresso do Projeto<br> diário do Projeto resumo </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma tarefa foi concluída em um projeto que eu patrocino</strong> </p> <p>O patrocinador do projeto recebe uma notificação por email.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;Nome da Tarefa&gt; em &lt;Nome do Projeto&gt;</em></p> <p> <p>Observação: se a tarefa for alterada para um status igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".</p> </p> <p>O assunto da notificação de resumo diário é:<em> Resumo dos projetos que você patrocina &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Status da Tarefa<br>Data e Hora em que o status da tarefa foi alterado<br>Status da Tarefa Anterior<br><strong>Botão Ver Mais Detalhes</strong><br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas<br>*Nome da Tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma tarefa em um projeto que eu patrocinar recebe atraso</strong> </p> <p>O Patrocinador do projeto recebe uma notificação por email quando uma tarefa do projeto atrasa o cronograma. "Uma tarefa está atrasada quando o Status do Progresso é "[!UICONTROL em Risco]", "[!UICONTROL Atrasado]" ou "[!UICONTROL Atrasado]"."</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração do Progresso da Tarefa]: &lt;Nome da Tarefa&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo dos Projetos que Você Patrocinou] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Novo Status de Progresso da Tarefa<br>Tarefa [!UICONTROL Data de Início Planejada]<br>Tarefa [!UICONTROL Data de Conclusão Planejada]<br>Tarefa [!UICONTROL Data de Início Projetada]<br>Tarefa [!UICONTROL Data de Conclusão Projetada]<br>Percentual de Tarefa Concluído<br>Status da Tarefa<br>Atribuído ao Nome<br>Inserido pelo Nome<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Total do Projeto número de tarefas atrasadas<br>*Nome da Tarefa<br>*Nome do usuário que inseriu a tarefa<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um problema foi adicionado ao patrocinador do projeto</strong> </p> <p>O patrocinador do projeto recebe uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Problema adicionado a] &lt;Nome do Projeto&gt;</em></p> <p>O assunto da notificação de resumo diário é: <em>[!UICONTROL Resumo dos Projetos que Você Patrocinou] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Problema<br>Nome do usuário que adicionou o problema<br>Nome do Problema<br>Tipo de Problema<br>Data de Inserção<br>Prioridade do Problema<br>Atribuído ao Nome <br>Status do Problema<br>Contato Principal<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados ao projeto<br>*Nome do Problema<br>*Nome do usuário atribuído ao problema<br>*Data do resumo diário<br><br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for concluído enviar email para o patrocinador do projeto</strong> </p> <p>O patrocinador do projeto recebe uma notificação por email.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;Nome do Problema&gt; em &lt;Nome do Projeto&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> Resumo dos projetos que você patrocina &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nome do usuário que concluiu o problema<br>Status do Problema<br>Data e Hora em que o problema foi concluído<br>Status do Problema Anterior<br><strong>Veja Mais Detalhes</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas concluídos<br>*Nome do Problema<br>*Nome do usuário atribuído ao problema<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um problema não atribuído foi adicionado ao patrocinador do projeto</strong> </p> <p>O Patrocinador do projeto recebe uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Quem deve ser atribuído a este novo problema no] &lt;Nome do Projeto&gt;?</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo dos Projetos que Você Patrocinou] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Problema<br>Nome do usuário que adicionou o problema<br>Nome do Problema<br>Tipo de Problema<br>Data de Inserção<br>Prioridade do Problema<br>Atribuído ao Nome (vazio)<br>Status do Problema<br>Contato Principal<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados<br>*Nome do Problema<br>*Nome do usuário que adicionou o problema<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estou definido como o patrocinador de um projeto</strong> </p> <p>O patrocinador do projeto recebe uma notificação por email quando é definido como patrocinador de um projeto.<br></p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Patrocinador do Projeto]: &lt;Nome do Projeto&gt;</em></p> <p>O texto a seguir está incluído no corpo do email de notificação:</p> <p><em>[!UICONTROL Olá] &lt;Seu Nome&gt;,</em> </p> <p><em>&lt;Nome do usuário que o atribuiu como Patrocinador do Projeto&gt; [!UICONTROL fez de você o patrocinador do] &lt;Nome do Projeto&gt;. [!UICONTROL Como Patrocinador do Projeto, você poderá receber notificações de email adicionais sobre as atividades do projeto ou envolver-se na aprovação de trabalho relacionado ao projeto. Aproveite.]</em> </p> <p>O assunto da notificação de resumo diário é: <em>Resumo dos projetos que você patrocina &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> <p>Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Data de Término Planejada do Projeto<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Data do resumo diário</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
