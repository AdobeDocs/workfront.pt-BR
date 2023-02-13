---
content-type: overview
product-area: documents
keywords: prova,permissão
navigation-topic: proofing-overview
title: Visão geral do perfil de permissão de prova
description: Perfis de permissão de prova determinam quais permissões gerais os usuários têm sobre todas as provas em sua conta. Perfis de permissão de prova são atribuídos aos usuários em seus Perfis de usuário. Perfis de permissão de prova são diferentes das funções de prova. Para obter mais informações sobre funções de prova, consulte a visão geral Funções de prova .
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
source-git-commit: 9b60133c4cc20deb410f507854597f44d0607228
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 2%

---

# Visão geral do perfil de permissão de prova

Perfis de permissão de prova determinam quais permissões gerais os usuários têm sobre todas as provas em sua conta. Perfis de permissão de prova são atribuídos aos usuários em seus Perfis de usuário. Perfis de permissão de prova são diferentes das funções de prova. Para obter mais informações sobre funções de prova, consulte [Visão geral das funções de prova](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).

>[!NOTE]
>
>Se você for um administrador, poderá criar perfis personalizados para usuários em sua organização. Para obter mais informações, consulte [Configurar perfis personalizados no Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the&nbsp;account settings&nbsp;and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in&nbsp;Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them.&nbsp;</li>
</ul>
-->

## Perfis de permissão de prova

A tabela a seguir exibe as permissões disponíveis com cada Perfil de permissão de prova.

<table>
  <tr>
   <td colspan="5" ><strong>Itens próprios</strong>
   </td>
   <td colspan="3" ><strong>Itens de outros usuários</strong>
   </td>
   <td><strong>Admin</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>Adicionar</strong>
   </td>
   <td><strong>Exibir</strong>
   </td>
   <td><strong>Editar</strong>
   </td>
   <td><strong>Excluir</strong>
   </td>
   <td><strong>Exibir</strong>
   </td>
   <td><strong>Editar</strong>
   </td>
   <td><strong>Excluir</strong>
   </td>
   <td><strong>Editar e excluir</strong>
   </td>
  </tr>
  <tr>
   <td>Admin
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
  </tr>
  <tr>
   <td>Supervisor
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Gerente
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Observador
   </td>
   <td>
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### Administrador

Os administradores têm acesso ao [Configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) e ter as seguintes permissões:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Os administradores podem:</td> 
   <td>Os administradores não podem:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Criar provas, carregar arquivos e criar pastas</p> </li> 
     <li> <p>Exibir, editar e excluir provas e arquivos que eles criaram</p> </li> 
     <li> <p>Exibir, editar e excluir provas e arquivos criados por todos os usuários na organização</p> </li> 
     <li> <p>Excluir as pastas públicas de outros usuários</p> </li> 
     <li> <p>Editar todas as provas criadas na conta</p> </li> 
     <li> <p>Ser definido como proprietário da zona de transferência*</p> </li> 
     <li> <p>Acesse a página Configurações da conta e edite os detalhes da conta</p> </li> 
     <li> <p>Esvaziar a lixeira</p> </li> 
     <li> <p>Adicionar, editar e excluir usuários</p> </li> 
     <li> <p>Criar grupos e adicionar novos contatos</p> </li> 
     <li> <p>Excluir contatos</p> </li> 
     <li> <p>Edite provas se não houver respostas sobre elas</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Edite as respostas da prova.</p> </li> 
     <li> <p>Excluir as pastas privadas de outros usuários</p> </li> 
     <li> <p>Acesse a página Faturamento ou edite os detalhes de faturamento</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Disponível somente no produto independente Workfront Proof.

### Supervisor

Os supervisores têm as seguintes permissões:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>As autoridades de supervisão podem:</td> 
   <td>Supervisores não podem:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Criar provas, carregar arquivos e criar pastas</p> </li> 
     <li> <p>Exibir, editar e excluir provas e arquivos que eles criaram</p> </li> 
     <li> <p>Exibir, editar e excluir provas e arquivos criados por todos os usuários na organização</p> </li> 
     <li> <p>Excluir as pastas públicas de outros usuários</p> </li> 
     <li> <p>Editar todas as provas criadas na conta</p> </li> 
     <li> <p>Criar grupos e adicionar novos contatos</p> </li> 
     <li> <p>Excluir contatos</p> </li> 
     <li> <p>Edite provas se não houver respostas sobre elas</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Edite as respostas da prova.</p> </li> 
     <li> <p>Excluir as pastas privadas de outros usuários</p> </li> 
     <li> <p>Acesse a página Faturamento ou edite os detalhes de faturamento</p> </li> 
     <li> <p>Adicionar, editar ou excluir usuários</p> </li> 
     <li> <p>Esvaziar a lixeira</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gerente

Os gerentes têm as seguintes permissões:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Os gerentes podem:</td> 
   <td>Os gerentes não podem:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Criar provas, carregar arquivos e criar pastas</p> </li> 
     <li> <p>Exibir, editar e excluir provas e arquivos que eles criaram</p> </li> 
     <li> <p>Ver, revisar e aprovar provas de outros usuários que são compartilhados explicitamente com eles (direitos somente leitura para tudo em uma pasta compartilhada)</p> </li> 
     <li> <p>Editar todas as provas criadas na conta</p> </li> 
     <li> <p>Criar grupos e adicionar novos contatos</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Exibir, editar ou excluir provas e arquivos criados por outros usuários na organização. </p> <p>Edite as respostas da prova.</p> </li> 
     <li> <p>Excluir as pastas privadas ou públicas de outros usuários</p> </li> 
     <li> <p>Acesse a página Faturamento ou edite os detalhes de faturamento</p> </li> 
     <li> <p>Adicionar, editar ou excluir usuários</p> </li> 
     <li> <p> Excluir contatos</p> </li> 
     <li> <p>Esvaziar a lixeira</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Observer</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers have the following permissions:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only&nbsp;rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot&nbsp;create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs&nbsp;or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access&nbsp;the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a>&nbsp;and&nbsp;<a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the&nbsp;trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts.&nbsp;</p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited.&nbsp;</p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings:&nbsp;Account settings,&nbsp;Billing </li>>
>  -->


<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Guest</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Guest profile is used to give access to proofs for reviewers who do not have their own Workfront Proof account. Guests can access proofs shared with them directly via their personal email notifications.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view, review, and approve proofs that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Dashboard.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot have folders shared with them. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be added as Authors or Moderators to the proofs. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<note type="note">
&nbsp;Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->
