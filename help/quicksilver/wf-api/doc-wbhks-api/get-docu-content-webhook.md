---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obter conteúdo de documento via Webhooks
description: Retorna os bytes brutos de um documento
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '53'
ht-degree: 7%

---

# Obter conteúdo de documento via Webhooks

Retorna os bytes brutos de um documento

## URL

GET /download

## Parâmetros de consulta

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> A ID do documento.</td> 
  </tr> 
 </tbody> 
</table>

## Resposta

Os bytes brutos do documento.

**Exemplo:**:  [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
