---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Marcar outros usuários em atualizações
description: Ao fornecer comentários de atualização em um objeto do Adobe Workfront, todos os usuários do projeto podem ver as informações enviadas. No entanto, pode haver momentos em que os usuários que não estão no projeto se beneficiem de visualizar essas informações. Em vez de incluir esses usuários no projeto, você pode marcá-los na atualização para compartilhá-los com eles. Os usuários marcados receberão uma notificação de evento.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 886b5d9084cb1bfb63157152f05fa20128d34903
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# Marcar outros usuários em atualizações

<!--Audited: April, 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

Você pode adicionar tags aos usuários ao fazer uma atualização em um objeto se quiser chamar a atenção deles para um objeto que, de outra forma, eles poderiam não seguir.

Em vez de incluir esses usuários no objeto atribuindo-os a ele ou fazendo com que eles se subscrevam a ele, você pode marcá-los na atualização para compartilhá-lo com eles. Os usuários marcados receberão uma notificação do Workfront sobre a atualização inserida. Dependendo das configurações de notificação, eles também receberão um email sobre a atualização inserida.

## Considerações sobre a marcação de usuários em atualizações

* Os usuários marcados em atualizações devem ativar uma notificação pessoal em seus perfis para que eles recebam a notificação por email. Para obter mais informações, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Para obter informações sobre como adicionar atualizações a objetos do Workfront, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Quando um problema é convertido em um projeto ou tarefa, as atualizações são copiadas para o novo projeto ou tarefa, mas os usuários marcados não. Para continuar a conversa, você deve marcar os participantes novamente.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Novo: Colaborador ou superior para problemas e documentos; Claro ou superior para todos os outros objetos</p>
   <p>Atual: solicitação ou superior para ocorrências e documentos; Revisão ou superior para todos os outros objetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuração do nível de acesso</strong></td> 
   <td> <p>Acesso de visualização ou superior aos objetos nos quais você deseja postar a resposta</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissão de objeto</strong></td> 
   <td> <p>Visualize ou aumente as permissões para os objetos em que deseja postar a resposta</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront. Para obter mais informações, consulte [Requisitos de acesso para a documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Marcar outros usuários em atualizações

Você pode marcar outras pessoas em atualizações das seguintes maneiras:

* **Automaticamente**: quando um usuário inicia um thread, adiciona um comentário ou adiciona uma resposta, ele é automaticamente marcado e adicionado à área Marcar pessoas ou equipes da caixa de comentários. <!--remove the tip below when the new commenting stream is the only stream and the legacy commenting is removed-->

* **Manualmente**: ao adicionar manualmente um usuário à área Marcar pessoas da caixa de comentários.

Também é possível remover usuários que foram marcados por engano ao editar ou responder a um comentário.

1. Comece a atualizar um item de trabalho, conforme descrito em [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Como proprietário do comentário, você é automaticamente marcado e adicionado à área Marcar pessoas ou equipes da caixa de comentários.

   >[!TIP]
   >
   >O proprietário do comentário não pode ver seu próprio nome na área Marcar pessoas ou equipes da caixa de comentários.

1. No **Marcar pessoas ou equipes** comece digitando o nome do usuário ou da equipe que deseja incluir e clique no nome quando ele aparecer na lista suspensa.

   Ou

   Digite o símbolo @ na caixa **Escreva um comentário** comece digitando o nome do usuário ou da equipe que deseja incluir na atualização e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   > 
   >Para identificar o usuário correto quando há usuários com nomes semelhantes ou idênticos, observe o avatar, a função principal do usuário ou seu endereço de email.
   > 
   >Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la quando você marcá-los em uma atualização.
   > 
   >Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![Marcar um usuário](assets/tag-others-unified-commenting-with-all-tab.png)

1. (Opcional) Para tornar a atualização privada, ative **Privativo(s) de minha empresa** no canto inferior direito da caixa de atualização. Isso torna a atualização visível apenas para os usuários em sua empresa. A variável **Privativo(s) de minha empresa** A opção está disponível somente quando uma Empresa é especificada no perfil do Workfront.

   >[!NOTE]
   >
   >* Essa opção é exibida somente quando o usuário está associado a uma Empresa.
   >* Os usuários marcados fora da empresa ainda podem receber uma notificação no aplicativo ou um email, mesmo que não vejam os comentários privados na guia Atualizações. Recomendamos não marcar usuários externos em uma atualização se você não quiser compartilhar as informações com eles.

1. (Opcional) Para adicionar vários usuários e equipes, repita a etapa 2. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Todos os usuários e membros da equipe listados no campo &quot;Marcar pessoas ou equipes&quot; recebem uma notificação no aplicativo para a atualização e podem receber um email, dependendo da configuração de suas configurações de notificação por email. Os usuários que marcam a si mesmos em um comentário ou resposta recebem uma notificação para esse comentário ou resposta e podem ver seu nome na lista como um membro do thread para o restante do thread, mas não recebem outra notificação, a menos que marquem a si mesmos novamente. Para obter mais informações, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) e [Configurar notificações de eventos para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Clique em **Enviar**.\
   Os usuários incluídos na atualização recebem automaticamente a permissão Exibir ao objeto e podem exibir e responder às atualizações feitas no objeto.

   Os nomes das entidades marcadas são exibidos ao lado de seus avatares, até duas entidades. Se mais de duas entidades forem marcadas, o nome da primeira será exibido, além de um número de entidades adicionais marcadas.

   ![](assets/members-icons-expanded-unshimmed.png)

   Quando você estiver marcado no texto do comentário, seu nome será destacado nesses comentários.

   Para obter informações sobre a funcionalidade adicional disponível ao atualizar um item de trabalho, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Opcional) Clique no link **Mais** menu ![](assets/more-menu.png) no canto superior direito do comentário e clique em **Editar**. Remova os usuários marcados e clique em **Enviar**.

   >[!IMPORTANT]
   >
   >Você pode editar um comentário somente dentro de 15 minutos após inseri-lo. Só é possível editar os comentários adicionados.


<!--
   >[!TIP]
   >
   >When using the legacy commenting experience to add comments and replies, comment owners that were not specifically tagged cannot be manually removed by people who use the new commenting experience.
-->

<!--
### Tag others on updates in the legacy Updates section

You can manually tag users in the legacy Updates section. 

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Notify** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. 
   >
   >Users must be associated with at least one job role to view it as you tag them in an update. 
   >
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company. The **Private to my company** option is available only when a Company is specified in your Workfront profile. 

   >[!NOTE]
   >
   >Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them.  

1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the Notify field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in the Notify field for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Update**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply at the top of the update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.

   ![](assets/tagging-transparency-350x192.png)
-->

Para obter informações sobre a funcionalidade adicional disponível ao atualizar um item de trabalho, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



