---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obter uma miniatura de um documento
description: Obter uma miniatura de um documento
author: Becky
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 7%

---


# Obter uma miniatura de um documento

Retorna os bytes de miniatura brutos de um documento.

**URL**

GET /miniatura

## Parâmetros de consulta

| Nome  | Descrição |
|---|---|
| id  | A ID do documento. |
| size  |  A largura da miniatura. |


## Resposta

Os bytes de miniatura brutos.

**Exemplo:**: https://www.acme.com/api/thumbnail?id=123456
