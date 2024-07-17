---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Evite que a ação Recalcular Finanças afete horas de histórico quando as taxas forem alteradas
description: Você precisa atualizar o custo por hora de um usuário ou função de trabalho (devido a um aumento ou outra circunstância), mas não deseja que essa alteração afete as horas que foram conectadas anteriormente aos projetos, ou que ela afete apenas uma parte das horas históricas.
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Evite que a ação Recalcular Finanças afete horas de histórico quando as taxas forem alteradas

## Problema

Você precisa atualizar o custo por hora de um usuário ou função de trabalho (devido a um aumento ou outra circunstância), mas não deseja que essa alteração afete as horas que foram conectadas anteriormente aos projetos, ou que ela afete apenas uma parte das horas históricas.

## Solução

Adicione as horas que você não quer que sejam alteradas para um Registro de cobrança no projeto e defina o status do registro de cobrança como Faturado.  Isso bloqueia a taxa antiga e será ignorado pela ação Recalcular finanças.  Quaisquer horas que não pertençam a um registro de faturamento Faturado serão calculadas com a nova taxa. Para obter mais informações, consulte [Recalcular as finanças do projeto](../../manage-work/projects/project-finances/recalculate-project-finances.md).
