---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular valor líquido
description: O valor líquido de um projeto é o valor total esperado do projeto após o cálculo do seu benefício e a eliminação dos custos.
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Calcular valor líquido

O valor líquido de um projeto é o valor total esperado do projeto após o cálculo do seu benefício e a eliminação dos custos. 

## Visão geral do valor líquido do projeto

O Adobe Workfront calcula o Valor Líquido de um projeto usando a seguinte fórmula: 

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

Os seguintes campos podem afetar o Valor Líquido de um projeto:

* **Benefício planejado**: Esta é uma entrada manual especificada pelo Proprietário do Projeto ao concluir a **Informações do projeto** área do Caso de negócios.\
   Para obter mais informações sobre o Benefício Planejado de um projeto, consulte o [Informações do projeto](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) seção no artigo [Visão geral das áreas do caso comercial](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Custo orçado**: esse é o custo total associado ao projeto, conforme estimado ao iniciar o projeto pela primeira vez.

   O **Custo orçado** usa a variável **Custo de Mão-de-Obra Orçada** valor que é calculado na área Orçamento de Recursos do Caso de Negócios e leva em conta as horas orçadas para suas funções de cargo no Planejador de Recursos e a taxa de Custo por Hora de cada função de cargo.\
   O Custo Orçamentado afeta o **Valor líquido** do projeto. Para obter mais informações sobre como o Custo Orçado é calculado, consulte [Calcular Custo Orçamentado](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Custo do Risco Potencial**: Esse é o custo associado a quaisquer riscos no projeto, conforme definido no Caso de negócios ou na guia Riscos do projeto.\
   Para obter mais informações sobre o cálculo do Custo de Risco Potencial de um projeto, consulte o artigo [Calcular Custo de Risco Potencial](../../../manage-work/projects/project-finances/potential-risk-cost.md).

    

## Localize o valor líquido do projeto

Você pode encontrar o Valor Líquido de um projeto nas seguintes áreas no Workfront:

* Na área Resumo do caso de negócios do caso de negócios \
   Para obter mais informações sobre a área Resumo do caso de negócios, consulte a seção &quot;Noções básicas sobre o resumo do caso de negócios&quot; no artigo [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

   ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* No Portfolio Otimizer se o projeto estiver associado a um portfólio

   >[!TIP]
   >
   >O total de todos os Valores Líquidos do projeto é o Valor Líquido do portfólio.

   Para obter mais informações sobre o Portfolio Otimizer, consulte [Visão geral do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* No campo Valor Líquido do Projeto das seguintes listas e relatórios:

   * Projeto
   * Tarefa
   * Problema
   * Projeto (Dado Financeiro)
   Para obter mais informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
