---
content-type: reference
navigation-topic: notifications
title: 'Notificações: informações sobre os projetos que possuo'
description: As notificações a seguir alertam você sobre atividades que ocorrem em um projeto que você possui. Para obter informações sobre como configurar as notificações recebidas, consulte Modificar suas próprias notificações por email.
author: Courtney
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 1%

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
   <td> <p><strong>Um documento foi adicionado a um projeto do qual sou proprietário</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando um documento é adicionado ao projeto, a menos que o usuário que adicionou o documento também seja o Proprietário do projeto.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual] e o documento não for Privado.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Documento adicionado a] &lt;Nome do Projeto&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que adicionou o documento<br>Nome do Documento<br>Adicionado na Data<br>Detalhes do Documento (formato, tamanho, Número da Versão)<br><strong>[!UICONTROL Pré-visualização]</strong> e <strong>[!UICONTROL Download]</strong> botões<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de documentos adicionados<br>*Nome do Documento<br>*Nome do usuário que adicionou o documento<br>*Data de resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma tarefa de etapa foi concluída em um projeto meu</strong> </p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;Nome da Tarefa&gt; em &lt;Nome do Projeto&gt;</em></p> <p>Observação: se a tarefa for alterada para um status igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".</p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa<br>Novo Status da Tarefa<br>Data e Hora em que a tarefa foi concluída<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas<br>*Nome da Tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um projeto for alterado de uma status positiva de progresso (no prazo) para uma status negativa de progresso (em atraso), enviar email para o proprietário do projeto</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando o projeto está atrasado. Um projeto está atrasado no agendamento quando o Status de Progresso é "[!UICONTROL em Risco]", "[!UICONTROL Atrasado]" ou "[!UICONTROL Atrasado]".</p> <p>A prática recomendada é manter essa notificação ativa. </p> <p>Os usuários com uma licença de [!UICONTROL Review] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de Progresso do Projeto]: &lt;Nome do Projeto&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Status de Progresso do Projeto<br>Data de Início Planejada do Projeto <br>Data de Conclusão Planejada do Projeto <br>Projeto [!UICONTROL Data de Início Projetada]<br>Projeto [!UICONTROL Data de Conclusão Projetada]<br>Percentual de Conclusão do Projeto<br>Status do Projeto<br>Proprietário do Projeto<br>*Nome da Referência do Projeto<br>*Número de Referência do Projeto<br>*Status de Progresso do Projeto<br> do Projeto do Projeto*Data do resumo diário<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um problema for adicionada enviar email para o proprietário do projeto</strong> </p> <p>O proprietário do projeto recebe uma notificação por email quando um problema é adicionado ao projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Problema adicionado a] &lt;Nome do Projeto&gt;</em></p> <p> </p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Problema<br>Nome do usuário que adicionou o problema<br>Nome do Problema<br>Tipo de Problema<br>Data de Inserção<br>Prioridade do Problema<br>Atribuído ao Nome <br>Status do Problema<br>Contato Principal<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados ao projeto<br>*Nome do Problema<br>*Nome do usuário que adicionou o problema<br>*Data do resumo diário</p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma tarefa foi concluída em um projeto que possuo</strong> </p> <p>O Proprietário do projeto recebe uma notificação quando uma tarefa é concluída em seu projeto.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;Nome da Tarefa&gt; em &lt;Nome do Projeto&gt;</em></p> <p> <p>Observação: se a tarefa for alterada para um status igual a [!UICONTROL Concluído], o assunto do email ainda exibirá "[!UICONTROL Concluído]".</p> </p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Nome do usuário que concluiu a tarefa <br>Status da Tarefa<br>Data e Hora em que a tarefa foi concluída<br>Status da Tarefa Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas concluídas <br>*Nome da Tarefa<br>*Nome do usuário que concluiu a tarefa<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma tarefa em um projeto que eu possuo fica atrasada</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando uma tarefa no projeto atrasa o agendamento. "Uma tarefa está atrasada quando o Status do Progresso é "[!UICONTROL em Risco]", "[!UICONTROL Atrasado]" ou "[!UICONTROL Atrasado]"."</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração do Progresso da Tarefa]: &lt;Nome da Tarefa&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Novo Status de Progresso da Tarefa<br>Tarefa [!UICONTROL Data de Início Planejada]<br>Tarefa [!UICONTROL Data de Conclusão Planejada]<br>Tarefa [!UICONTROL Data de Início Projetada]<br>Tarefa [!UICONTROL Data de Conclusão Projetada]<br>Percentual de Tarefa Concluído<br>Status da Tarefa<br>Atribuído ao Nome<br>Inserido pelo Nome<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Total do Projeto número de tarefas atrasadas<br>*Nome da Tarefa<br>*Atribuídas ao Nome<br>*Data do resumo diário </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um problema foi concluído em um projeto que possuo</strong> </p> <p>O Proprietário do projeto recebe uma notificação por email quando um problema é concluído em seu projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>Os usuários com uma licença de [!UICONTROL Review] não recebem uma notificação. </p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Concluído]: &lt;Nome do Problema&gt; em &lt;Nome do Projeto&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nome do usuário que concluiu o problema<br>Status do Problema<br>Data e Hora em que o problema foi concluído<br>Status do Problema Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão <br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas concluídos<br>*Nome do Problema<br>*Nome do usuário atribuído ao problema<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um problema não atribuído foi adicionado a um projeto do qual sou proprietário</strong> </p> <p>O proprietário do projeto recebe uma notificação por email quando um problema não atribuído é adicionado ao projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Quem deve ser atribuído a este novo problema no] &lt;Nome do Projeto&gt;?</em></p> <p> </p> <p> O assunto da notificação de resumo diário é: <em> Resumo dos projetos que você possui &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Problema<br>Nome do usuário que adicionou o problema<br>Nome do Problema<br>Tipo de Problema<br>Data de Inserção<br>Prioridade do Problema<br>Atribuído ao Nome (vazio)<br>Status do Problema<br>Contato Principal<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados<br>*Nome do Problema<br>*Nome do usuário que adicionou o problema<br>*Data do resumo diário<br></p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estou definido como proprietário de um novo projeto</strong> </p> <p>Quando um usuário é atribuído como o proprietário de um projeto, ele recebe uma notificação por email.</p> <p>Se o proprietário do projeto for o mesmo usuário que fez a atribuição, uma notificação por email não será enviada.</p> <p>Os usuários com uma licença de [!UICONTROL Review] não recebem uma notificação.</p> <p>Ligar este recurso porque eles estão sendo atribuídos a algo. </p> <p> Atribuir algo, compartilhar algo, obter acesso a algo.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Agora você é o proprietário do projeto de] &lt;Nome do Projeto&gt;</em></p> <p>O texto a seguir está incluído no corpo do email de notificação:<em><br></em></p> <p><em>[!UICONTROL Olá] &lt;Seu Nome&gt;,<br></em><em>&lt;Nome do usuário que o atribuiu como Proprietário do Projeto&gt; [!UICONTROL tornou você o proprietário de] &lt;Nome do Projeto&gt;. [!UICONTROL Como Proprietário do Projeto, você poderá receber notificações de email adicionais sobre as atividades do projeto, ter de aprovar horas para o projeto ou envolver-se na aprovação de trabalho relacionado ao projeto. É todo seu.]</em> </p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;Data do resumo diário&gt; </em></p> <p> </p> </td> 
   <td> <p>Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Data de Conclusão do Projeto<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Data do resumo diário</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A data de confirmação de uma tarefa em um dos meus projetos</strong> foi alterada </p> <p>O Proprietário do projeto recebe uma notificação por email quando a Data de confirmação é alterada para uma tarefa no projeto, a menos que o usuário que alterou a Data de confirmação também seja o Proprietário do projeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Data de confirmação para] &lt;Nome da Tarefa&gt; [!UICONTROL agora é] &lt;Nova Data de Confirmação&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> Resumo dos projetos que você possui &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Nome do usuário que alterou a Data de Confirmação<br>Nova Data de Confirmação<br>Tarefa [!UICONTROL Data de Conclusão Planejada]<br>Informações sobre como a Linha do Tempo do Projeto é afetada por essa alteração<br>Atribuído ao Nome<br>Inserido pelo Nome<br>Proprietário do Projeto<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de tarefas cuja Data de Confirmação tem alterado<br>*Nome da tarefa<br>*Data do resumo diário<br></p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e [!UICONTROL Diariamente]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A data de confirmação de um problema em um dos meus projetos</strong> foi alterada </p> <p>O Proprietário do projeto recebe uma notificação por email quando a Data de confirmação é alterada para um problema no projeto, a menos que o usuário que altera a Data de confirmação seja o mesmo usuário que o Proprietário do projeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Data de confirmação para] &lt;Nome do Problema&gt; [!UICONTROL agora é] &lt;Nova Data de Confirmação&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo dos Projetos que Você Possui] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nome do usuário que alterou a Data de Confirmação<br>Nova Data de Confirmação<br>Data de Conclusão Planejada do Problema<br>Atribuído ao Nome<br>Informado por Nome<br>Proprietário do Projeto<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas cuja Data de Confirmação foi alterada<br>*Nome do Problema<br>*Data do resumo diário<br></p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e [!UICONTROL Diariamente]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
