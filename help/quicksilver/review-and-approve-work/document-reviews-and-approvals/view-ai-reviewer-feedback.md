---
product-area: documents
navigation-topic: approvals
title: Exibir pontuação e feedback do revisor com IA
description: Segundos após enviar a solicitação de aprovação, é possível exibir a pontuação e o feedback do Revisor da IA no painel Resumo do documento.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 838e8f3d-0ea6-4844-a261-ef7b0e78a755
TQID: 'https://experienceleague.adobe.com/iPlcSTaPI-zhmWvRvO81RKFYnIzUoJqzM70mNcxrVbs'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 3%
---
# Exibir pontuação e feedback do revisor com IA

Segundos após enviar a solicitação de revisão e aprovação, é possível exibir a pontuação e o feedback do Revisor da IA no painel Resumo do documento.

O Revisor de IA não foi projetado para ser um tomador de decisão no fluxo de trabalho de revisão e aprovação. Ela só fornece uma pontuação e recomendações para alinhar o ativo aos requisitos da marca especificados.

![Comentários do revisor da IA](assets/ai-reviewer-output.png)

## Entender como as pontuações são calculadas

O Revisor da IA calcula as pontuações de forma diferente dependendo do tipo de revisão:

* Revisão da imagem: essa pontuação reflete a proporção entre as diretrizes aprovadas e as com falha.
* Revisão da cópia: essa pontuação usa uma ponderação equilibrada de resultados subjetivos e objetivos. Diretrizes de objetivo (exibidas em &quot;Fix&quot;) são ponderadas três vezes mais do que diretrizes subjetivas (exibidas em &quot;Considerar&quot;).

Como as diretrizes objetivas têm mais peso nas revisões de cópia, recomendamos escrever diretrizes concretas e mensuráveis na sua marca. Para obter mais informações, consulte a seção [Práticas recomendadas para escrever as diretrizes da marca](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md#best-practices-for-writing-brand-guidelines) no artigo Criar e gerenciar marcas para o Revisor da IA.

## Exibir pontuação e feedback

Você pode visualizar a pontuação e o feedback do revisor do AI no painel Resumo do documento ou na guia Aprovações na página Detalhes do documento.

1. No email de notificação do Workfront, clique em **Ir para revisão**.

   Ou

   Vá para a área Documentos onde o documento é carregado e abra o painel Resumo do documento.
1. Clique em **Pontuação**.
   ![exibir pontuação do documento](assets/view-score.png)

Na janela de pontuação e feedback, o Revisor da IA explica como o ativo não atende às diretrizes especificadas.
![O feedback do revisor da IA precisa de atenção](assets/ai-reviewer-needs-attention.png)

## Faça upload de uma nova versão e adicione o Revisor do AI novamente

Se você precisar ajustar o ativo com base no feedback do Revisor da IA, é possível fazer upload de uma nova versão e iniciar uma nova revisão.

Para obter mais informações, consulte [Carregar uma nova versão do documento e solicitar uma aprovação](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md).
