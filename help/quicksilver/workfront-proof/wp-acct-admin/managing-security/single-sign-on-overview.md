---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Logon único [!DNL Workfront Proof]
description: Logon único (SSO) permite que seus usuários façam logon [!DNL Workfront Proof] usando o nome de usuário e a senha existentes em sua organização.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Logon único [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Um [!UICONTROL Empresa] [!DNL Workfront] O plano é necessário para usar esse recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos da Workfront](https://www.workfront.com/plans).

Logon único (SSO) permite que seus usuários façam logon [!DNL Workfront Proof] usando o nome de usuário e a senha existentes em sua organização.

Para fornecer esse recurso, usamos [!DNL Security Assertion Markup Language] (SAML) 2.0, um protocolo baseado em XML que permite autorizar a autenticação de dados e troca entre um provedor de identidade e um serviço da Web.

Isso significa que você se autenticará em seu próprio sistema de logon, não contra [!DNL Workfront Proof]Página de logon do .

Você deve ter subdomínios ou domínios personalizados configurados no [!DNL Workfront] Conta de prova para ativar o SAML:

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Você pode ler mais sobre domínios totalmente personalizados no  [Marca [!DNL Workfront Proof] site - avançado](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Consulte [Configurar logon único para [!DNL Workfront Proof] usuários](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) para obter informações sobre como configurar o SSO em sua conta.
