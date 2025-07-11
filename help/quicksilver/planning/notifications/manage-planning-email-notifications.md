---
title: Gerenciar Notificações por Email do Adobe Workfront Planning
description: Quando alguém marca você em um comentário de registro no Adobe Workfront Planning, você recebe uma notificação por email para essa marca.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: 60f2890e431065d0eb034a9254680e43a51ecab8
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 1%

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

+++ Expanda para visualizar os requisitos de acesso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produtos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer um dos seguintes planos da Workfront:</p> 
<ul><li>Selecionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience.</p> 
<p>Os usuários em sua organização recebem notificações do Workfront Planning somente quando sua organização é integrada à Adobe Unified Experience. </p>
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Padrão, Claro ou Contribuinte</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Exibir ou aumentar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
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
