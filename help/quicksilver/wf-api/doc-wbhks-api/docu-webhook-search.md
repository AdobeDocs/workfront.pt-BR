---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Pesquisar por webhooks de documentos
description: Pesquisar por webhooks de documentos
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 5%

---

# Pesquisar por webhooks de documentos

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
   <td>máx</td> 
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

Exemplo:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
