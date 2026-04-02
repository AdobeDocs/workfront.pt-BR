---
product-area: documents
navigation-topic: approvals
title: Introdução ao Workfront Content Reviewer
description: Use o Workfront Content Reviewer AI Collaborator para avaliar o conteúdo em relação às diretrizes da marca durante os workflows de revisão e aprovação.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 2b3e2ac00126facab9cc45ba8fb193d8951a37ec
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 1%

---

# Introdução ao Workfront Content Reviewer

{{highlighted-preview-article-level}}

O Revisor de conteúdo é um Colaborador de IA, um tipo de agente de IA que pode ser adicionado aos seus projetos, tarefas e documentos. Os Colaboradores de IA podem ser configurados na área Configuração e atribuídos da mesma forma que os usuários.

No Workfront, o Revisor de conteúdo ajuda a aumentar a velocidade do conteúdo e melhorar a conformidade da marca em todo o processo de revisão e aprovação. É possível adicionar Revisores de conteúdo aos modelos de aprovação ou incluí-los em solicitações individuais de revisão e aprovação.

## Requisitos de acesso

Para configurar Revisores de conteúdo no Workfront, você deve ser um administrador do sistema.

Qualquer usuário pode adicionar o Revisor de conteúdo a uma solicitação de revisão e aprovação.

## Requisitos

* Sua instância do Workfront deve ter as Aprovações unificadas habilitadas.
* Sua organização deve ter o GenStudio Foundation.
   * O Revisor de conteúdo no Workfront fornece a funcionalidade disponível no GenStudio Foundation para revisão de ativos e fluxos de trabalho de aprovação. Não é necessário acessar o GenStudio Foundation diretamente para concluir o trabalho. Seu acesso à funcionalidade do GenStudio Foundation por meio do Revisor de conteúdo se enquadra nos termos de seu contrato com a Workfront.
* A Adobe deve ter um contrato de API Gen da Adobe assinado no arquivo.
Para obter mais informações sobre como assinar o contrato, consulte [Assinar o contrato da Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Tipos de arquivo compatíveis {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Tipo de arquivo incompatível"
>abstract="Este Revisor de Conteúdo não oferece suporte ao tipo de arquivo selecionado. Faça upload de um tipo de arquivo compatível ou remova o Revisor de conteúdo para enviar a solicitação."

O Revisor de conteúdo pode revisar os seguintes tipos de arquivos:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* GIF não animado (.gif)
* PDF (.pdf)
* PPT (.ppt, .pptx)
* DOC (.doc, .docx)

Se você fizer upload de um tipo de arquivo não compatível, a opção Revisor de conteúdo não estará disponível ao criar um fluxo de trabalho de aprovação.

## Configurar diretrizes da marca

O Revisor de conteúdo do Workfront usa as diretrizes da marca ao revisar seu conteúdo. Os administradores do Workfront podem configurar diretrizes de marca na área Configuração do Workfront. As marcas criadas na GenStudio Foundation também estão disponíveis no Workfront.

Para configurar as diretrizes da marca, os administradores do sistema devem:

1. [Conceder acesso às permissões da marca](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [Criar e gerenciar marcas para o Revisor de Conteúdo](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## Criar revisores de conteúdo

Depois que pelo menos uma marca for configurada, os administradores do Workfront poderão começar a criar Revisores de conteúdo na área Configuração. Você pode criar vários Revisores de conteúdo com foco em diferentes diretrizes:

* **Imagem**: este Revisor de Conteúdo revisará o ativo em relação às diretrizes de marca de imagem que você configurou no Workfront. [!BADGE Beta]{type=Positive tooltip="No momento, esse recurso está na versão beta."}
   * Os administradores do sistema devem assinar o contrato beta para habilitar esse recurso.
* **Voz da marca**: o revisor de conteúdo revisará o ativo em relação às diretrizes de voz da marca que você configurou no Workfront.

Os Revisores de conteúdo podem ser atribuídos a modelos de aprovação e a solicitações individuais de revisão e aprovação.

Para obter mais informações, consulte [Configurar colaboradores de IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Adicionar revisores de conteúdo para revisar e aprovar solicitações

Os usuários podem adicionar Revisores de conteúdo aos modelos de aprovação existentes ou às solicitações individuais de revisão e aprovação.

### Modelos de aprovação

Se sua organização costuma adicionar as mesmas pessoas para revisar e aprovar solicitações, os usuários da licença Standard poderão criar modelos de aprovação na área Configuração do Workfront.

Os usuários podem adicionar Revisores de conteúdo aos modelos de aprovação para verificar automaticamente a conformidade da marca quando um modelo é usado para criar uma solicitação.

Depois de criados, os modelos de aprovação podem ser aplicados a ativos na área Documentos de um projeto, tarefa ou problema.

Para obter mais informações, consulte [Criar um modelo de fluxo de trabalho de aprovação para documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

![lista de modelos mostrando os revisores de IA](assets/ai-review-templates.png)

### Solicitação de revisão e aprovação individual

Quando os usuários criam solicitações individuais de revisão e aprovação, eles podem adicionar um Revisor de conteúdo com outros participantes ou criar uma única solicitação com apenas o Revisor de conteúdo para verificar a conformidade da marca.

Para obter mais informações, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).


![Revisor de conteúdo adicionado à solicitação de aprovação individual](assets/new-stage.png)

## Exibir pontuação e feedback do revisor de conteúdo

Segundos após o envio da solicitação de revisão e aprovação com um Revisor de conteúdo, a pontuação e o feedback do Revisor de conteúdo ficam disponíveis no painel Resumo do documento, mesmo que outros participantes ainda estejam revisando e tomando decisões.

Os proprietários de aprovação também recebem um email notificando-os de que uma revisão foi concluída no ativo. No email, clique em **Ir para a revisão** e veja a pontuação e os comentários no Workfront.

O Revisor de conteúdo não foi projetado para ser um tomador de decisão no fluxo de trabalho de revisão e aprovação. Ela só fornece uma pontuação e recomendações para alinhar o ativo aos requisitos da marca especificados.

Se o ativo não atender às diretrizes da marca, o criativo poderá fazer upload de uma nova versão e o proprietário da aprovação poderá criar uma segunda solicitação de revisão e aprovação com o Revisor de conteúdo.

Para obter mais informações sobre como exibir pontuações e comentários, consulte [Exibir pontuação e feedback do revisor de conteúdo](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).

