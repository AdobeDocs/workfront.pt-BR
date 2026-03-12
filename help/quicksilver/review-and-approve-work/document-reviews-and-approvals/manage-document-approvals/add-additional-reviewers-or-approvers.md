---
product-area: documents
navigation-topic: approvals
title: Adicionar aprovadores ou revisores adicionais a um fluxo de trabalho de aprovação de documento
description: Você pode adicionar outros aprovadores ou revisores a um documento que já tem aprovações pendentes.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 4%

---

# Adicionar aprovadores ou revisores adicionais a um fluxo de trabalho de aprovação de documento

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

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
   <td> <p>Qualquer</p> </td> 
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


## Adicione aprovadores ou revisores adicionais na página Detalhes do documento no ambiente de produção

1. Vá para a página do documento clicando no nome do documento e selecione a versão do documento à qual deseja adicionar um aprovador ou revisor no menu suspenso de versões. A versão mais recente é selecionada por padrão.

1. Selecione **Aprovações** no painel esquerdo. Todos os aprovadores e revisores existentes estão listados aqui.

1. Para adicionar um aprovador, verifique se a caixa de seleção **Aprovador** está marcada e comece a digitar na caixa de texto **Revisores**. Você pode adicionar usuários ou equipes do Workfront por nome. Se você quiser adicionar um revisor, simplesmente desmarque a caixa de seleção **Aprovador** antes de digitar.

1. Repita a etapa anterior para adicionar aprovadores ou revisores adicionais.

## Adicionar aprovadores ou revisores adicionais do Resumo do documento em seu ambiente de produção

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.

1. Clique no documento necessário e o painel Resumo do documento será aberto.

1. Selecione a versão do documento à qual você deseja adicionar um aprovador ou revisor no menu suspenso de versões. A versão mais recente é selecionada por padrão.

1. Role para baixo até a seção **Aprovações** no painel Resumo do documento, onde todos os aprovadores e revisores existentes estão listados. Para adicionar um aprovador, verifique se a caixa de seleção **Aprovador** está marcada e comece a digitar na caixa de texto **Revisores**. Você pode adicionar usuários ou equipes do Workfront por nome. Se você quiser adicionar um revisor, simplesmente desmarque a caixa de seleção **Aprovador** antes de digitar.

1. Repita a etapa anterior para adicionar aprovadores ou revisores adicionais.

<div class="preview">

## Adicionar aprovadores ou revisores adicionais do Resumo do documento no ambiente de visualização na área de documentos herdados

Se sua organização estiver no armazenamento da Workfront, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento da Workfront, consulte [Armazenamento da Workfront vs. armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

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

</div>


## Adicionar aprovadores ou revisores adicionais do Resumo do documento na nova área de documentos

Se sua organização usar armazenamento corporativo, você verá a nova área de documentos ao acessar documentos no Workfront. Para obter mais informações sobre armazenamento corporativo, consulte [Visão geral sobre armazenamento corporativo](/help/quicksilver/review-and-approve-work/esm-overview.md).


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
