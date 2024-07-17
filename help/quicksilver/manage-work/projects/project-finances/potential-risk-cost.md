---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular Custo de Risco Potencial
description: O Custo do Risco Potencial de um projeto leva em conta os Custos Potenciais dos riscos do projeto e sua probabilidade de ocorrência.
author: Alina
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Calcular Custo de Risco Potencial

O Custo do Risco Potencial de um projeto leva em conta os Custos Potenciais dos riscos do projeto e sua probabilidade de ocorrência.

## Visão Geral do Custo de Risco Potencial de um projeto

A Adobe Workfront calcula o custo de risco potencial de um projeto usando a seguinte fórmula:

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

Considere o seguinte ao revisar o Custo de Risco Potencial de um projeto:

* O custo de risco planejado de um projeto é idêntico ao custo de risco potencial. 
* O custo de risco potencial não é incorporado no custo planejado de um projeto. Em vez disso, é usado para determinar seu Valor líquido. .

## Localizar o Custo Potencial de Risco de um projeto

Você pode encontrar os riscos de um projeto e seu custo potencial nas seguintes áreas no Workfront:

* Na guia Riscos do projeto.
* No Resumo de Business Case.\
  Para obter mais informações sobre o Business Case de um projeto, consulte o artigo [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* Em um relatório de projeto ao adicionar o campo Custo de risco planejado às colunas do relatório.\
  Para obter mais informações sobre a criação de relatórios no Workfront, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* No Otimizador de Portfolio, quando o projeto é associado a um Portfolio, na coluna Risco.\
  A soma de todos os Custos de Risco Potencial de todos os projetos no portfólio soma o Risco do Portfolio.\
  Para obter mais informações sobre o Portfolio Otimizer, consulte o artigo [visão geral do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Para obter mais informações sobre como criar riscos em um projeto, consulte o artigo [Criar e editar riscos em projetos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

Para obter mais informações sobre o Business Case de um projeto, consulte o artigo [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).
