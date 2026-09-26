---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatar datas em relatórios do modo texto
description: As datas podem ser configuradas para serem exibidas em vários formatos em relatórios e listas no Adobe Workfront. Para estabelecer um formato de data, você deve modificar a linha valueformat do código do modo de texto na coluna.
author: Courtney
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/-8gB8XDwLQTBCUsrex-PIAyxcF-rSPsoM2Gvw2EhTaU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 9%
---
# Formatar datas em relatórios do modo texto

<!-- Audited: 1/2025 -->

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

Você pode formatar datas usando os seguintes `valueformat` valores do modo de texto:

| **Formato** | Exemplo  | ***valueformat=*** |
|---|---|---|
| DD/MM/AA | 10/11/18 | `atDate` |
| Hora MM/DD/AA | 11/10/18 12h | `longAtDate` |
| DD/MM/AA | 10/11/18 | `shortAtDate` |
| Mês, DD, ANO | 11 de outubro de 2018 | `mediumAtDate` |
| DW, Mês, Dia, YR | Seg, 11 de outubro de 2018 | `partialAtDate` |
| Hora DW, Mês, Dia, Ano | Seg, outubro, 11, 2018 12:00 pm | `fullAtDate` |
