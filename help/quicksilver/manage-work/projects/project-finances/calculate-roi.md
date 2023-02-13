---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular o retorno sobre o investimento (ROI)
description: O retorno do investimento (ROI) é uma métrica da Adobe Workfront que permite que os gerentes de portfólio vejam rapidamente como o projeto está se saindo em relação ao benefício planejado original e ao custo orçado do projeto.
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Calcular o retorno sobre o investimento (ROI)

O retorno do investimento (ROI) é uma métrica da Adobe Workfront que permite que os gerentes de portfólio vejam rapidamente como o projeto está se saindo em relação ao benefício planejado original e ao custo orçado do projeto.

## Resumo do projeto Retorno do Investimento (ROI)

O Workfront calcula o ROI usando a seguinte fórmula:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

Os seguintes campos afetam o ROI de um projeto:

* **Benefício planejado do projeto**: Esta é uma entrada manual especificada pelo Proprietário do projeto ao concluir a área Informações do projeto do Caso de negócios. Esta é uma estimativa do que você, como Proprietário do projeto, acha que o benefício do projeto pode ser se você concluir o projeto. Trata-se de uma quantidade específica de moeda e deve ser um valor positivo.\
   Para obter mais informações sobre o Benefício planejado de um projeto, consulte a seção &quot;Informações do projeto&quot; no artigo [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Custo Orçado do Projeto**: esse é o custo total associado ao projeto, conforme estimado ao iniciar o projeto pela primeira vez.

   O **Custo orçado** usa a variável **Custo de Mão-de-Obra Orçada** valor que é calculado na área Orçamento de Recursos do Caso de Negócios e leva em conta as horas orçadas para suas funções de cargo no Planejador de Recursos e a taxa de Custo por Hora de cada função de cargo.\
   Para obter mais informações, consulte [Calcular Custo Orçamentado](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Localizar o retorno do investimento (ROI) no projeto

Você pode exibir o valor do ROI de um projeto nas seguintes áreas do Workfront:

* No Portfolio Otimizer se o projeto estiver associado a um portfólio

   >[!NOTE]
   >
   >O total de todos os valores de ROI do projeto é o ROI do portfólio.

   Para obter informações sobre o Portfolio Otimizer, consulte o artigo [Visão geral do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* No campo ROI do projeto , nas listas e relatórios a seguir: 

   * Projeto
   * Tarefa
   * Problema
   * Projeto (Dados Financeiros)
   Para obter mais informações sobre como criar relatórios no Workfront, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
