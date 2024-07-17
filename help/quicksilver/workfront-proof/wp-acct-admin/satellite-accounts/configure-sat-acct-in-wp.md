---
product-previous: workfront-proof
product-area: documents;system-administration;setup
navigation-topic: satellite-accounts
title: Configurar uma conta satélite em  [!DNL Workfront Proof]
description: Contas satélite são contas pagas que você configura e gerencia dentro da sua própria conta do  [!DNL Workfront] Proof. Para obter mais informações, consulte "Contas satélite no [!DNL Workfront] Proof.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 82c6dff3-6187-4145-951c-3f5312049b59
source-git-commit: 5be053a6ee99404673f6f3258a423ef5e5c7f431
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 0%

---

# Configurar uma conta satélite em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Contas satélite são contas pagas que você configura e gerencia na sua própria conta do [!DNL Workfront Proof]. Para obter mais informações, consulte [Contas satélite em [!DNL Workfront] Prova](../../../workfront-proof/wp-acct-admin/satellite-accounts/sat-accts-in-wp.md).

Qualquer administrador de cobrança pode criar uma conta satélite. Para obter informações sobre Administradores de Cobrança, consulte [[!UICONTROL Perfis de Permissões de Prova] em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
> Contas satélite devem ser definidas em um de nossos planos [!UICONTROL Padrão] ou superior.

## Criação de uma conta satélite {#creating-a-satellite-account}

Para criar uma conta satélite:

1. Vá para a página [!UICONTROL Faturamento].\
   Para obter mais informações sobre a página de faturamento, consulte [A [!DNL Workfront Proof] [!UICONTROL Página de]](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

1. Clique no botão de conta **[!UICONTROL Novo Satélite]**. (1)

   Uma janela pop-up é exibida.

   ![Nova_Conta_Satélite.png](assets/new-satellite-account-350x156.png)

1. Insira os detalhes do cliente, incluindo todos os códigos promocionais relevantes.
1. Clique em **[!UICONTROL Salvar]**. A conta satélite aparece automaticamente no menu suspenso [!UICONTROL Contas], na parte superior da página [!UICONTROL Faturamento].
1. Selecione a nova conta Satellite no menu suspenso.
1. Continue com [Selecionando um plano para sua conta satélite](#selecting-a-plan-for-your-satellite-account) para atualizar sua conta satélite.

## Seleção de um plano para sua conta satélite {#selecting-a-plan-for-your-satellite-account}

Após configurar a conta satélite conforme descrito em [Criando uma conta satélite](#creating-a-satellite-account), é necessário atualizá-la para o plano desejado.

1. Vá para a página [!UICONTROL Faturamento].\
   Para obter mais informações sobre a página de faturamento, consulte [A [!DNL Workfront Proof] [!UICONTROL Página de]](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

1. No menu suspenso **[!UICONTROL Suas contas]**, na parte superior da página (1), escolha a conta satélite relevante.

   A página de faturamento da conta satélite é exibida e os detalhes de contato de faturamento da sua conta são replicados automaticamente.

   ![Satellite_Account_Change_Plan.png](assets/satellite-account-change-plan-350x156.png)

1. Clique no botão **[!UICONTROL Plano de alteração]** no canto superior direito da página. (2)\
   Ou\
   Abra o pop-up clicando no nome atual ou no próximo plano. (3)

1. Atualize ou faça downgrade do seu plano.

## Adicionar usuários à sua conta satélite

Depois de ter atualizado a conta satélite para o plano escolhido, é necessário adicionar usuários à conta.

1. Faça logon em [!DNL Workfront Proof] como administrador [!DNL Workfront Proof].
1. Clique em **[!UICONTROL Configurações da conta]**.
1. No menu suspenso na parte superior da página, selecione a conta Satellite relevante. (1)\
   A página de configurações da conta satélite é exibida.
1. Clique no botão **[!UICONTROL Novo usuário]** no canto superior direito da página. (2)\
   A página [!DNL New User] é exibida.

1. Insira os detalhes do usuário e clique em **[!UICONTROL Salvar]**.\
   O usuário recebe uma notificação por email dando acesso à conta.

Os usuários adicionados à conta satélite aparecem como membros na lista de contatos da conta hub.

Da mesma forma, os usuários na conta hub aparecem como membros nos contatos da conta Satellite.

Para ver uma lista completa de todos os usuários na conta satélite, clique na guia **[!UICONTROL Usuários]**.

![SA_New_User.png](assets/sa-new-user-350x156.png)

## Vinculação de contas separadas existentes à conta do hub

Se você criou anteriormente outras contas separadas para seus clientes, elas poderão ser convertidas em contas satélite.

Cuidaremos disso para você vinculando-os à sua conta do [!DNL Workfront Proof] (tornando-a uma conta central).

Tudo o que você precisa fazer é fornecer os seguintes detalhes:

* O nome e o endereço de email da conta do [!DNL Workfront Proof] que você usou para configurá-la
* Os nomes das contas separadas que você deseja vincular à sua conta e os endereços de email usados para configurar as contas separadas.
