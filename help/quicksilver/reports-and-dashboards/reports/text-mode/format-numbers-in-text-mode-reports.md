---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatar números, valores de moeda e porcentagem em relatórios de modo de texto
description: Valores numéricos, incluindo moeda, podem ser configurados para exibição em vários formatos em relatórios e listas no Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Formatar números, valores de moeda e porcentagem em relatórios de modo de texto

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

