---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular o valor líquido
description: O Valor Líquido de um projeto é o valor total esperado do projeto após calcular seu benefício e remover os custos.
author: Lisa
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
TQID: https://experienceleague.adobe.com/Bj8-Lz2cRE0HeMF7xGryTucaqddQW25DzyPpbzWQR94
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 402
ht-degree: 6%

---

# Calcular o valor líquido

O Valor Líquido de um projeto é o valor total esperado do projeto após calcular seu benefício e remover os custos.

## Visão geral do Valor Líquido do projeto

O Adobe Workfront calcula o Valor líquido de um projeto usando a seguinte fórmula:

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

Os seguintes campos podem afetar o Valor líquido de um projeto:

* **Benefício Planejado**: esta é uma entrada manual especificada pelo Proprietário do Projeto ao concluir a área **Informações do Projeto** do Business Case.\
  Para obter mais informações sobre o Benefício Planejado de um projeto, consulte a seção [Informações do Projeto](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) no artigo [Visão Geral das Áreas do Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Custo orçado**: este é o custo total associado ao projeto conforme estimado quando você inicia o projeto pela primeira vez.

  O **Custo Orçado** usa o valor de **Custo Orçado do Trabalho**, que é calculado na área Orçamento de Recursos do Business Case, e leva em conta as horas orçadas para suas funções de trabalho no Planejador de Recursos e a taxa de Custo por Hora de cada função de trabalho.\
  O custo orçado afeta o **valor líquido** do projeto. Para obter mais informações sobre como o Custo Orçado é calculado, consulte [Calcular Custo Orçado](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Custo de Risco Potencial**: este é o custo associado a qualquer risco no projeto, conforme definido no Business Case ou na guia Riscos do projeto.\
  Para obter mais informações sobre como calcular o Custo de Risco Potencial de um projeto, consulte o artigo [Calcular Custo de Risco Potencial](../../../manage-work/projects/project-finances/potential-risk-cost.md).



## Localizar o Valor Líquido do projeto

Você pode encontrar o Valor líquido de um projeto nas seguintes áreas no Workfront:

* Na área Resumo de business case do business case\
  Para obter mais informações sobre a área Resumo de Business Case, consulte a seção &quot;Noções básicas sobre o Resumo de Business Case&quot; no artigo [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

  ![Valor líquido no business case](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* No Portfolio Otimizer, se o projeto estiver associado a um portfólio

  >[!TIP]
  >
  >O total de todos os Valores Líquidos do projeto é o Valor Líquido do portfólio.

  Para obter mais informações sobre o Portfolio Otimizer, consulte [visão geral do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* No campo Valor Líquido do Projeto das listas e relatórios a seguir:

   * Projeto
   * Tarefa
   * Problema
   * Projeto (Dado Financeiro)

  Para obter mais informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
