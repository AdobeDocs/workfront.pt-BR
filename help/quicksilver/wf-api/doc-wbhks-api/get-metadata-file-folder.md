---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obter metadados de um arquivo ou pasta
description: Obter metadados de um arquivo ou pasta
author: Becky
feature: Workfront API
role: Developer
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 2%

---


# Obter metadados de um arquivo ou pasta

Retorna os metadados do arquivo ou pasta especificada.

**URL**

GET /metadata?id=[ID de documento ou pasta]

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
   <td>A ID do arquivo ou pasta, conforme referenciado pelo provedor do webhook. Isso é diferente da ID de documento do Adobe Workfront. Para obter os metadados do diretório raiz, use o valor '/'.
   <p>Observação: o tamanho máximo da ID é de 255 caracteres.</p></td> 
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
   <td>título </td> 
   <td>String </td> 
   <td>O nome do documento ou pasta</td> 
  </tr> 
  <tr> 
   <td>tipo </td> 
   <td>String </td> 
   <td>Especifica se este item é um arquivo ou uma pasta ("arquivo" ou "pasta")</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>String </td> 
   <td>A ID do arquivo ou pasta.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>String </td> 
   <td> <p>O caminho de URL usado por um usuário para exibir o documento em uma janela do navegador. O URL pode ser hospedado pelo provedor de documentos ou pelo provedor de armazenamento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>String </td> 
   <td> <p>O caminho de URL usado por um usuário para baixar o documento em uma janela do navegador. O URL pode ser hospedado pelo provedor de documentos ou pelo provedor de armazenamento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>String </td> 
   <td>O tipo MIME do arquivo. (opcional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>String </td> 
   <td>Última vez que este arquivo foi modificado (carimbo de data/hora RFC 3339 formatado)</td> 
  </tr> 
  <tr> 
   <td>tamanho</td> 
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
<pre>&lbrace;<br>title:"Meu Documento",<br>kind:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45.251Z",<br>size: "32554699 "<br></pre>

>[!NOTE]
>
>O tratamento de erros deve ser consistente em todas as chamadas de API. Consulte a seção &quot;Tratamento de erros&quot; abaixo para obter detalhes.
