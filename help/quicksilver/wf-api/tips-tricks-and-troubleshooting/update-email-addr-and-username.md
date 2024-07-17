---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: A atualização para emailAddr não atualiza o nome de usuário
description: A atualização para emailAddr não atualiza o nome de usuário
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

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
