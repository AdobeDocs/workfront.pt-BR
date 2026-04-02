---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formate números, moedas e valores percentuais em relatórios do modo de texto
description: Valores numéricos, incluindo moeda, podem ser configurados para exibição em vários formatos em relatórios e listas no Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 20%

---

# Formate números, moedas e valores percentuais em relatórios do modo de texto

<!-- Audited: 1/2025 -->

Valores numéricos, incluindo moeda, podem ser configurados para exibição em vários formatos em relatórios e listas no Adobe Workfront.

Para modificar o formato de um valor numérico, edite a linha **valueformat** da coluna.

Por exemplo, se você deseja exibir a coluna Budget como $1000, a linha de formato de valor seria semelhante a:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Para obter mais informações sobre como aplicar formatação condicional nos relatórios e listas do Workfront usando o modo texto, consulte [Usar formatação condicional no Modo Texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Você pode formatar números usando os seguintes valores para a linha `valueformat` da sua coluna:

| Exemplo | `valueformat=` |
|---|---|
| 1234 | `doubleAsString`<br>ou<br>`int` |
| 1.234 | `doubleAsInt` |
| R$1,234 | `currencyStringCurrencyRounded` |
| 1234,56 | `doubleAsDouble` |
| R$1,234.56 | `currencyStringCurrency` |
| 12% | `doubleAsPercentRounded` |
| 12,34% | `doubleAsPercent` |
| (1.234,56) | `doubleAsFinancial` |
| (1.234) | `doubleAsFinancialRounded` |

