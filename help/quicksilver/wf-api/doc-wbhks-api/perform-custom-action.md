---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Executar uma ação personalizada
description: Executar uma ação personalizada
author: Becky
feature: Workfront API
role: Developer
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 2%

---


# Executar uma ação personalizada (ainda não implementada)

Esse endpoint permite que um usuário do Adobe Workfront (ou um evento de fluxo de trabalho automatizado) execute uma ação no sistema externo. O ponto de extremidade /customAction aceita um parâmetro &quot;name&quot;, que permite que o provedor de webhook implemente várias operações personalizadas.

O provedor de webhook registra ações personalizadas com o Workfront incluindo as ações na resposta /serviceInfo em customActions. O Workfront carrega essa lista ao configurar ou atualizar o provedor de webhook em Configurar > Documentos > Integrações personalizadas.

Os usuários podem acionar a ação personalizada selecionando a seção em &quot;Ações do documento&quot;

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
   <td> <p>O identificador que especifica o tipo de ação a ser executada. Esse valor corresponde a um dos valores de customAction listados retornados pelo ponto de extremidade /serviceInfo.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>A ID do documento do Workfront para a qual a ação está sendo executada.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> O ID da versão do documento do Workfront para o qual a ação está sendo executada.</td> 
  </tr> 
 </tbody> 
</table>

 

## Resposta

Uma string JSON que indica sucesso ou falha, conforme especificado na seção Tratamento de erros abaixo. Na falha (ou seja, status = &quot;failure&quot;), o Workfront exibirá a mensagem de erro fornecida para o usuário.

**Exemplo:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

resposta

```
{
status: "success"
}
```
