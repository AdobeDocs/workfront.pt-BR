---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatar datas em relatórios de modo de texto
description: As datas podem ser configuradas para serem exibidas em vários formatos em relatórios e listas no Adobe Workfront. Para estabelecer um formato de data, você deve modificar a linha de formato de valor do código do modo de texto na coluna .
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 2%

---

# Formatar datas em relatórios de modo de texto

As datas podem ser configuradas para serem exibidas em vários formatos em relatórios e listas no Adobe Workfront. Para estabelecer um formato de data, é necessário modificar a variável `valueformat` linha do código do modo de texto na coluna .

`valueformat= [new date format]` Por exemplo, se você quisesse que a Data de conclusão projetada fosse exibida como MM/DD/YY, o código seria semelhante a:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Se quiser mostrar a Data de Conclusão Planejada como *Mth, DD, Year*, o código seria semelhante a:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Para obter mais informações sobre como aplicar a formatação condicional em relatórios e listas do Workfront usando o modo de texto, consulte [Usar formatação condicional no Modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Você pode formatar datas usando o seguinte

```
valueformat
```

 valores do modo de texto:

| **Formatar** | Exemplo  | ***valueformat=*** |
|---|---|---|
| DD/MM/YY | 10/11/18 | `atDate` |
| MM/DD/YY Hora | 11/10/18 12:00 PM | `longAtDate` |
| DD/MM/YY | 10/11/18 | `shortAtDate` |
| Mth, DD, YR | 11 de outubro de 2018 | `mediumAtDate` |
| DW, Mth, Day, YR | Seg, 11 de outubro de 2018 | `partialAtDate` |
| DW, Mth, Day, YR Time | Seg, 11 de outubro de 2018 12:00 | `fullAtDate` |
