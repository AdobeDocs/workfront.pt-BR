---
title: As atribuições em um objeto excluído aparecem inesperadamente nos relatórios de responsáveis
description: As atribuições em um objeto excluído aparecem inesperadamente nos relatórios de responsáveis
author: Nolan
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
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
