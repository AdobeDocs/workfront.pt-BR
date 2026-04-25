---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Proof a linked asset for Experience Manager Assets or Assets Essentials
description: After you've linked an asset from Experience Manager Assets Essentials, you can create a proof and assign users to review and add comments to the asset.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 14%

---

# Proof a linked asset for Experience Manager Assets or Assets Essentials

After you&#39;ve linked an asset from Experience Manager Assets Essentials, you can create a proof and assign users to review and add comments to the asset.

>[!NOTE]
>
>Essa funcionalidade não está disponível na área de novos documentos.<br>
>Se sua organização usar armazenamento corporativo, você verá a nova área de documentos ao acessar documentos no Workfront. From there, you can add assets from Experience Manager Assets and review and approve them with the Frame.io viewer. Para obter mais informações, consulte [Usar o Adobe Experience Manager com a integração do Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

## Requisitos de acesso

<!-- Audited: 4/2025 -->

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront</td> 
   <td> 
   <p>Padrão</p>
   <p>Trabalho ou maior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Additonal products</td> 
   <td>You must have Experience Manager as a Cloud Service or Assets Essentials, and you must be added to the product as a user in the Admin Console. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>View access or higher</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Before you begin:

* Your Workfront Administrator must configure an Experience Manager integration. For more information, see [Configure the Experience Manager Assets as a Cloud Service integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) or [Configure the Experience Manager Assets Essentials integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Criar uma prova

You can create static, video, or interactive proofs.

To create a proof:

1. Go to the project, task, or issue where you want the proof, then click the **Documents** section.
1. Hover over the document, then click the **Create Proof** link that appears below the document name.

   >[!NOTE]
   >
   >If you have **Automatically generate proofs when uploading documents** enabled in your user profile, the system automatically creates a simple proof.

1. Choose one of the following from the drop-down:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Simple Proof</strong></td> 
      <td>This option creates a proof with no workflow attached and applies the default proof settings. You can update the default proof settings or add a workflow after you've created the proof. For more information on proof settings, see <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Edit proof settings</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Advanced Proof</strong></td> 
      <td> <p>This option allows you to configure a Basic or Advanced workflow and modify proof settings for the proof you create. Para obter mais informações, consulte: </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho Básico</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho automatizado</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Gerenciar uma prova existente

Depois de criar uma prova, faça o seguinte:

* Exibir atividade de estágio atual
* Atualizar revisores e prazos
* Editar o fluxo de trabalho

Para obter mais informações sobre como gerenciar uma prova existente, consulte [Gerenciar provas no Adobe Workfront: índice do artigo](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Revisar uma prova

Os revisores atribuídos podem fazer o seguinte:

* Exibir o ativo e fazer comentários
* Adicionar ações a comentários
* Comparar versões
* Aprovar ou rejeitar a prova

Para obter mais informações sobre o que você pode fazer com a ferramenta de revisão, consulte [Revisar provas no Adobe Workfront: índice do artigo](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
