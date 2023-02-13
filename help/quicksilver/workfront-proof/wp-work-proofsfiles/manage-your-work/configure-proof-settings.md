---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Definir configurações de prova em [!DNL Workfront Proof]
description: Você pode configurar uma prova que está criando ou editando de qualquer uma das seguintes maneiras - EDITE-ME.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 1%

---

# Definir configurações de prova em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Você pode configurar uma prova que está criando ou editando de qualquer uma das seguintes maneiras:

>[!NOTE]
>
>É possível definir essas configurações para todas as novas provas criadas. Para obter mais informações, consulte .

## Bloquear a prova quando a última decisão for tomada

Você pode definir um estado de prova para bloquear quando o Aprovador final tomar sua decisão. Isso é útil se você quiser garantir que seus revisores não poderão voltar à prova e adicionar comentários adicionais ou alterar suas decisões.

1. Crie uma nova prova, conforme descrito em [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página Detalhes da prova para uma prova existente, conforme descrito em [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Configurações de prova]**, selecione **[!UICONTROL Bloquear a prova quando todas as decisões necessárias forem tomadas]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Bloquear a prova quando todas as decisões forem tomadas]**.

Para obter informações sobre decisões, consulte [Tome uma decisão em uma prova no visualizador de prova](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## Exigir logon para todos os usuários que revisam a prova

Uma das grandes coisas sobre [!DNL Workfront Proof] é que qualquer um pode revisar uma prova, você não precisa ter sua própria [!DNL Workfront Proof] para fazer isso. Os recipients recebem um email com um URL Pessoal que os leva diretamente à página de prova, sem precisar fazer logon [!DNL Workfront Proof].

No entanto, se você precisar de níveis mais altos de segurança para o seu processo de revisão e aprovação, poderá usar o logon obrigatório na prova. Isso significa que somente [!DNL Workfront Proof] os usuários do podem ser adicionados à prova. E eles devem digitar o email e a senha para poder acessá-los.

>[!NOTE]
>
>* *Para que alguém faça logon na prova (quando o logon necessário tiver sido ativado), ele deve ter sido adicionado à prova.*
>* *Se o Logon necessário estiver ativado, as Assinaturas não poderão ser ativadas.*


Para exigir logon para todos os usuários que revisam a prova:

1. Crie uma nova prova, conforme descrito em [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página Detalhes da prova para uma prova existente, conforme descrito em [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Configurações de prova]**, selecione **[!UICONTROL Exigir logon]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Logon necessário]**.

## Exigir apenas uma decisão para a prova

Essa configuração é útil nos casos em que você precisa apenas de uma pessoa de um grupo, departamento ou empresa para tomar uma decisão sobre a prova.

Mesmo que você atribua a função de Aprovador ou Revisor e Aprovador a várias pessoas, uma vez que uma pessoa tome uma decisão em uma prova, o status da prova será atualizado (de acordo com a decisão tomada). Para obter mais informações sobre o status da prova, consulte [Exibir o progresso e o status de uma prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. Crie uma nova prova, conforme descrito em [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página Detalhes da prova para uma prova existente, conforme descrito em [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Fluxo de trabalho]**, selecione **[!UICONTROL Exigir apenas uma decisão para esta fase]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Apenas uma decisão é necessária]**.

Para obter informações sobre decisões, consulte [Tome uma decisão em uma prova no visualizador de prova](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## Exigir a assinatura eletrônica das decisões

Você pode exigir uma assinatura eletrônica de qualquer revisor que tome uma decisão na prova para fornecer seu email e senha. Quando um revisor toma uma decisão, um prompt é exibido, solicitando que ele insira seu email e senha e confirme sua decisão. Para obter mais informações, consulte [Noções básicas sobre assinaturas eletrônicas no [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. Crie uma nova prova, conforme descrito em [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página Detalhes da prova para uma prova existente, conforme descrito em [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Configurações de prova]**, selecione **[!UICONTROL Exigir a assinatura eletrônica das decisões]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Exigir a assinatura eletrônica das decisões]**.

Para obter informações sobre decisões, consulte [Configure as opções de decisão de aprovação em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## Não permitir que os usuários baixem o arquivo original

Você pode impedir que os revisores em uma prova baixem o arquivo original do qual uma prova foi criada.

1. Crie uma nova prova, conforme descrito em [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página Detalhes da prova para uma prova existente, conforme descrito em [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Configurações de prova]**, desmarcar **[!UICONTROL Baixar arquivo original]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Download do arquivo original]**.

## Permitir que outros usuários assinem a prova

A assinatura é uma configuração avançada que funciona com o URL de prova e a prova Mini.

Por padrão, as pessoas que não foram adicionadas especificamente à prova e estão usando o URL de prova ou a Mini prova para acessá-lo só podem exibir a prova no modo Somente leitura. As pessoas que já são revisores na prova podem fazer logon usando seu endereço de email. Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

Habilitar a assinatura na prova permite que as pessoas que não foram adicionadas explicitamente à prova se inscrevam na prova (ou seja, se adicionem à prova). Eles receberão a função e o alerta por email selecionados para eles nas configurações de Assinatura.

Se a opção Subscription tiver sido ativada em uma prova, os campos abaixo se tornarão ativos:

* **[!UICONTROL Validação necessária do assinante]** - O assinante deve clicar em um link em um email para acessar uma prova\
   Selecionar essa opção significa que a pessoa que está assinando não terá acesso imediato à prova, mas obterá um link para a prova em um email. O objetivo da validação do assinante é garantir que a pessoa tenha inserido um endereço de email correto ao qual tenha acesso.

* **[!UICONTROL Função padrão para novos assinantes]** - Essa é a função de prova padrão que será atribuída a todos os revisores que assinam a prova.
* **[!UICONTROL Alerta por email padrão para novos assinantes]** - Esse é o alerta por email padrão que será atribuído a todos os revisores que assinam a prova.

Consulte também [Assinar uma prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

Para permitir que outros usuários assinem uma prova:

1. Crie uma nova prova, conforme descrito em [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Abra a página Detalhes da prova para uma prova existente, conforme descrito em [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para uma nova prova, em **[!UICONTROL Configurações de prova]**, desmarcar **[!UICONTROL Assinar prova via URL público ou código incorporado]**.\
   Ou\
   Para uma prova existente, em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Assinatura]**.
