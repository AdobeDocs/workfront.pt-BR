---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Definir Configurações de Prova no  [!DNL Workfront Proof]
description: É possível configurar uma prova que você está criando ou editando nas provas.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 1%

---

# Definir Configurações de Prova em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

É possível configurar uma prova que você esteja criando ou editando de qualquer uma das seguintes maneiras:

>[!NOTE]
>
>É possível definir essas configurações para todas as novas provas criadas. Para obter mais informações, consulte.

## Bloquear a prova quando a última decisão for tomada

Você pode definir um estado de prova para bloquear quando o Aprovador final tomar a decisão. Isso é útil se você quiser garantir que os revisores não possam voltar para a prova e adicionar comentários adicionais ou alterar suas decisões.

1. Crie uma nova prova, conforme descrito em [Gerar Provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página de detalhes da Prova para uma prova existente, conforme descrito em [Gerenciar detalhes da prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Configurações de prova]**, selecione **[!UICONTROL Bloquear prova quando todas as decisões necessárias forem tomadas]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Bloquear a prova quando todas as decisões forem tomadas]**.

Para obter informações sobre decisões, consulte [Tomar uma decisão sobre uma prova no visualizador de provas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## Exigir logon para todos os usuários que revisam a prova

Uma das coisas excelentes sobre [!DNL Workfront Proof] é que qualquer pessoa pode revisar uma prova, você não precisa ter seu próprio [!DNL Workfront Proof] para fazê-lo. Os destinatários recebem um email com uma URL Pessoal que os leva diretamente para a página de prova, sem que precisem entrar no [!DNL Workfront Proof].

No entanto, se você exigir níveis mais altos de segurança para o processo de revisão e aprovação, poderá usar exigir logon na prova. Isso significa que somente [!DNL Workfront Proof] usuários podem ser adicionados à prova. Além disso, eles devem inserir seus emails e senhas antes de acessá-los.

>[!NOTE]
>
>* *Para que alguém entre na prova (quando o Logon necessário tiver sido habilitado), ele deve ter sido adicionado à prova.*
>* *Se o Logon necessário estiver habilitado, as Assinaturas não poderão ser habilitadas.*

Para exigir o logon de todos os usuários que revisam a prova:

1. Crie uma nova prova, conforme descrito em [Gerar Provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página de detalhes da Prova para uma prova existente, conforme descrito em [Gerenciar detalhes da prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Configurações de prova]**, selecione **[!UICONTROL Exigir logon]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Logon necessário]**.

## Exigir apenas uma decisão para a prova

Essa configuração é útil nos casos em que você precisa apenas de uma pessoa de um grupo, departamento ou empresa para tomar uma decisão sobre a prova.

Mesmo que você atribua a função de Aprovador ou Revisor e Aprovador a várias pessoas, uma vez que uma pessoa tome uma decisão sobre uma prova, o status da prova será atualizado (de acordo com a decisão tomada). Para obter mais informações sobre o status da prova, consulte [Exibir o progresso e o status de uma prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. Crie uma nova prova, conforme descrito em [Gerar Provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página de detalhes da Prova para uma prova existente, conforme descrito em [Gerenciar detalhes da prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Fluxo de trabalho]**, selecione **[!UICONTROL Exigir apenas uma decisão para este estágio]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Somente uma decisão necessária]**.

Para obter informações sobre decisões, consulte [Tomar uma decisão sobre uma prova no visualizador de provas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## Exigir Que As Decisões Sejam Assinadas Eletronicamente

Você pode exigir uma assinatura eletrônica de qualquer revisor que tome uma decisão sobre a prova para fornecer seu email e senha. Quando um revisor faz uma solicitação para tomada de decisão é exibida, pedindo que ele insira seu email e senha e confirme sua decisão. Para obter mais informações, consulte [Noções básicas sobre assinaturas eletrônicas [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. Crie uma nova prova, conforme descrito em [Gerar Provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página de detalhes da Prova para uma prova existente, conforme descrito em [Gerenciar detalhes da prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Configurações de prova]**, selecione **[!UICONTROL Solicitar que as decisões sejam assinadas eletronicamente]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Exigir que as decisões sejam assinadas eletronicamente]**.

Para obter informações sobre decisões, consulte [Configurar opções de decisão de aprovação em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## Não permitir que os usuários baixem o arquivo original

É possível impedir que os revisores em uma prova baixem o arquivo original do qual uma prova foi criada.

1. Crie uma nova prova, conforme descrito em [Gerar Provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página de detalhes da Prova para uma prova existente, conforme descrito em [Gerenciar detalhes da prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Configurações de prova]**, desmarque **[!UICONTROL Baixar arquivo original]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Baixar arquivo original]**.

## Permitir que outros usuários assinem a prova

A assinatura é uma configuração avançada que funciona com o URL de prova e a Miniprova.

Por padrão, as pessoas que não foram especificamente adicionadas à prova e estão usando o URL da prova ou a Mini prova para acessá-la só podem visualizar a prova no modo Somente leitura. As pessoas que já são revisores na prova podem fazer logon usando seu endereço de email. Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

Ativar a assinatura na prova permite que as pessoas que não foram adicionadas explicitamente à prova assinem a prova (ou seja, se adicionem à prova). Eles receberão a função e o alerta por email que você selecionar para eles nas Configurações de assinatura.

Se a Assinatura tiver sido habilitada em uma prova, os campos abaixo ficarão ativos:

* **[!UICONTROL Validação de assinante necessária]** - O assinante deve clicar em um link em um email para acessar uma prova\
   Selecionar essa opção significa que a pessoa que está assinando não terá acesso imediato à prova, mas receberá um link para a prova em um email. O objetivo da validação do assinante é garantir que a pessoa tenha inserido um endereço de email correto ao qual tem acesso.

* **[!UICONTROL Função padrão para novos assinantes]** - Essa é a função de prova padrão que será atribuída a todos os revisores que assinarem a prova.
* **[!UICONTROL Alerta de email padrão para novos assinantes]** - É o alerta de email padrão que será atribuído a todos os revisores que assinarem a prova.

Consulte também [Assinar uma prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

Para permitir que outros usuários assinem uma prova:

1. Crie uma nova prova, conforme descrito em [Gerar Provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página de detalhes da Prova para uma prova existente, conforme descrito em [Gerenciar detalhes da prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Configurações de prova]**, desmarque **[!UICONTROL Assinar prova via URL pública ou código de inserção]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Assinatura]**.
