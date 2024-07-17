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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 5%

---


# Excluir um documento ou uma pasta (Ainda não implementado)

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

PUT https://www.example.com/api/delete­­­­­­­­­­­­­­­­­­­­­­­­­­­­­id=1234
* retorna `status: "success"`

* retorna `status: "failure", error: "File not found"`
