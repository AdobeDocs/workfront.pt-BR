---
content-type: reference
navigation-topic: notifications
title: '"Notificações: Comunicação'''
description: As notificações a seguir alertam sobre a comunicação, como um comentário de atualização, que ocorre em um item de trabalho com o qual você está envolvido. Para obter informações sobre como configurar quais notificações você recebe, consulte Ativar ou desativar suas próprias notificações de evento.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1546'
ht-degree: 4%

---

# Notificações: Comunicação

As notificações a seguir alertam sobre a comunicação, como um comentário de atualização, que ocorre em um item de trabalho com o qual você está envolvido. Para obter informações sobre como configurar quais notificações você recebe, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Essas notificações alertam você sobre todos os comentários que foram publicados em um item específico. Por esse motivo, você deve selecionar ou desmarcar todas as notificações ao mesmo tempo para serem entregues em um email de resumo diário. Se quiser ser notificado sobre determinados comentários somente conforme eles ocorrerem, você poderá especificar que as notificações individuais sejam para entrega instantânea.

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
   <td> <p><strong>Alguém tiver me incluído em uma atualização direcionada</strong> </p> <p>Uma atualização direcionada ocorre quando um usuário inclui especificamente outro usuário em uma atualização, conforme descrito em <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Atualizações da [!UICONTROL Marcar outras pessoas]</a>.</p> <p>Nesse caso, o usuário que está incluído na atualização direcionada recebe uma notificação por email sobre a atualização.</p> <p>A notificação por email é enviada somente se o usuário tiver direitos de acesso ao objeto.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;name of="" the="" user="" who="" included="" you="" in="" the="" update=""&gt; [!UICONTROL queria que você soubesse]</em></p> <p>O objeto da notificação diária de resumo é: <em>[!UICONTROL Resumo da comunicação] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do objeto no qual a atualização foi feita<br>Nome do objeto pai<br>Número de referência do objeto<br>Nomes de todos os usuários e equipes incluídos na atualização direcionada<br>Data e hora em que a atualização foi efetuada<br>Texto de atualização direcionada<br><strong>[!UICONTROL Comentário]</strong> botão<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada objeto<br>*<strong>[!UICONTROL Ver todas as notificações]</strong> botão<br>*Data do resumo diário<br></td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando um usuário responde para uma requisição de trabalho, envie email para a pessoa que requisitou o trabalho.</strong> </p> <p>Depois que um usuário envia uma solicitação de trabalho e outro usuário responde a ela, o usuário que enviou a solicitação recebe uma notificação por email.</p> <p>Uma notificação por email não é enviada se:</p> 
    <ul> 
     <li> <p>O usuário que responde é o mesmo usuário que fez a solicitação</p> </li> 
     <li> <p>O usuário não tem acesso para visualizar a nota</p> </li> 
    </ul><strong>O assunto do email de notificação instantânea é: <em>[!UICONTROL Comentário sobre] &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></strong> O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo da comunicação] &lt;date of="" daily="" digest=""&gt;</em></td> 
   <td> Nome da solicitação<br>Nome do projeto<br>Número de referência<br>Nome do usuário que respondeu a sua solicitação<br>Data e hora em que o comentário foi feito<br>Texto do comentário feito em sua solicitação<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada pedido<br>*<strong>[!UICONTROL Ver todas as notificações]</strong> botão<br>*Data do resumo diário<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Foi postado um comentário na sua solicitação</strong> </p> <p>O contato principal de um problema recebe uma notificação por email quando um comentário é postado em uma solicitação do [!UICONTROL Help Desk], a menos que o usuário que postou o comentário também seja o contato principal para o problema.</p> <p>Qualquer usuário que esteja incluído diretamente no comentário também receberá uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Comentário sobre] &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p>O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo da comunicação] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome da solicitação<br>Nome do projeto<br>Número de referência<br>Nome do usuário que respondeu a sua solicitação<br>Data e hora em que o comentário foi feito<br>Texto do comentário feito em sua solicitação<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada pedido<br>*Nome do projeto<br>*<strong>[!UICONTROL Ver todas as notificações]</strong> botão<br>*Data do resumo diário<br></td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Foi adicionado um comentário ao seu documento</strong> </p> <p>O proprietário de um documento em [!DNL Adobe Workfront] O recebe uma notificação por email quando um comentário é postado no documento, a menos que o usuário que postou o comentário também seja o proprietário do documento.</p> <p>Qualquer usuário que esteja incluído diretamente no comentário também receberá uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual]. </p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Comentário sobre] &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo da comunicação] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td>Nome do documento<br>Nome do projeto, tarefa ou ocorrência<br>Número de referência<br>Nome do usuário que respondeu a sua solicitação<br>Data e hora em que o comentário foi feito<br>Texto do comentário feito no documento</td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando alguém comentar em um item de trabalho, envie email para qualquer um que tiver comentado este item de trabalho</strong> </p> <p>Os participantes no thread e os usuários incluídos em uma mensagem direta recebem uma notificação por email quando um usuário faz um comentário no thread.</p> <p>Os usuários devem ter acesso à [!UICONTROL View] para receber uma notificação.</p> <p>Os seguintes usuários não recebem uma notificação:</p> 
    <ul> 
     <li>Equipes incluídas em uma mensagem direta</li> 
     <li>O proprietário da Nota</li> 
     <li>O Contato Principal</li> 
    </ul> <p><strong>O assunto do email de notificação instantânea é: <em>[!UICONTROL RE: Comentar em] &lt;object name=""&gt;&lt;object type=""&gt; on &lt;project name=""&gt;(ref# &lt;object reference="" number=""&gt;</em>)</strong> </p> <p><strong> O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo da comunicação] &lt;date of="" daily="" digest=""&gt;</em></strong> </p> </td> 
   <td> Nome do objeto<br>Nome do objeto pai<br>Nome do usuário que comentou o thread<br>Texto do comentário feito no encadeamento<br>Data e hora em que o comentário foi feito<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada objeto<br>*Nome do projeto<br>*<strong>[!UICONTROL Ver todas as notificações]</strong> botão<br>*Data da compilação diária </td> 
   <td><strong>[!UICONTROL diariamente]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando alguém comentar no item de trabalho, envie email para os atribuídos</strong> </p> <p>O destinatário do item de trabalho recebe uma notificação por email sempre que um usuário adiciona uma atualização a um item de trabalho, a menos que o usuário que adiciona a atualização também seja o destinatário. </p> <p>Quando um comentário for postado em uma solicitação, envie um email para o contato principal da ocorrência.</p> <p>O contato principal de um problema recebe uma notificação por email quando um comentário é postado em uma solicitação, a menos que o usuário que postou o comentário também seja o contato principal para o problema.</p> <p>Qualquer usuário que esteja incluído diretamente no comentário também receberá uma notificação por email.</p> <p>Uma notificação é enviada somente se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Comentário sobre] &lt;work item="" name=""&gt; on &lt;project name="" ref="" work="" item="" reference="" number=""&gt;)</em></p> <p> O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo da comunicação] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome do Item de Trabalho<br>Nome do projeto<br>Número de Referência do Item de Trabalho<br>Nome do usuário que comentou o Item de Trabalho<br>Texto do comentário feito no item de trabalho<br>Data e hora em que o comentário foi feito<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada objeto<br>*Nome do projeto<br>*<strong>[!UICONTROL Ver todas as notificações]</strong> botão<br>*Data da compilação diária </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém tiver incluído minha equipe em uma atualização direta</strong> </p> <p>Uma atualização direcionada ocorre quando um usuário inclui especificamente outro usuário em uma atualização, conforme descrito em <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Marcar outras pessoas em atualizações</a>.</p> <p>Nesse caso, qualquer membro da equipe incluído na atualização direcionada recebe uma notificação por email sobre a atualização.</p> <p>A notificação por email é enviada somente para usuários que têm direitos de acesso ao objeto.</p> <p>Se o usuário que está enviando a atualização direcionada for membro da equipe que está sendo incluída, o usuário que está enviando a atualização não receberá uma notificação por email.</p> <p>O assunto do email de notificação instantânea é: [!UICONTROL Comentário sobre] &lt;object name=""&gt; on &lt;parent object="" name=""&gt; (ref# &lt;object reference="" number=""&gt;)</p> <p> O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo da comunicação] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome do objeto<br>Nome do objeto pai<br>Número de referência do objeto<br>Nome do usuário que fez a atualização direcionada<br>Nome de todas as equipes e usuários incluídos na atualização direcionada<br>Data e hora em que a atualização direcionada foi efetuada<br>Texto da atualização direcionada<br><strong>[!UICONTROL Comentário]</strong> botão<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada objeto<br>*Nome do projeto<br>*<strong>[!UICONTROL Ver todas as notificações]</strong> botão<br>*Data da compilação diária </p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando o comentário é adicionado sobre o usuário</strong> </p> <p>Você pode fazer um comentário em um usuário na guia [!UICONTROL Atualizações] do objeto do usuário. Você também pode fazer um comentário em um usuário ao editar as configurações do usuário. O usuário em relação ao qual o comentário é feito recebe um email para notificá-lo desse comentário. </p> <p>Você deve ter permissões para pelo menos [!UICONTROL Exibir] o usuário para inserir uma atualização na guia [!UICONTROL Atualizações] do usuário. Você deve ter permissões do [!UICONTROL Editar] no usuário para editar as configurações do usuário. </p> <p>Para obter mais informações sobre como fazer comentários sobre usuários na guia Atualizações , consulte <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Atualizar trabalho</a>.</p> <p>Para obter mais informações sobre como inserir um comentário em um usuário ao editar as configurações do usuário, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Definir minhas configurações</a>.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;user name=""&gt; [!UICONTROL queria que você soubesse]</em></p> <p>O objeto da notificação diária de resumo é:<em> [!UICONTROL Resumo da comunicação] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Seu nome de usuário<br>Nome do usuário que adicionou o comentário<br>Texto do comentário<br>Data e hora em que o comentário foi feito<br>*Número total de comentários recebidos<br>*Número de comentários recebidos para cada objeto<br>*<strong>[!UICONTROL Ver todas as notificações]</strong> botão<br>*Data da compilação diária </td> 
   <td> <p><strong>Instantâneo</strong> </p> <p><strong>e Diariamente</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
