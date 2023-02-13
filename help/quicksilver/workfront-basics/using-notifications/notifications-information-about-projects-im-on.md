---
content-type: reference
navigation-topic: notifications
title: "Notificações: Informações sobre projetos em que estou"
description: As notificações a seguir alertam sobre atividades que ocorrem em projetos em que você está trabalhando.
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 6%

---

# Notificações: Informações sobre projetos em que estou

As notificações a seguir alertam sobre atividades que ocorrem em projetos em que você está trabalhando.

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
   <td> <p><strong>Quando um documento for adicionado enviar email para a equipe.</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando um documento é adicionado ao projeto, exceto para o usuário que adicionou o documento.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] e o documento não for Privado.</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Documento adicionado ao] &lt;project name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é <em>[!UICONTROL Resumo dos projetos em que você está] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de referência do documento<br>Nome do usuário que adicionou o documento<br>Nome do documento<br>Adição Na Data<br>Detalhes do documento (formato, tamanho, número da versão)<br>Miniatura do documento<br><strong>[!UICONTROL Preview]</strong> e <strong>[!UICONTROL Download]</strong> botões<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de documentos adicionados<br>*Nome do documento<br>*Nome do usuário que carregou o documento<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma etapa for concluída, enviar email para a equipe.</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação quando uma tarefa de marco no projeto é concluída. As notificações não são enviadas quando uma tarefa pessoal é concluída.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>A linha de assunto é <em>[!UICONTROL concluído]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>O objeto da notificação diária de resumo é <em> [!UICONTROL Resumo dos projetos em que você está] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Status da tarefa<br>Data e hora em que a tarefa foi concluída<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão <br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas concluídas<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></td> 
   <td><strong>[!UICONTROL diariamente]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma status de projeto for alterada de ideia/aprovado/solicitado/em planejamento para atual, enviar email para a equipe</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando o status do projeto é definido como [!UICONTROL Atual].</p> <p>Observação: Os usuários devem ser listados na guia Pessoal de um projeto para receber uma notificação quando o status do projeto for definido como [!UICONTROL Atual]. Para obter informações sobre como adicionar usuários a uma equipe de projeto, consulte <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gerenciar a equipe do projeto</a>.</p> <p>O assunto do email de notificação instantânea é <em>&lt;project name=""&gt; [!UICONTROL é atual - Vá para o projeto e veja as tarefas!]</em></p> <p> O objeto da notificação diária de resumo é <em> [!UICONTROL Resumo dos projetos em que você está] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Status do projeto<br>Projeto [!UICONTROL Data de conclusão planejada]<br>Proprietário do projeto<br>Uma lista de tarefas atribuídas a você, a uma de suas funções ou a uma de suas equipes<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Status do projeto<br>*Data da compilação diária</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Um projeto em que minha equipe se torna ativa</strong> <p>Os membros de uma equipe recebem uma notificação por email quando um projeto se torna ativo. A equipe deve ser atribuída a pelo menos uma tarefa para receber a notificação.</p><p>Se um usuário individual e uma equipe forem atribuídos a uma tarefa no projeto. a equipe não receberá uma notificação.</p><p>O assunto do email de notificação instantânea é <i>&lt;project name=""&gt; [!UICONTROL está ativo - Vá para o projeto e veja as tarefas!]</i></p><p>O objeto da notificação diária de resumo é <em> [!UICONTROL Resumo dos projetos em que você está] &lt;date of="" daily="" digest=""&gt; </em></p></td> 
   <td>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Status do projeto<br>Projeto [!UICONTROL Data de conclusão planejada]<br>Proprietário do projeto<br>Uma lista de tarefas atribuídas à equipe<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Status do projeto<br>*Data da compilação diária</td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um projeto for concluído, enviar email para a equipe</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando o status do projeto é [!UICONTROL concluído].</p> <p>Dica: Se os projetos forem concluídos regularmente, ativar essa opção poderá criar muitos emails para usuários que têm um número limitado de tarefas em muitos projetos.</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Alteração de status do projeto]: &lt;project name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é <em> [!UICONTROL Resumo dos projetos em que você está] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que concluiu o projeto<br>Status do projeto<br>Data e hora em que o projeto foi concluído<br>Status do projeto anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Status do projeto<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma tarefa for concluída, enviar email para a equipe</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando uma tarefa é concluída em seu projeto. <br>Para obter mais informações sobre a equipe do projeto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral da equipe do projeto</a>.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL concluído]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>Observação: Se a tarefa for alterada para um status que seja igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".</p> </p> <p><em> O objeto da notificação diária de resumo é: [!UICONTROL Resumo dos projetos em que você está] &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> <p>Nome da tarefa<br>Nome do projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Status da tarefa<br>Data e hora em que o status da tarefa foi alterado<br>Status da Tarefa Anterior<br><strong>Veja mais detalhes</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de tarefas concluídas<br>*Nome da tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for adicionada enviar email para a equipe.</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Problema adicionado ao] &lt;project name=""&gt;</em></p> <p> </p> <p> O objeto da notificação diária de resumo é <em> [!UICONTROL Resumo dos projetos em que você está] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de referência da emissão<br>Nome do usuário que adicionou o problema<br>Tipo de problema<br>Nome do problema<br>Data Inserida<br>Prioridade do problema<br>Atribuído ao nome <br>Status do problema<br>Contato Principal<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas adicionados ao projeto<br>*Nome da ocorrência<br>*Nome do usuário atribuído ao problema<br>*Data da compilação diária </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for concluído enviar email para a equipe</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando um problema é concluído em seu projeto.<br>Para obter mais informações sobre a equipe do projeto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral da equipe do projeto</a>.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL concluído]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é <em> [!UICONTROL Resumo dos projetos em que você está] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome do problema<br>Nome do projeto<br>Nome do usuário que concluiu o problema<br>Status do problema<br>Data e hora em que o problema foi concluído<br>Status do problema anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas concluídos<br>*Nome da ocorrência<br>*Nome do usuário atribuído ao problema<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema não atribuída for adicionada enviar email para a equipe.</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Quem deve ser atribuído a este novo problema em] &lt;project name=""&gt;?</em></p> <p> O objeto da notificação diária de resumo é <em> [!UICONTROL Resumo dos projetos em que você está] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de referência da emissão<br>Nome do usuário que adicionou o problema<br>Nome do problema<br>Tipo de problema<br>Data Inserida<br>Prioridade do problema<br>Atribuído a Nome (vazio) <br>Status do problema<br>Contato Principal<br>*Nome do projeto<br>*Número de referência do projeto<br>*Número total de problemas adicionados<br>*Nome da ocorrência<br>*Nome do usuário que adicionou o problema<br>*Data do resumo diário<br></td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um usuário for adicionado à equipe do projeto, enviar email para o usuário</strong> </p> <p>O usuário que foi adicionado ao projeto recebe uma notificação por email quando é adicionado, a menos que o usuário se tenha adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Você foi adicionado ao projeto] &lt;project name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é <em> [!UICONTROL Resumo dos projetos em que você está] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que adicionou você ao projeto<br>Projeto [!UICONTROL Data de início planejada]<br>Projeto [!UICONTROL Data de conclusão planejada]<br>Porcentagem de Projeto Concluída<br>Nomes de Outros no Projeto <br>Proprietário do projeto<br><strong>Veja mais detalhes</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Data da compilação diária</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma status de projeto for alterado, enviar email para a equipe</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando o status do projeto é alterado. <br>Para obter mais informações sobre a equipe do projeto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral da equipe do projeto</a>.</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Alteração de status do projeto]: &lt;project name=""&gt;</em></p> <p> O objeto da notificação diária de resumo é <em> [!UICONTROL Resumo dos projetos em que você está] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que alterou o status do projeto<br>Novo status do projeto<br>Data e hora em que o status do projeto foi alterado<br>Status do projeto anterior<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br>*Nome do projeto<br>*Número de referência do projeto<br>*Status do projeto<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
 </tbody> 
</table>
