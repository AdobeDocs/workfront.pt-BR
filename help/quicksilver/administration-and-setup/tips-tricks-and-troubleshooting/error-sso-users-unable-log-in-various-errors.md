---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Erro: Os Usuários do SSO não podem fazer logon no [!DNL Adobe Workfront] Devido a vários erros'
description: Quando você recebe um erro de logon sobre o logon único federado, sua combinação de nome de usuário/senha ou seu acesso ao [!DNL Workfront], the problem might be that your [!DNL Workfront] A instância usa SSO e você está tentando fazer logon usando um URL incorreto. Certifique-se de fazer logon usando o URL correto sem nada depois de ".com".
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 13%

---

# Erro: Os Usuários do SSO não podem fazer logon no [!DNL Adobe Workfront] Devido a vários erros

## Problema

Não consigo fazer logon no [!DNL Workfront] e receberam um dos seguintes erros:

* Você não pode acessar [!DNL Workfront] por esta tela de logon. [!DNL Workfront] O está configurado para Federated Single Sign-On com SAML 2.0. Entre em contato com seu [!DNL Workfront] administrador.
* Combinação inválida de usuário/senha
* Lamento, você não tem acesso ao [!DNL Workfront]. Entre em contato com seu [!DNL Workfront] administrador para obter um nome de usuário e senha.

## Solução

Seu [!DNL Workfront] A instância usa SSO e você está tentando fazer logon por meio de um URL incorreto. Certifique-se de fazer logon usando o URL correto sem nada depois de &quot;.com&quot;

>[!TIP]
>
>Remova todos os marcadores existentes que tenham URLs inválidos.
