---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Renomear um documento ou pasta (ainda não implementado)
description: Renomear um documento ou pasta
author: John
feature: Workfront API, Digital Content and Documents
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: a62ae524f922326811423cd17d0656920b7cc9d3
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 6%

---


# Renomear um documento ou pasta (ainda não implementado)

Renomeia um documento ou uma pasta com a ID fornecida no sistema externo.

**URL**

PUT /rename

## Parâmetros de consulta

| Nome  | Descrição |
|---|---|
| id | O documento ou ID da pasta a ser renomeado |
| name  | O novo nome do documento ou pasta |


## Resposta

Uma string JSON indicando sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo.

**Exemplo:** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

devoluções

```
{status: “success”
 }returns
 {
 status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”
 }
```
