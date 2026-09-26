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
TQID: 'https://experienceleague.adobe.com/-LE1gxQ9aViRNuN0sI14HlZaIcLc6Mmm8XmS1zaRCFQ'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: 682536a8-4872-5ee6-a8a6-8012d713482c
    internal-label: Workfront API
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '55'
ht-degree: 45%
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
