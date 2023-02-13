---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)
description: Se sua organização tiver sido integrada à Adobe Business Platform, os usuários usarão a Adobe Business Platform para acessar o Adobe Workfront. Isso significa que o gerenciamento de usuários é feito em grande parte por meio da Adobe Admin Console e que o Single Sign-On (SSO) é realizado por meio da Adobe Business Platform, e não pela Workfront. Como administrador da Adobe Workfront, suas responsabilidades de administração e seus procedimentos diferem com base na integração de sua organização à Plataforma de negócios do Adobe. Este artigo lista os procedimentos que devem ser tratados de forma diferente e vincula às instruções do Workfront e da Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 1%

---

# Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)

Se sua organização tiver sido integrada à Adobe Business Platform, os usuários usarão a Adobe Business Platform para acessar o Adobe Workfront. Isso significa que:

* O gerenciamento de usuários é feito em grande parte por meio da Adobe Admin Console
* O Logon único (SSO) é feito por meio da Adobe Business Platform, e não pela Workfront

Como administrador da Adobe Workfront, suas responsabilidades de administração e seus procedimentos diferem com base na integração de sua organização à Plataforma de negócios do Adobe. Este artigo lista os procedimentos que devem ser tratados de forma diferente e vincula às instruções do Workfront e da Adobe Admin Console.

## Usuários

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Ação</th> 
   <th>Para obter instruções na Workfront, consulte</th> 
   <th>Para obter instruções no Admin Console do Adobe, consulte</th> 
  </tr> 
 </thead> 
 <tbody> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Conceder acesso a um administrador de usuário</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>A seção "Editar detalhes do usuário" em <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gerenciar usuários individualmente</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adicionar usuário ao Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Adicionar usuários</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Gerenciar usuários no Adobe Admin Console</a> </p> </li> 
     <li> <p>A seção "Adicionar usuários" em <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gerenciar usuários individualmente</a></p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Desativar um usuário</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>A seção "Remover usuários" em <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gerenciar usuários individualmente</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Excluir um usuário</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Excluir usuários</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>A seção "Excluir usuários permanentemente" em <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Gerenciar usuários do diretório</a>
     </p><p>Observação: Excluir um usuário do [!DNL Adobe Admin Console] desativa o usuário em [!DNL Workfront], mas não os exclui de [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Editar um perfil de usuário</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar o perfil de um usuário</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>A seção "Editar detalhes do usuário" em <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gerenciar usuários individualmente</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Editar perfis de usuário em massa</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Editar perfis de usuário em massa</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>A seção "Editar detalhes do usuário" em <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Upload em massa de CSV</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Importar usuários </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importar usuários</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>A seção "Adicionar usuários" em <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Upload em massa de CSV</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fazer logon como outro usuário</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Fazer logon como outro usuário</a> </p> </li> 
    </ul> </td> 
   <td>Não Disponível</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Renovar certificado SAML</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renovar o certificado de metadados SAML 2.0 do Adobe Workfront</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>A seção "A assinatura digital na resposta SAML não validou..." em <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Solução de problemas do Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO (Logon único)

Como a Adobe Business Platform controla o Single Sign-On (SSO) para usuários, as seguintes ações e funcionalidades são manipuladas automaticamente por meio da Adobe Business Platform. Se sua organização ainda não tiver sido integrada à Adobe Business Platform, você deve executar essas ações no Workfront.


* [Configurar o Adobe Workfront com o SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Configurar o Adobe Workfront com o SAML 2.0 usando ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Desativar logon único no Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [Atualize os metadados SAML 2.0 no seu provedor de identidade](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Atualizar usuários para logon único](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Configurar políticas de senha para autenticação](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Configurar preferências de segurança do sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
