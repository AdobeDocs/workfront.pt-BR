---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Logon único em  [!DNL Workfront Proof]
description: O Logon Único (SSO) permite que os usuários façam logon [!DNL Workfront Proof] usando o nome de usuário e a senha existentes da sua organização.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Logon único em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

É necessário um Plano [!UICONTROL Empresa] [!DNL Workfront] para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos do Workfront](https://business.adobe.com/products/workfront/pricing.html).

O Logon Único (SSO) permite que seus usuários façam logon no [!DNL Workfront Proof] usando o nome de usuário e a senha existentes de sua organização.

Para fornecer esse recurso, usamos o [!DNL Security Assertion Markup Language] (SAML) 2.0, um protocolo baseado em XML que permite autorizar a autenticação de dados e troca de dados entre um provedor de identidade e um serviço Web.

Isso significa que você irá autenticar em seu próprio sistema de logon, não na página de logon de [!DNL Workfront Proof].

Você deve ter subdomínios ou domínios personalizados configurados em sua conta de prova do [!DNL Workfront] para habilitar o SAML:

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Você pode ler mais sobre domínios totalmente personalizados em [Marque o [!DNL Workfront Proof] site - avançado](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Consulte [Configurar Logon Único para [!DNL Workfront Proof] usuários](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) para obter informações sobre como configurar o SSO em sua conta.
