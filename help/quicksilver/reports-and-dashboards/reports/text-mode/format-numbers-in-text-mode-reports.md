---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatar números, valores de moeda e porcentagem em relatórios de modo de texto
description: Valores numéricos, incluindo moeda, podem ser configurados para exibição em vários formatos em relatórios e listas no Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 8de9c79f6c62b74a652482ec10bf38fada8c5fc8
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 7%

---

# Formatar números, valores de moeda e porcentagem em relatórios de modo de texto

<!-- Audited: 2/2024 -->

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
| 1234 | <pre>doubleAsString</pre> <br>ou <br><pre>int</pre> |
| 1.234 | <pre>doubleAsInt</pre> |
| R$1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234,56 | <pre>doubleAsDouble</pre> |
| R$1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12,34% | <pre>doubleAsPercent</pre> |
| (1.234,56) | <pre>doubleAsFinancial</pre> |
| (1.234) | <pre>doubleAsFinancialRounded</pre> |

