---
product-area: documents
navigation-topic: approvals
title: Criar revisores de IA
description: Depois de ter pelo menos uma marca configurada no Workfront, você pode criar vários Revisores de IA, que podem ser atribuídos a modelos de aprovação e a solicitações individuais de revisão e aprovação.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 4673049e-119e-4315-95f0-f10d8b286856
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 551f316bcfd5e0a1390e7be4679e06cd6808e969
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 18%

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

Antes de começar, você deve configurar as diretrizes de marca de imagem no Workfront. Para obter mais informações, consulte [Criar e gerenciar marcas para o Revisor de Conteúdo](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Adicionar um revisor de IA

>[!NOTE]
>
>O Revisor de IA não foi projetado para ser um tomador de decisão no fluxo de trabalho de revisão e aprovação. Ela só fornece uma pontuação e recomendações para alinhar o ativo aos requisitos da marca especificados.

Para adicionar um Revisor de conteúdo:

{{step-1-to-setup}}

1. No painel esquerdo, vá para **Revisão e Aprovação** > **Revisores de IA**.
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
