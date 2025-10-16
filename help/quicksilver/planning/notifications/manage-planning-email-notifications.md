---
title: Gerenciar Notificações por Email do Adobe Workfront Planning
description: Quando alguém marca você ou suas equipes em um comentário de registro no Adobe Workfront Planning, você recebe uma notificação por email para essa tag.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# Gerenciar notificações por email do Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Você pode receber notificações por email do Workfront Planning quando os seguintes cenários existirem:

* Alguém marcar você ou suas equipes em um comentário de registro

  Para obter informações sobre como marcar outras pessoas em um comentário de registro, consulte [Gerenciar comentários de registro](/help/quicksilver/planning/records/manage-record-comments.md).
* Alguém solicitar sua permissão para acessar uma visualização ou um espaço de trabalho
* Alguém confirma que seu acesso foi concedido a uma exibição ou a um espaço de trabalho <!--Isk confirmed that there is nno email for denying access but did not test-->
* Você submete uma solicitação do Workfront Planning. Para obter informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* Alguém aprovar ou rejeitar uma solicitação do Workfront Planning que você enviou. Para obter informações, consulte [Aprovar uma solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
* O status é alterado para uma solicitação do Workfront Planning enviada.

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer Workfront e qualquer pacote do Planning</p> <p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Leve ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Exibir ou aumentar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> Os usuários com uma licença Light ou Contributor devem receber um modelo de layout que inclua o Planning.
   <p>Usuários padrão e Administradores do sistema têm as áreas do Planning habilitadas por padrão.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
OLD: 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard, Light, or Contributor</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>

</tbody> 
</table>
-->


## Gerenciar notificações por email quando alguém adicionar uma tag a você em um comentário

1. (Condicional e opcional) Depois que alguém marcar você ou sua equipe em um comentário em um registro, acesse a notificação por email que informa você sobre a tag e o comentário. O remetente do email é o Adobe Experience Cloud.

   ![Exemplo de notificações por email](assets/email-notification-example.png)

1. (Opcional) Clique na mensagem na caixa **Workfront** dentro do email.

   A página de detalhes do registro é aberta no Workfront. Você pode fazer atualizações no registro ou responder ao comentário.

1. (Condicional) Se disponível, clique em **Exibir todas as notificações**. <!--check with Lilit - do non-IMS users have this button??-->
A página **Notificações** é aberta no Adobe Experience Cloud. Todas as notificações de todos os aplicativos Adobe Experience Cloud são exibidas.

## Gerenciar notificações por email ao solicitar e conceder permissões

1. (Condicional e opcional) Depois que alguém solicitar ou conceder permissões para acessar uma visualização ou um espaço de trabalho, vá para o email que informa sobre a solicitação de permissão. O remetente do email é o Adobe Experience Cloud.

1. (Opcional) Clique na mensagem na caixa **Workfront** dentro do email.

   A página de detalhes do registro é aberta no Workfront. Você pode fazer atualizações no registro ou responder ao comentário.

1. (Condicional) Se disponível, clique em **Exibir todas as notificações**.
A página **Notificações** é aberta no Adobe Experience Cloud. Todas as notificações de todos os aplicativos Adobe Experience Cloud são exibidas.


Para obter informações sobre como solicitar, conceder ou negar permissões para uma exibição ou um espaço de trabalho, consulte [Solicitar permissões para uma exibição ou um espaço de trabalho](/help/quicksilver/planning/access/request-permissions.md).

Para obter informações sobre como gerenciar as notificações do Workfront Planning, consulte [Gerenciar preferências de notificação do Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Gerencie notificações por email sobre envio, aprovação ou rejeição de solicitações do Workfront Planning

1. (Opcional) Vá para o email enviado pelo Workfront
após submeter uma solicitação ou após uma solicitação submetida ter sido aprovada ou rejeitada. O remetente do email é o Adobe Workfront.

1. (Opcional) Clique em **Abrir solicitação**. Isso abre a solicitação no Workfront Planning.

1. Clique no ícone **Notificações** ![Ícone da área Notificações do Unified Shell](assets/notifications-area-icon-unified-shell.png) no canto superior direito da tela para acessar a página **Notificações**.

   Para obter informações sobre como gerenciar as notificações do Workfront Planning, consulte [Gerenciar preferências de notificação do Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
