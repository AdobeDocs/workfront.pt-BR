---
product-area: documents
navigation-topic: approvals
title: Criar revisores de IA
description: Depois de ter pelo menos uma marca configurada no Workfront, você pode criar vários Revisores de IA, que podem ser atribuídos a modelos de aprovação e a solicitações individuais de revisão e aprovação.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
exl-id: 4673049e-119e-4315-95f0-f10d8b286856
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/sfM3OtA-DVqywr3Up8VGjcycLRs5WtF22dcpXzRlnvQ'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
    internal-label: Requests
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 17%
---
# Criar revisores de IA

>[!NOTE]
>
>No momento, esse recurso está na versão beta.

Depois de ter pelo menos uma marca configurada no Workfront, você pode criar vários Revisores de IA, que podem ser atribuídos a modelos de aprovação e a solicitações individuais de revisão e aprovação.


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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do sistema.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar, você deve configurar as diretrizes de marca de imagem no Workfront. Para obter mais informações, consulte [Criar e gerenciar marcas para o Revisor da IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Adicionar um revisor de IA

>[!NOTE]
>
>O Revisor de IA não foi projetado para ser um tomador de decisão no fluxo de trabalho de revisão e aprovação. Ela só fornece uma pontuação e recomendações para alinhar o ativo aos requisitos da marca especificados.

Para adicionar um Revisor de IA:

{{step-1-to-setup}}

1. No painel esquerdo, vá para **Revisão e Aprovação** > **Revisor**.
1. Clique em **Adicionar novo**.
1. Nomeie o revisor.
1. Selecione uma **Marca**.
1. Selecione uma das seguintes opções no menu suspenso **Tipo de diretriz**:
   * **Imagem**: o Revisor da IA revisará o ativo em relação às diretrizes da marca da imagem que você configurou no Workfront.
   * **Voz da marca**: o Revisor da IA revisará o ativo em relação às diretrizes de voz da marca que você configurou no Workfront.
1. Clique em **Criar**.

   Depois que o Revisor de IA é criado, os usuários podem adicioná-lo aos modelos de aprovação ou aprovações individuais.

   Para obter mais informações, consulte

   * [Criar um modelo de fluxo de trabalho de aprovação para documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
   * [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)
