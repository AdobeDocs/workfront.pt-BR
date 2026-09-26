---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Erro: os usuários do SSO não conseguem fazer logon no [!DNL Adobe Workfront] devido a vários erros'
description: Quando você recebe um erro de logon sobre logon único federado, sua combinação de nome de usuário/senha ou seu acesso ao [!DNL Workfront], o problema pode ser que a instância do [!DNL Workfront] use SSO e você esteja tentando fazer logon usando uma URL incorreta.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
TQID: 'https://experienceleague.adobe.com/8L78zoOjC2KgtVKTorhvWDd8MvaficRL2pZKOfrlGSs'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 4%
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
