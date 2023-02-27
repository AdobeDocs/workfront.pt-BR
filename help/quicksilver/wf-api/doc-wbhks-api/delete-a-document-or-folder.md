---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Excluir um documento ou pasta
description: Excluir um documento ou pasta
author: Becky
feature: Workfront API
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 6%

---


# Excluir um documento ou pasta (ainda não implementado)

Exclui um documento ou pasta com a ID fornecida no sistema externo. A exclusão de uma pasta também exclui o conteúdo da pasta.

## URL

PUT /delete

## Parâmetros de consulta

| Nome  | Descrição |
|---|---|
| documentId  | A ID do documento a ser excluída |
| folderId  |  A ID da pasta a ser excluída |



## Resposta

Uma string JSON indicando sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo.

### Exemplo

PUT https://www.example.com/api/deleteid=1234
* devoluções `status: “success”`

* devoluções `status: “failure”, error: “File not found”`
