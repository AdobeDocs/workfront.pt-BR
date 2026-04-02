---
title: As atribuições em um objeto excluído aparecem inesperadamente nos relatórios de responsáveis
description: As atribuições em um objeto excluído aparecem inesperadamente nos relatórios de responsáveis
author: Courtney
draft: Probably
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
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
