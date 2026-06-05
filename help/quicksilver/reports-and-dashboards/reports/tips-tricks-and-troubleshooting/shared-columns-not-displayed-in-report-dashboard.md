---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Dados de colunas compartilhadas não são exibidos em relatórios de painel
description: Os dados de colunas compartilhadas não são exibidos quando o relatório é colocado em um layout de painel de várias colunas, mas são exibidos em um layout de coluna única. Quebras de linha também são substituídas.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OEFlwkdPf98g4-rC1tzaTmmEwb5-BXHx-j8XGrRR8sE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 12%

---

# Dados de colunas compartilhadas não são exibidos em relatórios de painel

## Problema

Os dados de colunas compartilhadas não são exibidos quando o relatório é colocado em um layout de painel de várias colunas, mas são exibidos em um layout de coluna única. Quebras de linha também são substituídas.

## Causa

Somente colunas marcadas como

```
shortview=true
```

são incluídos na visualização de painel do relatório quando o layout do painel tem a divisão esquerda/direita ou a divisão esquerda/meio/direita configurada.

## Solução

Acesse a visualização usada no relatório e abra o modo de texto. (Para obter mais informações, consulte [Editar um modo de exibição usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Rotular todas as colunas no relatório, incluindo as colunas usadas em uma coluna compartilhada/mesclada, com

```
shortview=true
```

. As colunas do relatório serão exibidas corretamente no painel.
