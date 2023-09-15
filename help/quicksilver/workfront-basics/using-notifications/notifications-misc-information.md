---
content-type: reference
navigation-topic: notifications
title: "Notificações: informações diversas"
description: As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você está patrocinando.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 8%

---

# Notificações: Informações diversas

As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você está patrocinando.

Para obter informações sobre como configurar as notificações recebidas, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte também [Notificações de eventos](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Não é possível ativar ou desativar as notificações diárias e você não recebe emails de resumo diários para os eventos desta categoria. Você pode ativar ou desativar notificações instantâneas individuais para o [!UICONTROL Diversos] categoria.

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
   <td> <p><strong>Uma mensagem foi enviada para o [!UICONTROL Centro de Notificações]</strong> </p> <p>Você receberá uma notificação por email quando uma nova mensagem for enviada para o [!UICONTROL Centro de Notificações]. </p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL [!DNL Adobe Workfront] Comunicado]: &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> Assunto do anúncio<br>Texto da mensagem incluído na notificação<br>Documento(s) anexado(s)<br>Nome do usuário que enviou a notificação<br>Data e hora em que a notificação foi enviada </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma atribuição primária de uma tarefa for alterada, enviar email para o proprietário do recurso</strong> </p> <p>Quando um dos Subordinados diretos de um usuário designado como gerente é atribuído a uma nova tarefa, o gerente recebe um e-mail sobre a atribuição. </p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Atribuição de Recurso de Tarefa]: &lt;task name=""&gt;</em></p> </td> 
   <td>Nome do projeto<br>Nome da tarefa<br>Data e hora de criação da tarefa<br>Nome do usuário que criou a tarefa<br>Nomes das Atribuições<br>Data de vencimento (data de conclusão planejada)<br>Status da tarefa<br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Depois de receber uma solicitação para carregar um documento, a solicitação é cancelada</strong> </p> <p>O Solicitante de documentos recebe uma notificação por email quando uma solicitação de documento é cancelada.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; cancelou a solicitação de documentos. </em></p> <p>O texto a seguir está incluído no corpo do email de notificação:</p> <p><em>[!UICONTROL Olá] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL não precisa mais que você carregue nada relacionado à solicitação recebida anteriormente. Nós só queríamos que você soubesse.]</em> </p> </td> 
   <td>Nome do usuário que cancelou a solicitação<br>O texto da solicitação de carregamento do documento original<br>Um banner "[!UICONTROL CANCELADO]" sobre a solicitação de documento original<br>Data e hora da solicitação de documento original<br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Foi encontrado um error que requer minha atenção</strong> </p> <p>O usuário que responde a um comentário por email recebe uma notificação por email quando a resposta não é entregue.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Falha ao Processar em] &lt;subject of="" original="" message=""&gt;</em></p> <p>Para obter informações sobre como usar o email para responder a comentários, consulte .<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma atribuição de problema for alterada, enviar email para o proprietário do recurso</strong> </p> <p>O gerente de um usuário atribuído a um problema recebe uma notificação por email quando esse usuário é removido ou atribuído a um problema. </p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>O assunto do email de notificação instantânea é: <em>Atribuição de problema: &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>Nome do problema<br>Nome do projeto<br>Número de referência da edição<br>Nome do usuário que fez a atribuição<br>Tipo de Problema<br>Nome do usuário atribuído ao problema<br>Data do Problema Inserida<br>Prioridade do problema<br>Contato Primário<br>Problema [!UICONTROL Data de Término Planejada]<br>Status do Problema<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um usuário for adicionado à equipe do projeto, enviar email para o proprietário do recurso</strong> </p> <p>Um gerente recebe uma notificação por email quando um de seus usuários é adicionado a um projeto. Essa notificação é enviada independentemente do status do projeto. </p> <p>Os usuários com uma licença de [!UICONTROL Review] não recebem uma notificação.</p> <p>O assunto do email é: <em>Atribuição de projeto: &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que adicionou a pessoa ao projeto<br>Nome do usuário adicionado ao projeto<br>Projeto [!UICONTROL Data de Início Planejada]<br>Projeto [!UICONTROL Data de Término Planejada]<br>Porcentagem Concluída do Projeto<br>Nomes de outros no projeto<br>Status do projeto<br>Proprietário do Projeto<br><strong>[!UICONTROL Ver Mais Detalhes]</strong> botão<br><br><br></p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém adicionar um projeto a um portfólio ou programa que possuo</strong> </p> <p>O portfólio e/ou o proprietário do programa recebem uma notificação quando um novo projeto é adicionado a um portfólio ou programa.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Projeto adicionado a] &lt;portfolio name=""&gt;[GUID do Projeto]</em></p> </td> 
   <td> Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que adicionou o projeto ao portfólio/programa<br><br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém compartilhar um objeto comigo</strong> </p> <p>Você recebe uma notificação por email quando alguém o adiciona à lista de permissões do [!UICONTROL Sharing] em um objeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Acesso Concedido]: &lt;object name=""&gt;</em></p> <p>Uma notificação só será enviada se o projeto estiver com o status [!UICONTROL Atual].</p> </td> 
   <td> Nome do objeto<br>Nome do objeto pai<br>Número de Referência do Objeto<br>Acesso Original ao objeto<br>Novo acesso concedido ao objeto<br>Data e hora em que o acesso foi concedido <br>Nome do usuário que concedeu o acesso </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém compartilhar um objeto com minha equipe</strong> </p> <p>Você recebe uma notificação por email quando alguém adiciona sua equipe à lista de permissões de compartilhamento em um objeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Acesso Concedido]: &lt;object name=""&gt; [GUID da Regra de Acesso]</em></p> </td> 
   <td> Nome do objeto<br>Nome do objeto pai<br>Número de Referência do Objeto<br>Acesso antigo<br>Novo acesso<br>Data e hora em que o acesso foi concedido<br>Nome da sua equipe<br>Nome do usuário que concedeu o acesso </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Foi feita uma atualização em uma tarefa, problema ou projeto que eu assino</strong> </p> <p>Você recebe uma notificação por email quando alguém comenta em um item no qual você está inscrito.</p> <p>O assunto do email de assinatura é: <em>[!UICONTROL Foi feita uma atualização no] &lt;object type=""&gt; você está inscrito em: &lt;object name=""&gt;</em></p> </td> 
   <td> Nome do objeto<br> Número de Referência do Objeto<br> Nome do usuário que fez um comentário no item assinado<br> Data em que o comentário foi feito<br> Comentário adicionado ao item inscrito  </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
