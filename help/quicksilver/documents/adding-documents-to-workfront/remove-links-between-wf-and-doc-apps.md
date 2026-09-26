---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Remover links entre o Adobe Workfront e provedores de armazenamento de documentos externos
description: Ao fazer upload de um documento de qualquer serviço pela primeira vez, o Adobe Workfront solicita permissão do usuário para acessar seu serviço de documentos. Quando o usuário fornece suas credenciais de serviço de documento para fazer logon, o serviço de documento vincula-se ao Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/wDii-Gr-3a0NfMhc9VPfbiUNSTyJaJuFHeXACI26NxU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 14%
---
# Remover links entre o Adobe Workfront e provedores de armazenamento de documentos externos

Ao fazer upload de um documento de qualquer serviço pela primeira vez, o Adobe Workfront solicita permissão do usuário para acessar seu serviço de documentos. Quando o usuário fornece suas credenciais de serviço de documento para fazer logon, o serviço de documento vincula-se ao Workfront.

Para obter informações sobre como vincular serviços de documentos externos ao Workfront, consulte [Vinculando Documentos de Aplicativos Externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Como o serviço de documentos é o que permite a permissão para vincular ao Workfront, não é possível para o Workfront remover a permissão concedida pelo serviço de documentos. Você deve remover a permissão de dentro do aplicativo de serviço de documento ou chamar nossa Equipe de Suporte para remover este link de nossos servidores.

>[!NOTE]
>
>Essa funcionalidade não está disponível na nova área Documentos.<br>
>Se sua organização usar o armazenamento em nuvem do Adobe, você verá a nova área Documentos ao acessar documentos no Workfront. Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront*</td> 
   <td> 
   <p>Colaborador ou posterior</p>
   <p>Solicitação ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remover o link entre o Workfront e o Dropbox

1. Faça logon no Dropbox.
1. Clique na imagem do seu perfil no canto superior direito e em **Configurações**.
1. Clique na guia **Aplicativos conectados** e role para baixo até **Aplicativos vinculados**.

1. Clique no **X** ao lado de Workfront.

## Remover o link entre o Workfront e o Box

1. Faça logon na sua conta do Box.
1. Clique na imagem do perfil no canto superior direito.
1. Clique em **Configurações da conta** e, em seguida, na guia **Segurança**.

1. Localize **MyWorkfront** e clique em **X** em Esquecer aplicativo.

## Remova o link entre o Workfront e o Google Drive

1. Faça logon na sua unidade Google.
1. Clique no ícone de engrenagem no canto superior direito e em **Configurações**.
1. Clique em **Gerenciar Aplicativos** no lado esquerdo e localize o **Workfront** na lista.

1. No menu suspenso Opções, clique em **Desconectar da Unidade**.

## Remova os links entre o Workfront e Outros provedores de armazenamento de documentos

Você deve ligar para nossa Equipe de suporte para desconectar o Microsoft One Drive ou WebDAM do Workfront.

Para obter informações sobre como entrar em contato com a Equipe de Suporte, consulte [Entrar em contato com o Suporte ao Cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
