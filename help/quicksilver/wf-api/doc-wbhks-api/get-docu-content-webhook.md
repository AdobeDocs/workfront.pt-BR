---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obter conteúdo de documento por meio de Webhooks
description: Retorna os bytes brutos de um documento
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
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
