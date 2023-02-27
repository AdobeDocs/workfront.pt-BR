---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Lista metadados para arquivos ou pastas
description: Lista metadados para arquivos ou pastas
author: Becky
feature: Workfront API
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 5%

---


# Obter lista de itens do conteúdo da pasta

Lista metadados para os arquivos e pastas de uma determinada pasta.

**URL**

GET /files

## Parâmetros de consulta

| Nome  | Descrição |
|---|---|
| parentId  | A ID da pasta. Para obter os metadados do diretório raiz, use o valor ‘/&#39;. |
| máx  | O número máximo de itens a serem retornados. Usado para paginação. |
| offset  |  O deslocamento da página, usado em conjunto com &quot;máx&quot;. |


## Resposta

JSON contendo uma lista de arquivos e pastas. Os metadados de cada item são os mesmos retornados pelo endpoint /metadata.

**Exemplo:** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ”,
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ”,
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
