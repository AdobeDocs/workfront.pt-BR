---
product-area: documents;workfront-integrations
navigation-topic: adobe-creative-cloud-projects
title: Usar documentos do Workfront em aplicativos Creative Cloud
description: Abra, edite e salve documentos do Workfront no Photoshop, Illustrator e InDesign e solicite aprovações para eles.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: db6d682b43caf1d28779599495b931da5c80d126
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 3%
---
# Usar documentos do Workfront em aplicativos Creative Cloud

Depois que um projeto do Workfront estiver disponível no painel Projetos do Creative Cloud, você poderá trabalhar com seus documentos diretamente da Photoshop, Illustrator ou InDesign.

## Pré-requisitos

* Sua organização deve ter uma versão do Workfront compatível com o armazenamento em nuvem da Adobe.
* O Workfront e o Photoshop, o Illustrator ou o InDesign devem ter direito à mesma organização do Adobe Identity Management System (IMS).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versão do Adobe Workfront</td> 
   <td>Ultimate de fluxo de trabalho, com o Adobe Cloud Storage ativado</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>
      <p>Visualizar o acesso a um projeto para vê-lo no painel Projetos do Creative Cloud</p>
      <p>Editar o acesso a um projeto para adicioná-lo, editá-lo ou excluí-lo</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acessar um projeto do Workfront

A estrutura de pastas Documentos em um projeto do Workfront é espelhada no painel Projetos. Ao abrir um documento de uma pasta de projeto, editá-lo e salvá-lo, suas alterações aparecem no Workfront.

>[!NOTE]
>
>Os projetos de armazenamento herdados do Workfront não são compatíveis com o painel Projetos — somente projetos de armazenamento em nuvem do Adobe.


Para acessar um projeto do Workfront no Photoshop, Illustrator ou InDesign:

1. Abra o Photoshop, o Illustrator ou o InDesign.
1. No painel **Projetos** no lado esquerdo do aplicativo, selecione o projeto do Workfront que deseja abrir.

   ![Projetos do Workfront listados no painel Projetos](assets/cc-projects.png)

1. Abra um documento no projeto para editá-lo. Depois de salvar as alterações, elas são salvas automaticamente no projeto do Workfront.


>[!TIP]
>
>Para editar um tipo de arquivo que não pode ser aberto pelo Photoshop, Illustrator ou InDesign, como um documento do Word ou Excel, use o Adobe Cloud Drive. Para obter mais informações, consulte [visão geral do Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md).

## Salvar um novo documento no Workfront a partir de um aplicativo Creative Cloud

Você pode salvar um novo arquivo no Workfront ou pode salvar uma nova cópia de um arquivo existente no Workfront a partir do Photoshop, Illustrator ou InDesign.

Para salvar um novo documento no Workfront:

1. Abra o Photoshop, Illustrator ou InDesign e crie um novo arquivo.
1. Se você estiver salvando um novo arquivo, clique em **Salvar** no menu superior.
Ou
Se você estiver salvando uma nova cópia de um arquivo existente, clique em **Salvar como** no menu superior.
1. Na caixa de diálogo **Salvar como**, selecione **Salvar em documentos na nuvem** e escolha o projeto do Workfront necessário.

   >[!NOTE]
   >
   >Ao salvar um documento que já está no projeto do Workfront, a caixa de diálogo Salvar como não abre. Você pode selecionar um projeto do Workfront, salvar em uma pasta diferente ou escolher outro projeto do Workfront.


   ![salvar novo documento no workfront](assets/save-new-to-wf.png)

1. Escolha uma pasta de documentos e clique em **Salvar**. Se você não escolher uma pasta, o documento será salvo na pasta raiz do projeto.

   ![escolha a pasta para salvar o novo documento no workfront](assets/save-to-folder.png)

## Solicitar uma aprovação em um documento

Você pode adicionar uma aprovação de documento no Workfront a qualquer documento carregado do Photoshop, Illustrator ou InDesign, ou do Adobe Cloud Drive, igual a qualquer outro documento. Para obter mais informações, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).



## Gerenciar versões de um documento no Workfront a partir de um aplicativo Creative Cloud

Quando você salva um documento do Photoshop, Illustrator ou InDesign no Workfront, as alterações salvas são exibidas no arquivo Atual na guia Versões e são marcadas com um selo &quot;Novas alterações&quot;.

Você pode solicitar uma aprovação no arquivo Atual em vez de carregar uma nova versão do documento. Para obter mais informações, consulte [Solicitar uma aprovação no arquivo Atual](#request-approval-on-the-current-file).

![arquivo atual com selo de novas alterações](assets/current-file.png)

### Solicitar aprovação no arquivo atual

Para solicitar uma aprovação no arquivo Atual de um documento no Workfront:

1. Vá para o projeto no Workfront que contém o documento no qual você deseja solicitar uma aprovação.
1. Abra o documento e vá para a guia **Versões**.
1. No arquivo Atual, clique no menu **Mais** e em **Solicitar Aprovação**.
1. Na caixa de diálogo **Solicitar Aprovação**, siga as etapas em [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) para criar a aprovação.

   ![solicitar aprovação no arquivo atual](assets/request-update-on-current-file.png)

