---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Excluir um documento ou uma pasta
description: Excluir um documento ou uma pasta
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '75'
ht-degree: 8%

---


# Excluir um documento ou uma pasta (ainda não implementado)

Exclui um documento ou pasta com o ID fornecido no sistema externo. A exclusão de uma pasta também exclui o conteúdo da pasta.

## URL

PUT /delete

## Parâmetros de consulta

| Nome  | Descrição |
|---|---|
| documentId  | A ID do documento a ser excluído |
| folderId  |  A ID da pasta a ser excluída |



## Resposta

Uma string JSON que indica sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo.

### Exemplo

```
PUT https://www.example.com/api/deleteid=1234

* returns `status: "success"`

* returns `status: "failure", error: "File not found"`
```
