---
title: Solicitar permissões para uma visualização ou um Workspace
description: Quando alguém compartilha um link para uma exibição ou um espaço de trabalho ao qual você não tem acesso, é possível solicitar permissões para poder abri-lo. Este artigo explica as etapas para solicitar acesso a uma exibição ou espaço de trabalho ao encontrar um link compartilhado que não pode ser aberto.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: c879d06cfe7ba76df3e974c160a7349f1503f17f
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Solicitar permissões para uma exibição ou um espaço de trabalho

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>A funcionalidade descrita neste artigo só estará disponível quando sua organização tiver sido integrada à Adobe Unified Experience.
>
>Para obter mais informações, consulte [Experiência unificada da Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


Você pode solicitar permissões para uma view ou um espaço de trabalho quando alguém compartilhar um link com você para a view ou o espaço de trabalho ao qual você não tem acesso.

A solicitação de permissões para uma visualização é semelhante à solicitação de permissões para um espaço de trabalho.

Este artigo descreve como solicitar acesso a uma visualização ou a um espaço de trabalho quando alguém compartilha um link com você e você não pode acessar a página compartilhada.

Para obter informações sobre a concessão de permissões para exibições e espaços de trabalho, consulte os seguintes artigos:

* [Compartilhar exibições](/help/quicksilver/planning/access/share-views.md)
* [Compartilhar espaços de trabalho](/help/quicksilver/planning/access/share-workspaces.md)


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront e do Planning</p> 
Ou
<p>Qualquer pacote de Fluxo de Trabalho e Planejamento</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Qualquer</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>  <p>Após receber sua solicitação de permissão, você pode obter as seguintes permissões:</p>
   <ul><li><p>Exibir ou Gerenciar para um modo de exibição</p></li>
   <li><p>Exibir, Contribute ou Gerenciar em um espaço de trabalho</p></li></ul>  
   <p>Somente usuários com permissões para Gerenciar um espaço de trabalho e uma visualização podem compartilhar uma visualização publicamente.</p></td> 
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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p><b>IMPORTANT</b></p>
<p>The users in your organization can request permissions for views and workspaces only when your organization is onboarded to the Adobe Unified Experience. </p>
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
   <td>  <p>After your request for permission is granted, you could gain the following permissions:</p>
   <ul><li><p>View or Manage for a view</p></li>
   <li><p>View, Contribute, or Manage to a workspace</p></li></ul>  
   <p>Only users with Manage permissions to a workspace and a view can share a view publicly.</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>
 
</tbody> 
</table> -->


## Solicitar permissões para uma exibição ou espaço de trabalho

A solicitação de permissões para uma visualização é semelhante à solicitação de permissão para um espaço de trabalho.

Quando alguém compartilha com você um link para um espaço de trabalho ou uma visualização à qual você não tem acesso:

1. Clique no link compartilhado com você para a exibição ou o espaço de trabalho.

   Uma página **Você não tem acesso** é exibida para informá-lo de que você não tem acesso à exibição ou ao espaço de trabalho.

   ![Solicitar acesso para exibição](assets/request-access-to-view.png)

1. (Condicional) Se o link compartilhado for para uma exibição de um espaço de trabalho ao qual você tem acesso, clique em **Abrir com exibição existente**. Se você tiver permissões para acessar o espaço de trabalho, a página do tipo de registro será aberta na exibição padrão.

1. (Opcional e condicional) Se você não tiver permissões para exibir o espaço de trabalho, adicione uma mensagem personalizada na caixa disponível e clique em **Solicitar acesso**.

   Todos os usuários com permissões para Gerenciar a exibição ou o espaço de trabalho recebem as seguintes notificações para a solicitação de acesso:
   * Uma notificação no aplicativo
     ![Notificação no aplicativo para solicitação de acesso](assets/in-app-notification-for-access-request.png)
   * Uma notificação por email
     ![Notificação por email para a solicitação de acesso](assets/email-notification-for-access-request.png)

1. (Condicional) Quando a exibição ou o gerenciador de espaço de trabalho concede permissões para a exibição ou o espaço de trabalho, você recebe uma notificação por email e uma notificação no aplicativo com uma confirmação de que a permissão foi concedida. <!--check this - I was not able to test this, but Isk confirmed.-->
