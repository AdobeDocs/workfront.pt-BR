---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatar números, moeda e valores de porcentagem em relatórios de modo de texto
description: Valores numéricos, incluindo moeda, podem ser configurados para exibição em vários formatos em relatórios e listas no Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 7%

---

# Formatar números, moeda e valores de porcentagem em relatórios de modo de texto

Valores numéricos, incluindo moeda, podem ser configurados para exibição em vários formatos em relatórios e listas no Adobe Workfront.

Para modificar o formato de um valor numérico, é necessário editar o **valueFormat** da sua coluna.

Por exemplo, se você quiser exibir a coluna Orçamento como $1000, a linha de formato de valor seria semelhante a:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Para obter mais informações sobre como aplicar a formatação condicional em relatórios e listas do Workfront usando o modo de texto, consulte [Usar formatação condicional no Modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

É possível formatar números usando os seguintes valores para a variável `valueformat` linha da coluna:

| Exemplo | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>ou <br><pre>int</pre> |
| 1.234 | <pre>doubleAsInt</pre> |
| R$1,234 | <pre>currencyStringCurrencyRounding</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| R$1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounds</pre> |
| 12,34% | <pre>doubleAsPercent</pre> |
| (1.234,56) | <pre>doubleAsFinancial</pre> |
| (1.234) | <pre>doubleAsFinancialRounds</pre> |
