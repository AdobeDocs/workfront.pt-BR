---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular Valor Líquido
description: O Valor Líquido de um projeto é o valor total esperado do projeto após calcular seu benefício e remover os custos.
author: Lisa
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Calcular Valor Líquido

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
  O custo orçado afeta o **valor líquido** do projeto. Para obter mais informações sobre como o Custo Orçado é calculado, consulte [Calcular Custo Orçado](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Custo de Risco Potencial**: este é o custo associado a qualquer risco no projeto, conforme definido no Business Case ou na guia Riscos do projeto.\
  Para obter mais informações sobre como calcular o Custo de Risco Potencial de um projeto, consulte o artigo [Calcular Custo de Risco Potencial](../../../manage-work/projects/project-finances/potential-risk-cost.md).

   

## Localizar o Valor Líquido do projeto

Você pode encontrar o Valor líquido de um projeto nas seguintes áreas no Workfront:

* Na área Resumo de business case do business case \
  Para obter mais informações sobre a área Resumo de Business Case, consulte a seção &quot;Noções básicas sobre o Resumo de Business Case&quot; no artigo [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

  ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* No Otimizador de Portfolio, se o projeto estiver associado a um portfólio

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
