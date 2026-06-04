---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Criar uma pasta com webhooks de documento
description: Criar uma pasta com webhooks de documento
author: Becky
feature: Workfront API
role: Developer
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
TQID: https://experienceleague.adobe.com/nneISzqXTIVje77d8QU29YPr6mOVplcwgzf48TEi-0A
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 66
ht-degree: 39%

---

# Criar uma pasta com webhooks de documento

Cria uma pasta em um determinado diretório.

## URL

POST /createFolder

## Parâmetros de consulta

| **Nome** | **Descrição** |
|---|---|
| parentId  | A ID da pasta na qual a pasta deve ser criada |
| name  | O nome da nova pasta |




**Resposta**

Os metadados da pasta recém-criada, conforme definido pelo endpoint /metadata.

## Exemplo

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

devoluções

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"",
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
