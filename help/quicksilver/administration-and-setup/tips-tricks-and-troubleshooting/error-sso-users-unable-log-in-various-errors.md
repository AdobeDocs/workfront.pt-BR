---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Erro: os usuários do SSO não conseguem fazer logon em  [!DNL Adobe Workfront] devido a vários erros"
description: Ao receber um erro de logon sobre logon único federado, sua combinação de nome de usuário/senha ou seu acesso à instância  [!DNL Workfront], the problem might be that your [!DNL Workfront]  usa SSO e você está tentando fazer logon usando uma URL incorreta.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Erro: os usuários do SSO não conseguem fazer logon no [!DNL Adobe Workfront] devido a vários erros

## Problema

Não consigo fazer logon no [!DNL Workfront] e recebi um dos seguintes erros:

* Você não pode acessar [!DNL Workfront] por meio desta tela de logon. [!DNL Workfront] está configurado para Logon Único Federado com SAML 2.0. Contate o administrador do [!DNL Workfront].
* Essa combinação de senha e nome de usuário não está correta. Verifique se as maiúsculas estão desligadas e tente novamente.
* Você não tem acesso a [!DNL Workfront]. Contate o administrador do [!DNL Workfront] para obter um nome de usuário e senha.

## Solução

Sua instância [!DNL Workfront] usa SSO e você está tentando fazer logon por meio de uma URL incorreta. Verifique se você está fazendo logon usando o URL correto sem nada depois de &quot;.com&quot;

>[!TIP]
>
>Remova todos os marcadores existentes que tenham URLs inválidos.
