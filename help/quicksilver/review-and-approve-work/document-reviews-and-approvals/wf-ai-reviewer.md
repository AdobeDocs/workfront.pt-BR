---
product-area: documents
navigation-topic: approvals
title: Introdução ao Workfront AI Reviewer
description: Revisor do Workfront AI
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
source-git-commit: da980cee8710570f52c724053d1e0f359c6a9fe1
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 3%

---

# Introdução ao Workfront AI Reviewer

Com o Workfront AI Reviewer, é possível aumentar a velocidade do conteúdo e otimizar a conformidade da marca no fluxo de trabalho de revisão e aprovação. Você pode adicionar Revisores de IA a modelos de aprovação ou a solicitações individuais de revisão e aprovação no Workfront.

## Requisitos de acesso

Para configurar Revisores de IA no Workfront, você deve ser um administrador do sistema.

Qualquer usuário pode adicionar o Revisor de IA a uma solicitação de revisão e aprovação.


## Pré-requisitos

* Sua organização deve ter migrado para o Adobe IMS (Identity Management System).
* Sua instância do Workfront deve ter as Aprovações unificadas habilitadas.
* A Adobe deve ter um contrato de API Gen da Adobe assinado no arquivo.
Para obter mais informações sobre como assinar o contrato, consulte [Assinar o contrato da Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Tipos de arquivo compatíveis {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Tipo de arquivo incompatível"
>abstract="Esse Revisor do AI não oferece suporte ao tipo de arquivo selecionado. Faça o upload de um tipo de arquivo compatível ou remova o revisor com IA para enviar a solicitação."

O Revisor do AI pode revisar os seguintes tipos de arquivos:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* GIF não animado (.gif)

## Configurar diretrizes da marca

O Workfront AI Reviewer usa as diretrizes de marca configuradas nos Genstudio Foundations ao revisar seu conteúdo.

Para saber mais sobre as diretrizes da marca, consulte

* [Marcas da GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/guidelines/brands)
* [Adicionar diretrizes](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/guidelines/add-guidelines)


## Criar revisores de IA

Depois que houver pelo menos uma marca configurada no GenStudio Foundations, os administradores do Workfront poderão começar a criar Revisores de IA na área Configuração. Esses Revisores de IA podem ser atribuídos a modelos de aprovação e solicitações individuais de revisão e aprovação.

Para obter mais informações, consulte [Criar Revisores de IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/set-up-ai-reviewer.md).

## Adicionar Revisores de IA para revisar e aprovar solicitações

Os usuários podem adicionar Revisores de IA a modelos de aprovação existentes ou a solicitações individuais de revisão e aprovação.

### Modelos de aprovação

Se sua organização costuma adicionar as mesmas pessoas para revisar e aprovar solicitações, os usuários da licença Standard poderão criar modelos de aprovação na área Configuração do Workfront.

Os usuários podem adicionar Revisores de IA a modelos de aprovação para verificar automaticamente a conformidade da marca quando um modelo é usado para criar uma solicitação.

Depois de criados, os modelos de aprovação podem ser aplicados a ativos na área Documentos de um projeto, tarefa ou problema.

Para obter mais informações, consulte [Criar um modelo de aprovação para ativos e documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

![lista de modelos mostrando os revisores de IA](assets/ai-review-templates.png)

### Solicitação de revisão e aprovação individual

Quando os usuários criam solicitações individuais de revisão e aprovação, eles podem adicionar um Revisor de IA com outros participantes ou criar uma única solicitação com apenas o Revisor de IA para verificar a conformidade da marca.

Para obter mais informações, consulte [Criar uma revisão de documento ou solicitação de aprovação](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)


![Revisor de IA adicionado à solicitação de aprovação individual](assets/ad-ai-reviewer-to-request.png)

## Exibir pontuação e feedback do revisor da IA

Segundos após o envio da solicitação de revisão e aprovação com um Revisor de IA, a pontuação e o feedback do Revisor de IA ficam disponíveis no painel Resumo do documento, mesmo que outros participantes ainda estejam revisando e tomando decisões.

Os proprietários de aprovação também recebem um email notificando-os de que uma revisão foi concluída no ativo. No email, clique em **Ir para a revisão** e veja a pontuação e os comentários no Workfront.

O Revisor de IA não foi projetado para ser um tomador de decisão no fluxo de trabalho de revisão e aprovação. Ela só fornece uma pontuação e recomendações para alinhar o ativo aos requisitos da marca especificados.

Se a imagem não atender às diretrizes da marca por muito tempo, o criativo poderá fazer upload de uma nova versão e o proprietário da aprovação poderá criar uma segunda solicitação de revisão e aprovação com o Revisor da IA, permitindo alternar entre versões e comparar feedback.

Para obter mais informações sobre como exibir pontuações e feedback, consulte [Exibir pontuação e feedback do revisor da IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).


![Comentários do revisor de IA](assets/ai-reviewer-feedback.png)


