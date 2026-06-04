---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Email de prova criada
description: Um email de Prova feita é enviado ao criador da prova somente quando ele cria uma prova. Se uma pessoa tiver criado uma prova e tornado outra pessoa a Proprietária, somente o novo Proprietário também receberá o email de Prova feita. O Criador e/ou Proprietário não receberá um; ele receberá somente o email Prova feita. Para obter mais informações sobre o Novo email de prova, consulte Novo email de prova.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a6bfe471-2032-4b74-8316-584f923e8651
TQID: https://experienceleague.adobe.com/GmmKj5aqXNRDlKfo8BBcN7-6-jCtf2-8Dv4o2m1mPAY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 441
ht-degree: 1%

---

# O email [!UICONTROL Prova feita]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Um email [!UICONTROL Prova feita] é enviado ao criador da prova somente quando ele cria uma prova. Se uma pessoa tiver criado uma prova e tornado Proprietário outra pessoa, somente o novo Proprietário também receberá o email [!UICONTROL Prova feita]. O Criador e/ou Proprietário não receberá um; eles recebem somente o email [!UICONTROL Prova feita]. Para obter mais informações sobre o email [!UICONTROL Nova prova], consulte [[!UICONTROL Novo email de prova]](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

Os usuários podem desabilitar emails do [!UICONTROL Prova feita] em suas configurações de perfil, conforme explicado abaixo.

>[!NOTE]
>
> Se o Criador ou Proprietário da prova tiver emails do [!UICONTROL Prova feita] desabilitados por padrão em suas configurações pessoais, ele não receberá emails do [!UICONTROL Prova feita] ou [!UICONTROL Nova Prova], mesmo se a caixa [!UICONTROL Notificar pessoas por email] estiver marcada na página [!UICONTROL Nova prova].

![Proof_Made_Email.png](assets/proof-made-email-350x214.png)

Um email [!UICONTROL Prova feita] inclui sua mensagem pessoal (se você incluir uma) e os seguintes detalhes de prova:

* Nome da prova
* Link pessoal para a prova
* Número da versão
* Miniatura da prova
* Progresso da prova
* Um link para compartilhar a prova com outra pessoa
* Isso permite compartilhar o URL da prova e/ou o link de download do arquivo original.

>[!NOTE]
>
> O compartilhamento de links de prova não permite que você adicione explicitamente revisores à prova. Você só compartilhará o URL de prova pública e o recipient receberá acesso somente leitura à prova.

Consulte [Compartilhar uma prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) para obter mais informações.

Se não quiser que este link apareça no email do destinatário, desabilite as configurações de [!UICONTROL Compartilhamento público] na prova ([!UICONTROL Baixar arquivo original] e [!UICONTROL URL público]).

## Desabilitando o email [!UICONTROL Prova feita]

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações pessoais]**, abra a guia **[!UICONTROL Padrões de provas]** e clique em **[!UICONTROL Desabilitar]** ao lado de **[!UICONTROL Confirmação por email quando as provas estiverem prontas]**.

1. ![Proof_Made_-_proof_defaults.png](assets/proof-made---proofing-defaults-350x103.png)

1. Consulte [Definir configurações de notificação por email no Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) para obter instruções mais detalhadas.
1. Se as notificações por email estiverem desabilitadas como padrão nas [!UICONTROL Configurações da conta], o Criador ou Proprietário da prova não receberá emails do [!UICONTROL Comprovação feita] ou do [!UICONTROL Nova Prova], mesmo que isso esteja habilitado nas configurações Pessoais e a caixa [!UICONTROL Notificar pessoas por email] esteja marcada na página [!UICONTROL Nova prova].
