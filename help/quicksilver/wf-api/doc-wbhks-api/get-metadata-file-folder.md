---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obter metadados para um arquivo ou pasta
description: Obter metadados para um arquivo ou pasta
author: Becky
feature: Workfront API
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 6%

---


# Obter metadados para um arquivo ou pasta

Retorna metadados para o arquivo ou pasta especificado.

**URL**

GET /metadata?id=[ID do documento ou da pasta]

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
   <td>id</td> 
   <td>A ID do arquivo ou pasta, conforme referenciado pelo provedor do webhook. Isso é diferente da ID de documento do Adobe Workfront. Para obter os metadados do diretório raiz, use o valor ‘/'.
   <p>Observação: O comprimento máximo da ID é de 255 caracteres.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Resposta

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Tipo </th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>String </td> 
   <td>O nome do documento ou pasta</td> 
  </tr> 
  <tr> 
   <td>tipo </td> 
   <td>String </td> 
   <td>Especifica se este item é um arquivo ou pasta ("arquivo" ou "pasta")</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>String </td> 
   <td>O ID do arquivo ou pasta.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>String </td> 
   <td> <p>O caminho do URL usado por um usuário para exibir o documento em uma janela do navegador. O URL pode ser hospedado pelo provedor de documentos ou pelo provedor de armazenamento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>String </td> 
   <td> <p>O caminho do URL usado por um usuário para baixar o documento em uma janela do navegador. O URL pode ser hospedado pelo provedor de documentos ou pelo provedor de armazenamento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>String </td> 
   <td>O tipo MIME do arquivo. (opcional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>String </td> 
   <td>Última vez que este arquivo foi modificado (carimbo de data e hora RFC 3339 formatado)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Long</td> 
   <td> O tamanho do arquivo em bytes. (opcional)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booleano</td> 
   <td> Indica se este arquivo ou pasta é somente leitura para o usuário autenticado.(opcional) </td> 
  </tr> 
 </tbody> 
</table>

**Exemplo:** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title: "My Document",<br>tipo: "ficheiro"<br>id": "12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45.251Z",<br>tamanho: "32554694"<br>}</pre>

>[!NOTE]
>
>O tratamento de erros deve ser consistente em todas as chamadas de API. Consulte a seção &quot;Tratamento de erros&quot; abaixo para obter detalhes.
