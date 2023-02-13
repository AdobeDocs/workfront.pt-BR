---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Impedir que a ação Recalcular Finanças afete as horas históricas quando as taxas mudarem
description: Você precisa atualizar o custo por hora de um usuário ou função de cargo (devido a um aumento ou outra circunstância), mas não deseja que essa alteração afete as horas que já foram conectadas em projetos anteriormente ou que afete apenas uma parte das horas do histórico.
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Impedir que a ação Recalcular Finanças afete as horas históricas quando as taxas mudarem

## Problema

Você precisa atualizar o custo por hora de um usuário ou função de cargo (devido a um aumento ou outra circunstância), mas não deseja que essa alteração afete as horas que já foram conectadas em projetos anteriormente ou que afete apenas uma parte das horas do histórico.

## Solução

Adicione as horas que você não deseja alterar para um Registro de Faturamento no projeto e defina o status do registro de faturamento como Faturado.  Isso bloqueia a taxa antiga e será ignorado pela ação Recalcular Finanças.  Qualquer hora que não pertencer a um registro de faturamento faturado é calculada na nova taxa. Para obter mais informações, consulte [Recalcular as finanças do projeto](../../manage-work/projects/project-finances/recalculate-project-finances.md).
