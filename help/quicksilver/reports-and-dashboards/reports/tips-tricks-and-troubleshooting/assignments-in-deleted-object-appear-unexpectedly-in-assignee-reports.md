---
title: As atribuições em um objeto excluído aparecem inesperadamente nos relatórios do destinatário
description: As atribuições em um objeto excluído aparecem inesperadamente nos relatórios do destinatário
author: Nolan
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# As atribuições em um objeto excluído aparecem inesperadamente nos relatórios do destinatário

## Problema

Após excluir um objeto que tenha uma atribuição, tanto o objeto quanto a atribuição serão excluídos. Mas a atribuição ainda pode aparecer em alguns relatórios.

Por exemplo, se você excluir uma tarefa que foi atribuída a um usuário, a atribuição ao usuário também será excluída. No entanto, se você executar posteriormente um relatório de tarefa filtrado pelo destinatário, com esse usuário especificado, o relatório ainda listará a tarefa excluída se a tarefa ainda estiver na Lixeira.

## Causa

Isso se deve às limitações arquiteturais da Lixeira. Atualmente, não existem planos no roteiro para abordar esta questão devido à escala de reformulação arquitetônica que seria necessária.
