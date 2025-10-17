---
content-type: reference
navigation-topic: notifications
title: 'Notificações: Informações sobre projetos em que estou'
description: As notificações a seguir alertam sobre atividades que ocorrem em projetos nos quais você está trabalhando.
author: Courtney
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 0%

---

# Notificações: Informações sobre projetos em que estou

As notificações a seguir alertam sobre atividades que ocorrem em projetos nos quais você está trabalhando.

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
   <td> <p><strong>Um documento foi adicionado a um projeto em que estou</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando um documento é adicionado ao projeto, exceto para o usuário que adicionou o documento.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual] e o documento não for Privado.</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Documento adicionado a] &lt;Nome do Projeto&gt;</em></p> <p>O assunto da notificação de resumo diário é <em>[!UICONTROL Resumo dos Projetos em que você está] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Documento<br>Nome do usuário que adicionou o documento<br>Nome do Documento<br>Adicionado na Data<br>Detalhes do Documento (formato, tamanho, Número da Versão)<br>Miniatura do Documento<br><strong>[!UICONTROL Preview]</strong> e <strong>[!UICONTROL Download]</strong> botões<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de documentos adicionados<br>*Nome do Documento<br>*Nome do usuário que carregou documento<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma tarefa de etapa foi concluída em um projeto em que estou</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação quando uma tarefa de etapa do projeto é concluída. As notificações não são enviadas quando uma tarefa pessoal é concluída.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>A linha de assunto é <em>[!UICONTROL Concluído]: &lt;Nome da Tarefa&gt; em &lt;Nome do Projeto&gt;</em></p> <p>O assunto da notificação de resumo diário é <em> [!UICONTROL Resumo dos Projetos em que você está] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Status da Tarefa<br>Data e Hora de conclusão da tarefa<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão <br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas<br>*Nome da Tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></td> 
   <td><strong>[!UICONTROL Diário]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma status de projeto for alterada de ideia/aprovado/solicitado/em planejamento para atual, enviar email para a equipe</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando o status do projeto é definido como [!UICONTROL Atual].</p> <p>Observação: os usuários devem ser listados na guia Equipe de um projeto para receber notificações quando o status do projeto for definido como [!UICONTROL Atual]. Para obter informações sobre como adicionar usuários a uma equipe de projeto, consulte <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gerenciar a Equipe de Projeto</a>.</p> <p>O assunto do email de notificação instantânea é <em>&lt;Nome do Projeto&gt; [!UICONTROL é Atual - Vá para o seu projeto e veja as suas tarefas!]</em></p> <p> O assunto da notificação de resumo diário é <em> [!UICONTROL Resumo dos Projetos em que você está] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Status do Projeto<br>Data de Conclusão Planejada do Projeto <br>Proprietário do Projeto<br>Uma lista de tarefas atribuídas a você, a uma de suas funções de trabalho ou a uma de suas equipes<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Status do Projeto<br>*Data do resumo diário</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Um projeto em que minha equipe se torna ativa</strong> <p>Os membros de uma equipe recebem uma notificação por email quando um projeto se torna ativo. A equipe deve ser atribuída a pelo menos uma tarefa para receber a notificação.</p><p>Se um usuário individual e uma equipe forem atribuídos a uma tarefa no projeto. a equipe não receberá uma notificação.</p><p>O assunto do email de notificação instantânea é <i>&lt;Nome do Projeto&gt; [!UICONTROL está Ativo - Vá para o seu projeto e veja as suas tarefas!]</i></p><p>O assunto da notificação de resumo diário é <em> [!UICONTROL Resumo dos Projetos em que você está] &lt;Data do resumo diário&gt; </em></p></td> 
   <td>Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Status do Projeto<br>Data de Conclusão Planejada do Projeto <br>Proprietário do Projeto<br>Uma lista de tarefas atribuídas à sua equipe<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Status do Projeto<br>*Data do resumo diário</td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um projeto for concluído, enviar email para a equipe</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando o status do projeto é [!UICONTROL Concluído].</p> <p>Dica: se os projetos forem concluídos regularmente, habilitar essa opção pode criar muitos emails para usuários que têm um número limitado de tarefas em muitos projetos.</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Alteração de Status do Projeto]: &lt;Nome do Projeto&gt;</em></p> <p> O assunto da notificação de resumo diário é <em> [!UICONTROL Resumo dos Projetos em que você está] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que concluiu o projeto<br>Status do Projeto<br>Data e Hora em que o projeto foi concluído<br>Status Anterior do Projeto<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Status do Projeto<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma tarefa foi concluída em um projeto em que estou</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando uma tarefa é concluída em seu projeto. <br>Para obter mais informações sobre a equipe do projeto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral da Equipe do Projeto</a>.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Concluído]: &lt;Nome da Tarefa&gt; em &lt;Nome do Projeto&gt;</em></p> <p> <p>Observação: se a tarefa for alterada para um status igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".</p> </p> <p><em> O assunto da notificação de resumo diário é: [!UICONTROL Resumo dos Projetos em que você está] &lt;Data do resumo diário&gt; </em> </p> </td> 
   <td> <p>Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Status da Tarefa<br>Data e Hora em que o status da tarefa foi alterado<br>Status da Tarefa Anterior<br><strong>Botão Ver Mais Detalhes</strong><br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas<br>*Nome da Tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um problema foi adicionado a um projeto em que estou</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação é enviada somente se o status do projeto for Atual.</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Problema adicionado a] &lt;Nome do Projeto&gt;</em></p> <p> </p> <p> O assunto da notificação de resumo diário é <em> [!UICONTROL Resumo dos Projetos em que você está] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Problema<br>Nome do usuário que adicionou o problema<br>Tipo de Problema<br>Nome do Problema<br>Data de Inserção<br>Prioridade do Problema<br>Atribuído ao Nome <br>Status do Problema<br>Contato Principal<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados ao projeto<br>*Nome do Problema<br>*Nome do usuário atribuído ao problema<br>*Data do resumo diário </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um problema foi concluído em um projeto em que estou</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando um problema é concluído em seu projeto.<br>Para obter mais informações sobre a equipe do projeto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral da Equipe do Projeto</a>.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Concluído]: &lt;Nome do Problema&gt; em &lt;Nome do projeto&gt;</em></p> <p> O assunto da notificação de resumo diário é <em> [!UICONTROL Resumo dos Projetos em que você está] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome do Problema<br>Nome do Projeto<br>Nome do usuário que concluiu o problema<br>Status do Problema<br>Data e Hora em que o problema foi concluído<br>Status do Problema Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas concluídos<br>*Nome do Problema<br>*Nome do usuário atribuído ao problema<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um problema não atribuído foi adicionado a um projeto em que estou</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Quem deve ser atribuído a este novo problema no] &lt;Nome do Projeto&gt;?</em></p> <p> O assunto da notificação de resumo diário é <em> [!UICONTROL Resumo dos Projetos em que você está] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Problema<br>Nome do usuário que adicionou o problema<br>Nome do Problema<br>Tipo de Problema<br>Data de Inserção<br>Prioridade do Problema<br>Atribuído ao Nome (vazio) <br>Status do Problema<br>Contato Principal<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados<br>*Nome do Problema<br>*Nome do usuário que adicionou o problema<br>*Data do resumo diário<br></td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sou adicionado a um projeto</strong> </p> <p>O usuário que foi adicionado ao projeto recebe uma notificação por email quando é adicionado, a menos que o usuário se adicione ao projeto.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Você foi adicionado ao projeto] &lt;Nome do Projeto&gt;</em></p> <p> O assunto da notificação de resumo diário é <em> [!UICONTROL Resumo dos Projetos em que você está] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome do Projeto<br>Nome da Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que adicionou você ao projeto<br>Projeto [!UICONTROL Data de Início Planejada]<br>Projeto [!UICONTROL Data de Conclusão Planejada]<br>Percentual de Conclusão do Projeto<br>Nomes de Outros Usuários no Projeto <br>Proprietário do Projeto<br><strong>Cf. Mais Detalhes</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Data do resumo diário</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mudanças de status em um projeto em que estou</strong> </p> <p>Os membros de uma equipe de projeto recebem uma notificação por email quando o status do projeto é alterado. <br>Para obter mais informações sobre a equipe do projeto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral da Equipe do Projeto</a>.</p> <p>O assunto do email de notificação instantânea é <em>[!UICONTROL Alteração de Status do Projeto]: &lt;Nome do Projeto&gt;</em></p> <p> O assunto da notificação de resumo diário é <em> [!UICONTROL Resumo dos Projetos em que você está] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que alterou o status do projeto<br>Novo Status do Projeto<br>Data e Hora em que o status do projeto foi alterado<br>Status do Projeto Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Status do Projeto<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
 </tbody> 
</table>
