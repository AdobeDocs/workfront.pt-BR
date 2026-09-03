---
title: Aprimoramentos nos documentos do quarto trimestre de 2026
description: Aprimoramentos nos documentos do quarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: ee1fceee828c97db535ccc03c8b428940d6f7eed
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 2%

---

# Aprimoramentos nos documentos do quarto trimestre de 2026

Esta página descreve as melhorias de documentos feitas com a versão do quarto trimestre de 2026 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento do ciclo de lançamento do quarto trimestre de 2026, consulte [Visão geral da versão do quarto trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## Frame comment visibility in Workfront

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

When an approval workflow is created for a document, users can leave comments and make annotations in the Frame.io viewer. These comments are not displayed in the Workfront Comments panel, but you can view them in the Frame.io viewer.

Now, the Comments panel in Workfront displays a message letting you know when new comments are available in Frame.io.

For more information, see [Add an update to a document](/help/quicksilver/documents/managing-documents/add-update-documents.md).

-->

## Acesso à prova direta por meio de links de email de aprovação

>[!NOTE]
>
>Visualização: N/D
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Quando um documento tem uma prova anexada, o link &quot;Ir para revisão&quot; nos emails de aprovação agora abre o visualizador de prova diretamente, para que revisores e aprovadores possam iniciar sua revisão imediatamente. Se um documento não tiver prova, o link continuará a abrir a seção Aprovações do documento, como antes.

<!--

## Add teams to approvals for objects using Adobe cloud storage

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now add a Workfront Team as an approver or reviewer on a document approval or approval template, instead of adding each person individually:

* Objects on Adobe cloud storage: Workfront adds each active team member individually, so the approver list always reflects who's currently on the team.
* Objects using legacy Workfront storage: The team is added as a single participant by default, but you can now choose to add each team member as an individual participant.
* In approval templates, Workfront stores a reference to the team and expands it into active members when you apply the template to a document, not when you save the template.

For more information, see:

* [Create an approval workflow in the new Documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [Create an approval workflow in the legacy documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

-->

## Definir um espaço de trabalho Frame.io em modelos de projeto

>[!NOTE]
>
>Visualização: 3 de setembro de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Se sua organização usa o armazenamento na nuvem do Adobe e você tem uma licença Frame.io Enterprise, agora é possível escolher um espaço de trabalho Frame.io nos Detalhes do projeto em um modelo de projeto. Os projetos criados a partir do modelo usam automaticamente o espaço de trabalho definido no modelo, de modo que os projetos são direcionados para o espaço de trabalho Frame.io desejado sem nenhuma ação extra necessária na criação do projeto.

O novo campo lista os espaços de trabalho Frame.io aos quais você tem permissão para atribuir projetos. O campo permanece editável no modelo a qualquer momento; as alterações se aplicam somente aos projetos criados após a atualização, para que os projetos existentes mantenham seu espaço de trabalho original.

Depois que um projeto é criado a partir do modelo, seu campo do espaço de trabalho Frame.io é somente leitura e vincula ao espaço de trabalho no Frame.io.

Se você não tiver uma licença Frame.io Enterprise, os projetos continuarão a ir para o espaço de trabalho padrão do Workfront.

Para obter mais informações, consulte [Editar modelos de projeto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) e [Gerenciar informações na área Visão Geral do projeto](/help/quicksilver/manage-work/projects/manage-projects/understand-project-overview-area.md).

<!--

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Review and approval buttons now look and work the same everywhere you review documents: My approvals widget in Home, Document summary panel, the Document Details page, and the document preview page.

In addition to a new look and feel, some buttons have new names:

| Previous name | New name |
| --- | --- |
| Open proof | Open viewer |
| Review and approve | Make decision |
| Complete my review | Complete review |
| Open in Frame.io | Open viewer |

For more information, see [Review and approve documents](/help/quicksilver/documents/review-and-approve-documents.md).

-->

## Mensagem personalizada na linha de assunto do email

>[!NOTE]
>
>Visualização: N/D
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Ao definir uma mensagem personalizada em uma aprovação de documento, essa mensagem agora também aparece na linha de assunto do email de solicitação de aprovação, precedida pela data de vencimento quando uma é definida. Isso permite que os revisores vejam o que precisa de atenção e quando diretamente da caixa de entrada, sem abrir o email.

Para obter mais informações, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

<!--

## Redesigned Versions panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Versions panel in the new Documents area has a new design:

* Versions are labeled V1, V2, and so on to drive consistency with Frame.io.
* Each version shows its approval status, such as "Approved" or "Withdrawn", directly in the list.
* The panel now lists only Version history — there's no longer a separate "latest file" entry at the top.

Previously, versions were timestamped instead of numbered.

For more information, see [Manage document versions](/help/quicksilver/documents/managing-documents/manage-document-versions.md).

## Redesigned Approvals panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Approvals panel in the new Documents area now shows approval history across versions:

* The panel lists the approval workflow for every version that has one, not just the current version.
* Withdrawn workflows stay in the list, so you can still review their prior decisions.
* Expand any version to see its stages, approver decisions, decision rule, and due dates without leaving the panel.

Previously, the Approvals panel only showed the current version's workflow.

For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

-->

## Anexar imagens a comentários em objetos de armazenamento na nuvem do Adobe

>[!NOTE]
>
>Visualização: 30 de julho de 2026
>Versão rápida de produção: 30 de julho de 2026
>Produção para todos: 30 de julho de 2026
>[!BADGE Fora do cronograma]{type=Neutral}

Organizações que usam o armazenamento em nuvem da Adobe como parte da revisão e aprovação unificadas agora podem anexar arquivos de imagem diretamente a comentários, mantendo feedback, contexto e visuais de suporte juntos em uma única thread de comentários rastreável. Isso fecha uma lacuna anterior, em que somente as organizações no armazenamento herdado do Workfront podiam anexar imagens aos comentários.

Todos os formatos de imagem de tipo de mídia agora são compatíveis com as organizações de armazenamento em nuvem da Adobe. (Comentários de objetos herdados continuam a suportar apenas arquivos .jpg, .gif e .png.) Arquivos que não sejam de imagem não são aceitos em comentários para objetos de armazenamento na nuvem herdados ou do Adobe.

Para obter mais informações, consulte [Atualizar trabalho](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Vincular ativos do Experience Manager Assets com o Adobe Cloud Storage

>[!NOTE]
>
>Visualização: 30 de julho de 2026
>Versão rápida de produção: 13 de agosto de 2026
>Produção para todos: 15 de outubro de 2026

Se sua organização usar o armazenamento em nuvem da Adobe, você poderá vincular ativos individuais do Experience Manager Assets a qualquer objeto do Workfront que ofereça suporte a documentos. O conteúdo vinculado permanece sincronizado automaticamente: as alterações feitas no Experience Manager Assets aparecem no Workfront e você pode obter novas versões de ativos sem sair do Workfront.

A vinculação é disponibilizada pelo Supervisor de conteúdo, para que você também receba Pesquisas com IA, sugestões inteligentes, análise resumida da campanha e muito mais, enquanto seleciona o conteúdo.

Para obter mais informações, consulte [Vincular conteúdo do Experience Manager Assets com o Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/native-integrations/link-aem-assets-cloud-storage.md).
