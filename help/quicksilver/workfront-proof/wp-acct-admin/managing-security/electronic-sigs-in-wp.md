---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Compreendendo assinaturas eletrônicas em  [!DNL Workfront Proof]
description: As assinaturas eletrônicas permitem aprimorar a segurança em suas provas e estão em conformidade com os padrões do setor, como o ISO.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Compreendendo assinaturas eletrônicas em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

As assinaturas eletrônicas permitem aprimorar a segurança em suas provas e estão em conformidade com os padrões do setor, como o ISO.

Essa configuração pode ser obrigatória ou não no nível da conta. Se for obrigatório por padrão, ele será ativado em todas as provas criadas em sua conta e não poderá ser desativado no nível de prova. Se essa configuração não for obrigatória por padrão, você poderá habilitá-la/desabilitá-la no nível da prova.

Para obter mais informações, consulte.

Quando a configuração de assinatura eletrônica é ativada em uma prova, uma caixa de assinatura eletrônica solicita que qualquer revisor que tome uma decisão sobre a prova forneça seu email e senha.

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## Assinaturas eletrônicas na página [!UICONTROL Detalhes da prova]

Se um revisor tomar sua decisão selecionando sua decisão na página [!UICONTROL Detalhes da prova] (1), uma caixa pop-up [!UICONTROL Assinatura eletrônica] será exibida pedindo que ele insira seus detalhes (2) e confirme sua decisão (3).

A janela pop-up exibirá o conjunto de mensagens padrão (se houver) e o revisor precisará inserir seu email e senha.

O pop-up [!UICONTROL Assinatura eletrônica] será exibido no visualizador de provas e também na página [!UICONTROL Detalhes da prova] se o revisor decidir tomar sua decisão a partir desse nível.

![Assinatura_Eletrônica_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Assinatura_Eletrônica_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

Se a opção [!UICONTROL Logon único] estiver habilitada na prova, os detalhes do email e da senha não serão exibidos na janela pop-up [!UICONTROL Assinatura eletrônica] quando você tomar uma decisão.

Em vez disso, depois de clicar no botão [!UICONTROL Confirmar] (4) neste pop-up, o revisor será redirecionado para a página [!UICONTROL Logon Único].

Após inserir suas credenciais de SSO, o revisor será automaticamente redirecionado de volta para a página [!UICONTROL Detalhes da prova] (ou de volta para o [!UICONTROL Visualizador da Prova] se a decisão for tomada a partir dessa página).

![Assinatura_Eletrônica_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> Se a decisão for assinada eletronicamente, o **[!UICONTROL ícone de assinatura]** (5) aparecerá ao lado da decisão na seção [!UICONTROL Fluxo de trabalho] da página [!UICONTROL Detalhes da prova]. Se a decisão for alterada não pelo revisor, mas por outra pessoa com direitos de edição sobre a prova, essa pessoa não será solicitada a assinar eletronicamente a decisão e não haverá um ícone de assinatura ao lado da decisão (6).

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)Para obter informações sobre logon único, consulte [Logon único no Workfront Proof](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

Para obter informações sobre a página de detalhes da prova, consulte [Gerenciar detalhes da prova em [!DNL Workfront] Prova](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
