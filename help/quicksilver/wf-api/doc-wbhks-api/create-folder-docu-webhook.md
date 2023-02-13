---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Criar uma pasta com Webhooks de documento
description: Criar uma pasta com Webhooks de documento
author: John
feature: Workfront API
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 1b11a4c5f0fdf1987e9f02f7aa06ec6ec36426d3
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 7%

---


# Criar uma pasta com Webhooks de documento

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
 viewLink:"”,
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
