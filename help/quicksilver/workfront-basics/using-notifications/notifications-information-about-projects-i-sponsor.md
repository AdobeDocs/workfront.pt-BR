---
content-type: reference
navigation-topic: notifications
title: "Notificações: Informações sobre projetos que patrocínio"
description: As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você está patrocinando.
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1316'
ht-degree: 6%

---

# Notificações: Informações sobre projetos que patrocínio

As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você está patrocinando.

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
   <td> <p><strong>Quando um documento for adicionado, enviar email para o patrocinador do projeto.</strong> </p> <p>O Patrocinador de projeto recebe uma notificação por email quando um documento é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] e se o documento não for [!UICONTROL Privado].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Documento adicionado ao] &lt;project name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo dos projetos que você patrocinou] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de referência do documento<br>Nome do usuário que adicionou o documento<br>Nome do documento<br>Adição Na Data<br>Detalhes do documento (formato, tamanho, número da versão)<br>Miniatura do documento<br><strong>[!UICONTROL Preview]</strong> e <strong>[!UICONTROL Download]</strong> botões<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de documentos adicionados<br>*Nome do documento<br>*Nome do usuário que adicionou o documento<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma etapa for concluída, enviar email para o patrocinador de projeto</strong> </p> <p>O Patrocinador de projeto recebe uma notificação por email quando uma tarefa de marco é concluída em um projeto que ele patrocina.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL concluído]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>Observação: Se a tarefa for alterada para um status que seja igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".<br></p> <p>O objeto da notificação diária de resumo é:<em> Resumo dos projetos que você patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Novo Status da Tarefa<br>Data e hora em que a tarefa foi concluída<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão <br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas concluídas<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um projeto for alterado de uma status de progresso positiva (no prazo) para uma status negativa de progresso (em atraso), enviar email para o patrocinador do projeto</strong> </p> <p>O Patrocinador de projeto recebe uma notificação por email quando o projeto fica atrasado. Um projeto está atrasado quando o Status do Andamento é "[!UICONTROL Em Risco]" ou "[!UICONTROL Em Problema]".</p> <p>Os usuários com uma licença da [!UICONTROL Review] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de progresso do projeto]: &lt;project name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é: <em>[!UICONTROL Resumo dos projetos que você patrocinou] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Status de progresso do projeto<br>Projeto [!UICONTROL Data de início planejada]<br>Projeto [!UICONTROL Data de conclusão planejada]<br>Projeto [!UICONTROL Data de início prevista]<br>Projeto [!UICONTROL Data de conclusão prevista]<br>Porcentagem de Projeto Concluída<br>Status do projeto<br>Proprietário do projeto<br>*Nome do projeto<br>*Número de referência do projeto<br>*Status de progresso do projeto<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma tarefa for concluída, enviar email para o patrocinador do projeto</strong> </p> <p>O patrocinador do projeto recebe uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL concluído]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>Observação: Se a tarefa for alterada para um status que seja igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".</p> </p> <p>O objeto da notificação diária de resumo é:<em> Resumo dos projetos que você patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Status da tarefa<br>Data e hora em que o status da tarefa foi alterado<br>Status da Tarefa Anterior<br><strong>Veja mais detalhes</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas concluídas<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma tarefa for alterada de uma status de progresso positivo (no prazo) para uma status de progresso negativo (em atraso), enviar email para o patrocinador do projeto</strong> </p> <p>O Patrocinador de projeto recebe uma notificação por email quando uma tarefa no projeto fica atrasada. Uma tarefa está atrasada quando o Status do Andamento é "[!UICONTROL Em Risco]" ou "[!UICONTROL Atrás]" ou "[!UICONTROL Atrasado]".</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de progresso da tarefa]: &lt;task name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo dos projetos que você patrocinou] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Novo Status de Andamento da Tarefa<br>Tarefa [!UICONTROL Data de início planejada]<br>Tarefa [!UICONTROL Data de conclusão planejada]<br>Data de Início Projetada da Tarefa [!UICONTROL]<br>Data de Conclusão Projetada da Tarefa [!UICONTROL]<br>Porcentagem de Tarefa Concluída<br>Status da tarefa<br>Atribuído ao nome<br>Digitado por nome<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas que estão atrasadas<br>*Nome da tarefa<br>*Nome do usuário que inseriu a tarefa<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for adicionada enviar email para o patrocinador do projeto.</strong> </p> <p>O Patrocinador de projeto recebe uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Problema adicionado ao] &lt;project name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é: <em>[!UICONTROL Resumo dos projetos que você patrocinou] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de referência da emissão<br>Nome do usuário que adicionou o problema<br>Nome do problema<br>Tipo de problema<br>Data Inserida<br>Prioridade do problema<br>Atribuído ao nome <br>Status do problema<br>Contato Principal<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas adicionados ao projeto<br>*Nome da ocorrência<br>*Nome do usuário atribuído ao problema<br>*Data do resumo diário<br><br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for concluído enviar email para o patrocinador do projeto</strong> </p> <p>O patrocinador do projeto recebe uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL concluído]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é:<em> Resumo dos projetos que você patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do problema<br>Nome do projeto<br>Número de referência da emissão<br>Nome do usuário que concluiu o problema<br>Status do problema<br>Data e hora em que o problema foi concluído<br>Status do problema anterior<br><strong>Veja mais detalhes</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas concluídos<br>*Nome da ocorrência<br>*Nome do usuário atribuído ao problema<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema não atribuída for adicionada enviar email para o patrocinador do projeto</strong> </p> <p>O Patrocinador de projeto recebe uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Quem deve ser atribuído a este novo problema em] &lt;project name=""&gt;?</em></p> <p>O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo dos projetos que você patrocinou] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de referência da emissão<br>Nome do usuário que adicionou o problema<br>Nome do problema<br>Tipo de problema<br>Data Inserida<br>Prioridade do problema<br>Atribuído a Nome (vazio)<br>Status do problema<br>Contato Principal<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas adicionados<br>*Nome da ocorrência<br>*Nome do usuário que adicionou o problema<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando o patrocinador do projeto mudar ou na criação do projeto, enviar email para o patrocinador recentemente atribuído</strong> </p> <p>O patrocinador do projeto recebe uma notificação por e-mail quando é definido como patrocinador de um projeto.<br></p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Project Sponsor]: &lt;project name=""&gt;</em></p> <p>O texto a seguir está incluído no corpo da notificação por email:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,</em> </p> <p><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" sponsor=""&gt; [!UICONTROL o tornou patrocinador do] &lt;project name=""&gt;. [!UICONTROL Como patrocinador do projeto, você pode receber notificações adicionais por email sobre a atividade do projeto ou estar envolvido na aprovação do trabalho relacionado ao projeto. Aproveite.]</em> </p> <p>O objeto da notificação diária de resumo é: <em>Resumo dos projetos que você patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Data de Conclusão Planejada do Projeto<br>*Nome do projeto<br>*Número de referência do projeto<br>*Data da compilação diária</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
