---
content-type: reference
navigation-topic: notifications
title: "Notificações: solicitações que fiz"
description: As notificações a seguir informam sobre solicitações feitas no Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: 9f351a16c2a741b922e8ee51efb3ea3d7d2d18e1
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 0%

---

# Notificações: Solicitações que fiz

As notificações a seguir informam sobre as solicitações feitas em [!DNL Adobe Workfront].

Para obter informações sobre como configurar as notificações recebidas, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte também [Notificações de eventos](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Solicitações que fiz</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de aprovação de documento foi concluída</strong> </p> <p>O usuário que solicitou uma aprovação para um documento recebe uma notificação por email quando a solicitação de aprovação de documento é concluída.</p> <p>O assunto do email de notificação instantânea é: <em> &lt;Nome do Aprovador&gt; tem &lt;Decisão de Aprovação ([!UICONTROL Aprovado], [!UICONTROL Aprovado com Alterações], [!UICONTROL Rejeitado])&gt; este documento.</em></p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </td> 
   <td> Nome do Documento<br>Nome do Aprovador </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um documento foi alterado ou carregado sobre um problema para o qual sou o contato principal</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando um documento é carregado ou alterado no problema, a menos que o usuário que carregou ou alterou o documento também seja o contato principal.</p> <p>Uma notificação só será enviada se o projeto estiver configurado como uma [!UICONTROL Fila de Solicitação de Ajuda] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma Fila de Solicitação]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>Documento adicionado a &lt;Nome do Problema&gt;</em></p> <p>O assunto da notificação de resumo diário é: <em>Resumo de suas solicitações &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Objeto no qual o documento foi carregado<br>Nome do Objeto Pai<br>Número de Referência do Documento<br>Nome do usuário que carregou o documento<br>Nome do Documento<br>Adicionado na Data<br>Detalhes do Documento (formato, tamanho, Número da Versão)<br>Miniatura do Documento<br><strong>[!UICONTROL Visualização]</strong> e <strong>[!UICONTROL Download]</strong> botões<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de documentos carregados<br>*Nome do documento{1 5}*Nome do Objeto Pai<br>*Nome do usuário que adicionou o documento<br>*Data do resumo diário<br> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma solicitação de carregamento de documento foi atendida</strong> </p> <p>O Solicitante de documentos recebe uma notificação por email quando uma solicitação de upload de documento é atendida.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Sua solicitação de documento de] &lt;Nome de Usuário&gt; foi atendida</em></p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </td> 
   <td> <p>Nome do usuário que carregou o documento<br>Nome do Objeto onde o documento foi carregado<br>Nome do Documento<br><br></p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma tarefa pessoal que eu atribuí a outra pessoa foi concluída</strong> </p> <p>Uma notificação é enviada ao usuário que atribuiu uma tarefa ad-hoc a outra pessoa quando essa tarefa for concluída. </p> <p>Para obter mais informações sobre tarefas ad hoc, consulte <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Criar itens de trabalho e projetos na área [!UICONTROL Início]</a>.</p> <p>O assunto do email de notificação instantânea é: <em>Conclusão da tarefa: &lt;Nome da tarefa&gt;</em></p> <p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </p> </td> 
   <td> Nome da Tarefa<br>Nome Padrão do Projeto (Projeto Pessoal do usuário que recebeu a tarefa pessoal)<br>Número de Referência da Tarefa<br>Nome do Proprietário da Tarefa<br>Novo Status da Tarefa<br>Data e Hora em que a tarefa foi concluída<br>Status Anterior da Tarefa<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br><br><br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Um problema para o qual sou o contato principal foi concluído</strong> </p> <p>O contato principal sobre um problema recebe uma notificação quando o problema é concluído.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Conclusão de Problema]: &lt;Nome do Problema&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> Resumo das suas solicitações &lt;Data do resumo diário&gt;</em></p> <p> </p> </td> 
   <td> Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nome do usuário que concluiu o problema<br>Novo Status<br>Data e Hora em que o problema foi concluído<br>Status do Problema Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão <br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas concluídos<br>*Nome do Problema<br>*Nome do usuário que concluiu o problema<br>*Data do resumo diário </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Adiciono um problema a um projeto</strong> </p> <p>O contato principal em um problema recebe uma notificação quando adiciona um problema em um projeto.</p> <p>Uma notificação será enviada somente se o status do projeto for [!UICONTROL Atual] ou [!UICONTROL Planning].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Problema enviado]: &lt;Nome do Problema&gt; em &lt;Nome do Projeto&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> Resumo das suas solicitações &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Problema<br>Seu Nome<br>Nome do Problema<br>Data de Inserção<br>Prioridade do Problema<br>Status do Problema<br>Atribuído ao Nome<br>Contato Principal<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de problemas adicionados<br>*Nome do Problema<br>*Data do resumo diário </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envio uma solicitação (confirmação)</strong> </p> <p>O contato principal sobre o problema recebe uma notificação por email quando envia um problema.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual] e se o projeto estiver configurado como uma [!UICONTROL Fila de Solicitações de Ajuda] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma Fila de Solicitações]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Solicitação Enviada]: &lt;Nome da Solicitação&gt; em &lt;Nome do Projeto (Fila de Solicitações)&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> Resumo das suas solicitações &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> <p>Nome do Projeto (Nome da Fila de Solicitações)<br>Nome do Portfolio<br>Número de Referência do Problema<br>Nome do Problema<br>Data de Inserção<br>Prioridade do Problema<br>Status do Problema<br>Atribuído ao Nome<br>Contato Principal<br>*Número de Referência do Projeto<br>*Nome do Projeto<br>*Número total de solicitações enviadas<br>*Nome da Solicitação<br>*Prioridade da Solicitação<br>*Data do resumo diário</p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Minha solicitação foi fechada (confirmação)</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando a solicitação é fechada.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual e se o projeto estiver configurado como uma [!UICONTROL Fila de Solicitações de Ajuda] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma Fila de Solicitações</a>).</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Sua solicitação foi fechada]:"&lt;Nome da Solicitação&gt;"</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo de suas Solicitações] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome da Solicitação<br>Nome do Projeto<br>Número de Referência da Solicitação<br>Nome do usuário que fechou a Solicitação<br>Status do Problema<br>Data e Hora em que a Solicitação foi fechada<br>Status da Solicitação Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Número de Referência do Projeto<br>*Nome do Projeto<br>*Número total de solicitações fechadas<br>*Nome da Solicitação<br>*Nome do usuário que fechou a solicitação<br>*Data do resumo diário </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém foi atribuído à minha solicitação</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando um usuário é atribuído ao problema, a menos que o contato principal e o usuário atribuído sejam o mesmo usuário.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual e se o projeto estiver configurado como uma [!UICONTROL Fila de Solicitações de Ajuda] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma Fila de Solicitações]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>&lt;Nome do usuário atribuído à sua solicitação&gt; [!UICONTROL foi atribuído à sua solicitação]: "&lt;Nome da Solicitação&gt;"</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo de suas Solicitações] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> <p>Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nome da Solicitação<br>Tipo de Solicitação<br>Data de Inserção<br>Prioridade do Problema<br>Contato Principal<br>Data de Conclusão Planejada<br>Status do Problema<br><strong>Ver Mais Detalhes</strong> botão <br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de solicitações atribuídas<br>*Nome da Solicitação<br>*Atribuído ao Nome<br>*Data do resumo diário</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>O status de um projeto que criei</strong> mudou </p> <p>O usuário que criou o projeto recebe uma notificação por email quando o status do projeto é alterado.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Alteração de Status do Projeto]: &lt;Nome do Projeto&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo de suas Solicitações] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> <p>Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que alterou o status<br>Novo Status<br>Data e Hora em que o Status do Projeto foi alterado<br>Status Anterior do Projeto<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Novo Status do Projeto<br>*Nome do usuário que alterou o status do projeto<br>*Data do resumo diário</p> </td> 
   <td> <p><strong>Instantâneo</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>O status é alterado em minha solicitação</strong> </p> <p>O contato principal do problema recebe uma notificação por email quando o status do problema é alterado, a menos que o usuário que alterou o status também seja o contato principal.</p> <p>Uma notificação será enviada somente se o status do projeto for Atual e o projeto estiver configurado como uma [!UICONTROL Fila de Solicitações de Ajuda] (conforme descrito em <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Criar uma Fila de Solicitações]</a>).</p> <p>O assunto do email de notificação instantânea é: <em>&lt;Nome da Solicitação&gt; é &lt;Novo Status&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> Resumo das suas solicitações &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome da Solicitação<br>Nome do Projeto<br>Número de Referência da Solicitação<br>Nome do usuário que alterou o Status da Solicitação<br>Novo Status<br>Data e Hora em que o Status da Solicitação foi alterado<br>Status da Solicitação Anterior<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br>*Nome do Projeto<br>*Número de Referência do Projeto<br>*Número total de solicitações cujo status foi alterado<br>*Nome da Solicitação<br>*Status da Solicitação Anterior<br>*Novo Status da Solicitação<br>*Nome do usuário que alterou o status<br>*Data do resumo diário<br></td> 
   <td> <p><strong>Diariamente</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
