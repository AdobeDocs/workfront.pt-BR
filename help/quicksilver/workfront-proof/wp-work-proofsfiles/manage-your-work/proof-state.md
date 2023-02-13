---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Compreender o estado de prova na prova do Workfront
description: Em [!DNL Workfront Proof], as provas existem em estados diferentes. Esses estados determinam quais ações você pode realizar na prova, como comentar ou tomar decisões.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Compreender o estado de prova na prova do Workfront

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Em [!DNL Workfront Proof], as provas existem em estados diferentes. Esses estados determinam quais ações você pode realizar na prova, como comentar ou tomar decisões.

## Compreender o Estado da Prova

Os quatro estados são os seguintes:

* [Ativo](#active)
* [Bloqueado](#locked)
* [Rascunho (somente Dropzone)](#draft-dropzone-only)
* [Enviado (somente Dropzone)](#submitted-dropzone-only)

### Ativo {#active}

Provas que são carregadas para [!DNL Workfront Proof] na página Nova prova ou na Zona de controle exibida como Ativa após o processamento. Quando uma prova é ativa, os usuários podem revisar, fazer comentários e tomar decisões sobre a prova.

>[!NOTE]
>
>Provas que são carregadas por meio do Dropzone aparecem como Ativas somente se a opção Ativar prova no envio estiver ativada. Se a opção não estiver ativada, você deverá ativar manualmente a prova.

Para obter mais informações sobre as configurações do Dropzone, consulte [Configure a área suspensa em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### Bloqueado {#locked}

Você pode bloquear uma prova quando terminar de revisá-la. Bloquear uma prova significa que não é possível fazer mais comentários ou decisões na prova, mas a prova ainda pode ser aberta.

Qualquer usuário com direitos de edição na prova pode desbloqueá-la.

Para obter mais informações sobre direitos, consulte [Perfis de prova de permissões em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>As notificações por email não enviam mais quando uma prova é bloqueada. Por exemplo, se uma prova estiver bloqueada antes de seu prazo final, um email de notificação não será enviado quando o prazo for atingido.

### Rascunho (somente Dropzone) {#draft-dropzone-only}

Ao enviar uma prova pelo Dropzone, ela vai para o estado Rascunho antes de o administrador ativá-la. Quando estiver na zona de rascunho, não será possível executar nenhuma ação na prova.

### Enviado (somente Dropzone) {#submitted-dropzone-only}

Depois que um rascunho é ativado pelo administrador, sua prova é mostrada como Enviada na Zona. Depois de enviá-lo, você pode executar ações na prova.

## Exibindo e Alterando o Estado da Prova

Para obter informações sobre como visualizar uma lista de todas as provas em um estado específico, como visualizar todas as provas Ativas ou Bloqueadas, consulte [Gerenciar itens na página de exibições em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) no artigo [Gerenciar itens na página de exibições em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Acesse seu [!DNL Workfront Proof] Painel.

   Para obter mais informações, consulte [Acesso [!DNL Workfront Proof] do Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. No **[!UICONTROL Painel]**, clique no botão **[!UICONTROL Expandir]** ao lado da prova que deseja visualizar ou alterar o estado de.

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   O **[!UICONTROL Processo de workflow]** é exibida.

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. Visualize o **[!UICONTROL Estado]** no **[!UICONTROL Processo de workflow]**.

1. (Opcional) Para alterar o estado, passe o mouse sobre a **[!UICONTROL Estado]** e clique no menu suspenso e selecione um novo estado.

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
