---
title: Gerenciar notificações no aplicativo do Adobe Workfront Planning
description: Quando alguém marcar você ou suas equipes em um comentário de registro, você receberá uma notificação por email para essa tag.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 1%

---


# Gerenciar notificações no aplicativo do Adobe Workfront Planning

{{planning-important-intro}}

Você pode receber notificações no aplicativo do Workfront Planning quando os seguintes cenários existirem:

* Alguém marcar você ou suas equipes em um comentário de registro

  Para obter informações sobre como marcar outras pessoas em um comentário de registro, consulte [Gerenciar comentários de registro](/help/quicksilver/planning/records/manage-record-comments.md).
* Alguém solicitar sua permissão para acessar uma visualização ou um espaço de trabalho
* Alguém confirma que seu acesso foi concedido a uma exibição ou a um espaço de trabalho <!--Isk confirmed there is no notification for denying permissions - did not test-->

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
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> Os usuários com uma licença Light ou Contributor devem receber um modelo de layout que inclua o Planning.
   <p>Usuários padrão e Administradores do sistema têm as áreas do Planning habilitadas por padrão.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD:

+++ Expand to view access requirements. 

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
   <p>In order to receive notifications from Workfront Planning, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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

+++
-->

## Gerenciar notificações no aplicativo quando alguém adicionar uma tag a você em um comentário

1. (Condicional) Depois que alguém marcar você ou suas equipes em um comentário sobre um registro, vá para o ícone **Notificações** no aplicativo ![ícone Notificações da Experience Cloud](assets/experience-cloud-notifications-icon.png) na Adobe Experience Cloud.

   ![Exemplo de notificação no aplicativo](assets/in-app-notification-example.png)

1. Clique na notificação.

   A página de detalhes do registro é aberta no Workfront Planning. Você pode fazer atualizações no registro ou responder ao comentário.

1. (Opcional) Clique em **Marcar tudo como lido** para indicar que você leu todas as notificações.
1. (Opcional) Clique em **Exibir tudo** para ir para a página **Notificações** no Adobe Experience Cloud.

## Gerenciar notificações no aplicativo ao solicitar e conceder permissões

Você recebe notificações no aplicativo quando alguém solicita ou concede permissões para uma visualização ou um espaço de trabalho.

Para obter informações sobre como solicitar, conceder ou negar permissões para uma exibição ou um espaço de trabalho, consulte [Solicitar permissões para uma exibição ou um espaço de trabalho](/help/quicksilver/planning/access/request-permissions.md).

Para obter informações sobre como gerenciar as notificações do Workfront Planning, consulte [Gerenciar preferências de notificação do Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
