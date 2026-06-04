---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Upload de arquivo por meio de webhooks de documentos
description: Upload de arquivo por meio de webhooks de documentos
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
TQID: https://experienceleague.adobe.com/qLRbcWkbOxvBp5Xw1aCLjGZXHMtu2k70NgOonZsZ0lk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 266
ht-degree: 11%

---

# Upload de arquivo por meio de webhooks de documentos

O upload de um arquivo para um provedor de armazenamento de documentos é um processo de duas etapas que requer dois endpoints de API separados. O Adobe Workfront inicia o processo de upload chamando /uploadInit. Esse ponto de extremidade retorna uma ID de documento que é passada para /upload ao carregar os bytes do documento. Dependendo do sistema de armazenamento de documentos subjacente, pode ser necessário criar um documento de comprimento zero e, em seguida, atualizar o conteúdo do documento posteriormente.

Adicionado à versão 1.1 desta especificação, o ID do documento e o ID da versão do documento podem ser usados para recuperar informações adicionais do Workfront.

**Exemplo:** se o sistema de gerenciamento de documentos desejar obter informações adicionais sobre o documento, o código de implementação do webhook poderá usar a ID do documento para recuperar essas informações usando a API RESTful do Workfront. Como prática recomendada, essas informações podem vir de campos de dados personalizados no documento e estão contendo tarefas, problemas ou projetos.

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
   <td>A ID da pasta pai, conforme referenciado pelo provedor do webhook.</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>O nome do documento</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>A ID do documento do Workfront (adicionada na versão 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>A ID da versão do documento do Workfront (adicionada na versão 1.1) </td> 
  </tr> 
 </tbody> 
</table>

## Resposta

Os metadados do arquivo, conforme definido pelo endpoint /metadata. Isso inclui a ID do documento usada pelo provedor.

**Exemplo:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## Método PUT

Carrega os bytes de um documento para o provedor de webhook.

**URL**

PUT/upload

## Parâmetros de consulta

| Nome  | Descrição |
|---|---|
| id  |  A ID do documento que acabou de ser criada. |


**Solicitar corpo**

Os bytes de conteúdo bruto do documento.

**Resposta**

```
{
result: "success"
}
```

ou

```
{
result: "fail"
}
```

**Exemplo**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

resposta

```
{
result:"success"
}
```
