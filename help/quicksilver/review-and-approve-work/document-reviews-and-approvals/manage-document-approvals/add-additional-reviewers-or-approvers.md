---
product-area: documents
navigation-topic: approvals
title: Adicionar aprovadores ou revisores adicionais a um fluxo de trabalho de aprovação de documento
description: Você pode adicionar outros aprovadores ou revisores a um documento que já tem aprovações pendentes.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 6%

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



## Adicionar aprovadores ou revisores adicionais do Resumo do documento na área de documentos herdados

Se sua organização estiver no armazenamento da Workfront, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento Workfront, consulte [Diferenças entre o armazenamento na nuvem Adobe e o armazenamento Workfront herdado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Para adicionar aprovadores ou revisores adicionais a partir do Resumo do Documento:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento necessário e o painel Resumo do documento desse documento será aberto.

1. Selecione a versão do documento à qual você deseja adicionar um aprovador ou revisor no menu suspenso de versões. A versão mais recente é selecionada por padrão.

1. Role para baixo até a seção **Aprovações** e clique em **Editar fluxo de trabalho**.

   ![editar fluxo de trabalho de aprovação](assets/edit-approval-in-legacy.png)

1. Localize o estágio no qual você deseja adicionar aprovadores ou revisores e adicione o nome do usuário ou email na caixa de texto. Você também pode adicionar uma equipe inteira, se necessário.

1. Depois que o nome for adicionado, escolha se ele é um aprovador ou revisor.

   ![menu suspenso de aprovador ou revisor](assets/choose-approver-or-reviewer.png)

1. Repita as etapas 5 a 6 para adicionar aprovadores ou revisores adicionais.
Depois de salvar, os participantes adicionados receberão uma notificação por email informando que sua aprovação ou revisão é necessária no documento.



## Adicionar aprovadores ou revisores adicionais do Resumo do documento na nova área Documentos

Se sua organização usar o armazenamento em nuvem do Adobe, você verá a nova área Documentos ao acessar documentos no Workfront. Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento e, em seguida, clique no ícone **Aprovações**, no lado direito da página.

   ![Adicionar aprovadores no resumo do documento](assets/approvals-icon-new.png)


1. Clique em **Editar workflow**.

1. Localize o estágio no qual você deseja adicionar aprovadores ou revisores e adicione o nome do usuário ou email na caixa de texto. Você também pode adicionar uma equipe inteira, se necessário.

1. Depois que o nome for adicionado, escolha se ele é um aprovador ou revisor.

   ![menu suspenso de aprovador ou revisor](assets/choose-approver-or-reviewer.png)

1. Repita as etapas 5 a 6 para adicionar aprovadores ou revisores adicionais.
Depois de salvar, os participantes adicionados receberão uma notificação por email informando que sua aprovação ou revisão é necessária no documento.







<!--
## Add additional approvers or reviewers from Home

1. Click the **Home** icon ![Home icon](assets/home-icon-30x29.png) in the upper-left corner of Adobe Workfront.

   >[!NOTE]
   >
   >Your Workfront administrator might make the following changes to the Home icon in your environment:
   >
   >* Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. 
   >* Replace the page linked to it with a different page. In this case, click the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of the page, then click **Home**.

1. In the **Work List** area, Go to the **Approvals I've Submitted** grouping.

1. Select a **Document** approval.  

1. Click **Manage Approvals**&nbsp;in the upper-right corner of the right panel.
1. In the **Have someone approve this document** box, type the name of the approver.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

1. Click **Save**.
-->
