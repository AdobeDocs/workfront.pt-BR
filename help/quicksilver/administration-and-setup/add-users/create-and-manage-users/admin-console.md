---
title: Gerenciar usuários na Adobe Admin Console
description: Como administrador do Adobe, você pode criar usuários e administradores de sistema do Adobe Workfront usando o Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 3c21d2ac594d4dfe309ed4227e46a9cb535f0501
workflow-type: tm+mt
source-wordcount: '1564'
ht-degree: 0%

---

# Gerenciar usuários na Adobe Admin Console

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>A funcionalidade deste artigo só estará disponível se a instância da Workfront da sua organização tiver sido integrada à Adobe Business Platform.
>
>Para obter uma lista de procedimentos que diferem dependendo de sua organização ter sido integrada à Adobe Business Platform, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador do Adobe, você pode criar administradores de sistema do Adobe Workfront usando o Adobe Admin Console. O console é um local central para gerenciar os direitos da Adobe em toda a organização. Para obter mais informações, consulte a [Visão geral do Admin Console](https://helpx.adobe.com/br/enterprise/using/admin-console.html).

>[!NOTE]
>
>* **Os Administradores do Workfront devem ser configurados no Adobe Admin Console.** Para obter informações e instruções, consulte [Criar administradores do sistema no Workfront com o Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console) neste artigo.
>* **Se sua organização usa Logon Único (SSO)**, recomendamos criar usuários e atribuí-los ao Workfront na Adobe Admin Console. A criação desses usuários no Workfront é possível, mas pode haver problemas ao transferir essas informações para a Adobe Admin Console, com base em como o Admin Console da sua organização é configurado.
>  &#x200B;>   Depois de criar o usuário no Adobe Admin Console, você pode configurar as informações do usuário no Workfront, como atribuir funções, grupos, equipes e níveis de acesso.
>* **Se sua organização não usar o Logon Único (SSO)**, você poderá adicionar usuários não administradores do sistema diretamente no Workfront. É possível adicionar usuários na Adobe Admin Console, mas adicioná-los no Workfront permite definir seus níveis de acesso ao criá-los, o que pode economizar seu tempo.

Ao fazer alterações nos perfis de usuários na Admin Console, uma atualização é adicionada à guia Atividade do sistema do usuário no Workfront. A atualização é exibida conforme estabelecido pelo &quot;Sistema&quot;. Refere-se ao administrador do Adobe Admin Console e não ao administrador principal do Workfront.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Direitos de administrador do Adobe</td> 
   <td> <p>Você deve ser um Administrador de perfil de produto de produtos da Adobe para sua organização</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de usar o Admin Console para Workfront, você deve receber um email convidando você para o console.

1. Se você é novo no Adobe e recebeu um email informando que agora tem direitos de administrador para gerenciar o software e os serviços da Adobe para sua organização, clique no botão no email para criar uma conta do Adobe e abrir o Admin Console.

   Ou

   Se você já tiver uma conta do Adobe, vá para a [página do Adobe Admin Console](https://adminconsole.adobe.com/).

## Detalhes adicionais sobre a Adobe Admin Console

* Os administradores de sistema do Workfront podem desativar um usuário do Workfront no Workfront, mas isso não desativa o usuário no Admin Console.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* O usuário **Grupo Padrão** é determinado com base no usuário que o criou. Isso não é personalizável no Admin Console.
* O nível de acesso do Administrador de sistema do Workfront só pode ser editado no Adobe Admin Console.

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* A alteração do acesso de um usuário do Administrador do sistema para qualquer outro nível de acesso deve ser feita primeiro por meio do Admin Console.

  <!--
   This is not clear
  -->

* Para remover o acesso de um usuário ao Administrador do sistema no Workfront, você deve usar o Adobe Admin Console para remover o usuário como Administrador de perfil de produto. Isso altera o nível de acesso do usuário ao Workfront de Administrador do sistema para Solicitante.

  >[!IMPORTANT]
  >
  >Não faça alterações no próprio Perfil do produto.

* Os administradores do Adobe Admin Console podem configurar regras de atribuição automática para automatizar o processo de atribuição de produtos Adobe a usuários em suas organizações. Sua organização deve ser migrada para a Experiência unificada da Adobe para usar essa funcionalidade. Para obter mais informações e instruções, consulte [Gerenciar regras de atribuição automática](https://helpx.adobe.com/enterprise/using/automatic-assignment-rules.html) na documentação do Adobe.

  >[!NOTE]
  >
  >Se você estiver selecionando uma organização confiável ao configurar atribuições automáticas, a organização poderá ser encontrada na área Usuários nos diretórios ou domínios selecionados. Clique na seta suspensa ao lado do campo **Selecionar diretório** e selecione as organizações. As organizações confiáveis estão marcadas com um selo Confiável.

## Acesse a área de usuário e administrador da sua Instância de produção do Workfront {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. Na [página do Adobe Admin Console](https://adminconsole.adobe.com/), selecione a guia **Produtos** na barra de navegação superior e selecione **Workfront**.

   <!--![Admin Console product](assets/admin-product-1.png)-->

1. Na lista exibida, selecione o link na parte superior.

   Essa é a instância de Produção na qual os usuários trabalham.

   <!--![Admin Console instances](assets/instances-1.png)-->

   >[!TIP]
   >
   >O segundo link na lista, sua instância de Pré-visualização, é um ambiente de teste que replica seu ambiente de Produção ativo. Para obter mais informações, consulte [O Ambiente de Sandbox de Visualização do Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >Você também pode ver links para ambientes de sandbox na lista. Para obter mais informações, consulte [O Ambiente de Sandbox de Visualização do Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. Na lista exibida, com a guia **Perfis de produto** selecionada, clique no nome do link Perfil de Produto do Workfront.

   ![Perfis de produto](assets/prod-profile-1.png)

   Essa lista inclui todos os usuários que já estão atribuídos à sua instância de Produção do Workfront.

   >[!IMPORTANT]
   >
   >Não faça alterações no próprio Perfil do produto.

1. Prossiga para uma das seguintes seções neste artigo:

   * [Criar usuários no Workfront com o Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Criar administradores de sistema no Workfront com a Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Criar administradores de sistema no Workfront com a Adobe Admin Console {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

<!--Audited: 12/2023-->

O nível de acesso de Administrador do sistema é concedido somente no Adobe Admin Console. Não é possível conceder ou remover o acesso de administrador no Workfront.

Você deve adicionar um usuário à instância de Produção do Workfront antes de poder torná-lo um administrador do sistema do Workfront.

1. Vá para a área de usuário e administrador na Admin Console, conforme descrito na seção [Acessar a área de usuário e administrador para sua instância de Produção do Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) neste artigo.
1. Selecione a guia **Administradores** acima da lista de usuários.
1. Selecione **Adicionar Administrador**.
1. Na caixa **Adicionar administradores de perfil de produto**, digite os endereços de email ou nomes dos administradores que deseja adicionar e selecione **Salvar**.

   ![Adicionar um administrador](assets/add-admin-1.png)

   Os administradores do sistema são criados no Workfront.

   >[!IMPORTANT]
   >
   >* Não faça alterações no próprio Perfil do produto.
   >* Verifique se você está na página com o cabeçalho &quot;Adicionar administradores de perfil de produto&quot;. Os administradores de produtos desempenham uma função diferente dos administradores de perfil de produto no Adobe Admin Console e não são discutidos neste artigo.


## Criar usuários no Workfront com a Adobe Admin Console {#create-users-in-workfront-with-the-adobe-admin-console}

>[!NOTE]
>
>Recomendamos adicionar usuários que não são administradores do sistema diretamente no Workfront. É possível adicionar usuários na Adobe Admin Console, mas adicioná-los no Workfront permite definir seus níveis de acesso ao criá-los, o que pode economizar seu tempo.

* [Criar usuários no Workfront diretamente no Adobe Admin Console](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [Crie usuários no Workfront e aprove-os para a Adobe Admin Console](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### Criar usuários no Workfront diretamente no Adobe Admin Console

1. Vá para a área de usuário e administrador na Admin Console, conforme descrito na seção [Acessar a área de usuário e administrador para sua instância de Produção do Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) neste artigo.
1. Com a guia **Usuários** selecionada acima da lista, selecione **Adicionar usuário**.
1. Na caixa **Adicionar usuários a este perfil de produto**, digite o endereço de email ou o nome de um usuário que deseja adicionar e selecione **Salvar**.

   O usuário é criado no Workfront com o nível de acesso Solicitante ou Colaborador, dependendo do pacote do Workfront da sua organização.

   >[!IMPORTANT]
   >
   >Não faça alterações no próprio Perfil do produto.

1. No Workfront, altere o nível de acesso do usuário.

   Para obter instruções sobre como um administrador do Workfront pode alterar o nível de acesso do usuário, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Repita as etapas 3 e 4 para adicionar mais usuários.

   >[!NOTE]
   >
   >Para novos usuários do Adobe, a Admin Console fornece um email convidando-os a concluir o processo de registro. Todos os usuários devem concluir o processo de registro para acessar qualquer aplicativo do Adobe.
   >
   >Para usuários existentes do Adobe, o usuário pode ou não receber um email sobre a disponibilidade do Workfront. Esta é uma preferência controlada pelo administrador do Adobe para o produto. O administrador do Adobe pode ser uma pessoa diferente do administrador do Workfront.

### Crie usuários no Workfront e aprove-os para a Adobe Admin Console

Esse fluxo de trabalho permite que administradores de grupos que não têm acesso à Adobe Admin Console criem usuários.

Primeiro, o administrador de grupo cria o usuário no Workfront. Isso cria o usuário com status Desativado e Aprovação pendente.

Em seguida, um administrador do Workfront aprova o usuário. Isso ativa o usuário no Workfront e o adiciona à Adobe Admin Console.

#### Criar o usuário no Workfront (Administrador de grupo)

Para obter instruções sobre como criar um usuário no Workfront, consulte [Adicionar usuários](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md).

#### Aprovar o usuário (administrador do Workfront)

Para aprovar um usuário:

{{step-1-to-users}}

1. Selecione o usuário e clique no ícone **Mais** ícone ![Mais](assets/more-icon.png).

1. Para aprovar o usuário, clique em **Aprovar** e em **Enviar**.

   Ou

   Para rejeitar o usuário e excluí-lo do Workfront, clique em **Rejeitar** e em **Enviar**.

   Os usuários aprovados são adicionados automaticamente à Adobe Admin Console.

   Os usuários rejeitados são excluídos automaticamente do Workfront.


## Editar usuários existentes na Adobe Admin Console

Você pode editar os seguintes detalhes do usuário no Adobe Admin Console:

* Grupos de usuários e produtos associados ao usuário
* Direitos administrativos
* País

Para obter informações sobre como editar um único usuário no Adobe Admin Console, consulte [Editar detalhes do usuário](https://helpx.adobe.com/enterprise/using/manage-users-individually.html#edit-user-details) no artigo Gerenciar usuários individualmente na documentação do Adobe.

Para obter informações sobre a edição de usuários em massa no Adobe Admin Console, consulte
[Editar detalhes do usuário](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html#edit-user-details) no artigo Gerenciar vários usuários na documentação do Adobe.
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
