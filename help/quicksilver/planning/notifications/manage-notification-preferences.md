---
title: Gerenciar preferências de notificação do Adobe Workfront Planning
description: Talvez seja possível gerenciar suas preferências de notificação para o Adobe Workfront Planning. Este artigo descreve como configurar as preferências de notificações.
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
last-update: 2026-04-01T18:23:03.000Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
TQID: https://experienceleague.adobe.com/C3hvRU9XvH3yqP21zXa4mxH6NrST85Jz98AvqeEHNY4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 614b25d3255b27f09f2624afd8691e08cfb7ddf4
workflow-type: tm+mt
source-wordcount: 522
ht-degree: 10%

---

# Gerenciar preferências de notificação do Adobe Workfront Planning

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Este artigo descreve como gerenciar notificações do Adobe Workfront Planning, e não notificações do Adobe Workfront, em geral.

Você pode receber notificações no aplicativo ou por email quando as seguintes ações ocorrerem no Workfront Planning:

* Alguém adicionar você ou suas equipes a um comentário na página de gravação
* Alguém solicitar permissão para acessar uma visualização, um espaço de trabalho ou um registro
* Alguém concede a você permissão para acessar uma visualização, um espaço de trabalho ou um registro
* Você submete uma solicitação do Workfront Planning.
* Alguém aprovar ou rejeitar uma solicitação do Workfront Planning que você enviou.
* O status é alterado para uma solicitação do Workfront Planning enviada.

Você pode receber e gerenciar os seguintes tipos de notificações das atividades do Workfront Planning:

* No aplicativo
* Email

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
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--
Old:
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
</table>
-->

Para obter mais informações sobre notificações do Workfront Planning, consulte também os seguintes artigos:

* Para obter informações sobre comentários em registros, consulte [Gerenciar comentários de registro](/help/quicksilver/planning/records/manage-record-comments.md).
* Para obter informações sobre notificações de aprovação, consulte os seguintes artigos:

  * [Aprovar uma solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
  * [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md)
* Para obter informações sobre notificações no aplicativo do Workfront Planning, consulte [Gerenciar notificações no aplicativo do Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md).
* Para obter informações sobre notificações por email do Workfront Planning, consulte [Gerenciar notificações por email do Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md).


## Gerenciar preferências de notificação

>[!NOTE]
>
>Você gerencia as notificações do Workfront Planning usando a área Preferências da Adobe, e não a área Notificações da Workfront na página de perfil do usuário.

1. Faça logon no Workfront com suas credenciais da Adobe Experience Cloud.
1. Clique no ícone **menu de conta** ícone ![menu de Conta na Experience Cloud](assets/account-menu-icon-on-experience-cloud.png), no canto superior direito da tela, e clique em **Preferências**.
1. Na seção **Notificações**, clique em **Workfront**.
1. Selecione as notificações que deseja receber.
Ou
Desmarque as notificações que deseja parar de receber.

   ![Painel de notificações da Adobe Experience Cloud para o Workfront Planning](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. As seguintes notificações estão disponíveis para o Workfront:

   * **Aprovações**: você recebe uma notificação quando alguém envia uma solicitação do Planning para aprovação ou quando deseja solicitar acesso a um objeto do Planning.
   * **Menções**: você recebe uma notificação quando alguém marca você ou sua equipe em um comentário no Workfront Planning
   * **Solicitações**: você receberá uma notificação quando alguém executar uma das seguintes ações:

     * Solicita ou concede permissão a um objeto do Workfront Planning
     * Você submeteu uma solicitação do Workfront Planning
     * O status de uma solicitação do Workfront Planning que você submeteu alterações
     * Solicita, concede ou rejeita uma aprovação para uma solicitação do Workfront Planning

   Para obter mais informações sobre como gerenciar notificações, consulte [Preferências e notificações da conta](https://experienceleague.adobe.com/pt-br/docs/core-services/interface/features/account-preferences).

<!--
OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
