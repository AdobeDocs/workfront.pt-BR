---
title: As atribuições em um objeto excluído aparecem inesperadamente nos relatórios do destinatário
description: As atribuições em um objeto excluído aparecem inesperadamente nos relatórios do destinatário
author: Courtney
draft: Probably
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# As atribuições em um objeto excluído aparecem inesperadamente nos relatórios do destinatário

## Problema

Depois que você exclui um objeto que tem uma atribuição, tanto o objeto quanto a atribuição são excluídos. Mas a tarefa ainda pode aparecer em alguns relatórios.

Por exemplo, se você excluir uma tarefa que foi atribuída a um usuário, a atribuição ao usuário também será excluída. No entanto, se você executar posteriormente um relatório de tarefas que é filtrado por destinatário, com esse usuário especificado, o relatório ainda listará a tarefa excluída se a tarefa ainda estiver na Lixeira.

## Causa

Isso se deve às limitações arquitetônicas da Lixeira. Atualmente, não há planos no roteiro para resolver esse problema devido à escala de reformulação arquitetônica que seria necessária.
