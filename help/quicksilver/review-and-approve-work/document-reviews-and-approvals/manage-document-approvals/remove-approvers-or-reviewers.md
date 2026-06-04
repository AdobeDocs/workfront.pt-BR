---
product-area: documents
navigation-topic: approvals
title: Remover aprovadores ou revisores de um fluxo de trabalho de aprovação de documento
description: Você pode remover aprovadores ou revisores individuais de um documento.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/zSKSGDHN8vNwozS4R-GYqsxP52Iob6SqcY0G32-3FyQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 544
ht-degree: 6%

---

# Remover aprovadores ou revisores de um fluxo de trabalho de aprovação de documento

Você pode remover aprovadores ou revisores individuais de um ativo ou documento depois que eles tiverem sido atribuídos.

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
   <td> <p>Qualquer pacote do Workfront para gerenciar aprovações usando o armazenamento herdado do Workfront</p>
<p>Qualquer pacote de fluxo de trabalho para gerenciar aprovações usando o Adobe Cloud Storage</p>  </td> 
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
   <td> <p>Gerenciar acesso ao objeto associado à solicitação de acesso ou aprovação </p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Remover aprovadores ou revisores de um fluxo de trabalho de aprovação na área de documentos herdados

Se sua organização estiver no armazenamento da Workfront, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento Workfront, consulte [Diferenças entre o armazenamento na nuvem Adobe e o armazenamento Workfront herdado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Para remover aprovadores ou revisores de um fluxo de trabalho de aprovação:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento necessário e o painel Resumo do documento desse documento será aberto.

1. Role para baixo até a seção **Aprovações** no painel Resumo do documento.

1. Clique em **Editar workflow**.

1. Localize o participante que você deseja remover e clique no ícone **Remover** ao lado do nome.

   A solicitação de aprovação ou revisão é removida e o aprovador recebe uma notificação de que sua aprovação não é mais necessária. O acesso compartilhado relacionado à aprovação também é removido.

   ![editar fluxo de trabalho de aprovação](assets/edit-approval-in-legacy.png)

1. (Opcional) Para alterar a função de um aprovador para um revisor, ou vice-versa, clique no menu suspenso ao lado do nome de usuário e selecione a nova função.

1. Repita a etapa anterior para remover aprovadores ou revisores adicionais.

</div>


## Remover aprovadores ou revisores de um fluxo de trabalho de aprovação na nova área Documentos

Se sua organização usar o armazenamento em nuvem do Adobe, você verá a nova área Documentos ao acessar documentos no Workfront. Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para criar um workflow de aprovação:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento e, em seguida, clique no ícone **Aprovações**, no lado direito da página.

   ![Adicionar aprovadores no resumo do documento](assets/approvals-icon-new.png)


1. Clique em **Editar workflow**.

1. Localize o participante que você deseja remover e clique no ícone **Remover** ao lado do nome.

   A solicitação de aprovação ou revisão é removida e o aprovador recebe uma notificação de que sua aprovação não é mais necessária.

1. (Opcional) Para alterar a função de um aprovador para um revisor, ou vice-versa, clique no menu suspenso ao lado do nome de usuário e selecione a nova função.

1. Repita a etapa anterior para remover aprovadores ou revisores adicionais.

   ![remover participantes de um estágio](assets/add-or-remove-participants.png)

1. Clique em **Salvar**.