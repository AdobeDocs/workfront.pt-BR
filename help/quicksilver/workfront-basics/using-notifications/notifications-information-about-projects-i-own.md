---
content-type: reference
navigation-topic: notifications
title: '"Notificações: Informações sobre os projetos que eu possuo'''
description: As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você possui. Para obter informações sobre como configurar quais notificações você recebe, consulte Ativar ou desativar suas próprias notificações de evento.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 6%

---

# Notificações: Informações sobre os projetos que eu possuo

As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você possui. Para obter informações sobre como configurar quais notificações você recebe, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Quando um documento for adicionado, enviar email para o proprietário do projeto.</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando um documento é adicionado ao projeto, a menos que o usuário que adicionou o documento também seja o Proprietário do projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] e o documento não for Privado.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Documento adicionado ao] &lt;project name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo dos projetos que você possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que adicionou o documento<br>Nome do documento<br>Adição Na Data<br>Detalhes do documento (formato, tamanho, número da versão)<br><strong>[!UICONTROL Preview]</strong> e <strong>[!UICONTROL Download]</strong> botões<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de documentos adicionados<br>*Nome do documento<br>*Nome do usuário que adicionou o documento<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma etapa for concluída, enviar email para o proprietário do projeto.</strong> </p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL concluído]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>Observação: Se a tarefa for alterada para um status que seja igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".</p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo dos projetos que você possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Novo Status da Tarefa<br>Data e hora em que a tarefa foi concluída<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas concluídas<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um projeto for alterado de uma status positiva de progresso (no prazo) para uma status negativa de progresso (em atraso), enviar email para o proprietário do projeto</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando o projeto estiver atrasado. Um projeto está atrasado quando o Status do Andamento é "[!UICONTROL Em Risco]", "[!UICONTROL Atrás]" ou "[!UICONTROL Atrasado]".</p> <p>A prática recomendada é manter essa notificação ativa. </p> <p>Os usuários com uma licença da [!UICONTROL Review] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de progresso do projeto]: &lt;project name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo dos projetos que você possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Status de progresso do projeto<br>Projeto [!UICONTROL Data de início planejada]<br>Projeto [!UICONTROL Data de conclusão planejada]<br>Projeto [!UICONTROL Data de início prevista]<br>Projeto [!UICONTROL Data de conclusão prevista]<br>Porcentagem de Projeto Concluída<br>Status do projeto<br>Proprietário do projeto<br>*Nome do projeto<br>*Número de referência do projeto<br>*Status de progresso do projeto<br>*Data do resumo diário<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for adicionada enviar email para o proprietário do projeto.</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Problema adicionado ao] &lt;project name=""&gt;</em></p> <p> </p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo dos projetos que você possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de referência da emissão<br>Nome do usuário que adicionou o problema<br>Nome do problema<br>Tipo de problema<br>Data Inserida<br>Prioridade do problema<br>Atribuído ao nome <br>Status do problema<br>Contato Principal<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas adicionados ao projeto<br>*Nome da ocorrência<br>*Nome do usuário que adicionou o problema<br>*Data da compilação diária</p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma tarefa for concluída, enviar email para o proprietário do projeto</strong> </p> <p>O Proprietário do projeto recebe uma notificação quando uma tarefa é concluída em seu projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL concluído]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>Observação: Se a tarefa for alterada para um status que seja igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".</p> </p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo dos projetos que você possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa <br>Status da tarefa<br>Data e hora em que a tarefa foi concluída<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas concluídas <br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma tarefa for alterada de uma status de progresso positivo (no prazo) para uma status de progresso negativo (em atraso), enviar email para o proprietário da tarefa</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando uma tarefa no projeto fica atrasada. Uma tarefa está atrasada quando o Status do Andamento é "[!UICONTROL Em Risco]" ou "[!UICONTROL Atrás]" ou "[!UICONTROL Atrasado]".</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de progresso da tarefa]: &lt;task name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo dos projetos que você possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Novo Status de Andamento da Tarefa<br>Tarefa [!UICONTROL Data de início planejada]<br>Tarefa [!UICONTROL Data de conclusão planejada]<br>Data de Início Projetada da Tarefa [!UICONTROL]<br>Data de Conclusão Projetada da Tarefa [!UICONTROL]<br>Porcentagem de Tarefa Concluída<br>Status da tarefa<br>Atribuído ao nome<br>Digitado por nome<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas que estão atrasadas<br>*Nome da tarefa<br>*Atribuído ao nome<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for concluído enviar email para o proprietário do projeto</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando um problema é concluído em seu projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>Os usuários com uma licença da [!UICONTROL Review] não recebem uma notificação. </p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL concluído]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo dos projetos que você possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome do problema<br>Nome do projeto<br>Número de referência da emissão<br>Nome do usuário que concluiu o problema<br>Status do problema<br>Data e hora em que o problema foi concluído<br>Status do problema anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão <br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas concluídos<br>*Nome da ocorrência<br>*Nome do usuário atribuído ao problema<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema atribuída for adicionada enviar email para o proprietário do projeto.</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Quem deve ser atribuído a este novo problema em] &lt;project name=""&gt;?</em></p> <p> </p> <p> O objeto da notificação diária de resumo é: <em> Resumo dos projetos que você possui &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de referência da emissão<br>Nome do usuário que adicionou o problema<br>Nome do problema<br>Tipo de problema<br>Data Inserida<br>Prioridade do problema<br>Atribuído a Nome (vazio)<br>Status do problema<br>Contato Principal<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas adicionados<br>*Nome da ocorrência<br>*Nome do usuário que adicionou o problema<br>*Data do resumo diário<br></p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando o proprietário do projeto mudar ou na criação do projeto, enviar email para o usuário recentemente atribuído</strong> </p> <p>Quando um usuário é atribuído como proprietário de um projeto, ele recebe uma notificação por email.</p> <p>Se o proprietário do Projeto for o mesmo usuário que fez a atribuição, uma notificação por email não será enviada.</p> <p>Os usuários com uma licença da [!UICONTROL Review] não recebem uma notificação.</p> <p>Ligue isto porque eles estão sendo atribuídos a algo. </p> <p> Atribuir algo, compartilhar algo, obter acesso para algo.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Agora você é o proprietário do projeto] &lt;project name=""&gt;</em></p> <p>O texto a seguir está incluído no corpo da notificação por email:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL o tornou proprietário] &lt;project name=""&gt;. [!UICONTROL Como proprietário do projeto, você pode receber notificações adicionais por email sobre a atividade do projeto, ser obrigado a aprovar horas para o projeto ou participar da aprovação do trabalho relacionado ao projeto. É tudo seu.]</em> </p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo dos projetos que você possui] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Data de conclusão do projeto<br>*Nome do projeto<br>*Número de referência do projeto<br>*Data da compilação diária</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A data de compromisso de uma tarefa em um dos meus projetos mudou</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando a Data da confirmação é alterada para uma tarefa no projeto, a menos que o usuário que alterou a Data da confirmação também seja o Proprietário do projeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Confirmar data para] &lt;task name=""&gt; [!UICONTROL está agora] &lt;new commit="" date=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> Resumo dos projetos que você possui &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que alterou a Data de confirmação<br>Nova Data de Confirmação<br>Tarefa [!UICONTROL Data de conclusão planejada]<br>Informações sobre como a Linha do Tempo do Projeto é afetada por essa alteração<br>Atribuído ao nome<br>Digitado por nome<br>Proprietário do projeto<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas cuja Data de Confirmação foi alterada<br>*Nome da tarefa<br>*Data do resumo diário<br></p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e [!UICONTROL diariamente]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mudança da data de compromisso de um problema em um dos meus projetos</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando a Data da confirmação for alterada para um problema no projeto, a menos que o usuário que alterar a Data da confirmação seja o mesmo usuário que o Proprietário do projeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Confirmar data para] &lt;issue name=""&gt; [!UICONTROL está agora] &lt;new commit="" date=""&gt;</em></p> <p> O objeto da notificação diária de resumo é: <em> [!UICONTROL Resumo dos projetos que você possui] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome do problema<br>Nome do projeto<br>Número de referência da emissão<br>Nome do usuário que alterou a Data de confirmação<br>Nova Data de Confirmação<br>Data de Conclusão Planejada da Emissão<br>Atribuído ao nome<br>Digitado por nome<br>Proprietário do projeto<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas cuja Data de Confirmação foi alterada<br>*Nome da ocorrência<br>*Data do resumo diário<br></p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e [!UICONTROL diariamente]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
