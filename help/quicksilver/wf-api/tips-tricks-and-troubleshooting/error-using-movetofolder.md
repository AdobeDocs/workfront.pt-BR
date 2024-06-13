---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: A ação moveToFolder do documento não funciona
description: Ao usar a ação moveToFolder de documento, um erro 422 é retornado.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 86c0517443537ec5af640036c290b3a495825fdc
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# A ação moveToFolder do documento não funciona

## Problema

Ao usar a função do objeto Documento `moveToFolder` , um erro 422 é retornado.

Ou

Se estiver usando essa ação por meio do módulo do Adobe Authenticator no Workfront Fusion, o documento não será movido, mas não há nenhuma indicação do erro. O erro é o mesmo, mas o módulo Adobe Authenticator não o exibe.

## Solução

Uma possível causa de um erro 422 para essa ação é que a ação está tentando mover um Documento em uma Pasta vinculada para outra Pasta vinculada.

Verifique se o documento que você deseja mover ainda não está em uma pasta vinculada.
