---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Atualizar para emailAddr não atualiza o nome de usuário
description: Atualizar para emailAddr não atualiza o nome de usuário
author: Becky
feature: Workfront API
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Atualizar para emailAddr não atualiza o nome de usuário

## Problema

Normalmente, `emailAddr` e `username` são o mesmo atributo. Portanto, se você alterar o `emailAddr` , o `username` é atualizado automaticamente para corresponder.

Quando a variável `username` não corresponde a `emailAddr`, uma atualização do `emailAddr` não atualiza o `username` automaticamente. Isso é verdadeiro para ambos `emailAddr` alterações por meio da interface do usuário e da API.

## Causa

A incompatibilidade pode ser criada de várias maneiras:

* Os usuários criados antes da regra de sincronização existia. Contas de usuário muito antigas podem não ter esses atributos sincronizados.

* Usuários criados por SSO em um momento em que o emailAddr no Workfront fazia distinção entre maiúsculas e minúsculas. A opção de provisionamento automático SSO executaria uma verificação que diferencia maiúsculas e minúsculas para usuários com base nos atributos do usuário do provedor de identidade. Quando não existia uma correspondência exata, os serviços de provisionamento automático criariam um novo usuário. Se um usuário já existia, havia um potencial de que o nome de usuário e `emailAddr` não teria o mesmo invólucro.

* Usuários que tiveram a `username` atributo atualizado diretamente pela API e seus `emailAddr` não foi atualizado. O `username` e `emailAddr` possivelmente não correspondem.

## Solução

Use a API para alterar a variável `username` deve ser igual ao `emailAddr`. Depois de sincronizar os atributos, qualquer atualização na `emailAddr` também atualizará o `username` para corresponder (quando o campo de nome de usuário não estiver incluído na atualização).
