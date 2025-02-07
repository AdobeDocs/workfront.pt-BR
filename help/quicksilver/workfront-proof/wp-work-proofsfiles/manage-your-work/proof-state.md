---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Entender o estado da prova no Workfront Proof
description: Em  [!DNL Workfront Proof], as provas existem em diferentes estados. Esses estados determinam quais ações você pode realizar na prova, como comentar ou tomar decisões.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Entender o estado da prova no Workfront Proof

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Em [!DNL Workfront Proof], as provas existem em diferentes estados. Esses estados determinam quais ações você pode realizar na prova, como comentar ou tomar decisões.

## Noções básicas sobre o estado da prova

Os quatro estados são os seguintes:

* [Ativo](#active)
* [Bloqueado](#locked)
* [Rascunho (somente Área de lançamento)](#draft-dropzone-only)
* [Enviado (somente zona de lançamento)](#submitted-dropzone-only)

### Ativo {#active}

As provas carregadas para [!DNL Workfront Proof] por meio da página Nova prova ou da Dropzone são exibidas como Ativas após serem processadas. Quando uma prova está ativa, os usuários podem revisar, fazer comentários e tomar decisões sobre a prova.

>[!NOTE]
>
>As provas carregadas por meio da Zona de lançamento aparecerão como Ativas somente se a opção Ativar prova no envio estiver ativada. Se a opção não estiver ativada, ative manualmente a prova.

Para obter mais informações sobre as configurações de Dropzone, consulte [Configurar a dropzone em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### Bloqueado {#locked}

Você pode bloquear uma prova quando terminar de revisá-la. Bloquear uma prova significa que não é possível fazer mais comentários ou tomar decisões sobre a prova, mas a prova ainda poderá ser aberta.

Qualquer usuário com direitos de Edição na prova pode desbloqueá-la.

Para obter mais informações sobre direitos, consulte [Perfis de permissões de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>As notificações por email não são mais enviadas quando uma prova é bloqueada. Por exemplo, se uma prova for bloqueada antes do prazo, um email de notificação não será enviado quando o prazo for atingido.

### Rascunho (somente Área de lançamento) {#draft-dropzone-only}

Quando você envia uma prova por meio da Zona de lançamento, ela entra no estado Rascunho antes de ser ativada pelo administrador. Quando estiver na zona de rascunho, não será possível realizar nenhuma ação na prova.

### Enviado (somente zona de lançamento) {#submitted-dropzone-only}

Depois que um rascunho é ativado pelo administrador, sua prova é exibida como Enviado na área de lançamento. Depois de enviado, você pode executar ações na prova.

## Exibindo e alterando o estado da prova

Para obter informações sobre como exibir uma lista de todas as provas em um estado específico, como exibir todas as provas Ativas ou Bloqueadas, consulte [Gerenciar Itens na Página Exibições em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) no artigo [Gerenciar Itens na Página Exibições em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Acesse seu Painel do [!DNL Workfront Proof].

   Para obter mais informações, consulte [Acesso [!DNL Workfront Proof] a partir do Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. No **[!UICONTROL Painel]**, clique na seta **[!UICONTROL Expandir]** ao lado da prova que você deseja exibir ou alterar o estado de.

   ![Expandir](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   A seção **[!UICONTROL Processo de fluxo de trabalho]** é exibida.

   ![Processo de fluxo de trabalho](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. Exiba o **[!UICONTROL Estado]** no **[!UICONTROL processo de fluxo de trabalho]**.

1. (Opcional) Para alterar o estado, passe o mouse sobre o **[!UICONTROL Estado]** atual, clique no menu suspenso e selecione um novo estado.

   ![Novo estado](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
