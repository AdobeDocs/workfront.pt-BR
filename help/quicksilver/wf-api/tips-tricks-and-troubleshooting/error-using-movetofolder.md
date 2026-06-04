---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: A ação moveToFolder do documento não funciona
description: Ao usar a ação moveToFolder de documento, um erro 422 é retornado.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
TQID: https://experienceleague.adobe.com/UV4VnQEs-jGJau1UqXTLnp7Ak-cmKRpjuJqxgNTF5z8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 11%

---

# A ação moveToFolder do documento não funciona

## Problema

Ao usar a ação `moveToFolder` do objeto Document, um erro 422 é retornado.

Ou

Se estiver usando essa ação por meio do módulo do Adobe Authenticator no Workfront Fusion, o documento não será movido, mas não há nenhuma indicação do erro. O erro é o mesmo, mas o módulo Adobe Authenticator não o exibe.

## Solução

Uma possível causa de um erro 422 para essa ação é que a ação está tentando mover um Documento em uma Pasta vinculada para outra Pasta vinculada.

Verifique se o documento que você deseja mover ainda não está em uma pasta vinculada.
