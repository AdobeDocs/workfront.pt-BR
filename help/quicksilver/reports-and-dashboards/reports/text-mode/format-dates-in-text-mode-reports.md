---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatar datas em relatórios do modo texto
description: As datas podem ser configuradas para serem exibidas em vários formatos em relatórios e listas no Adobe Workfront. Para estabelecer um formato de data, você deve modificar a linha valueformat do código do modo de texto na coluna.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Formatar datas em relatórios do modo texto

As datas podem ser configuradas para serem exibidas em vários formatos em relatórios e listas no Adobe Workfront. Para estabelecer um formato de data, você deve modificar a linha `valueformat` do código do modo de texto na coluna.

`valueformat= [new date format]` Por exemplo, se você quisesse que a Data de Conclusão Projetada fosse exibida como MM/DD/AA, o código seria semelhante a:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Se você quiser exibir a Data de conclusão planejada como *Mês, DD, Ano*, o código terá esta aparência:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Para obter mais informações sobre como aplicar formatação condicional nos relatórios e listas do Workfront usando o modo texto, consulte [Usar formatação condicional no Modo Texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

É possível formatar datas usando o seguinte

```
valueformat
```

 valores do modo texto:

| **Formato** | Exemplo  | ***valueformat=*** |
|---|---|---|
| DD/MM/AA | 11/10/18 | `atDate` |
| Hora MM/DD/AA | 11/10/18 12h | `longAtDate` |
| DD/MM/AA | 11/10/18 | `shortAtDate` |
| Mês, DD, ANO | 11 de outubro de 2018 | `mediumAtDate` |
| DW, Mês, Dia, YR | Seg, 11 de outubro de 2018 | `partialAtDate` |
| Hora DW, Mês, Dia, Ano | Seg, outubro, 11, 2018 12:00 pm | `fullAtDate` |
