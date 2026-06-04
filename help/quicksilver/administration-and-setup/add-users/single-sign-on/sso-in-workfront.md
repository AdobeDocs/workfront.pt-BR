---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Visão geral do logon único no Adobe Workfront
description: A Workfront fornece uma configuração de logon único (SSO) gerenciada centralmente que integra facilmente o Workfront à sua solução corporativa de SSO existente. Essa configuração é fácil de definir e gerenciar e está disponível para clientes OnDemand e OnPremise Enterprise.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
TQID: https://experienceleague.adobe.com/3Eti-Ucz19uff3H03Go6JuU5hhiTstjg4dbWPLMDl3s
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 251
ht-degree: 0%

---

# Visão geral do logon único no Adobe Workfront

<!--Audited: 12/2023-->

{{important-admin-console-onboard}}


A Workfront fornece uma configuração de logon único (SSO) gerenciada centralmente que integra o Workfront à sua solução corporativa de SSO existente. Essa configuração está disponível para clientes OnDemand e OnPremise Enterprise.

Para usar a funcionalidade SSO no Workfront, sua organização precisa configurar um aplicativo SSO. Em seguida, você pode configurar o Workfront para que ele possa se comunicar com sua solução de SSO.

As Federated Solutions permitem que os usuários façam logon em todos os aplicativos inserindo seu nome de usuário e senha em um portal de logon centralizado.

![SSO federado](assets/overview-sso-wf-fed-only.png)


## Configurar o firewall

Ao usar uma solução SSO, o Workfront inicia uma conexão com o servidor na porta especificada.

Se o firewall ou o servidor de e-mail estiver configurado para permitir o acesso somente a fornecedores específicos, você deve adicionar determinados endereços IP Workfront ao incluo na lista de permissões de firewall. Para obter mais informações, consulte [Configurar incluo na lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurar Logon Único

O Workfront integra-se com as seguintes soluções de SSO:

* Soluções agrupadas compatíveis com SAML 2.0

  Para obter informações sobre como integrar o Workfront com SAML 2.0, consulte [Configurar o Adobe Workfront com SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Soluções agrupadas que oferecem suporte ao SAML 2.0 usando ADFS

  Para obter informações sobre como integrar o Workfront com SAML 2.0 usando ADFS, consulte [Configurar o Adobe Workfront com SAML 2.0 usando ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
