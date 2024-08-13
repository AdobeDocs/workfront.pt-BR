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
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Visão geral do logon único no Adobe Workfront

<!--Audited: 12/2023-->

{{important-admin-console-onboard}}


A Workfront fornece uma configuração de logon único (SSO) gerenciada centralmente que integra o Workfront à sua solução corporativa de SSO existente. Essa configuração está disponível para clientes OnDemand e OnPremise Enterprise.

Para usar a funcionalidade SSO no Workfront, sua organização precisa configurar um aplicativo SSO. Em seguida, você pode configurar o Workfront para que ele possa se comunicar com sua solução de SSO.

As Federated Solutions permitem que os usuários façam logon em todos os aplicativos inserindo seu nome de usuário e senha em um portal de logon centralizado.

![](assets/overview-sso-wf-fed-only.png)


## Configurar o firewall

Ao usar uma solução SSO, o Workfront inicia uma conexão com o servidor na porta especificada.

Se o firewall ou o servidor de e-mail estiver configurado para permitir o acesso somente a fornecedores específicos, você deverá adicionar determinados endereços IP Workfront ao seu arquivo de inclui na lista de permissões do firewall. Incluir na lista de permissões Para obter mais informações, consulte [Configurar o arquivo do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurar Logon Único

O Workfront integra-se com as seguintes soluções de SSO:

* Soluções agrupadas compatíveis com SAML 2.0

  Para obter informações sobre como integrar o Workfront com SAML 2.0, consulte [Configurar o Adobe Workfront com SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Soluções agrupadas que oferecem suporte ao SAML 2.0 usando ADFS

  Para obter informações sobre como integrar o Workfront com SAML 2.0 usando ADFS, consulte [Configurar o Adobe Workfront com SAML 2.0 usando ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
