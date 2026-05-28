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
source-git-commit: 315ec33fdcb79c6ba739a40de92be92e829a96d5
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 3%

---

# Criar um fluxo de trabalho de aprovação de documento

{{highlighted-preview}}

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

## Crie um fluxo de trabalho de aprovação por meio do painel Resumo na área de documentos herdados na Produção

Se sua organização estiver no armazenamento da Workfront, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento Workfront, consulte [Diferenças entre o armazenamento na nuvem Adobe e o armazenamento Workfront herdado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

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


<div class="preview">

## Crie um fluxo de trabalho de aprovação no painel Resumo na área Documentos herdados em Visualização

Se sua organização estiver no armazenamento da Workfront, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento Workfront, consulte [Diferenças entre o armazenamento na nuvem Adobe e o armazenamento Workfront herdado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Para criar um workflow de aprovação:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento necessário e o painel Resumo do documento desse documento será aberto.

1. Selecione a versão do documento para a qual você deseja criar uma aprovação no menu suspenso de versões. A versão mais recente é selecionada por padrão.

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
   <td><strong>É necessária apenas uma decisão (opcional)</strong></td>
   <td>A primeira pessoa que toma uma decisão completa a etapa.</td>
   </tr>
   <tr>
   <td><strong>Vencimento em (opcional)</strong></td>
   <td>Defina uma data de vencimento para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes da data de vencimento especificada.</td>
   </tr>
   <tr>
   <td><strong>Adicionar mensagem personalizada (opcional)</strong></td>
   <td>Digite uma mensagem na caixa de texto <strong>Adicionar mensagem personalizada</strong>. A mensagem aparece na notificação por email de aprovação e na guia Approvals no Workfront.
   <p>Ao adicionar um segundo estágio, <strong>Mostrar esta mensagem em todos os estágios</strong> é selecionado por padrão. Deixe-a selecionada para usar a mesma mensagem em cada estágio. Para usar uma mensagem diferente para cada estágio, desmarque <strong>Mostrar esta mensagem em todos os estágios</strong> e digite a mensagem específica do estágio na caixa de texto <strong>Adicionar Mensagem Personalizada</strong> de cada estágio, conforme necessário.</p></td>
   </tr>
   </table>

1. (Opcional) Repita a etapa anterior para adicionar etapas adicionais, conforme necessário.

   >[!NOTE]
   >
   >* Se você adicionar vários estágios, o workflow de aprovação continuará na ordem em que os estágios são listados. Quando todas as decisões necessárias forem tomadas, o próximo estágio será iniciado e o estágio anterior será bloqueado.
   >* Se você editar uma mensagem personalizada após a criação do fluxo de trabalho de aprovação, uma notificação por email atualizada será enviada a todos os participantes existentes. Se você adicionar um participante posteriormente, a mensagem personalizada será incluída em sua notificação por email.

   ![Adicionar mensagem personalizada a um estágio](assets/add-custom-message.jpeg)

</div>


## Crie um fluxo de trabalho de aprovação por meio do painel Resumo na nova área Documentos na Produção

Se sua organização usar o armazenamento em nuvem do Adobe, você verá a nova área Documentos ao acessar documentos no Workfront. Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para criar um workflow de aprovação:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento e, em seguida, clique no ícone **Aprovações**, no lado direito da página.

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


<div class="preview">

## Crie um fluxo de trabalho de aprovação no painel Resumo na nova área Documentos em Visualização

Se sua organização usar o armazenamento em nuvem do Adobe, você verá a nova área Documentos ao acessar documentos no Workfront. Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para criar um workflow de aprovação:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento e, em seguida, clique no ícone **Aprovações**, no lado direito da página.

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
   <td><strong>É necessária apenas uma decisão (opcional)</strong></td>
   <td>A primeira pessoa que toma uma decisão completa a etapa.</td>
   </tr>
   <tr>
   <td><strong>Vencimento em (opcional)</strong></td>
   <td>Defina uma data de vencimento para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes da data de vencimento especificada.</td>
   </tr>
   <tr>
   <td><strong>Adicionar mensagem personalizada (opcional)</strong></td>
   <td>Digite uma mensagem na caixa de texto <strong>Adicionar mensagem personalizada</strong>. A mensagem aparece na notificação por email de aprovação e na guia Approvals no Workfront.
   <p>Ao adicionar um segundo estágio, <strong>Mostrar esta mensagem em todos os estágios</strong> é selecionado por padrão. Deixe-a selecionada para usar a mesma mensagem em cada estágio. Para usar uma mensagem diferente para cada estágio, desmarque <strong>Mostrar esta mensagem em todos os estágios</strong> e digite a mensagem específica do estágio na caixa de texto <strong>Adicionar Mensagem Personalizada</strong> de cada estágio.</p></td>
   </tr>
   </table>

1. (Opcional) Repita a etapa anterior para adicionar etapas adicionais, conforme necessário.

   >[!NOTE]
   >
   >* Se você adicionar vários estágios, o workflow de aprovação continuará na ordem em que os estágios são listados. Quando todas as decisões necessárias forem tomadas, o próximo estágio será iniciado e o estágio anterior será bloqueado.
   >* Se você editar uma mensagem personalizada após a criação do fluxo de trabalho de aprovação, uma notificação por email atualizada será enviada a todos os participantes existentes. Se você adicionar um participante posteriormente, a mensagem personalizada será incluída em sua notificação por email.

   ![Adicionar mensagem personalizada a um estágio](assets/add-custom-message.jpeg)

</div>



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
