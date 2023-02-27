---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Executar uma ação personalizada
description: Executar uma ação personalizada
author: Becky
feature: Workfront API
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 3%

---


# Executar uma ação personalizada (ainda não implementada)

Esse terminal permite que um usuário do Adobe Workfront (ou um evento de workflow automatizado) execute uma ação no sistema externo. O endpoint /customAction aceita um parâmetro &quot;name&quot;, que permite ao provedor do webhook implementar várias operações personalizadas.

O provedor webhook registra ações personalizadas no Workfront, ao incluir as ações na resposta /serviceInfo em customActions. O Workfront carrega essa lista ao configurar ou atualizar o provedor do webhook em Configurar > Documentos > Integrações personalizadas.

Os usuários podem acionar a ação personalizada selecionando a seção &quot;Ações do documento&quot;

**URL**

GET /customAction

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
   <td> <p>name</p> </td> 
   <td> <p>O identificador que especifica o tipo de ação a ser executada. Esse valor corresponde a um dos valores customAction listados retornados pelo endpoint /serviceInfo.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>A ID do documento da frente de trabalho para a qual a ação está sendo executada.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> A ID da versão do documento da frente de trabalho para a qual a ação está sendo executada.</td> 
  </tr> 
 </tbody> 
</table>

 

## Resposta

Uma string JSON indicando sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo. Em caso de falha (ou seja, status = &quot;falha&quot;), o Workfront exibirá a mensagem de erro fornecida ao usuário.

**Exemplo:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

response

```
{
status: “success”
}
```
