---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configurar o acesso de revisão de um usuário
description: Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode configurar o acesso de um usuário para criar e exibir provas no Workfront e no Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
TQID: 'https://experienceleague.adobe.com/L-AMDvQYgtXJwxmtwekimbEA9OQQN72QHIcoQ2iKzGU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4ea8bc003ce17978be5e5a6fd838012dfcfeae78
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 6%
---
# Configurar o acesso à revisão de um usuário

Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode configurar o acesso de um usuário para criar e exibir provas no Workfront e no Workfront Proof.

Para obter informações sobre a funcionalidade de revisão de texto disponível para revisões básicas e integradas, consulte [Acesso à funcionalidade de revisão de texto no Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

Você deve ter o seguinte acesso para realizar as etapas descritas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador do Workfront ou do Workfront Proof. Para obter informações sobre administradores do Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

+++

<!--

## Configure a user's proof permission profile

The permission profile you select is granted to the users for each proof that exists within your organization.

{{step-1-to-users}}
 
1. Select one or more users, then click **Edit**.  

1. In the **Access** section, click one of the following Workfront Proof permission options in the **Proof Permission Profile** drop-down menu:

   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the **User can generate proofs** option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only). 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Users can manage and view all proofs created on your organization's account. They can also edit reviewers added to these proofs. Users with this permission profile can't manage users or edit Workfront Proof settings.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Users can manage and view proofs created or owned on your organization's account. They can view other users' proofs only when added as a reviewer. This is a default setting. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Users are given Administrator permissions in Workfront Proof and can edit account settings. Users can manage and view all proofs created on your organization's account. This includes adding and removing reviewers, proofs, and comments.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custom</strong> </td> 
      <td> <p>Available only if you have configured a custom permission profile within Workfront Proof.</p> <p><b>NOTE</b>:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's Access Level setting in Workfront (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher access, the user can access proofs within Workfront Proof that he or she cannot access within Workfront.</p> <p>This is especially important if you plan to allow all Workfront users to access Workfront Proof directly from the Workfront as described in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only Workfront administrators have access to a direct link to the Workfront Proof site from the Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click **Save Changes** to complete the update to the user settings.

   >[!NOTE]
   >
   >When you create or update a user in Workfront and the user's Workfront email address matches that of a licensed Workfront Proof user, the system enables proofing for the user within Workfront. For more information, see [User synchronization between Adobe Workfront and Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerations

Consider the following information when setting permissions:

* If you change a user's permission profile to a profile with fewer permissions, the user might lose visibility to existing proofs within Workfront. This can occur when someone shares a task with a user within Workfront, but doesn't share the proof attached to the task (see [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set Workfront Proof permissions from Workfront only if your Workfront environment is integrated with a Workfront Proof Premium account. If you cannot use proofing as discussed in this section, contact your Workfront administrator.
* At least one user in your Workfront environment must have Administrator permissions for proofing. An error message appears if you try to attempt to remove Administrator permissions for proofing from all users.
* When you change a user's Workfront Access level to any level other than System Administrator, the user's Workfront Proof permission profile defaults to Manager.   

* When you change the Workfront Access level to System Administrator, the Proof Permission profile changes to Administrator.

-->

## Configuração do acesso ao Workfront Proof pelo menu principal do Workfront para todos os usuários {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Por padrão, somente usuários com direitos administrativos no Workfront podem acessar o Workfront Proof conforme descrito [Acessar o Workfront Proof pelo Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Você pode conceder a todos os usuários acesso ao botão Workfront Proof no Menu principal do Workfront, entrando em contato com o Suporte da Workfront e enviando uma solicitação.

>[!IMPORTANT]
>
> Se você planeja permitir que todos os usuários do Workfront acessem o Workfront Proof diretamente da Barra de navegação global da Workfront, verifique se o perfil de permissão para cada usuário não fornece mais acesso do que o nível de acesso do usuário no Workfront. Isso impede que os usuários acessem provas no Workfront Proof que não podem acessar no Workfront. Para obter mais informações, consulte [Habilitar e desabilitar revisões para um usuário (somente planos herdados)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configurar o acesso do usuário ao Desktop Proofing Viewer

Se os usuários em sua organização preferirem usar o Visualizador de provas de desktop em vez do Visualizador de provas de web para revisar o conteúdo interativo, você poderá configurar o Visualizador de provas de desktop para ser iniciado automaticamente quando os usuários abrirem provas de conteúdo interativo. Para obter informações sobre este o Desktop Proofing Viewer e como ele difere do Web Proofing Viewer, consulte [Entender o Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) e [Diferenças entre o Web Proofing Viewer e a visão geral do Desktop Proofing Viewer](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. No Workfront, clique no ícone Workfront Proof na Barra de navegação global para acessar o Workfront Proof.

   ![Ícone de prova](assets/proof-access-proofhq-350x39.png)

1. Clique em **Configurações da conta** próximo ao canto superior direito do Workfront Proof e clique na guia **Configurações**.

1. Em **Padrões de Prova**, no final da linha **Visualizador de Provas de Área de Trabalho para Prova Interativa**, clique em **Configurar**.

1. Modifique as configurações do Desktop Proofing Viewer, conforme descrito no [Desktop Proofing Viewer](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) do artigo [Definir configurações de prova para sua organização](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Clique em **Salvar**.

## Configurar dispositivos personalizados para provas interativas

Você pode adicionar qualquer dispositivo personalizado ao seu sistema, permitindo que os usuários revisem o conteúdo interativo e simulem como o conteúdo aparece em um dispositivo específico quando estão usando o Visualizador de provas de desktop. (Essa funcionalidade não está disponível no Visualizador de provas da Web, onde os usuários podem revisar o conteúdo interativo, mas somente como ele aparece em várias resoluções, não em vários dispositivos.)

Para obter mais informações, consulte [Alterar resolução de prova interativa no visualizador de provas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. No Workfront, acesse a interface do Workfront Proof, conforme descrito em [Acessar o Workfront Proof do Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modifique as configurações do Desktop Proofing Viewer, conforme descrito em [Configurar dispositivos personalizados para provas](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) no artigo [Definir configurações de prova para sua organização](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
