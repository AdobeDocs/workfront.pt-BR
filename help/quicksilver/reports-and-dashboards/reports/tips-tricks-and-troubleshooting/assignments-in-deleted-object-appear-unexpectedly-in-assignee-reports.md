---
title: As atribuições em um objeto excluído aparecem inesperadamente nos relatórios de responsáveis
description: As atribuições em um objeto excluído aparecem inesperadamente nos relatórios de responsáveis
author: Courtney
draft: Probably
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%
---
# As atribuições em um objeto excluído aparecem inesperadamente nos relatórios de responsáveis

## Problema

Depois de excluir um objeto que tem uma atribuição, o objeto e a atribuição são excluídos. Mas a tarefa ainda pode aparecer em alguns relatórios.

Por exemplo, se você excluir uma tarefa atribuída a um usuário, a atribuição ao usuário também será excluída. No entanto, se posteriormente você executar um relatório de tarefa que é filtrado pelo destinatário, com esse usuário especificado, o relatório ainda listará a tarefa excluída se a tarefa ainda estiver na Lixeira.

## Causa

Isso se deve às limitações de arquitetura da Lixeira. Atualmente, não há planos no roteiro para abordar esse problema devido à escala de reformulação arquitetônica que seria necessária.
