---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obter informações sobre o serviço
description: Obter informações sobre o serviço
author: John
feature: Workfront API
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 3%

---


# Obter informações sobre o serviço (ainda não implementado)

>[!NOTE]
>
>A data de lançamento desse recurso ainda não foi determinada.

Retorna informações sobre o serviço, como recursos e recursos. A Adobe Workfront usará essas informações para personalizar a interface do usuário no Workfront. Por exemplo, se a implementação do webhook contiver algumas ações personalizadas, o JSON deverá listar essas operações no JSON. Os usuários seriam capazes de invocar essas ações do Workfront.

**URL**

GET /serviceInfo

## Parâmetros de consulta

Nenhum. Além disso, as chamadas para esse endpoint não devem exigir autenticação.

## Resposta

JSON contendo informações sobre esse serviço

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
   <td>A versão do webhook implementada por este serviço. Este é o número de versão listado na parte superior desta especificação.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>String </td> 
   <td>O número de versão interno deste serviço. Esse número é determinado pelo provedor de serviços do webhook e é usado somente para fins informativos.<br><br></td> 
  </tr> 
  <tr> 
   <td>editor </td> 
   <td>String </td> 
   <td>O nome da empresa que fornece a implementação do webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>String </td> 
   <td>Uma lista que contém os Endpoints de API implementados por esse serviço. Isso pode ser usado para garantir que a interface do usuário no Workfront reflita os recursos oferecidos pelo provedor do webhook. Cada item na lista deve incluir o nome do ponto de extremidade (como "pesquisa").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>String</td> 
   <td>  <p>Uma lista contendo as operações personalizadas implementadas por este webhook. Cada item de lista inclui um nome e um nome de exibição. O nome de exibição será exibido na lista suspensa "Ações do documento" no Workfront. Clicar no item na lista suspensa chamará a ação no webhook chamando o endpoint /customAction .</p></td> 
  </tr> 
 </tbody> 
</table>

**Exemplo:** `https://www.acme.com/api/serviceInfo`

devoluções

```
{
webhook version: “1.2”, version: “1.0”, publisher: “Acme, LLC”, availableEndpoints: [“files”, “metadata”, “search”, “download”
“thumbnail”, “uploadInit”, “upload” ], customActions [
{
name: “archive”, displayName: “Archive” 
}, 
{name: “doSomethingElse”, displayName: “Do Something” }, 
] 
}
```
