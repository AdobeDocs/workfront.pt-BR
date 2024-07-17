---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular o retorno sobre o investimento (ROI)
description: O ROI (Return On Investment, retorno sobre o investimento) é uma métrica da Adobe Workfront que permite que os gerentes de portfólio vejam rapidamente o desempenho do projeto em relação ao benefício planejado original e ao custo orçado do projeto.
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Calcular o retorno sobre o investimento (ROI)

O ROI (Return On Investment, retorno sobre o investimento) é uma métrica da Adobe Workfront que permite que os gerentes de portfólio vejam rapidamente o desempenho do projeto em relação ao benefício planejado original e ao custo orçado do projeto.

## Visão geral do retorno sobre o investimento (ROI) do projeto

A Workfront calcula o ROI usando a seguinte fórmula:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

Os seguintes campos afetam o ROI de um projeto:

* **Benefício Planejado do Projeto**: esta é uma entrada manual especificada pelo Proprietário do Projeto ao concluir a área Informações do Projeto do Business Case. Esta é uma estimativa do que você, como o Proprietário do projeto, acha que o benefício do projeto pode ser se você concluir o projeto. Esse é um valor específico de moeda e deve ser um valor positivo.\
  Para obter mais informações sobre o Benefício Planejado de um projeto, consulte a seção &quot;Informações do Projeto&quot; no artigo [Criar um Plano de Negócio para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Custo orçado do projeto**: este é o custo total associado ao projeto conforme estimado quando você inicia o projeto pela primeira vez.

  O **Custo Orçado** usa o valor de **Custo Orçado do Trabalho**, que é calculado na área Orçamento de Recursos do Business Case, e leva em conta as horas orçadas para suas funções de trabalho no Planejador de Recursos e a taxa de Custo por Hora de cada função de trabalho.\
  Para obter mais informações, consulte [Calcular Custo Orçado](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Localize o Retorno do Investimento (ROI) do projeto

Você pode visualizar o valor do ROI de um projeto nas seguintes áreas no Workfront:

* No Otimizador de Portfolio, se o projeto estiver associado a um portfólio

  >[!NOTE]
  >
  >O ROI total de todos os valores de ROI do projeto é o ROI do portfólio.

  Para obter informações sobre o Portfolio Otimizer, consulte o artigo [visão geral do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* No campo ROI do projeto, nas listas e relatórios a seguir: 

   * Projeto
   * Tarefa
   * Problema
   * Projeto (Dados Financeiros)

  Para obter mais informações sobre a criação de relatórios no Workfront, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
