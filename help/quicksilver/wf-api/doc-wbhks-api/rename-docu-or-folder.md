---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Renomear um documento ou uma pasta (ainda não implementado)
description: Renomear um documento ou uma pasta
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
TQID: https://experienceleague.adobe.com/-HmJkcMckTK6upblNcqX5LZkdYQxoWPDeuHkFjJarh4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 81
ht-degree: 29%

---

# Renomear um documento ou uma pasta (ainda não implementado)

Renomeia um documento ou uma pasta com o ID fornecido no sistema externo.

**URL**

PUT /rename

## Parâmetros de consulta

| Nome  | Descrição |
|---|---|
| id | A ID do documento ou da pasta a ser renomeada |
| name  | O novo nome do documento ou pasta |


## Resposta

Uma string JSON que indica sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo.

**Exemplo:** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

devoluções

```
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```
