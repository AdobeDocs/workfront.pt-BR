---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Pesquisar via Webhooks do Documento
description: Pesquisar via Webhooks do Documento
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 4%

---

# Pesquisar via Webhooks do Documento

Retorna metadados para os arquivos e pastas retornados de uma pesquisa. Isso pode ser implementado como uma pesquisa de texto completo ou como um query de banco de dados regular. O Adobe Workfront chama o endpoint /search quando o usuário realiza uma pesquisa a partir do navegador de arquivos externo.

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
   <td>O termo de pesquisa ou frase.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(opcional) A ID da pasta da qual a pesquisa foi executada. Observação: Este é um espaço reservado para um recurso futuro no Workfront. Atualmente, o workfront não passa esse parâmetro. </p> </td> 
  </tr> 
  <tr> 
   <td>máx</td> 
   <td>O número máximo de itens a serem retornados. Usado para paginação.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> O deslocamento da página, usado em conjunto com "máx".</td> 
  </tr> 
 </tbody> 
</table>

 

## Resposta

JSON contendo uma lista de metadados para arquivos e pastas correspondentes ao query. O que constitui uma &quot;correspondência&quot; é determinado pelo provedor do webhook. Idealmente, ele deve fazer uma pesquisa de texto completo. Fazer uma pesquisa baseada em nome de arquivo também funciona.

**Exemplo:**

Exemplo:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
