---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: O email de prova feita
description: Um email Prova feita é enviado ao criador de prova somente quando ele tiver criado uma prova. Se uma pessoa tiver criado uma prova e tornado outra pessoa o Proprietário, somente o novo Proprietário também receberá o email Prova feita . O criador e/ou o proprietário não receberão um. eles recebem somente o email Proof Made . Para obter mais informações sobre o email Nova prova, consulte Novo email de prova .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a6bfe471-2032-4b74-8316-584f923e8651
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# O [!UICONTROL Prova Feita] email

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

A [!UICONTROL Prova Feita] o email é enviado ao criador de prova somente quando ele tiver criado uma prova. Se uma pessoa tiver criado uma prova e tiver feito outra pessoa o Proprietário, somente o novo Proprietário também receberá a variável [!UICONTROL Prova feita] email. O criador e/ou o proprietário não receberão um. eles recebem somente o [!UICONTROL Prova Feita] email. Para obter mais informações sobre o [!UICONTROL Nova prova] email, consulte [[!UICONTROL Nova prova] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

Os usuários podem desativar [!UICONTROL Prova Feita] emails nas configurações do perfil, conforme explicado abaixo.

>[!NOTE]
>
> Se o Criador ou o Proprietário da prova tiver [!UICONTROL Prova Feita] emails desativados por padrão em suas configurações pessoais, eles não receberão nenhum [!UICONTROL Prova Feita] ou [!UICONTROL Nova prova] emails, mesmo se a variável [!UICONTROL Notificar pessoas por email] estiver marcada na caixa [!UICONTROL Nova prova] página.

![Proof_Made_Email.png](assets/proof-made-email-350x214.png)

A [!UICONTROL Prova Feita] o email inclui sua mensagem pessoal (se você incluir uma) e os seguintes detalhes de prova:

* Nome da prova
* Link pessoal para a prova
* Número da versão
* Miniatura da prova
* Progresso da prova
* Um link para Compartilhar a prova com outra pessoa
* Isso permite compartilhar o URL de prova e/ou o link de download do arquivo original.

>[!NOTE]
>
> O compartilhamento de links de prova não permite adicionar revisores explicitamente à prova, você só compartilhará o URL de prova pública e o recipient receberá acesso Somente leitura à prova.

Consulte [Compartilhar uma prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) para obter mais informações.

Se você não quiser que esse link apareça no email do destinatário, desative o [!UICONTROL Compartilhamento público] na prova ([!UICONTROL Baixar arquivo original] e [!UICONTROL URL público]).

## Desabilitação do [!UICONTROL Prova Feita] Email

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações pessoais]**, abra o **[!UICONTROL Padrões de prova]** e, em seguida, clique em **[!UICONTROL Desativar]** ao lado de **[!UICONTROL Confirmação de email quando as provas estiverem prontas]**.

1. ![Proof_Made_-_proofing_defaults.png](assets/proof-made---proofing-defaults-350x103.png)

1. Consulte [Definir configurações de notificação de email no Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) para obter instruções mais detalhadas.
1. Se as notificações por email estiverem desabilitadas como padrão no [!UICONTROL Configurações da conta], o Criador ou o Proprietário da prova não receberá [!UICONTROL Prova Feita] ou [!UICONTROL Nova prova] emails, mesmo que isso esteja ativado em suas configurações Pessoais e na variável [!UICONTROL Notificar pessoas por email] estiver marcada na caixa [!UICONTROL Nova prova] página.
