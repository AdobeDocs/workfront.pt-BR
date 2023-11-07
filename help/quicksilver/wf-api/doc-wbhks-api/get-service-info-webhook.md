---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obter informações sobre o serviço
description: Obter informações sobre o serviço
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 4%

---


# Obter informações sobre o serviço (ainda não implementado)

>[!NOTE]
>
>A data de lançamento desse recurso ainda não foi determinada.

Retorna informações sobre o serviço, como recursos e funcionalidades. O Adobe Workfront usará essas informações para personalizar a interface do usuário no Workfront. Por exemplo, se a implementação de webhook contiver algumas ações personalizadas, o JSON deverá listar essas operações no JSON. Os usuários poderão então invocar essas ações a partir do Workfront.

**URL**

GET /serviceInfo

## Parâmetros de consulta

Nenhum. Além disso, as chamadas para esse endpoint não devem exigir autenticação.

## Resposta

JSON contendo informações sobre este serviço

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome</th> 
   <th>Tipo </th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>String </td> 
   <td>A versão de webhook implementada por este serviço. Esse é o número da versão listado na parte superior desta especificação.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>String </td> 
   <td>O número da versão interna deste serviço. Esse número é determinado pelo provedor de serviços de webhook e é usado apenas para fins informativos.<br><br></td> 
  </tr> 
  <tr> 
   <td>editor </td> 
   <td>String </td> 
   <td>O nome da empresa que fornece a implementação do webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>String </td> 
   <td>Uma lista contendo os endpoints de API implementados por este serviço. Isso pode ser usado para garantir que a interface do usuário no Workfront reflita os recursos oferecidos pelo provedor de webhook. Cada item na lista deve incluir o nome do endpoint (como "pesquisa").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>String</td> 
   <td>  <p>Uma lista contendo as operações personalizadas implementadas por este webhook. Cada item da lista inclui um nome e um nome de exibição. O nome de exibição aparecerá na lista suspensa "Ações do documento" no Workfront. Clicar no item na lista suspensa chamará a ação no webhook, chamando o ponto de extremidade /customAction.</p></td> 
  </tr> 
 </tbody> 
</table>

**Exemplo:** `https://www.acme.com/api/serviceInfo`

devoluções

```
{
webhook version: "1.2", version: "1.0", publisher: "Acme, LLC", availableEndpoints: ["files", "metadata", "search", "download"
"thumbnail", "uploadInit", "upload" ], customActions [
{
name: "archive", displayName: "Archive" 
}, 
{name: "doSomethingElse", displayName: "Do Something" }, 
] 
}
```
