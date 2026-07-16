---
product-area: documents
navigation-topic: approvals
title: Criar um fluxo de trabalho de aprovação de documento
description: Você pode solicitar aprovação de outros usuários para um documento no Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OoGv4oNg6GkKeo-zoVi5lSxtPK3UE64-EYW21Mz7GRA
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
source-wordcount: 2231
ht-degree: 2%

---

# Criar um fluxo de trabalho de aprovação de documento

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

<!--

## Create an approval workflow in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To create an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document opens.

1. Select the version of the document you would like to create an approval for in the version dropdown. The latest version is selected by default.

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

   ![Document details](assets/new-stage.png)

-->

## Criar um fluxo de trabalho de aprovação na área de documentos herdados

Se sua organização estiver no armazenamento da Workfront, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento Workfront, consulte [Diferenças entre o armazenamento na nuvem Adobe e o armazenamento Workfront herdado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

### Criar um fluxo de trabalho básico de aprovação

Para criar um workflow de aprovação de estágio único:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento necessário e o painel Resumo do documento desse documento será aberto.

1. Selecione a versão do documento para a qual deseja criar uma aprovação no menu suspenso versão. A versão mais recente é selecionada por padrão.

1. Role para baixo até a seção **Aprovações** e clique em **Criar fluxo de trabalho**. A caixa de diálogo **Solicitar aprovação** é aberta no modo Básico.

1. Preencha os seguintes detalhes:

   <table>
   <tr>
   <td><strong>Usar um modelo de aprovação (opcional)</strong></td>
   <td>Selecione um modelo no menu suspenso. Se o modelo tiver um caminho e um estágio, ele se aplica no modo Básico. Se o modelo tiver mais de um estágio ou mais de um caminho, a caixa de diálogo alternará automaticamente para o modo Avançado e qualquer entrada inserida no modo Básico será substituída pelo conteúdo do modelo.</td>
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
   <p>Observação: se você editar uma mensagem personalizada após a criação do fluxo de trabalho de aprovação, uma notificação por email atualizada será enviada a todos os participantes existentes. Se você adicionar um participante posteriormente, a mensagem personalizada será incluída em sua notificação por email.</p>
   </td>
   </tr>
   </table>

1. Clique em **Solicitar aprovação**.

   ![Solicitar aprovação no modo Básico](assets/request-approval-basic.jpeg)

### Criar um fluxo de trabalho de aprovação avançado

O modo avançado suporta vários estágios, bem como caminhos paralelos. Cada caminho é executado independentemente e contém um ou mais estágios sequenciais. Quando todas as decisões necessárias em um estágio são tomadas, o próximo estágio nesse caminho começa, o estágio anterior é bloqueado e os revisores e aprovadores do novo estágio recebem uma notificação por email.

Uma decisão &quot;Precisa de trabalho&quot; interrompe o caminho em seu, mas não afeta o fluxo de trabalho de aprovação em outros caminhos. É possível configurar até 30 caminhos e um total de 100 estágios.

Para criar um workflow avançado de aprovação:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento necessário e o painel Resumo do documento desse documento será aberto.

1. Selecione a versão do documento para a qual deseja criar uma aprovação no menu suspenso versão. A versão mais recente é selecionada por padrão.

1. Role para baixo até a seção **Aprovações** e clique em **Criar fluxo de trabalho**.

1. Na parte superior direita da caixa de diálogo **Solicitar aprovação**, clique em **Ir para avançado**. Qualquer entrada inserida no modo Básico é preservada e aplicada ao **Caminho 1**, **Estágio 1**.

   >[!TIP]
   >
   >Ao criar a aprovação, você pode retornar ao modo Básico clicando em **Ir para básico** no canto superior direito. Depois de clicar em **Solicitar aprovação**, a opção **Ir para básico** não estará mais disponível.

1. Preencha os detalhes para o Estágio 1 do Caminho 1:

   <table>
   <tr>
   <td><strong>Nome do estágio</strong></td>
   <td>Os estágios são nomeados como <em>Estágio 1</em>, <em>Estágio 2</em> e assim por diante por padrão. Renomeie o estágio para algo mais descritivo, como <em>Revisão inicial</em> ou <em>Aprovação final</em>.</td>
   </tr>
   <tr>
   <td><strong>Adicionar nomes ou emails</strong></td>
   <td>Comece a digitar um nome de usuário ou de equipe para adicionar como aprovador ou revisor. Se você tiver apenas revisores, eles serão notificados e terão a opção de concluir a revisão, mas nenhuma decisão será necessária ou tomada.<p>Nota: Um revisor ou aprovador pode ser atribuído a apenas um estágio aberto por vez no mesmo ativo. Se vários estágios paralelos forem abertos simultaneamente, a mesma pessoa não poderá ser adicionada a mais de um.</p></td>
   </tr>
   <tr>
   <td><strong>É necessária apenas uma decisão (opcional)</strong></td>
   <td>A primeira pessoa que toma uma decisão completa a etapa.</td>
   </tr>
   <tr>
   <td><strong>Vencimento em (opcional)</strong></td>
   <td>O primeiro estágio de cada caminho suporta uma data de vencimento absoluta. Cada estágio subsequente no caminho oferece suporte a uma data de vencimento relativa — o número de dias a partir de quando esse estágio é aberto. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo.</td>
   </tr>
   <tr>
   <td><strong>Adicionar mensagem personalizada (opcional)</strong></td>
   <td>Digite uma mensagem na caixa de texto <strong>Adicionar mensagem personalizada</strong>. A mensagem aparece na notificação por email de aprovação e na guia Approvals no Workfront.<p>Ao adicionar um segundo estágio, <strong>Mostrar esta mensagem em todos os estágios</strong> é selecionado por padrão. Deixe-a selecionada para usar a mesma mensagem em cada estágio. Para usar uma mensagem diferente para cada estágio, desmarque <strong>Mostrar esta mensagem em todos os estágios</strong> e digite a mensagem específica do estágio na caixa de texto <strong>Adicionar Mensagem Personalizada</strong> de cada estágio.</p></td>
   </tr>
   </table>

1. (Opcional) Clique em **Adicionar estágio** para adicionar outro estágio ao caminho. Os estágios em um caminho são executados sequencialmente na ordem em que estão listados. É possível reordenar os estágios em um caminho, mas não é possível mover um estágio de um caminho para outro. Cada caminho pode ter um número diferente de estágios.

1. (Opcional) Em **Caminhos paralelos**, clique em **Adicionar caminho** para adicionar outro caminho. O novo caminho começa com uma etapa vazia e se torna o caminho selecionado. Para renomear um caminho, passe o mouse sobre o rótulo do caminho, clique no ícone de lápis e digite um novo nome.

1. (Opcional) Para remover um caminho, passe o mouse sobre o rótulo do caminho e clique no ícone de lixeira. **O Caminho 1** não pode ser removido e os caminhos não podem ser reordenados. Outros caminhos podem ser removidos somente se nenhum estágio no caminho estiver bloqueado ou concluído.

   ![Modo avançado com caminhos paralelos](assets/request-approval-parallel-paths.jpeg)

1. (Opcional) Para limpar todos os caminhos e estágios e começar novamente, clique em **Redefinir** na parte superior direita.

1. Clique em **Solicitar aprovação**.


<!--

## Create an approval workflow in the new Documents area in Production

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

To create an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page.

   ![Add approvers in document summary](assets/approvals-icon-new.png)

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

   ![Document details](assets/new-stage.png)
   
-->

## Criar um fluxo de trabalho de aprovação na nova área Documentos

Se sua organização usar o armazenamento em nuvem do Adobe, você verá a nova área Documentos ao acessar documentos no Workfront. Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

A caixa de diálogo **Solicitar aprovação** é aberta no modo **Básico** por padrão. O modo básico é um estágio único com um conjunto de aprovadores ou revisores. Mudar para o modo **Avançado** para configurar aprovações de vários estágios ou caminhos paralelos.

### Criar um fluxo de trabalho básico de aprovação

Para criar um workflow de aprovação de estágio único:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento e, em seguida, clique no ícone **Aprovações**, no lado direito da página.

   ![Adicionar aprovadores no resumo do documento](assets/approvals-icon-new.png)

1. Clique em **Criar workflow**. A caixa de diálogo **Solicitar aprovação** é aberta no modo Básico.

1. Preencha os seguintes detalhes:

   <table>
   <tr>
   <td><strong>Usar um modelo de aprovação (opcional)</strong></td>
   <td>O campo templates é recolhido por padrão. Clique no campo para expandi-lo e selecione um template no menu suspenso. Se o modelo tiver um caminho e um estágio, ele se aplica no modo Básico. Se o modelo tiver mais de um estágio ou mais de um caminho, a caixa de diálogo alternará automaticamente para o modo Avançado e qualquer entrada inserida no modo Básico será substituída pelo conteúdo do modelo.</td>
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
   <td>Digite uma mensagem na caixa de texto <strong>Adicionar mensagem personalizada</strong>. A mensagem aparece na notificação por email de aprovação e na guia Approvals no Workfront.</td>
   </tr>
   </table>

1. Clique em **Solicitar aprovação**.

   ![Solicitar aprovação no modo Básico](assets/request-approval-basic.jpeg)

>[!NOTE]
>
>* A caixa de diálogo **Solicitar aprovação** é aberta no modo Básico sempre, independentemente da sessão anterior.
>* Se você editar uma mensagem personalizada após a criação do fluxo de trabalho de aprovação, uma notificação por email atualizada será enviada a todos os participantes existentes. Se você adicionar um participante posteriormente, a mensagem personalizada será incluída em sua notificação por email.
>* Depois que uma aprovação é salva, não é possível alterná-la de volta para o modo Básico. Você pode alternar uma aprovação em andamento de Básico para Avançado, desde que a aprovação não esteja bloqueada ou concluída.

### Criar um fluxo de trabalho de aprovação avançado

O modo avançado suporta caminhos paralelos. Cada caminho é executado independentemente e contém um ou mais estágios sequenciais. Quando todas as decisões necessárias em um estágio são tomadas, o próximo estágio nesse caminho começa, o estágio anterior é bloqueado e os revisores e aprovadores do novo estágio recebem uma notificação por email.

Uma decisão &quot;Precisa de trabalho&quot; interrompe o caminho em seu, mas não afeta o fluxo de trabalho de aprovação em outros caminhos. É possível configurar até 30 caminhos e um total de 100 estágios.

Para criar um workflow avançado de aprovação:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos** no painel esquerdo.

1. Clique no documento e, em seguida, clique no ícone **Aprovações**, no lado direito da página.

   ![Adicionar aprovadores no resumo do documento](assets/approvals-icon-new.png)

1. Clique em **Criar workflow**.

1. Na parte superior direita da caixa de diálogo **Solicitar aprovação**, clique em **Ir para avançado**. Qualquer entrada inserida no modo Básico é preservada e aplicada ao **Caminho 1**, **Estágio 1**.

   >[!TIP]
   >
   >Ao criar a aprovação, você pode retornar ao modo Básico clicando em **Ir para básico** no canto superior direito. Depois de clicar em **Solicitar aprovação**, a opção **Ir para básico** não estará mais disponível.

1. Preencha os detalhes para o Estágio 1 do Caminho 1:

   <table>
   <tr>
   <td><strong>Nome do estágio</strong></td>
   <td>Os estágios são nomeados como <em>Estágio 1</em>, <em>Estágio 2</em> e assim por diante por padrão. Renomeie o estágio para algo mais descritivo, como <em>Revisão inicial</em> ou <em>Aprovação final</em>.</td>
   </tr>
   <tr>
   <td><strong>Adicionar nomes ou emails</strong></td>
   <td>Comece a digitar um nome de usuário ou de equipe para adicionar como aprovador ou revisor. Se você tiver apenas revisores, eles serão notificados e terão a opção de concluir a revisão, mas nenhuma decisão será necessária ou tomada.<p>Nota: Um revisor ou aprovador pode ser atribuído a apenas um estágio aberto por vez no mesmo ativo. Se vários estágios paralelos forem abertos simultaneamente, a mesma pessoa não poderá ser adicionada a mais de um.</p></td>
   </tr>
   <tr>
   <td><strong>É necessária apenas uma decisão (opcional)</strong></td>
   <td>A primeira pessoa que toma uma decisão completa a etapa.</td>
   </tr>
   <tr>
   <td><strong>Vencimento em (opcional)</strong></td>
   <td>O primeiro estágio de cada caminho suporta uma data de vencimento absoluta. Cada estágio subsequente no caminho oferece suporte a uma data de vencimento relativa — o número de dias a partir de quando esse estágio é aberto. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo.</td>
   </tr>
   <tr>
   <td><strong>Adicionar mensagem personalizada (opcional)</strong></td>
   <td>Digite uma mensagem na caixa de texto <strong>Adicionar mensagem personalizada</strong>. A mensagem aparece na notificação por email de aprovação e na guia Approvals no Workfront.<p>Ao adicionar um segundo estágio, <strong>Mostrar esta mensagem em todos os estágios</strong> é selecionado por padrão. Deixe-a selecionada para usar a mesma mensagem em cada estágio. Para usar uma mensagem diferente para cada estágio, desmarque <strong>Mostrar esta mensagem em todos os estágios</strong> e digite a mensagem específica do estágio na caixa de texto <strong>Adicionar Mensagem Personalizada</strong> de cada estágio.</p></td>
   </tr>
   </table>

1. (Opcional) Clique em **Adicionar estágio** para adicionar outro estágio ao caminho. Os estágios em um caminho são executados sequencialmente na ordem em que estão listados. É possível reordenar os estágios em um caminho, mas não é possível mover um estágio de um caminho para outro. Cada caminho pode ter um número diferente de estágios.


1. (Opcional) Em **Caminhos paralelos**, clique em **Adicionar caminho** para adicionar outro caminho. O novo caminho começa com uma etapa vazia e se torna o caminho selecionado. Para renomear um caminho, passe o mouse sobre o rótulo do caminho, clique no ícone de lápis e digite um novo nome.

1. (Opcional) Para remover um caminho, passe o mouse sobre o rótulo do caminho e clique no ícone de lixeira. **O Caminho 1** não pode ser removido e os caminhos não podem ser reordenados. Outros caminhos podem ser removidos somente se nenhum estágio no caminho estiver bloqueado ou concluído.

   ![Modo avançado com caminhos paralelos](assets/request-approval-advanced.jpeg)

1. (Opcional) Para limpar todos os caminhos e estágios e começar novamente, clique em **Redefinir** na parte superior direita.

1. Clique em **Solicitar aprovação**.

<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->