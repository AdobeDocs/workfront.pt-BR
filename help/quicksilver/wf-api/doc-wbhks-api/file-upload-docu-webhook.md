---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Upload de arquivo via Webhooks de documento
description: Upload de arquivo via Webhooks de documento
author: John
feature: Workfront API
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: b117eb11e4e9325e6249687448d3de98a11e5e00
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 3%

---


# Upload de arquivo via Webhooks de documento

O upload de um arquivo para um provedor de armazenamento de documentos é um processo de duas etapas que requer dois pontos de extremidade de API separados. O Adobe Workfront inicia o processo de upload chamando /uploadInit . Esse ponto de extremidade retorna uma ID de documento que é passada para /upload ao carregar os bytes do documento. Dependendo do sistema de armazenamento de documentos subjacente, pode ser necessário criar um documento de comprimento zero e, em seguida, atualizar o conteúdo do documento posteriormente.

Adicionada à versão 1.1 desta especificação, a ID do documento e a ID da versão do documento podem ser usadas para recuperar informações adicionais do Workfront.

**Exemplo:** Se o sistema de gerenciamento de documentos quiser informações adicionais sobre o documento, o código de implementação do webhook poderá usar a ID do documento para recuperar essas informações usando a API RESTful do Workfront. Como uma boa prática, essas informações podem vir de campos de dados personalizados no documento e estão contendo tarefa, problema ou projeto.

## Método POST

**URL**

POST /uploadInit

### Parâmetros de consulta

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
   <td>parentId </td> 
   <td>A ID da pasta principal, conforme referenciado pelo provedor do webhook.</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>O nome do documento</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>A ID de documento do Workfront (adicionada na versão 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>A ID da versão do documento do Workfront (adicionada na versão 1.1) </td> 
  </tr> 
 </tbody> 
</table>

## Resposta

Os metadados do arquivo, conforme definido pelo endpoint /metadata. Isso inclui a ID de documento usada pelo provedor.

**Exemplo:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## Método PUT

Carrega os bytes de um documento para o provedor do webhook.

**URL**

PUT /upload

## Parâmetros de consulta

| Nome  | Descrição |
|---|---|
| id  |  A ID do documento, que acabou de ser criada. |


**Corpo da solicitação**

Os bytes de conteúdo bruto do documento.

**Resposta**

```
{
result: “success”
}
```

ou

```
{
result: “fail”
}
```

**Exemplo**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

response

```
{
result:"success"
}
```
