---
title: Aprimoramentos nos documentos do quarto trimestre de 2026
description: Aprimoramentos nos documentos do quarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 1b37b57f764d1579629e019c2025c809530124ea
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 2%

---

# Aprimoramentos nos documentos do quarto trimestre de 2026

Esta página descreve as melhorias de documentos feitas com a versão do quarto trimestre de 2026 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento do ciclo de lançamento do quarto trimestre de 2026, consulte [Visão geral da versão do quarto trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## System Administrators full access to approval templates

>[!NOTE]
>
>Preview: September 4, 2026
>Production fast release: September 4, 2026
>Production for everyone: September 4, 2026
>[!BADGE Off schedule]{type=Neutral}

System Administrators can now view, edit, delete, and bulk-delete every approval template in the account, regardless of who created or shared it. Previously, System Administrators were subject to the same sharing rules as other users, and could only see or manage templates they created or that were shared with them.

For more information, see [Manage approval templates](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md).

-->

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

## Adicionar equipes a aprovações de objetos usando o armazenamento em nuvem do Adobe

>[!NOTE]
>
>Visualização: 3 de setembro de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Agora é possível adicionar uma Equipe do Workfront como aprovador ou revisor em uma aprovação de documento ou modelo de aprovação, em vez de adicionar cada pessoa individualmente:

* Objetos no armazenamento na nuvem do Adobe: o Workfront adiciona cada membro ativo da equipe individualmente, de modo que a lista de aprovadores sempre reflete quem está atualmente na equipe.
* Objetos usando o armazenamento herdado do Workfront: por padrão, a equipe é adicionada como um único participante, mas agora você pode optar por adicionar cada membro da equipe como um participante individual.
* Nos modelos de aprovação, o Workfront armazena uma referência à equipe e a expande para membros ativos quando você aplica o modelo a um documento, não quando você salva o modelo.

Para obter mais informações, consulte:

* [Criar um fluxo de trabalho de aprovação na nova área Documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [Criar um fluxo de trabalho de aprovação na área de documentos herdados](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [Criar um modelo de fluxo de trabalho de aprovação para documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

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

## Painel Versões reprojetado na nova área de documentos

>[!NOTE]
>
>Visualização: 3 de setembro de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Se sua organização usar o armazenamento em nuvem do Adobe, o painel Versões na nova área Documentos terá um novo design:

* As versões são rotuladas como V1, V2 e assim por diante para promover a consistência com o Frame.io.
* Cada versão mostra seu status de aprovação, como &quot;Aprovado&quot; ou &quot;Retirado&quot;, diretamente na lista.
* O painel agora lista somente o Histórico de versões. Não há mais uma entrada separada de &quot;arquivo mais recente&quot; na parte superior.

Anteriormente, as versões tinham carimbo de data e hora em vez de numeradas.

Para obter mais informações, consulte [Gerenciar versões do documento](/help/quicksilver/documents/managing-documents/manage-document-versions.md).

## Painel Aprovações reprojetado na nova área de documentos

>[!NOTE]
>
>Visualização: 3 de setembro de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Se sua organização usar o armazenamento na nuvem da Adobe, o painel Aprovações na nova área Documentos agora mostrará o histórico de aprovação nas versões:

* O painel lista o fluxo de trabalho de aprovação para cada versão que tem uma, não apenas a versão atual.
* Os workflows retirados permanecem na lista, para que você ainda possa revisar suas decisões anteriores.
* Expanda qualquer versão para ver seus estágios, decisões do aprovador, regra de decisão e datas de vencimento sem sair do painel.

Anteriormente, o painel Aprovações mostrava somente o fluxo de trabalho da versão atual.

Para obter mais informações, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

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

<!--

## Approval workflow templates are private by default

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

Approval templates are now private by default. Previously, every approval requester could see every template in the system, which made template lists long and hard to navigate. Now, a template is visible only to the user who created it, unless the creator shares it.

For more information, see:

* [Share a template](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md#share-a-template) in Manage approval templates
* [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)

-->

