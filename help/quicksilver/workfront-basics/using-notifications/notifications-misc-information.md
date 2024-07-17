---
content-type: reference
navigation-topic: notifications
title: "Notificações: informações diversas"
description: As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você está patrocinando.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 298b74c2d228a76c02d34470fa8298028605cab4
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 0%

---

# Notificações: Informações diversas

As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você está patrocinando.

Para obter informações sobre como configurar as notificações recebidas, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte também [Notificações de eventos](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Não é possível ativar ou desativar as notificações diárias e você não recebe emails de resumo diários para os eventos desta categoria. Você pode habilitar ou desabilitar notificações instantâneas individuais para a categoria [!UICONTROL Diversos].

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
   <td> <p><strong>Uma mensagem foi enviada para o [!UICONTROL Centro de Notificações]</strong> </p> <p>Você receberá uma notificação por email quando uma nova mensagem for enviada para o [!UICONTROL Centro de Notificações]. </p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL [!DNL Adobe Workfront] Aviso]: &lt;Assunto do Aviso&gt;</em></p> </td> 
   <td> Assunto do Aviso<br>Texto da mensagem incluído no Aviso<br>Documento(s) Anexado(s)<br>Nome do usuário que enviou o Aviso<br>Data e Hora em que o Aviso foi enviado </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma alteração de atribuição de tarefa afeta uma de minhas pessoas</strong> </p> <p>Quando um dos Subordinados diretos de um usuário designado como gerente é atribuído a uma nova tarefa, o gerente recebe um e-mail sobre a atribuição. </p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Atribuição de Recurso de Tarefa]: &lt;Nome da Tarefa&gt;</em></p> </td> 
   <td>Nome do projeto<br>Nome da tarefa<br>Data e hora de criação da tarefa<br>Nome do usuário que criou a tarefa<br>Nomes das atribuições<br>Data de vencimento (Data de conclusão planejada)<br>Status da tarefa<br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Depois de receber uma solicitação para carregar um documento, a solicitação foi cancelada</strong> </p> <p>O Solicitante de documentos recebe uma notificação por email quando uma solicitação de documento é cancelada.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;Nome do usuário que cancelou a solicitação&gt; cancelou a solicitação de documento. </em></p> <p>O texto a seguir está incluído no corpo do email de notificação:</p> <p><em>[!UICONTROL Olá] &lt;Seu Nome&gt;, <br><br>&lt;Nome do usuário que cancelou a solicitação&gt;[!UICONTROL não precisa mais que você carregue nada relacionado à solicitação recebida anteriormente. Só queremos que você saiba.]</em> </p> </td> 
   <td>Nome do usuário que cancelou a solicitação<br>O texto da solicitação de carregamento do documento original<br>Um banner "[!UICONTROL CANCELED]" sobre a solicitação do documento original<br>Data e hora da solicitação do documento original<br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Foi encontrado um erro que precisa de minha atenção</strong> </p> <p>O usuário que responde a um comentário por email recebe uma notificação por email quando a resposta não é entregue.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Falha ao Processar em] &lt;assunto da mensagem original&gt;</em></p> <p>Para obter informações sobre como usar o email para responder a comentários, consulte <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">Responder a notificações por email</a>.</p> </td>
   <td> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma alteração de atribuição de problema afeta uma de minhas pessoas</strong> </p> <p>O gerente de um usuário atribuído a um problema recebe uma notificação por email quando esse usuário é removido ou atribuído a um problema. </p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>O assunto do email de notificação instantânea é: <em>Atribuição de Problema: &lt;Nome do Problema&gt;</em></p> </td> 
   <td> <p>Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nome do usuário que fez a atribuição<br>Tipo de Problema<br>Nome do usuário atribuído ao problema<br>Data do Problema Inserida<br>Prioridade do Problema<br>Contato Principal<br>Problema [!UICONTROL Data de Conclusão Planejada]<br>Status do Problema<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uma de minhas pessoas foi adicionada a um projeto</strong> </p> <p>Um gerente recebe uma notificação por email quando um de seus usuários é adicionado a um projeto. Essa notificação é enviada independentemente do status do projeto. </p> <p>Os usuários com uma licença de [!UICONTROL Review] não recebem uma notificação.</p> <p>O assunto do email é: <em>Atribuição do Projeto: &lt;Nome do Usuário&gt;[&lt;GUID do Projeto&gt;_ &lt;GUID do Usuário&gt;]</em></p> </td> 
   <td> <p>Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que adicionou a pessoa ao projeto<br>Nome do usuário que foi adicionado ao projeto<br>Data de Início Planejada do Projeto [!UICONTROL]<br>Data de Conclusão Planejada do Projeto [!UICONTROL]<br>Percentual de Conclusão do Projeto<br>Nomes de Outros no Projeto<br>Status do Projeto<br>Proprietário do Projeto<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br><br><br></p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém adicionar um projeto a um portfólio ou programa que possuo</strong> </p> <p>O portfólio e/ou o proprietário do programa recebem uma notificação quando um novo projeto é adicionado a um portfólio ou programa.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Projeto adicionado a] &lt;Nome do Portfolio&gt;[GUID do Projeto]</em></p> </td> 
   <td> Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que adicionou o projeto ao portfólio/programa<br><br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém compartilhar um objeto comigo</strong> </p> <p>Você recebe uma notificação por email quando alguém o adiciona à lista de permissões do [!UICONTROL Sharing] em um objeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Acesso Concedido]: &lt;Nome do Objeto&gt;</em></p> <p>Uma notificação só será enviada se o projeto estiver com o status [!UICONTROL Atual].</p> </td> 
   <td> Nome do Objeto<br>Nome do Objeto Pai<br>Número de Referência do Objeto<br>Acesso Original ao objeto<br>Novo Acesso concedido ao objeto<br>Data e Hora em que o acesso foi concedido <br>Nome do usuário que concedeu o acesso </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém compartilhar um objeto com minha equipe</strong> </p> <p>Você recebe uma notificação por email quando alguém adiciona sua equipe à lista de permissões de compartilhamento em um objeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Acesso Concedido]: &lt;Nome do Objeto&gt; [GUID da Regra de Acesso]</em></p> </td> 
   <td> Nome do Objeto<br>Nome do Objeto Pai<br>Número de Referência do Objeto<br>Acesso Antigo<br>Novo Acesso<br>Data e Hora em que o acesso foi concedido<br>Nome da sua equipe<br>Nome do usuário que concedeu o acesso </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Foi feita uma atualização em uma tarefa, problema ou projeto que eu assino</strong> </p> <p>Você recebe uma notificação por email quando alguém comenta em um item no qual você está inscrito.</p> <p>O assunto do email de assinatura é: <em>[!UICONTROL Foi feita uma atualização no] &lt;Tipo de Objeto&gt; ao qual você está inscrito: &lt;Nome do Objeto&gt;</em></p> </td> 
   <td> Nome do Objeto<br> Número de Referência do Objeto<br> Nome do usuário que fez um comentário no item inscrito<br> Data em que o comentário foi feito<br> Comentário adicionado ao item inscrito  </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
