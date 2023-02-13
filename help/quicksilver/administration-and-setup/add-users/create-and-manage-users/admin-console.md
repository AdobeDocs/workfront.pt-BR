---
title: Gerenciar usuários no Adobe Admin Console
description: Como administrador do Adobe, você pode criar usuários e administradores de sistema da Adobe Workfront usando a Adobe Admin Console.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Gerenciar usuários no Adobe Admin Console

>[!IMPORTANT]
>
>A funcionalidade neste artigo está disponível somente se a instância do Workfront de sua organização tiver sido integrada à Adobe Business Platform.
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Plataforma de negócios do Adobe, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador do Adobe, você pode criar usuários e administradores de sistema da Adobe Workfront usando a Adobe Admin Console. O console é um local central para gerenciar os direitos do Adobe em toda a organização. Para obter mais informações, consulte o [Visão geral do Admin Console](https://helpx.adobe.com/br/enterprise/using/admin-console.html).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Direitos de administrador do Adobe</td> 
   <td> <p>Você deve ser um Administrador de configuração de produtos do Adobe para sua organização</p> </td> 
  </tr> 
 </tbody> 
</table>

## Pré-requisitos

Antes de usar o Admin Console para Workfront, você deve receber um email convidando você para o console.

1. Se você nunca usou o Adobe e recebeu um email informando que agora tem direitos de administrador para gerenciar o software e os serviços do Adobe para sua organização, clique no botão no email para criar uma conta do Adobe e abra o Admin Console.

   Ou

   Se você já tiver uma conta do Adobe, acesse [página do Adobe Admin Console](https://adminconsole.adobe.com/).

## Acesse o usuário e a área de administrador para sua instância de produção do Workfront {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. No [página do Adobe Admin Console](https://adminconsole.adobe.com/), selecione o **Produtos** na barra de navegação superior e selecione o **Workfront** bloco do produto.

   ![](assets/admin-product-1.png)

1. Na lista exibida, selecione o link na parte superior.

   Esta é a instância de produção em que os usuários trabalham.

   ![](assets/instances-1.png)

   >[!TIP]
   >
   >Sua instância de Visualização, o segundo link na lista, é um ambiente de teste que replica seu ambiente de produção ativo. Para obter mais informações, consulte [O Ambiente de sandbox de visualização do Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >Você também pode ver links para ambientes sandbox na lista. Para obter mais informações, consulte [O Ambiente de sandbox de visualização do Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. Na lista que é exibida, com a variável **Perfis de produto** , clique no nome do link Perfil do produto Workfront .

   ![](assets/prod-profile-1.png)

   Essa lista inclui todos os usuários que já estão atribuídos à sua instância Produção do Workfront.

   >[!IMPORTANT]
   >
   >Não faça alterações no próprio Perfil do produto.

1. Continue para uma das seguintes seções neste artigo:

   * [Criar usuários no Workfront com a Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Criar administradores de sistema no Workfront com a Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Criar usuários no Workfront com a Adobe Admin Console {#create-users-in-workfront-with-the-adobe-admin-console}

1. Vá para a área de usuário e administrador no Admin Console, conforme descrito em [Acesse o usuário e a área de administrador para sua instância de produção do Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) neste artigo.
1. Com o **Usuários** selecionada acima da lista, selecione **Adicionar usuário**.
1. No **Adicionar usuários a este perfil de produto** , digite o endereço de email ou o nome de um usuário que deseja adicionar e selecione **Salvar**.

   O usuário é criado no Workfront com o nível de acesso Solicitante .

   >[!IMPORTANT]
   >
   >Não faça alterações no próprio Perfil do produto.

1. No Workfront, altere o nível de acesso do usuário.

   Para obter instruções sobre como um administrador do Workfront pode alterar o nível de acesso do usuário, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Repita as etapas 3 e 4 para adicionar mais usuários.

   >[!NOTE]
   >
   >Para novos usuários do Adobe, o Admin Console fornece um email convidando-os a concluir o processo de registro. Todos os usuários devem concluir o processo de registro para acessar qualquer sistema de Adobe.
   >
   >Para usuários existentes do Adobe, o usuário pode ou não receber um email sobre a disponibilidade do Workfront. Esta é uma preferência controlada pelo administrador do Adobe para o produto.

## Criar administradores de sistema no Workfront com a Adobe Admin Console {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

O nível de acesso Administrador do sistema é concedido somente na Adobe Admin Console. Não é possível conceder ou remover o acesso do administrador no Workfront.

Você deve adicionar um usuário à sua instância de Produção do Workfront antes de tornar o usuário um administrador de sistema do Workfront. Para obter instruções, consulte [Criar usuários no Workfront com a Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console) neste artigo.

1. Vá para a área de usuário e administrador no Admin Console, conforme descrito em [Acesse o usuário e a área de administrador para sua instância de produção do Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) neste artigo.
1. Selecione o **Administradores** acima da lista de usuários.
1. Selecionar **Adicionar administrador**.
1. No **Adicionar administradores de perfil de produto** digite os endereços de email ou nomes dos administradores que deseja adicionar e selecione **Salvar**.

   ![](assets/add-admin-1.png)

   Os administradores do sistema são criados no Workfront.

   >[!IMPORTANT]
   >
   >Não faça alterações no próprio Perfil do produto.

## Detalhes adicionais sobre a Adobe Admin Console:

* Os administradores do sistema do Workfront podem desativar um usuário do Workfront no Workfront, mas isso não desativa o usuário no Admin Console.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* O usuário **Grupo Doméstico** é determinada com base no usuário que os criou. No momento, isso não é personalizável no Admin Console.
* O nível de acesso do Administrador do sistema do Workfront só pode ser editado na Adobe Admin Console.

   <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* A edição de um usuário que é administrador do sistema para qualquer outro nível de acesso deve ser feita através do Admin Console primeiro.

   <!--
   This is not clear
  -->

* Para remover o acesso do Administrador do sistema de um usuário no Workfront, é necessário usar o Adobe Admin Console para remover o usuário como Administrador do perfil do produto. Isso altera o nível de acesso do usuário ao Workfront do Administrador do sistema para Requestor.

   >[!IMPORTANT]
   >
   >Não faça alterações no próprio Perfil do produto.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>You can create Adobe Workfront users and system administrators with the <a href="https://adminconsole.adobe.com/" alt="Admin Console link">Adobe Admin Console</a>. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the <a href="https://helpx.adobe.com/enterprise/using/admin-console.html" alt="Admin Console Overview">Admin Console Overview</a>.</p>
<p>Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. Click in the invitation to accept it and create an account. You can also use an existing account, if already available.</p>
<h2>Create users</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Create users in WF with the Adobe admin console</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">May need to add something about oging throug WF -- check with Jonah</p>

<p>To create users in Workfront with the Admin Console:</p>
<ol>
<li value="1"> <p>From the <a href="https://adminconsole.adobe.com/">Admin Console page</a>, select the <b>Products</b> tab and then select the <b>Workfront</b> product tile.</p> </li>
<li value="2"> <p>Select the link to the Workfront instance you want to change.</p> </li>
<li value="3"> <p>Select the Product profile link. This shows a list of the currently-assigned users. If the list is very long, you can also search for users in the search field above the list.</p> </li>
<li value="4"> <p>Select the <b>Add User</b> button.</p> </li>
<li value="5"> <p>In the <b>Add users</b> box, enter the email address or name of the user you want to add. Select <b>Save</b>. The administrator is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Create system administrators</h2>
<p>To create system administrators:</p>
<ol>
<li value="1"> <p>Make product profile assignments first. To be a Workfront System Administrator, the user must be assigned the Workfront product profile and be an admin for that product profile.</p> </li>
<li value="2"> <p>From the console, select the <b>Products</b> tab and then select the <b>Admins</b> tab. </p> </li>
<li value="3"> <p>Select <b>Add Admin</b>.</p> </li>
<li value="4"> <p>In the <b>Add product profile administrators</b> box, enter the email address or name of the administrator you want to add. Select <b>Save</b>. The user is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Additional details for the Admin Console</h2>
<ul>
<li> <p>System Administrator access level is granted only on the Admin Console. You cannot grant or remove admin access from within Workfront.</p> </li>
</ul>
<ul>
<li> <p>Creating and deleting users inside Workfront is only possible through the Admin Console.</p> </li>
<li> <p>Workfront System Administrators can deactivate Workfront users from within Workfront, but this does not deactivate the user in the Admin Console.</p> </li>
<li> <p>All new users are are assigned <b>Requestor</b> access level upon creation. Also, the user <b>Home Group</b> is determined based on the user who created them. This is currently not customizable from within the Admin Console.</p> </li>
<li> <p>The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.</p> </li>
<li> <p>Editing a user who is a system admin to any other access level must be done through the Admin Console first.</p> </li>
<li> <p>To remove Workfront system admin access, remove users as Product Profile Administrators. This action changes the user access level in Workfront from a system admin to a <b>Requestor</b>.</p> </li>
</ul>
</div>
-->
