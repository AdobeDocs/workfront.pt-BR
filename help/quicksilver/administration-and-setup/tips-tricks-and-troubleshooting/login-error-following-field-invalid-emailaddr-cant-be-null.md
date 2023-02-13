---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Erro de logon: Os seguintes campos são inválidos: emailAddr não pode ser nulo'
description: Quando eu tento fazer login [!DNL Adobe Workfront] o URL do meu domínio, sou redirecionado para o portal de login SAML e redirecionado para [!DNL Workfront] com um erro informando que o campo emailAddr não pode ser nulo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%

---

# Erro de logon: Os seguintes campos são inválidos: emailAddr não pode ser nulo

## Problema

Quando eu tento fazer login [!DNL Adobe Workfront] com meu URL (https://customerdomain.my.workfront.com), sou redirecionado para o portal de login SAML e redirecionado para [!DNL Workfront] com o seguinte erro:

“Vamos tentar novamente. Os seguintes campos são inválidos: emailAddr não pode ser nulo.&quot;

## Causa

Esse erro é causado por um item incorreto na área Mapear atributos de usuário da configuração SAML 2.0. Para obter mais informações sobre o mapeamento de atributos do usuário para SAML 2.0, consulte [Configurar o Adobe Workfront com o SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Solução

Atualize o Mapeamento de atributos para o endereço de email e clique em **[!UICONTROL Salvar]**.
