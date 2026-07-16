---
product-area: documents
navigation-topic: approvals
title: Adicionar aprovadores ou revisores adicionais a um fluxo de trabalho de aprovação de documento
description: Você pode adicionar outros aprovadores ou revisores a um documento que já tem aprovações pendentes.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jo3N878hmvHRqo6kCepxPDk2-zlalLvqQbMjHHB8aGE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 746
ht-degree: 5%

---

# Adicionar aprovadores ou revisores adicionais a um fluxo de trabalho de aprovação de documento

É possível adicionar aprovadores ou revisores adicionais a um fluxo de trabalho de aprovação de documento que já tem aprovações pendentes.

>[!IMPORTANT]
>
>O conteúdo deste artigo se refere à funcionalidade atualizada de aprovação de documentos, disponível somente para contas específicas. Para obter informações sobre processos de aprovação padrão, consulte os artigos listados em [Aprovações de trabalho](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer pacote do Workfront para gerenciar aprovações usando o armazenamento herdado do Workfront</p>
<p>Qualquer pacote de fluxo de trabalho para gerenciar aprovações usando o Adobe Cloud Storage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Colaborador ou posterior</p>
   <p>Revisar ou superior</p> 
   <p>Se você estiver usando a integração Frame.io, é necessário ter uma licença Standard para criar workflows de aprovação.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualize ou tenha acesso superior a projetos, tarefas, problemas, modelos, portfólios, programas, relatórios, painéis, calendários e documentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso de visualização ou superior ao objeto associado à solicitação de acesso ou aprovação </p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



<!--
## Add additional approvers or reviewers in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To add additional approvers or reviewers from the Document Summary:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document will open.

1. Select the version of the document you would like to add an approver or reviewer to in the version drop-down menu. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Edit workflow**.

   ![edit approval workflow](assets/edit-approval-in-legacy.png)

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.
-->

## Adicionar aprovadores ou revisores adicionais na área de documentos herdados

Se sua organização estiver no armazenamento da Workfront, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento Workfront, consulte [Diferenças entre o armazenamento na nuvem Adobe e o armazenamento Workfront herdado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Para adicionar aprovadores ou revisores adicionais a partir do Resumo do Documento:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento necessário. O painel Resumo do documento desse documento é aberto.

1. Selecione a versão do documento à qual deseja adicionar um aprovador ou revisor no menu suspenso de versões. A versão mais recente é selecionada por padrão.

1. Role para baixo até a seção **Aprovações** e clique em **Editar fluxo de trabalho**. A caixa de diálogo Solicitar aprovação é aberta no modo em que a aprovação foi salva pela última vez: Básico para aprovações de estágio único ou Avançado para aprovações de vários estágios e aprovações com caminhos paralelos.

1. Adicionar usuário, equipe ou email:

   * No modo Básico, digite o nome ou email no campo **Adicionar nomes ou emails**.
   * No modo Avançado, selecione o caminho que contém o estágio que você deseja atualizar e digite o nome ou email no campo **Adicionar nomes ou emails** do estágio.

1. Para cada pessoa adicionada, escolha se ela é um aprovador ou revisor.

   ![menu suspenso de aprovador ou revisor](assets/choose-reviewer-or-approver.png)

1. Clique em **Salvar**. Os participantes adicionados receberão uma notificação por email informando que sua aprovação ou revisão é necessária no documento.

>[!TIP]
>
>Para reestruturar uma aprovação de modo Básico para uma aprovação de vários estágios ou de vários caminhos, clique em **Ir para avançado** no canto superior direito. Seus participantes existentes são preservados como Caminho 1, Estágio 1. Depois de salvar, não é possível voltar para o modo Básico. Para obter detalhes, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

<!--
## Add additional approvers or reviewers in the new Documents area in Production

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page. 

   ![Add approvers in document summary](assets/approvals-icon-new.png)


1. Click **Edit workflow**.

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.
-->

## Adicionar aprovadores ou revisores adicionais do Resumo do documento na nova área Documentos

Se sua organização usar o armazenamento em nuvem do Adobe, você verá a nova área Documentos ao acessar documentos no Workfront. Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para adicionar aprovadores ou revisores adicionais a partir do Resumo do Documento:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento e, em seguida, clique no ícone **Aprovações**, no lado direito da página.

   ![Adicionar aprovadores no resumo do documento](assets/approvals-icon-new.png)

1. Clique em **Editar workflow**. A caixa de diálogo Solicitar aprovação é aberta no modo em que a aprovação foi salva pela última vez: Básico para aprovações de estágio único ou Avançado para aprovações de vários estágios e aprovações com caminhos paralelos.

1. Adicionar usuário, equipe ou email:

   * No modo Básico, digite o nome ou email no campo **Adicionar nomes ou emails**.
   * No modo Avançado, selecione o caminho que contém o estágio que você deseja atualizar e digite o nome ou email no campo **Adicionar nomes ou emails** do estágio.

1. Para cada pessoa adicionada, escolha se ela é um aprovador ou revisor.

   ![menu suspenso de aprovador ou revisor](assets/choose-reviewer-or-approver.png)

1. Clique em **Salvar**. Os participantes adicionados receberão uma notificação por email informando que sua aprovação ou revisão é necessária no documento.

>[!TIP]
>
>Para reestruturar uma aprovação de modo Básico para uma aprovação de vários estágios ou de vários caminhos, clique em **Ir para avançado** no canto superior direito. Seus participantes existentes são preservados como Caminho 1, Estágio 1. Depois de salvar, não é possível voltar para o modo Básico. Para obter detalhes, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).
