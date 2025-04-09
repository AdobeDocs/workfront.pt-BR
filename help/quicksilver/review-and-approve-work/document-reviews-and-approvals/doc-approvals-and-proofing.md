---
product-area: documents
navigation-topic: approvals
title: Usar aprovações unificadas e provas juntas
description: Você pode usar Aprovações unificadas com revisões.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
source-git-commit: 300de02b81bc6abc8be9bdceb2bd028b0c4aabfe
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# Usar aprovações unificadas e provas juntas

Aprovações unificadas no Workfront apresenta um novo conjunto de recursos para ajudar você a revisar e aprovar documentos. Você pode usar um fluxo de trabalho de Aprovações unificadas com o visualizador de provas existente para adicionar comentários e marcação a documentos em revisão.

Existem algumas diferenças principais no fluxo de trabalho ao usar aprovações unificadas e provas juntas:

* Os botões de decisão não aparecem no visualizador de provas

* Os participantes são mostrados no Resumo do documento, não no fluxo de trabalho de comprovação

* Enviado, Aberto, Comentário, Detalhes de decisão (SOCD) na lista de documentos estão relacionados à revisão e não refletem o status de decisão do documento.

## Carregar um documento e criar uma prova

1. Vá para o projeto, tarefa ou problema em que deseja adicionar um novo documento.
1. Clique na **guia documentos** e no **menu suspenso Adicionar Novo** .
Ou
Arraste e solte a documento na lista de documento.

   >[!NOTE]
   >
   >Se você tiver **gerado provas automaticamente ao carregar documentos** ativado no usuário perfil, o sistema cria automaticamente uma prova simples.

1. Passe o mouse sobre a documento e clique na **Criar Proof** link exibida abaixo do nome documento e selecione **Prova** simples. Você precisa criar uma prova simples porque não usará os fluxo de Trabalho de prova para aprovações.

Os usuários atribuídos como participantes podem usar o visualizador de provas para adicionar comentários e marcações no documento. Prossiga para a próxima seção para saber como adicionar participantes de revisão.

## Abrir o Resumo do documento e atribuir os participantes

Você tem a opção de atribuir revisores, aprovadores ou uma combinação de ambos:

* **Os revisores** podem adicionar comentários e marcar ativos. Uma vez concluída, eles podem marcar sua revisão como concluída. A marcação da revisão como concluída não é necessária para que a documento avance no processo de aprovação.
* **Os aprovadores** podem adicionar comentários e marcar ativos. Eles devem tomar uma decisão para avançar no processo de aprovação.

Para atribuir participantes:

1. Selecione o documento que você carregou e abra o documento Resumo.
   ![Abrir resumo do documento](assets/open-doc-summary.png)

1. Role para baixo até a seção Aprovações e clique em **Adicionar**.

1. (Opcional) Escolha um modelo de aprovação existente. Os usuários com uma licença Standard podem criar Modelos de aprovação reutilizáveis na área Configuração. Para obter mais informações, consulte [Criar um Modelo de Aprovação para ativos e documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Opcional) Defina um prazo para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo especificado.

1. Para adicionar um aprovador, clique no botão Aprovador e comece a digitar o nome de um usuário ou de uma equipe.

1. Para adicionar um revisor, clique no botão Revisor e comece a digitar um nome de usuário ou de equipe.

   ![Adicionar aprovadores](assets/add-approvers.png)

1. Depois de adicionar todos os revisores e aprovadores, clique **em Enviar solicitação**. Os participantes são notificados por e-mail.

## Criar uma nova versão, conforme necessário

Se precisar de outra rodada de revisão e aprovação, crie uma nova versão de prova.  <!-- and add the previous participants, new participants, or a mix of both. --> Você pode visualização informações sobre versões anteriores e participantes no Resumo documento.

Para adicionar uma nova versão:

1. Arraste e solte o novo arquivo sobre o documento anterior no Workfront. Isso cria uma nova versão automaticamente.

1. Depois que o documento terminar de ser carregado, selecione-o e clique em **Criar prova** > **Prova simples**.

1. Selecione a documento novamente e abra o Resumo da documento.
   ![Abra documento resumo](assets/open-doc-summary.png)

1. Role para baixo até a seção Aprovações e clique **em Adicionar**.

1. (Opcional) Escolha um modelo de aprovação existente. Os usuários com uma licença Standard podem criar Modelos de aprovação reutilizáveis na área Configuração. Para obter mais informações, consulte [Criar um Modelo de Aprovação para ativos e documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Opcional) Defina um prazo para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo especificado.

1. Para adicionar um aprovador, clique no botão Aprovador e comece a digitar um nome de usuário ou de equipe,<span class="preview">, ou escolha um aprovador da versão anterior.</span>

1. Para adicionar um revisor, clique no botão Revisor e comece a digitar um nome de usuário ou de equipe, <span class="preview">ou escolha um revisor da versão anterior. </span>

   ![Adicionar aprovadores](assets/add-approvers.png)

1. Depois de adicionar todos os revisores e aprovadores, clique **em Enviar solicitação**. Os participantes são notificados por e-mail.

<!-- add info about reusing previous participants once released -->


## Revise o prova e tome uma decisão

A documento não passa para um status aprovado até que todos os aprovadores atribuídos escolham &quot;aprovado&quot;.

Se qualquer aprovador escolher &quot;precisa de trabalho&quot;, o status do documento imediatamente muda para Necessidades de trabalho. A documento precisará ser revisada e carregada como uma nova versão com um novo fluxo de Trabalho de aprovação.

>[!IMPORTANT]
>
>Os botões de decisão do documento não aparecem no visualizador de provas. Você deve navegar de volta para a página Resumo do documento ou Detalhes do documento para tomar sua decisão ou marcar sua revisão como concluída.

Para revisar e aprovar um documento:

1. Vá para a notificação por email de revisão e clique em **Ir para revisão**.

1. Depois de entrar no Workfront, clique em **Ir para prova**.

1. Revise a conteúdo e adicione qualquer comentários ou marcação. Para obter mais informações sobre como usar as visualizador de prova, consulte [Provas de revisão dentro Adobe Systems Workfront: índice](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md) de artigo.

1. Quando terminar a revisão, feche o visualizador de provas.

1. Se você estiver na página Detalhes do documento, os botões de decisão estarão localizados no canto superior direito da tela.

1. Escolha uma das seguintes decisões:

   * **Aprovar**: o documento não precisa de alterações e está pronto para uso.
   * **Aprovar com alterações**: o documento precisa de alterações e está pronto para uso quando elas forem feitas. Aprovação adicional não é necessária.
   * **Precisa do trabalho**: o documento precisa de alterações e não está pronto para uso. Depois que as alterações especificadas forem feitas, o documento deverá ser carregado como uma nova versão e passar por outra rodada de aprovações. Para obter mais informações sobre como carregar uma nova versão, consulte [Criar uma nova versão conforme necessário](#create-a-new-version-as-needed) neste artigo.

Depois de tomar uma decisão, o proprietário do documento é notificado por email.
