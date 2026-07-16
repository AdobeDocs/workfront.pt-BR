---
product-area: documents
navigation-topic: approvals
title: Usar recursos de aprovação unificada e revisão juntos
description: Você pode usar Aprovações unificadas com revisões.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UBrLQv-1DRwZ-TO3c1SAUn8OF0yOAYnKPGrf-lSS0xM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 678
ht-degree: 1%

---

# Usar recursos de aprovação unificada e revisão juntos

Aprovações unificadas no Workfront apresenta um novo conjunto de recursos para ajudar você a revisar e aprovar documentos. Você pode usar um fluxo de trabalho de Aprovações unificadas com o visualizador de provas existente para adicionar comentários e marcação a documentos em revisão.

Existem algumas diferenças principais no fluxo de trabalho ao usar aprovações unificadas e provas juntas:

* Os participantes são mostrados no Resumo do documento, não no fluxo de trabalho de prova.

* Enviado, Aberto, Comentário, Detalhes de decisão (SOCD) na lista de documentos estão relacionados à revisão e não refletem o status de decisão do documento.

## Carregar um documento e criar uma prova

1. Vá para o projeto, tarefa ou problema em que deseja adicionar um novo documento.
1. Clique na guia **Documentos** e no menu suspenso **Adicionar novo**.
Ou
Arraste e solte o documento na lista de documentos.

   >[!NOTE]
   >
   >Se você tiver o **Gerar provas automaticamente ao carregar documentos** habilitado no seu perfil de usuário, o sistema criará automaticamente uma prova simples.

1. Passe o mouse sobre o documento, clique no link **Criar Prova** que aparece abaixo do nome do documento e selecione **Prova Simples**. Você precisa criar uma prova simples porque não usará o fluxo de trabalho de prova para aprovações.

Os usuários atribuídos como participantes podem usar o visualizador de provas para adicionar comentários e marcações no documento. Prossiga para a próxima seção para saber como adicionar participantes de revisão.

<!--
## Open the document Summary and assign participants in Production

You have the option to assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the document to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

To assign participants:

1. Select the document you uploaded and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

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

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## Abrir o Resumo do documento e atribuir os participantes

A caixa de diálogo Solicitar aprovação é aberta no modo Básico por padrão para uma aprovação de estágio único. Alterne para o modo Avançado para configurar aprovações de vários estágios ou caminhos paralelos.

Para atribuir participantes:

1. Selecione o documento que você carregou e abra o documento Resumo.

   ![Abrir resumo do documento](assets/open-doc-summary.png)

1. Role para baixo até a seção **Aprovações** e clique em **Criar fluxo de trabalho**. A caixa de diálogo **Solicitar aprovação** é aberta no modo Básico.

1. Configure o fluxo de trabalho de aprovação. Para obter descrições dos campos, a opção Modo avançado e o fluxo de caminhos paralelos, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Clique em **Solicitar aprovação**. Os participantes são notificados por email.

<!--
## Create a new version as needed in Production

If you need another round of review and approval, you can create a new proof version and add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants in the document Summary.

To add a new version:

1. Drag and drop the new file on top of the previous document in Workfront. This automatically creates a new version. 

1. Once the document finishes uploading, select the document, then click **Create proof** > **Simple proof**. 

1. Select the document again, and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

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

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## Crie uma nova versão conforme necessário

Se precisar de outra rodada de revisão e aprovação, poderá criar uma nova versão de prova e adicionar os participantes anteriores, novos participantes ou uma combinação de ambos. Você pode exibir informações sobre versões anteriores e participantes no Resumo do documento.

A caixa de diálogo Solicitar aprovação é aberta no modo Básico por padrão para uma aprovação de estágio único. Alterne para o modo Avançado para configurar aprovações de vários estágios ou caminhos paralelos.

Para adicionar uma nova versão:

1. Arraste e solte o novo arquivo sobre o documento anterior no Workfront. O Workfront cria automaticamente uma nova versão.

1. Depois que o documento terminar de ser carregado, selecione-o e clique em **Criar prova** > **Prova simples**.

1. Selecione o documento novamente e, em seguida, abra o documento Resumo.

   ![Abrir resumo do documento](assets/open-doc-summary.png)

1. Role para baixo até a seção **Aprovações** e clique em **Criar fluxo de trabalho**. A caixa de diálogo **Solicitar aprovação** é aberta no modo Básico.

1. Configure o fluxo de trabalho de aprovação. Para obter descrições dos campos, a opção Modo avançado e o fluxo de caminhos paralelos, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Clique em **Solicitar aprovação**. Os participantes são notificados por email.

## Revise a prova e tome uma decisão

O documento não passará para um status de aprovado até que todos os aprovadores atribuídos escolham &quot;aprovado&quot;.

Para revisar e aprovar um documento:

1. Vá para a notificação por email de revisão e clique em **Ir para revisão**.

1. Depois de entrar no Workfront, clique em **Ir para prova**.

1. Revise o conteúdo e adicione comentários ou marcações. Para obter mais informações sobre como usar o visualizador de provas, consulte [Revisar provas no Adobe Workfront: índice do artigo](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Escolha uma das seguintes decisões:

   * **Aprovar**: o documento não precisa de alterações e está pronto para uso.
   * **Aprovar com alterações**: o documento precisa de alterações e está pronto para uso quando elas forem feitas. Aprovação adicional não é necessária.
   * **Precisa do trabalho**: o documento precisa de alterações e não está pronto para uso. Depois que as alterações especificadas forem feitas, o documento deverá ser carregado como uma nova versão e passar por outra rodada de aprovações. Para obter mais informações sobre como carregar uma nova versão, consulte [Criar uma nova versão conforme necessário](#create-a-new-version-as-needed) neste artigo.

Depois de tomar uma decisão, o proprietário do documento é notificado por email.