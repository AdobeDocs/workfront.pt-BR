---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: A atualização para emailAddr não atualiza o nome de usuário
description: A atualização para emailAddr não atualiza o nome de usuário
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
TQID: https://experienceleague.adobe.com/dkceJuJ6WfaZTnbD6zdP6TsHR5bvkERD-EiBgVmrCck
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 7%

---

# A atualização para emailAddr não atualiza o nome de usuário

## Problema

Normalmente, `emailAddr` e `username` são o mesmo atributo. Portanto, se você alterar o atributo `emailAddr` de um usuário, o atributo `username` será atualizado automaticamente para corresponder a.

Quando o `username` não corresponde ao `emailAddr`, uma atualização do `emailAddr` não atualiza o `username` automaticamente. Isso é verdadeiro para as alterações de `emailAddr` por meio da interface do usuário e da API.

## Causa

A incompatibilidade pode ser criada de várias maneiras:

* Usuários criados antes da regra de sincronização. Contas de usuário muito antigas podem não ter esses atributos em sincronia.

* Os usuários criados por SSO em um momento em que o emailAddr no Workfront diferenciava maiúsculas de minúsculas. A opção de provisionamento automático de SSO executaria uma verificação que diferencia maiúsculas e minúsculas para usuários com base nos atributos do usuário do provedor de identidade. Quando não havia uma correspondência exata, os serviços de provisionamento automático criavam um novo usuário. Se um usuário já existisse, havia uma possibilidade de que seu nome de usuário e `emailAddr` não tivessem a mesma capitalização.

* Os usuários que tiveram o atributo `username` atualizado diretamente por meio da API, e seus `emailAddr` não foram atualizados. `username` e `emailAddr` possivelmente não correspondem.

## Solução

Use a API para alterar o atributo `username` para ser o mesmo que `emailAddr`. Após sincronizar os atributos, qualquer atualização no `emailAddr` também atualizará o `username` para corresponder (quando o campo de nome de usuário não estiver incluído na atualização).
