---
product-area: documents
navigation-topic: approvals
title: Fazer upload de uma nova versão do documento e solicitar uma aprovação
description: Você pode fazer upload de uma nova versão do documento e solicitar aprovação de outros usuários no Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grwYgMUQc-Ft08jC1Fb1n7y18cLi1HNcXvJ3wPX0URg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 66a134507a06c0ce0b4fd78bfa5e32bd95f8f08c
workflow-type: tm+mt
source-wordcount: 798
ht-degree: 7%

---

# Fazer upload de uma nova versão do documento e solicitar uma aprovação

Se um documento estiver marcado como &quot;Precisa de trabalho&quot; em uma revisão anterior, você poderá fazer upload de uma nova versão para o documento original e iniciar outra rodada de aprovações. Após carregar uma nova versão do documento, as versões anteriores serão bloqueadas.

Se o nome do arquivo da nova versão for diferente do nome do arquivo da versão anterior, o Workfront exibirá o documento com o nome de arquivo mais recente.

Quando uma nova versão é adicionada a um documento com aprovações pendentes, a aprovação da versão anterior é exibida como &quot;Retirada&quot;. O processo de aprovação anterior é encerrado, mesmo que alguns participantes ainda não tenham tomado uma decisão.

Se a versão mais recente do documento for excluída, as versões anteriores permanecerão bloqueadas. Se precisar editar uma versão anterior, desbloqueie-a manualmente.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer pacote do Workfront para gerenciar aprovações usando o armazenamento herdado do Workfront</p>
<p>Qualquer pacote de fluxo de trabalho para gerenciar aprovações usando o Adobe Cloud Storage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront</td> 
   <td> <p>Solicitação ou posterior</p>
   <p>Colaborador ou posterior</p>
   <p>Se você estiver usando a integração Frame.io, é necessário ter uma licença Standard para criar workflows de aprovação.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Editar acesso ao objeto associado ao documento</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



<!--
## Use drag-and-drop to add a new version in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Drag-and-drop does not work with Internet Explorer.


If you need another round of review and approval on a document, you can create a new document version in Workfront.

You can add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page. 

To add a new version:

1. Navigate to the document in Workfront.
1. Drag and drop the new file on top of the previous document. This automatically creates a new version. 

1. Once the document finishes uploading, select the document to open the Document Summary panel. Here you'll see the version number at the top of the panel.


1. Scroll down to the **Approvals** section.

1. Click **Create workflow**, then fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.



1. (Optional) To add an existing approval template, select a template from the left side of the dialog.

   >[!TIP]
   >
   >   Users with a Standard license can create reusable Approval Templates from the Setup area. For more information, see [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Once you have added all the stages and participants you need, click **Request approval**.

   The approval workflow starts and the approvers receive a notification that their approval is needed on the new document version. The previous document version is locked and any outstanding approvals on the previous version are withdrawn.

    ![request approval](assets/request-approval.png)
-->

<!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->

## Usar o recurso arrastar e soltar para adicionar uma nova versão na área de documentos herdados

Se sua organização estiver no armazenamento da Workfront, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento Workfront, consulte [Diferenças entre o armazenamento na nuvem Adobe e o armazenamento Workfront herdado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Arrastar e soltar não funciona com o Internet Explorer.

Se você precisar de outra rodada de revisão e aprovação em um documento, poderá criar uma nova versão do documento no Workfront. Você pode adicionar os participantes anteriores, novos participantes ou uma combinação de ambos. Você pode exibir informações sobre versões anteriores e participantes na página Detalhes do documento.

A caixa de diálogo Solicitar aprovação é aberta no modo Básico por padrão para uma aprovação de estágio único. Alterne para o modo Avançado para configurar aprovações de vários estágios ou caminhos paralelos.

Para adicionar uma nova versão e solicitar aprovação:

1. Navegue até o documento no Workfront.

1. Arraste e solte o novo arquivo sobre o documento anterior. O Workfront cria automaticamente uma nova versão.

1. Quando o documento terminar de ser carregado, selecione-o para abrir o painel Resumo do documento. O número da versão é exibido na parte superior do painel.

1. Role para baixo até a seção **Aprovações** e clique em **Criar fluxo de trabalho**. A caixa de diálogo **Solicitar aprovação** é aberta no modo Básico.

1. Configure o fluxo de trabalho de aprovação. Para obter descrições dos campos, a opção Modo avançado e o fluxo de caminhos paralelos, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Para copiar os mesmos revisores e aprovadores da versão anterior do documento, clique em **Copiar**.
1. Clique em **Solicitar aprovação**.

   O fluxo de trabalho de aprovação é iniciado e os aprovadores recebem uma notificação de que sua aprovação é necessária na nova versão do documento. A versão anterior do documento está bloqueada e todas as aprovações pendentes na versão anterior são retiradas.

## Use arrastar e soltar para adicionar uma nova versão na nova área Documentos

Se sua organização usar o armazenamento em nuvem do Adobe, você verá a nova área Documentos ao acessar documentos no Workfront. Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

>[!NOTE]
>
>Arrastar e soltar não funciona com o Internet Explorer.

Se você precisar de outra rodada de revisão e aprovação em um documento, poderá criar uma nova versão do documento no Workfront. É possível adicionar um fluxo de trabalho de aprovação à nova versão do documento.

<!--
the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page.
-->

A caixa de diálogo Solicitar aprovação é aberta no modo Básico por padrão para uma aprovação de estágio único. Alterne para o modo Avançado para configurar aprovações de vários estágios ou caminhos paralelos.

Para adicionar uma nova versão e solicitar aprovação:

1. Navegue até o documento no Workfront.

1. Arraste e solte o novo arquivo sobre o documento anterior. O Workfront cria automaticamente uma nova versão.

1. Quando o documento terminar de ser carregado, selecione-o para abrir o painel Resumo. A versão mais recente do documento é selecionada por padrão.

1. Role para baixo até a seção **Aprovações** e clique em **Criar fluxo de trabalho**. A caixa de diálogo **Solicitar aprovação** é aberta no modo Básico.

1. Configure o fluxo de trabalho de aprovação. Para obter descrições dos campos, a opção Modo avançado e o fluxo de caminhos paralelos, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Para copiar os mesmos revisores e aprovadores da versão anterior do documento, clique em **Copiar**.
1. Clique em **Solicitar aprovação**.

   O fluxo de trabalho de aprovação é iniciado e os aprovadores recebem uma notificação de que sua aprovação é necessária na nova versão do documento. A versão anterior do documento está bloqueada e todas as aprovações pendentes na versão anterior são retiradas.
