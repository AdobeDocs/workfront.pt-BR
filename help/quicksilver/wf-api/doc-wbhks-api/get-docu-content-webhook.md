---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obter conteúdo de documento por meio de Webhooks
description: Retorna os bytes brutos de um documento
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 54d1753b9062b6d4910e4478c1f072b7fedc87eb
workflow-type: tm+mt
source-wordcount: '43'
ht-degree: 13%

---

# Obter conteúdo de documento por meio de Webhooks

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

**Exemplo**:  `https://www.acme.com/api/download?id=123456`
