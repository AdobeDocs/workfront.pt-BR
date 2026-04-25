---
product-area: documents
navigation-topic: approvals
title: Request a legacy document approval
description: You can request approval from managers or other users for a document in Adobe Workfront. You can also request document approvals from people without Workfront accounts if your Workfront administrator has enabled this capability, as described in Configure system security preferences.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 6%

---

# Request a legacy document approval

You can request approval from managers or other users for a document in Adobe Workfront. You can also request document approvals from people without Workfront accounts if your Workfront administrator has enabled this capability, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

>[!NOTE]
>
>The information in this article refers to legacy document approvals. <br>
>For information about new Unified Review and Approval, see [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).


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
   <p>Contrbute or higher</p>
   <p>Revisar ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualize ou tenha acesso superior a projetos, tarefas, problemas, modelos, portfólios, programas, relatórios, painéis e calendários, documentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar acesso ao objeto associado à solicitação de acesso ou aprovação </p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Request a document approval

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Scroll down to the **Approvals** section in the Summary, and begin typing in the **Add Approver** text box. You can add Workfront users by name or external users by email.

1. Se o administrador do Adobe Workfront tiver habilitado a capacidade de colaborar com pessoas que não usam o Workfront, conforme descrito em [Configurar preferências de segurança do sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), você poderá digitar seus endereços de email para incluí-los.

   You cannot request approval from teams or groups.

1. Repeat the previous step to add other approvers.

## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show &quot;changes&quot; as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Role para baixo até a seção **Aprovações** no Resumo, clique no ícone Mais e, em seguida, clique em Reenviar.

   ![Reenviar aprovação](assets/nwe-resubmit-approval-350x149.png)

## Excluir uma solicitação de aprovação de documento

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Role para baixo até a seção **Aprovações** no Resumo e clique no menu **Mais** incorporado com o nome do aprovador e selecione **Excluir**.

   A solicitação de aprovação é removida e o aprovador recebe uma notificação de que sua aprovação não é mais necessária. O acesso compartilhado relacionado à aprovação também é removido.

## Enviar um lembrete a um aprovador

Você pode enviar uma mensagem para lembrar um documento a um aprovador que você está esperando pelo feedback dele.

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Role para baixo até a seção **Aprovações** no Resumo e clique no menu **Mais** incorporado com o nome do aprovador e selecione **Lembrar**.

   O aprovador recebe uma notificação informando que a aprovação ainda está pendente. Eles também podem receber um lembrete por email se tiverem essa opção ativada.
