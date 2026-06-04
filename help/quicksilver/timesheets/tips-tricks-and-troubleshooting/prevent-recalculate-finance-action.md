---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Evitar que a ação Recalcular finanças afete o histórico de horas quando as taxas forem alteradas
description: Você precisa atualizar o custo por hora de um usuário ou função de trabalho (devido a um aumento ou outra circunstância), mas não deseja que essa alteração afete as horas que foram conectadas anteriormente aos projetos, ou que ela afete apenas uma parte das horas históricas.
author: Lisa
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
TQID: https://experienceleague.adobe.com/TBeLp0FaUmlRk2uk5SdCqntrUWeAAVucox6Dyx5M0Uw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 188
ht-degree: 13%

---

# Evitar que a ação Recalcular finanças afete o histórico de horas quando as taxas forem alteradas

## Problema

Você precisa atualizar o custo por hora de um usuário ou função de trabalho (devido a um aumento ou outra circunstância), mas não deseja que essa alteração afete as horas que foram conectadas anteriormente aos projetos, ou que ela afete apenas uma parte das horas históricas.

## Solução

Adicione as horas que você não quer que sejam alteradas para um Registro de cobrança no projeto e defina o status do registro de cobrança como Faturado.  Isso bloqueia a taxa antiga e será ignorado pela ação Recalcular finanças.  Quaisquer horas que não pertençam a um registro de faturamento Faturado serão calculadas com a nova taxa. Para obter mais informações, consulte [Recalcular as finanças do projeto](../../manage-work/projects/project-finances/recalculate-project-finances.md).
