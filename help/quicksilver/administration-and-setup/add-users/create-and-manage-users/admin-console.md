---
title: Gerenciar usuários no Adobe Admin Console
description: Como admin da Adobe, você pode criar usuários e admins de sistema do Adobe Workfront usando o Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 793419db3e9552e2e425aec26300b8c2b4ab8583
workflow-type: tm+mt
source-wordcount: '1638'
ht-degree: 94%

---

# Gerenciar usuários no Adobe Admin Console

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>A funcionalidade descrita neste artigo está disponível apenas se a instância do Workfront da sua organização tiver sido integrada à Adobe Business Platform.
>
>Para obter uma lista de procedimentos que diferem dependendo se sua organização foi integrada à Adobe Business Platform, consulte [Diferenças na administração baseada na plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como admin da Adobe, você pode criar admins do sistema Adobe Workfront usando o Adobe Admin Console. O console é um local central para gerenciar os direitos da Adobe em toda a sua organização. Para obter mais informações, consulte a [Visão geral do Admin Console](https://helpx.adobe.com/br/enterprise/using/admin-console.html).

>[!NOTE]
>
>* **Admins do Workfront devem ser configurados no Adobe Admin Console.** Para obter informações e instruções, consulte [Criar admins de sistema no Workfront com o Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console) neste artigo.
>* **Se sua organização usa logon único (SSO)**, recomendamos criar usuários e atribuí-los ao Workfront no Adobe Admin Console. Criar esses usuários no Workfront é possível, mas pode haver problemas ao transferir essas informações para o Adobe Admin Console, dependendo de como o Admin Console da sua organização está configurado.
>   Após criar o usuário no Adobe Admin Console, você pode configurar as informações do usuário no Workfront, como atribuir funções, grupos, equipes e níveis de acesso.
>* **Se a sua organização não usa logon único (SSO)**, você pode adicionar usuários não admins do sistema diretamente no Workfront. É possível adicionar usuários no Adobe Admin Console, mas adicioná-los no Workfront permite definir o nível de acesso durante a criação, o que pode economizar tempo.

Ao fazer alterações nos perfis dos usuários a partir do Admin Console, a atualização é adicionada à aba Atividade do sistema do usuário no Workfront. A atualização aparece como feita pelo “Sistema”. Isso se refere a um(a) admin do Adobe Admin Console, e não ao(à) admin principal do Workfront.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer<p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Direitos de admin da Adobe</td> 
   <td> <p>Você deve ser um(a) admin de perfis de produtos da Adobe na sua organização</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de usar o Admin Console do Workfront, você deve receber um e-mail de convite para acessar o console.

1. Se você começou agora na Adobe e recebeu um email informando que agora tem direitos de admin para gerenciar o software e os serviços da Adobe na sua organização, clique no botão no email para criar uma conta Adobe e abrir o Admin Console.

   Ou

   Se você já possui uma conta Adobe, acesse a página [Adobe Admin Console](https://adminconsole.adobe.com/).

## Detalhes adicionais sobre o Adobe Admin Console

* Admins do sistema Workfront podem desativar um usuário do Workfront a partir do Workfront, mas isso não desativa o usuário no Admin Console.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* O **Grupo de origem** do usuário é determinado com base no usuário que os criou. Isso não é personalizável no Admin Console.
* O nível de acesso de admin do sistema do Workfront só pode ser editado no Adobe Admin Console.

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* Alterar o acesso de um usuário de Admin do sistema para qualquer outro nível de acesso deve ser feito primeiro pelo Admin Console.

  <!--
   This is not clear
  -->

* Para remover o acesso de admin do sistema de um usuário no Workfront, você deve usar o Adobe Admin Console para remover o usuário como Admin do perfil de produto. Isso altera o nível de acesso do usuário no Workfront de Admin do sistema para Solicitante.

  >[!IMPORTANT]
  >
  >Não faça nenhuma alteração no perfil de produto em si.

* Admins do Adobe Admin Console podem definir regras de atribuição automática para automatizar o processo de atribuição de produtos da Adobe aos usuários da organização. Sua organização deve migrar para a experiência unificada da Adobe para usar essa funcionalidade. Para mais informações e instruções, consulte [Gerenciar regras de atribuição automática](https://helpx.adobe.com/enterprise/using/automatic-assignment-rules.html) na documentação da Adobe.

  >[!NOTE]
  >
  >Se você estiver selecionando uma organização confiável ao configurar atribuições automáticas, a organização pode ser encontrada na área Usuários em diretórios ou domínios selecionados. Clique na seta da lista suspensa ao lado do campo **Selecionar diretório** e selecione as organizações. Organizações confiáveis são marcadas com um selo de Confiável.

## Acesse a área de usuários e administração da sua instância de produção do Workfront {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. Na página [Adobe Admin Console](https://adminconsole.adobe.com/), selecione a aba **Produtos** na barra de navegação superior e, em seguida, selecione **Workfront**.

   <!--![Admin Console product](assets/admin-product-1.png)-->

1. Na lista exibida, selecione o link na parte superior.

   Esta é a sua instância de produção, onde seus usuários trabalham.

   <!--![Admin Console instances](assets/instances-1.png)-->

   >[!TIP]
   >
   >O segundo link na lista, a sua instância de pré-visualização, é um ambiente de teste que replica o seu ambiente de produção ativo. Para mais informações, consulte [O ambiente de sandbox de pré-visualização do Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >Você também pode ver links para ambientes de sandbox na lista. Para mais informações, consulte [O ambiente de sandbox de pré-visualização do Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. Na lista exibida, com a aba **Perfis de produto** selecionada, clique no nome do link do Perfil de produto do Workfront.

   ![Perfis de produto](assets/prod-profile-1.png)

   Esta lista inclui todos os usuários que já estão atribuídos à sua instância de produção do Workfront.

   >[!IMPORTANT]
   >
   >Não faça nenhuma alteração no perfil de produto em si.

1. Continue para uma das seções a seguir neste artigo:

   * [Criar usuários no Workfront com o Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Criar administradores do sistema no Workfront com o Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Criar administradores do sistema no Workfront com o Adobe Admin Console {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

<!--Audited: 12/2023-->

O nível de acesso de Administrador do sistema é concedido somente no Adobe Admin Console. Não é possível conceder ou remover o acesso de administrador no Workfront.

Você deve adicionar um usuário à instância de Produção do Workfront antes de poder torná-lo um administrador do sistema do Workfront.

1. Acesse a área de usuários e administração no Admin Console, conforme descrito na seção [Acessar a área de usuários e administração da sua instância de produção do Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) neste artigo.
1. Selecione a aba **Administradores** acima da lista de usuários.
1. Selecione **Adicionar administrador**.
1. Na caixa **Adicionar administradores de perfil de produto**, insira os endereços de email ou nomes dos administradores que deseja adicionar e, em seguida, selecione **Salvar**.

   ![Adicionar um administrador](assets/add-admin-1.png)

   Os administradores do sistema são criados no Workfront.

   >[!IMPORTANT]
   >
   >* Não faça nenhuma alteração no perfil de produto em si.
   >* Certifique-se de que está na página com o cabeçalho “Adicionar administradores do perfil do produto”. Os administradores de produtos têm uma função diferente dos administradores de perfis de produtos no Adobe Admin Console e não são abordados neste artigo.


## Criar usuários no Workfront com a Adobe Admin Console {#create-users-in-workfront-with-the-adobe-admin-console}

>[!NOTE]
>
>Recomendamos adicionar usuários que não sejam administradores do sistema diretamente no Workfront. É possível adicionar usuários no Adobe Admin Console, mas adicioná-los no Workfront permite definir o nível de acesso durante a criação, o que pode economizar tempo.

* [Criar usuários no Workfront diretamente no Adobe Admin Console](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [Criar usuários no Workfront e aprová-los para o Adobe Admin Console](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### Criar usuários no Workfront diretamente no Adobe Admin Console

1. Acesse a área de usuários e administração no Admin Console, conforme descrito na seção [Acessar a área de usuários e administração da sua instância de produção do Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) neste artigo.
1. Com a aba **Usuários** selecionada acima da lista, selecione **Adicionar usuário**.
1. Na caixa **Adicionar usuários a este perfil de produto**, insira o endereço de email ou o nome do usuário que deseja adicionar e, em seguida, selecione **Salvar**.

   O usuário é criado no Workfront com o nível de acesso de Solicitante ou Colaborador, dependendo do pacote do Workfront da sua organização.

   >[!IMPORTANT]
   >
   >Não faça nenhuma alteração no perfil de produto em si.

1. No Workfront, altere o nível de acesso do usuário.

   Para obter instruções sobre como um administrador do Workfront pode alterar o nível de acesso do usuário, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Repita as etapas 3 e 4 para adicionar mais usuários.

   >[!NOTE]
   >
   >Para novos usuários da Adobe, o Admin Console envia um email para convidá-los a concluir o processo de registro. Todos os usuários devem concluir o processo de registro para acessar qualquer aplicativo da Adobe.
   >
   >Os usuários já existentes da Adobe podem ou não receber um email informando que o Workfront está disponível. Essa é uma preferência controlada pelo administrador da Adobe para o produto. O administrador da Adobe pode ser uma pessoa diferente do administrador do Workfront.

### Criar usuários no Workfront e aprová-los para o Adobe Admin Console

Esse fluxo de trabalho permite que administradores de grupo que não têm acesso ao Adobe Admin Console criem usuários.

Primeiro, o administrador de grupo cria o usuário no Workfront. Isso cria o usuário com o status Desativado e Aprovação pendente.

Em seguida, um administrador do Workfront aprova o usuário. Isso ativa o usuário no Workfront e o adiciona ao Adobe Admin Console.

#### Criar o usuário no Workfront (Administrador de grupo)

Para obter instruções sobre como criar um usuário no Workfront, consulte [Adicionar usuários](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md).

#### Aprovar o usuário (administrador do Workfront)

Para aprovar um usuário:

{{step-1-to-users}}

1. Selecione o usuário e, em seguida, clique no ícone de **Mais** ![Ícone de Mais](assets/more-icon.png).

1. Para aprovar o usuário, clique em **Aprovar** e, em seguida, clique em **Enviar**.

   Ou

   Para rejeitar o usuário e excluí-lo do Workfront, clique em **Rejeitar** e, em seguida, clique em **Enviar**.

   Os usuários aprovados são adicionados automaticamente ao Adobe Admin Console.

   Os usuários rejeitados são automaticamente excluídos do Workfront.


## Editar usuários no Adobe Admin Console

Você pode editar os seguintes detalhes do usuário no Adobe Admin Console:

* Grupos de usuários e produtos associados ao usuário
* Direitos administrativos
* País

Para obter informações sobre como editar um único usuário no Adobe Admin Console, consulte [Editar detalhes do usuário](https://helpx.adobe.com/enterprise/using/manage-users-individually.html#edit-user-details) no artigo Gerenciar usuários individualmente na documentação do Adobe.

Para obter informações sobre a edição de usuários em massa no Adobe Admin Console, consulte
[Editar detalhes do usuário](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html#edit-user-details) no artigo Gerenciar vários usuários na documentação do Adobe.

## Excluir um usuário

>[!NOTE]
>
>* Se um usuário estiver em um Grupo de usuários do Admin Console e o perfil de produto tiver sido adicionado a um ou mais desses Grupos de usuários, a desativação do usuário do Workfront não o removerá do produto. O usuário deve ser removido do(s) grupo(s) de usuários no Admin Console.
>* Excluir um usuário da Adobe Admin Console desativa o usuário no Workfront, mas não o exclui do Workfront.

Para obter instruções sobre como excluir usuários no Adobe Admin Console, consulte [Gerenciar usuários do diretório](https://helpx.adobe.com/enterprise/using/manage-directory-users.html) na documentação do Adobe.

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
