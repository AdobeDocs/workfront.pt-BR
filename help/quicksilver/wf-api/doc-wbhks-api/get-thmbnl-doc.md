---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obter uma miniatura de um documento
description: Obter uma miniatura de um documento
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 11%

---


# Obter uma miniatura de um documento

Retorna os bytes brutos da miniatura de um documento.

**URL**

GET /miniatura

## Parâmetros de consulta

| Nome  | Descrição |
|---|---|
| id  | A ID do documento. |
| tamanho  |  A largura da miniatura. |


## Resposta

Os bytes brutos da miniatura.

**Exemplo:**: https://www.acme.com/api/thumbnail?id=123456
