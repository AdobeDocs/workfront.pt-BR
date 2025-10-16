---
title: Compartilhar espaços de trabalho
description: Você pode compartilhar um espaço de trabalho com outras pessoas para garantir a colaboração ao trabalhar no Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: f2fe6ef78b3032f7a89d4c816cb11b525634c067
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 1%

---

# Compartilhar espaços de trabalho

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Você pode compartilhar um espaço de trabalho com outras pessoas para garantir a colaboração ao trabalhar no Adobe Workfront Planning.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>Conceder permissões a um espaço de trabalho não concede a outros usuários permissões para as exibições nas páginas do tipo de registro. Você deve conceder permissões a exibições individuais em uma página de tipo de registro para compartilhá-las com outros usuários. Para obter informações, consulte [Compartilhar uma exibição](/help/quicksilver/planning/access/share-views.md).


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront e do Planning</p> 
Ou
<p>Qualquer pacote de Fluxo de Trabalho e Planejamento</p> 
 </tr>
<tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr>

<td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>  <p>Gerenciar permissões em um espaço de trabalho</p>  </td> 
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
<p>Your organization must be onboarded to the Adobe Unified Experience for users to be able to request and grant permissions to a workspace from a permission request. </p> 
<p>Users must be added to the Adobe Admin Console in order to gain permissions to Workfront Planning workspaces.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
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
   <td>  <p>Manage permissions to a workspace</p>  </td> 
  </tr> 

</tbody> 
</table> -->

## Considerações sobre compartilhamento de espaços de trabalho

* Para obter informações gerais sobre o compartilhamento de objetos no Workfront Planning, consulte também [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* Você pode compartilhar espaços de trabalho com usuários, equipes, funções, grupos ou empresas dentro da organização.
* Além de equipes, grupos, empresas e funções de trabalho, você pode compartilhar somente com usuários que foram adicionados à Adobe Admin Console.
* Não é possível compartilhar espaços de trabalho com usuários fora da organização.
* Quando você compartilha um espaço de trabalho, todos os tipos de registro, registros e campos associados aos espaços de trabalho também são compartilhados.
* Quando você compartilha um espaço de trabalho, as exibições não são compartilhadas. Você deve compartilhar exibições separadamente.
* As permissões do Workspace são exibidas como permissões herdadas em tipos de registro.

## Compartilhar permissões em um espaço de trabalho

Os seguintes usuários podem compartilhar um espaço de trabalho com outros usuários:

* Os administradores do sistema podem compartilhar todos os espaços de trabalho, incluindo aqueles que não foram criados.
* Todos os outros usuários podem compartilhar somente espaços de trabalho para os quais tenham permissões de gerenciamento.

Para compartilhar um espaço de trabalho com outras pessoas:

{{step1-to-planning}}

1. Abra o espaço de trabalho que deseja compartilhar e clique em **Compartilhar** no canto superior direito da tela.

   ![Botão Compartilhar no canto superior direito do espaço de trabalho](assets/share-button-on-workspace-top-right.png)

1. No campo **Conceder acesso a este espaço de trabalho**, comece digitando o nome de um usuário, grupo, equipe, empresa ou função de trabalho e clique nele quando ele for exibido na lista.

   ![Compartilhando a interface com grupos](assets/sharing-ui-with-groups.png)

   >[!NOTE]
   >
   >   Além de equipes, grupos, empresas e funções de trabalho, você pode compartilhar somente com usuários que foram adicionados à Adobe Admin Console. Não é possível adicionar usuários somente do Workfront. Para obter informações, consulte [Gerenciar usuários na Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).


1. Selecione um dos seguintes níveis de permissão no menu suspenso:
   * Exibir
   * Contribuir
   * Gerenciar

     Para obter informações sobre níveis de permissão e quais ações os usuários podem executar para cada nível, consulte [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Clique em **Copiar link** para copiar um link para o espaço de trabalho para a área de transferência.
1. Compartilhar o link copiado com outras pessoas. Os usuários que recebem o link devem ser usuários ativos e fazer logon no Workfront para acessar o espaço de trabalho.
1. Clique em **Salvar**.

   Os usuários com os quais você compartilhou o espaço de trabalho recebem uma notificação no aplicativo e por email sobre permissões para ele.

## Conceder permissões a um espaço de trabalho a partir de uma solicitação de permissão

Os usuários que acessam um link para um espaço de trabalho para o qual não têm permissões podem solicitar permissões para o espaço de trabalho. Todos os usuários com permissões para Gerenciar o espaço de trabalho recebem a solicitação de permissão e podem conceder ou negar as permissões.

1. (Condicional) Se você for o gerente de um espaço de trabalho, poderá receber uma solicitação de outro usuário para acessar a view nas seguintes áreas:

   * Uma notificação no aplicativo
     ![Notificação no aplicativo para solicitação de acesso](assets/in-app-notification-for-access-request.png)
   * Uma notificação por email
     ![Notificação por email para a solicitação de acesso](assets/email-notification-for-access-request.png)
1. (Condicional) Na área de notificação do Workfront, clique no link de notificação no aplicativo
Ou
Na notificação por email, clique em **Exibir todas as notificações** e clique na notificação na lista.

   A caixa **Solicitações de acesso pendentes** é exibida.

   ![Caixa de aprovação da lista de notificações](assets/notifications-list-approval-box.png)

1. (Opcional) Para o usuário cujas permissões você deseja aprovar, selecione uma das seguintes opções no menu suspenso à direita do nome do usuário:
   * **Exibir**
   * **Contribute**
   * **Gerenciar**
1. Selecione o usuário para o qual você deseja aprovar ou negar a permissão e clique em **Aprovar tudo** ou **Negar tudo**.
1. Clique na seta à esquerda de **Solicitações de acesso pendentes** e clique em **Salvar**.

   Se você aprovou a solicitação, os usuários são adicionados à caixa de compartilhamento do espaço de trabalho. O usuário que solicita a permissão recebe uma confirmação por email de que sua solicitação foi aprovada. <!--will they also get an in-app notification??-->


## Remover permissões para um espaço de trabalho


{{step1-to-planning}}

1. Abra o espaço de trabalho para o qual você deseja remover permissões e clique em **Compartilhar** no canto superior direito da tela.
1. Clique no menu suspenso à direita do nome de uma entidade com a qual você está compartilhando o espaço de trabalho e clique em **Remover**.
1. Clique em **Salvar**.

   Os usuários removidos não terão mais acesso ao espaço de trabalho ou a seus objetos.
