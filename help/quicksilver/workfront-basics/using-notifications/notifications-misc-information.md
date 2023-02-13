---
content-type: reference
navigation-topic: notifications
title: "Notificações: Informações diversas"
description: As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você está patrocinando.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 8%

---

# Notificações: Informações diversas

As notificações a seguir alertam sobre atividades que ocorrem em um projeto que você está patrocinando.

Para obter informações sobre como configurar quais notificações você recebe, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte também [Notificações de evento](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Não é possível ativar ou desativar as notificações diárias e você não recebe emails de resumo diários para os eventos desta categoria. Você pode ativar ou desativar notificações instantâneas individuais para a variável [!UICONTROL Diversos] categoria .

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
   <td> <p><strong>Uma mensagem é enviada para a [!UICONTROL Announcing Center]</strong> </p> <p>Você recebe uma notificação por email quando uma nova mensagem é enviada para a [!UICONTROL Announce Center]. </p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL [!DNL Adobe Workfront] Anúncio]: &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> Objeto do anúncio<br>Texto da mensagem incluída no Anúncio<br>Documento(s) em anexo<br>Nome do usuário que enviou o Anúncio<br>Data e hora em que o Anúncio foi enviado </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma atribuição primária de uma tarefa for alterada, enviar email para o proprietário do recurso</strong> </p> <p>Quando um dos Relatórios Diretos de um usuário designado como gerente é atribuído a uma nova tarefa, o gerente recebe um email sobre a atribuição. </p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Atribuição de recurso de tarefa]: &lt;task name=""&gt;</em></p> </td> 
   <td>Nome do projeto<br>Nome da tarefa<br>Data e hora em que a tarefa foi criada<br>Nome do usuário que criou a tarefa<br>Nomes da Atribuição<br>Data de Vencimento (Data de Conclusão Planejada)<br>Status da tarefa<br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Depois de receber uma solicitação para carregar um documento, a solicitação é cancelada</strong> </p> <p>A Solicitação de documento recebe uma notificação por email quando uma solicitação de documento é cancelada.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; solicitação de documento cancelada. </em></p> <p>O texto a seguir está incluído no corpo da notificação por email:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL não precisa mais fazer upload de nada relacionado à solicitação que você recebeu anteriormente. Só queríamos que você soubesse.]</em> </p> </td> 
   <td>Nome do usuário que cancelou a solicitação<br>O texto da solicitação de upload do documento original<br>Um banner "[!UICONTROL CANCELADO]" sobre a solicitação do documento original<br>Data e hora da solicitação do documento original<br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Foi encontrado um error que requer minha atenção</strong> </p> <p>O usuário que responde a um comentário por email recebe uma notificação por email quando a resposta não é entregue.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Falha ao processar em] &lt;subject of="" original="" message=""&gt;</em></p> <p>Para obter informações sobre como usar email para responder aos comentários, consulte .<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando uma atribuição de problema for alterada, enviar email para o proprietário do recurso</strong> </p> <p>O gerente de um usuário atribuído a um problema recebe uma notificação por email quando esse usuário é removido ou atribuído a um problema. </p> <p>Uma notificação é enviada somente se o status do projeto for Atual ou Planejamento.</p> <p>O assunto do email de notificação instantânea é: <em>Atribuição de Emissão: &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>Nome do problema<br>Nome do projeto<br>Número de referência da emissão<br>Nome do usuário que fez a atribuição<br>Tipo de problema<br>Nome do usuário atribuído ao problema<br>Data de Emissão Inserida<br>Prioridade do problema<br>Contato Principal<br>Emitir [!UICONTROL Data de conclusão planejada]<br>Status do problema<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um usuário for adicionado à equipe do projeto, enviar email para o proprietário do recurso</strong> </p> <p>Um gerente recebe uma notificação por email quando um de seus usuários é adicionado a um projeto. Essa notificação é enviada independentemente do status do projeto. </p> <p>Os usuários com uma licença da [!UICONTROL Review] não recebem uma notificação.</p> <p>O assunto do email é: <em>Atribuição do projeto: &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>Nome do projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que adicionou a pessoa ao projeto<br>Nome do usuário que foi adicionado ao projeto<br>Projeto [!UICONTROL Data de início planejada]<br>Projeto [!UICONTROL Data de conclusão planejada]<br>Porcentagem de Projeto Concluída<br>Nomes de Outros no Projeto<br>Status do projeto<br>Proprietário do projeto<br><strong>[!UICONTROL Ver mais detalhes]</strong> botão<br><br><br></p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém adicionar um projeto a um portfólio ou programa que possuo</strong> </p> <p>O portfólio e/ou o proprietário do programa recebem uma notificação quando um novo projeto é adicionado a um portfólio ou programa.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Projeto adicionado] &lt;portfolio name=""&gt;[GUID do projeto]</em></p> </td> 
   <td> Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que adicionou o projeto ao portfólio/programa<br><br></td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém compartilhar um objeto comigo</strong> </p> <p>Você recebe uma notificação por email quando alguém o adiciona à lista de permissões do [!UICONTROL Sharing] em um objeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Acesso concedido]: &lt;object name=""&gt;</em></p> <p>Uma notificação É enviada somente se o projeto estiver no status [!UICONTROL Atual].</p> </td> 
   <td> Nome do objeto<br>Nome do objeto pai<br>Número de referência do objeto<br>Acesso original ao objeto<br>Novo acesso concedido ao objeto<br>Data e hora em que o acesso foi concedido <br>Nome do usuário que concedeu o acesso </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém compartilhar um objeto com minha equipe</strong> </p> <p>Você recebe uma notificação por email quando alguém adiciona sua equipe à lista de permissões de compartilhamento em um objeto.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Acesso concedido]: &lt;object name=""&gt; [GUID da Regra de Acesso]</em></p> </td> 
   <td> Nome do objeto<br>Nome do objeto pai<br>Número de referência do objeto<br>Acesso antigo<br>Novo acesso<br>Data e hora em que o acesso foi concedido<br>Nome da equipe<br>Nome do usuário que concedeu o acesso </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>É feita uma atualização em uma tarefa, problema ou projeto para o qual estou inscrito</strong> </p> <p>Você recebe uma notificação por e-mail quando alguém comenta sobre um item para o qual você está inscrito.</p> <p>O assunto do email de assinatura é: <em>[!UICONTROL Uma atualização foi feita na] &lt;object type=""&gt; você está inscrito em: &lt;object name=""&gt;</em></p> </td> 
   <td> Nome do objeto<br> Número de referência do objeto<br> Nome do usuário que fez um comentário no item assinado<br> Data em que o comentário foi feito<br> Comentário adicionado ao item assinado  </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
