---
product-area: documents
navigation-topic: approvals
title: Usar novas aprovações e revisões de documentos juntas
description: Você pode usar novas aprovações de documentos com revisões.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
source-git-commit: 8270a107ba2501eddbb27f52c843c337aa1f8a99
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 0%

---

# Usar novas aprovações e revisões de documentos juntas

As novas aprovações de documentos no Workfront apresentam um novo conjunto de recursos para ajudar você a revisar e aprovar documentos. Você pode usar o novo fluxo de trabalho de aprovações de documentos com o visualizador de provas existente para adicionar comentários e marcação a documentos em revisão.

Existem algumas diferenças principais no fluxo de trabalho ao usar as novas aprovações e provas de documentos juntas:

* Os botões de decisão não aparecem no visualizador de provas

* Os participantes são mostrados no Resumo do documento, não no fluxo de trabalho de comprovação

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

## Abrir o Resumo do documento e atribuir os participantes

Você tem a opção de atribuir revisores, aprovadores ou uma combinação de ambos:

* **Os revisores** podem adicionar comentários e marcar ativos. Depois de concluído, eles podem marcar sua revisão como concluída. Não é necessário marcar a revisão como concluída para que o documento avance no processo de aprovação.
* **Aprovadores** podem adicionar comentários e marcar ativos. Eles devem tomar a decisão de mover o processo de aprovação para frente.

Para atribuir participantes:

1. Selecione o documento que você carregou e abra o documento Resumo.
   ![Abrir resumo do documento](assets/open-doc-summary.png)

1. Role para baixo até a seção Aprovações e clique em **Adicionar**.

1. (Opcional) Escolha um modelo de aprovação existente. Os usuários com uma licença Standard podem criar Modelos de aprovação reutilizáveis na área Configuração. Para obter mais informações, consulte [Criar um Modelo de Aprovação para ativos e documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Opcional) Defina um prazo para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo especificado.

1. Para adicionar um aprovador, clique no botão Aprovador e comece a digitar o nome de um usuário ou de uma equipe.

1. Para adicionar um revisor, clique no botão Revisor e comece a digitar um nome de usuário ou de equipe.

   ![Adicionar aprovadores](assets/add-approvers.png)

1. Depois de adicionar todos os revisores e aprovadores, clique em **Enviar solicitação**. Os participantes são notificados por email.

## Crie uma nova versão conforme necessário

Se precisar de outra rodada de revisão e aprovação, crie uma nova versão de prova.  <!-- and add the previous participants, new participants, or a mix of both. --> Você pode exibir informações sobre versões anteriores e participantes no Resumo do documento.

Para adicionar uma nova versão:

1. Arraste e solte o novo arquivo sobre o documento anterior no Workfront. Isso cria uma nova versão automaticamente.

1. Depois que o documento terminar de ser carregado, selecione-o e clique em **Criar prova** > **Prova simples**.

1. Selecione o documento novamente e abra o Resumo do documento.
   ![Abrir resumo do documento](assets/open-doc-summary.png)

1. Role para baixo até a seção Aprovações e clique em **Adicionar**.

1. (Opcional) Escolha um modelo de aprovação existente. Os usuários com uma licença Standard podem criar Modelos de aprovação reutilizáveis na área Configuração. Para obter mais informações, consulte [Criar um Modelo de Aprovação para ativos e documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Opcional) Defina um prazo para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo especificado.

1. Para adicionar um aprovador, clique no botão Aprovador e comece a digitar um nome de usuário ou de equipe,<span class="preview">, ou escolha um aprovador da versão anterior.</span>

1. Para adicionar um revisor, clique no botão Revisor e comece a digitar um nome de usuário ou de equipe, <span class="preview">ou escolha um revisor da versão anterior. </span>

   ![Adicionar aprovadores](assets/add-approvers.png)

1. Depois de adicionar todos os revisores e aprovadores, clique em **Enviar solicitação**. Os participantes são notificados por email.

<!-- add info about reusing previous participants once released -->


## Revise a prova e tome uma decisão

O documento não passará para um status de aprovado até que todos os aprovadores atribuídos escolham &quot;aprovado&quot;.

Se qualquer aprovador escolher &quot;precisa de trabalho&quot;, o status do documento será alterado imediatamente para Precisa de trabalho. O documento precisará ser revisado e carregado como uma nova versão com um novo workflow de aprovação.

>[!IMPORTANT]
>
>Os botões de decisão do documento não aparecem no visualizador de provas. Você deve navegar de volta para a página Resumo do documento ou Detalhes do documento para tomar sua decisão ou marcar sua revisão como concluída.

Para revisar e aprovar um documento:

1. Vá para a notificação por email de revisão e clique em **Ir para revisão**.

1. Depois de entrar no Workfront, clique em **Ir para prova**.

1. Revise o conteúdo e adicione comentários ou marcações. Para obter mais informações sobre como usar o visualizador de provas, consulte [Revisar provas no Adobe Workfront: índice do artigo](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Quando terminar a revisão, feche o visualizador de provas.

1. Se você estiver na página Detalhes do documento, os botões de decisão estarão localizados no canto superior direito da tela.

1. Escolha uma das seguintes decisões:

   * **Aprovar**: o documento não precisa de alterações e está pronto para uso.
   * **Aprovar com alterações**: o documento precisa de alterações e está pronto para uso quando elas forem feitas. Aprovação adicional não é necessária.
   * **Precisa do trabalho**: o documento precisa de alterações e não está pronto para uso. Depois que as alterações especificadas forem feitas, o documento deverá ser carregado como uma nova versão e passar por outra rodada de aprovações. Para obter mais informações sobre como carregar uma nova versão, consulte [Criar uma nova versão conforme necessário](#create-a-new-version-as-needed) neste artigo.

Depois de tomar uma decisão, o proprietário do documento é notificado por email.
