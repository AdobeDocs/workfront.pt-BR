---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Responder a Atualizações
description: Quando alguém adiciona ou responde a uma atualização em um objeto de trabalho, sua resposta é exibida no thread de comunicação na seção Atualizações do objeto. Você pode adicionar uma resposta a uma atualização ou Curtir se tiver acesso de Visualização ao objeto.
author: Nolan and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Responder a atualizações

<!-- Audited: April 2024-->

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

Quando alguém responde a um comentário ou a uma atualização do sistema em um objeto de trabalho, sua resposta é exibida no thread de comunicação nas guias Comentários e Todos na seção Atualizações do objeto.

>[!IMPORTANT]
>
>Não é possível responder às atualizações do sistema na guia System Activity (Atividade do sistema). Quaisquer respostas a atualizações do sistema feitas na experiência de comentários herdada antes de 11 de abril de 2024 são exibidas como somente leitura .

Este artigo descreve como você responde aos comentários da maioria dos objetos no Workfront. Para ver as diferenças entre as seções Atualizações de vários objetos, consulte [Visão geral da seção Atualizações](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Pacote do Adobe Workfront</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença do Adobe Workfront</strong></td> 
   <td> <p>Para problemas e documentos:</p>

<ul><li><p>Colaborador ou superior</p></li>
   <li><p>Solicitação ou superior</p></li></ul>

<p>Para todos os outros objetos:</p>
   <ul><li><p>Leve ou superior</p></li>
   <li><p>Revisar ou superior</p></li></ul>

</td>  
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuração do nível de acesso</strong></td> 
   <td> <p>Acesso de Visualização ou Edição para o objeto no qual a atualização está</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Exibir permissões para o objeto</p> </td> 
  </tr> 
 </tbody> 
   </table>

Para obter mais informações, consulte [Requisitos de acesso para a documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>New: Contributor or higher for issues and documents; Light or higher for all other objects</p> 
   <p>Current: Request or higher for issues and documents; Review or higher for all other objects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configuration</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator. For more information, see [Access requirements for Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Responder a uma atualização ou uma resposta no Workfront

Você pode responder a um comentário na thread de um objeto que pode ser exibido ou pode fazer logon como administrador de Workfront ou de grupo e responder a um comentário em nome de outro usuário. Para obter mais informações, consulte [Fazer logon como outro usuário](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

### Responder a um comentário

A resposta a um comentário na seção Atualizações de um objeto é semelhante para a maioria dos objetos no Workfront.

1. Vá para o objeto ao qual deseja adicionar uma resposta.
1. Clique em **Atualizações**, depois clique na guia **Comentários** do objeto e localize o comentário ou a resposta à qual deseja responder

   Ou

   Clique na guia **Todos** e em **Responder em Comentários** para abrir o comentário na guia Comentários e respondê-lo. Não é possível responder na guia All.

1. (Opcional) Para incluir texto de uma atualização anterior em sua resposta, clique no menu **Mais** no canto superior direito do comentário que deseja responder e clique em **Citar resposta**. O texto da atualização anterior é exibido na área de entrada, marcado com uma linha cinza vertical.
1. Clique em **Responder**.

   ![Caixa vazia Responder para atualizar](assets/reply-to-update-empty-box.png)

   Você pode ver os usuários que estão ativamente envolvidos na conversa na parte inferior da caixa **Adicionar resposta...** e pode adicionar mais ou remover os que não são mais relevantes. Esses usuários, juntamente com quaisquer usuários que se inscreveram no objeto, recebem uma notificação sempre que uma atualização ou resposta é feita no objeto. Você também pode adicionar tags a mais usuários para incluí-los em sua resposta.  Para marcar mais usuários, consulte [Marcar outros usuários em atualizações](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   >[!TIP]
   >
   >   Para adicionar respostas adicionais a uma resposta existente, você pode começar a digitar na caixa **Adicionar resposta...** ou clicar em **Responder** no comentário original. Sua resposta é adicionada ao final da thread.

1. Comece a digitar sua resposta e use qualquer opção adicional da barra de ferramentas Rich Text. Para obter informações sobre como usar Rich Text ou outros recursos de atualização, consulte [Trabalho de atualização](../updating-work-items-and-viewing-updates/update-work.md).

1. Clique em **Enviar** para salvar a resposta.

1. (Opcional) Clique no menu **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do comentário ao qual você deseja responder para obter mais opções para gerenciar a resposta. Para obter mais informações, consulte [Atualizar trabalho](../updating-work-items-and-viewing-updates/update-work.md).

<!--
### Reply to an update or reply in the legacy Updates section

1. Go to the object to which you want to add a reply.
1. On the **Updates** tab for the object, find the update or reply to which you want to reply.

1. (Optional) To view an image in the existing update do one of the following:

   * Click the **Preview** icon ![](assets/previewimageicon-31x31.png) on the image thumbnail to open the full-size image in a new browser tab.
   * Click the **Download** icon ![](assets/downloadimageicon.png) on the image thumbnail to download the image.

1. Click **Reply** on the update, then type a reply in the box that appears.

   You can see the users who are actively engaged in the conversation or tagged in each reply at the top of that update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object. You can also tag more users to include them in your reply.  To tag more users, see [Tag others on updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)
   
1. (Optional) To include text from a previous update in your reply, click the **More** menu next to the update or reply you want to quote, then click **Quote Reply**. Text from the previous update appears in the input area, marked with a vertical gray line.
1. (Optional) Use formatting, emojis, include links, or images as explained in the section "Use Rich Text in a Workfront update" in the article [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Click **Reply** to save the reply.

-->

## Resposta a uma atualização de uma notificação por email

Dependendo de como suas notificações por email estão configuradas, você poderá receber uma notificação por email quando for feita uma atualização em determinados objetos aos quais tem acesso.

Você pode responder a uma atualização por meio de uma notificação por email das seguintes maneiras:

* Responda ao email recebido. O email de resposta é adicionado como uma resposta do Workfront ao comentário original.
* Use o botão Comentário no email para navegar de volta para o Workfront e responder à atualização na área Atualizações.

Este é um exemplo de uma notificação por email acionada como resultado de uma atualização feita na guia Updates de uma tarefa:

![email.png](assets/email-350x202.png)

Para obter informações, consulte [Responder às notificações por email](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).






