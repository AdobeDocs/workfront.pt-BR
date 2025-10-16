---
product-area: documents
navigation-topic: approvals
title: Criar uma revisão de documento ou solicitação de aprovação
description: Você pode solicitar aprovação de outros usuários para um documento no Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: b615236d2666ebcc6db0d1f796fb0baaf362e0f2
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Criar uma revisão de documento ou solicitação de aprovação

Você pode solicitar aprovação de outros usuários ou equipes para um documento no Adobe Workfront ou solicitar que eles revisem um documento sem precisar aprová-lo.

>[!IMPORTANT]
>
>O conteúdo deste artigo se refere à funcionalidade atualizada de aprovação de documentos, disponível somente para contas específicas. Para obter informações sobre processos de aprovação padrão, consulte os artigos listados em [Aprovações de trabalho](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <p>Colaborador ou superior</p>
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

## Criar uma solicitação de revisão ou aprovação de documento a partir da página do documento

1. Passe o mouse sobre o documento e clique em Detalhes do documento.
   ![Detalhes do documento](assets/doc-details.png)

1. Próximo ao nome do documento, selecione a versão do documento para a qual deseja criar uma aprovação na lista suspensa versão. A versão mais recente será selecionada por padrão.

1. Clique em **Aprovações** no painel esquerdo.

1. (Opcional) Defina um prazo para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo especificado.

1. Para adicionar um aprovador, clique em **Aprovador** e comece a digitar um nome de usuário ou de equipe.

1. Para adicionar um revisor, clique na caixa de seleção **Revisor** e comece a digitar um nome de usuário ou de equipe.

   ![Adicionar aprovador e prazo final](assets/add-approver-and-deadline.png)

1. Repita a etapa anterior para adicionar aprovadores ou revisores adicionais.

## Criar uma solicitação de revisão ou aprovação de documento a partir do painel Resumo de documentos

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.

1. Clique no documento necessário e o painel Resumo do documento desse documento será aberto.

1. Selecione a versão do documento para a qual você deseja criar uma aprovação na lista suspensa de versões. A versão mais recente será selecionada por padrão.

1. Role para baixo até a seção **Aprovações** no painel Resumo do documento e clique em **Adicionar**.

![Adicionar aprovadores no resumo do documento](assets/doc-summary-add-approvers.png)

1. (Opcional) Defina um prazo para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo especificado.

1. Para adicionar um aprovador, clique em **Aprovador** e comece a digitar um nome de usuário ou de equipe.

1. Para adicionar um revisor, clique na caixa de seleção **Revisor** e comece a digitar um nome de usuário ou de equipe.

   ![Adicionar aprovador e prazo final](assets/add-approver-and-deadline.png)

1. Repita a etapa anterior para adicionar aprovadores ou revisores adicionais.





<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
