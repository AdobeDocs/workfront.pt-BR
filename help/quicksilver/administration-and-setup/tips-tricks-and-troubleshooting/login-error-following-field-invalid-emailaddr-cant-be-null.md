---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Erro de logon: os seguintes campos são inválidos: emailAddr não pode ser nulo'
description: Quando tento fazer logon [!DNL Adobe Workfront] no URL do meu domínio, sou redirecionado para o portal de logon SAML e redirecionado para [!DNL Workfront] com um erro informando que o campo emailAddr não pode ser nulo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
TQID: https://experienceleague.adobe.com/MfWVOYcQAVjlbxwiqVaPwipyq5ulv0toajH-2tX7c9k
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 4%

---

# Erro de logon: os seguintes campos são inválidos: emailAddr não pode ser nulo

## Problema

Quando tento fazer logon no [!DNL Adobe Workfront] com minha URL (https://customerdomain.my.workfront.com), sou redirecionado para o portal de logon SAML e redirecionado para [!DNL Workfront] com o seguinte erro:

“Vamos tentar novamente. Os seguintes campos são inválidos: emailAddr não pode ser nulo.&quot;

## Causa

Esse erro é causado por um item incorreto na área Mapear atributos do usuário da configuração SAML 2.0. Para obter mais informações sobre como mapear atributos de usuário para SAML 2.0, consulte [Configurar o Adobe Workfront com SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Solução

Atualize o Mapeamento de Atributos para o endereço de email e clique em **[!UICONTROL Salvar]**.
