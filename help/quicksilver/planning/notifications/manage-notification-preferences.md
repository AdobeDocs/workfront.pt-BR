---
title: Gerenciar preferências de notificação do Adobe Workfront Planning
description: Talvez seja possível gerenciar suas preferências de notificação para o Adobe Workfront Planning. Este artigo descreve como configurar as preferências de notificações.
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: 5404cec0cb02d363154a3696b63aaedaafc82688
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 2%

---


# Gerenciar preferências de notificação do Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Você pode receber notificações no aplicativo ou por email quando as seguintes ações ocorrerem no Workfront Planning:

* Alguém adicionar você ou suas equipes a um comentário na página de gravação
* Alguém solicitou permissão para acessar uma exibição ou um espaço de trabalho <!--or <span class="preview">or a record</span>-->
* Alguém concede a você permissão para acessar uma exibição ou um espaço de trabalho <!--or <span class="preview">or a record</span>--> <!--I could not test this but Isk confirmed-->
* Você submete uma solicitação do Workfront Planning.
* Alguém aprovar ou rejeitar uma solicitação do Workfront Planning que você enviou.
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

<!--Old:
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
   <td><p><p>Standard, Light, or Contributor
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
</table> -->

Para obter mais informações sobre notificações do Workfront Planning, consulte também os seguintes artigos:

* Para obter informações sobre comentários em registros, consulte [Gerenciar comentários de registro](/help/quicksilver/planning/records/manage-record-comments.md).
* Para obter informações sobre notificações no aplicativo do Workfront Planning, consulte [Gerenciar notificações no aplicativo do Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md).
* Para obter informações sobre notificações por email do Workfront Planning, consulte [Gerenciar notificações por email do Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md).


## Gerenciar preferências de notificação

1. Faça logon no Workfront com as credenciais da Adobe Experience Cloud.
1. Clique no ícone **menu de conta** ícone ![menu de Conta no Experience Cloud](assets/account-menu-icon-on-experience-cloud.png) no canto superior direito da tela e clique em **Preferências**.
1. Na seção **Notificações**, clique em **Workfront**.
1. Selecione as notificações que deseja receber.
Ou
Desmarque as notificações que deseja parar de receber.

   ![Painel de notificações do Adobe Experience Cloud para o Workfront Planning](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. As seguintes notificações estão disponíveis para o Workfront:

   * **Menções**: você recebe uma notificação quando alguém marca você ou sua equipe em um comentário no Workfront Planning
   * **Solicitações**: você receberá uma notificação quando alguém executar uma das seguintes ações:

      * Solicita ou concede permissão a um objeto do Workfront Planning
      * Você submeteu uma solicitação do Workfront Planning
      * O status de uma solicitação do Workfront Planning que você submeteu alterações
      * Solicita, concede ou rejeita uma aprovação para uma solicitação do Workfront Planning

   Para obter mais informações sobre como gerenciar notificações, consulte [Preferências e notificações da conta](https://experienceleague.adobe.com/pt-br/docs/core-services/interface/features/account-preferences).

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
