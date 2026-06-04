---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Pesquisar por meio de webhooks de documentos
description: Pesquisar por meio de webhooks de documentos
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
TQID: https://experienceleague.adobe.com/flRrmTOPVSGP83tVYfKG9AZOT7CNZN4IeWZNsVwcOO4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 139
ht-degree: 14%

---

# Pesquisar por meio de webhooks de documentos

Retorna metadados dos arquivos e pastas retornados de uma pesquisa. Isso pode ser implementado como uma pesquisa de texto completo ou como uma consulta de banco de dados regular. O Adobe Workfront chama o endpoint /search quando o usuário realiza uma pesquisa no navegador de arquivos externos.

## URL

GET /search

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
   <td>query</td> 
   <td>O termo ou frase de pesquisa.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(opcional) A ID da pasta da qual a pesquisa foi executada. Observação: este é um espaço reservado para um recurso futuro no Workfront. Atualmente, o Workfront não passa este parâmetro. </p> </td> 
  </tr> 
  <tr> 
   <td>max</td> 
   <td>O número máximo de itens a serem retornados. Usado para paginação.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> O deslocamento de página, usado em conjunto com "max".</td> 
  </tr> 
 </tbody> 
</table>

 

## Resposta

JSON que contém uma lista de metadados para arquivos e pastas que correspondem à consulta. O que constitui uma &quot;correspondência&quot; é determinado pelo provedor de webhook. Idealmente, ele deve fazer uma pesquisa de texto completo. Fazer uma pesquisa baseada em nome de arquivo também funciona.

**Exemplo:**

Exemplo: `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
