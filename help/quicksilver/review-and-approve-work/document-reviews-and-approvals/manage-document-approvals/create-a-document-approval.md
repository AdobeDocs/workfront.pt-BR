---
product-area: documents
navigation-topic: approvals
title: Criar um fluxo de trabalho de aprovação de documento
description: Você pode solicitar aprovação de outros usuários para um documento no Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 4%

---

# Criar um fluxo de trabalho de aprovação de documento

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

Você pode solicitar aprovação de outros usuários ou equipes para um documento no Adobe Workfront ou solicitar que eles revisem um documento sem precisar aprová-lo.

>[!IMPORTANT]
>
>O conteúdo deste artigo se refere à funcionalidade atualizada de aprovação de documentos, disponível somente para contas específicas. Para obter informações sobre processos de aprovação padrão, consulte os artigos listados em [Aprovações de trabalho](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>Visualize ou tenha acesso superior a projetos, tarefas, problemas, modelos, portfólios, programas, relatórios, painéis e calendários, documentos</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar acesso ao objeto associado à solicitação de acesso ou aprovação </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Crie um documento de revisão ou solicitação de aprovação a partir da página de documentos no seu ambiente de produção

1. Passe o mouse sobre o documento e clique em Detalhes do documento.
   ![Detalhes do documento](assets/doc-details.png)

1. Próximo ao nome do documento, selecione a versão do documento para a qual deseja criar uma aprovação na lista suspensa versão. A versão mais recente é selecionada por padrão.

1. Clique em **Aprovações** no painel esquerdo.

1. (Opcional) Defina um prazo para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo especificado.

1. Para adicionar um aprovador, clique em **Aprovador** e comece a digitar um nome de usuário ou de equipe.

1. Para adicionar um revisor, clique na caixa de seleção **Revisor** e comece a digitar um nome de usuário ou de equipe.

   ![Adicionar aprovador e prazo final](assets/add-approver-and-deadline.png)

1. Repita a etapa anterior para adicionar aprovadores ou revisores adicionais.

## Crie uma solicitação de revisão ou aprovação de documento a partir do painel Resumo de documentos em seu ambiente de produção

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.

1. Clique no documento necessário e o painel esquerdo Resumo do documento desse documento será aberto.

1. Selecione a versão do documento para a qual você deseja criar uma aprovação na lista suspensa de versões. A versão mais recente é selecionada por padrão.

1. Role para baixo até a seção **Aprovações** no painel Resumo do documento e clique em **Adicionar**.

![Adicionar aprovadores no resumo do documento](assets/doc-summary-add-approvers.png)

1. (Opcional) Defina um prazo para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo especificado.

1. Para adicionar um aprovador, clique em **Aprovador** e comece a digitar um nome de usuário ou de equipe.

1. Para adicionar um revisor, clique na caixa de seleção **Revisor** e comece a digitar um nome de usuário ou de equipe.

   ![Adicionar aprovador e prazo final](assets/add-approver-and-deadline.png)

1. Repita a etapa anterior para adicionar aprovadores ou revisores adicionais.

<div class="preview">

## Crie um fluxo de trabalho de aprovação por meio do painel Resumo no seu ambiente de visualização na área de documentos herdados

Se sua organização estiver no armazenamento da Workfront, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento da Workfront, consulte [Armazenamento da Workfront vs. armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

Para criar um workflow de aprovação:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento necessário e o painel Resumo do documento desse documento será aberto.

1. Selecione a versão do documento para a qual você deseja criar uma aprovação na lista suspensa de versões. A versão mais recente é selecionada por padrão.

1. Role para baixo até a seção **Aprovações** e clique em **Criar fluxo de trabalho**.


1. Preencha os seguintes detalhes:

   <table>
   <tr>
   <td><strong>Nome do estágio</strong></td>
   <td>Adicione um nome de estágio. Você pode alterar o nome para algo mais descritivo, como <em>Revisão inicial</em> ou <em>Aprovação final</em>.</td>
   </tr>
   <tr>
   <td><strong>Adicionar nomes ou emails</strong></td>
   <td>Comece a digitar um nome de usuário ou de equipe para adicionar como aprovador ou revisor. Se você tiver apenas revisores, eles serão notificados e terão a opção de concluir a revisão, mas nenhuma decisão será necessária ou tomada.</td>
   </tr>
   <tr>
   <td><strong>É necessária uma decisão (opcional)</strong></td>
   <td>A primeira pessoa que toma uma decisão completa a etapa.</td>
   </tr>
   <tr>
   <td><strong>Data de vencimento (opcional)</strong></td>
   <td>Defina uma data de vencimento para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes da data de vencimento especificada.</td>
   </tr>
   </table>

1. (Opcional) Repita a etapa anterior para adicionar etapas adicionais, conforme necessário.

   >[!NOTE]
   >
   >Se você adicionar vários estágios, o workflow de aprovação continuará na ordem em que os estágios são listados. Quando todas as decisões necessárias forem tomadas, o próximo estágio será iniciado e o estágio anterior será bloqueado.

   ![Detalhes do documento](assets/new-stage.png)

</div>

## Crie um fluxo de trabalho de aprovação por meio do painel Resumo na nova área de documento

Se sua organização usar armazenamento corporativo, você verá a nova área de documentos ao acessar documentos no Workfront. Para obter mais informações sobre armazenamento corporativo, consulte [Visão geral sobre armazenamento corporativo](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para criar um workflow de aprovação:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento e, em seguida, clique no ícone Aprovações no lado direito da página.

   ![Adicionar aprovadores no resumo do documento](assets/approvals-icon-new.png)

1. Clique em **Criar fluxo de trabalho** e preencha os seguintes detalhes:

   <table>
   <tr>
   <td><strong>Nome do estágio</strong></td>
   <td>Adicione um nome de estágio. Você pode alterar o nome para algo mais descritivo, como <em>Revisão inicial</em> ou <em>Aprovação final</em>.</td>
   </tr>
   <tr>
   <td><strong>Adicionar nomes ou emails</strong></td>
   <td>Comece a digitar um nome de usuário ou de equipe para adicionar como aprovador ou revisor. Se você tiver apenas revisores, eles serão notificados e terão a opção de concluir a revisão, mas nenhuma decisão será necessária ou tomada.</td>
   </tr>
   <tr>
   <td><strong>É necessária uma decisão (opcional)</strong></td>
   <td>A primeira pessoa que toma uma decisão completa a etapa.</td>
   </tr>
   <tr>
   <td><strong>Data de vencimento (opcional)</strong></td>
   <td>Defina uma data de vencimento para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes da data de vencimento especificada.</td>
   </tr>
   </table>

1. (Opcional) Repita a etapa anterior para adicionar etapas adicionais, conforme necessário.

   >[!NOTE]
   >
   >Se você adicionar vários estágios, o workflow de aprovação continuará na ordem em que os estágios são listados. Quando todas as decisões necessárias forem tomadas, o próximo estágio será iniciado e o estágio anterior será bloqueado.

   ![Detalhes do documento](assets/new-stage.png)



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
