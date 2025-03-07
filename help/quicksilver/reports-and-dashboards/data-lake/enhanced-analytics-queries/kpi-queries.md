---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Consultas de KPI
description: Consultas do Enhanced Analytics
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: eccecaece64b78aa19444407b182ea80b2115a63
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 2%

---


# Consultas de KPI

Você pode usar as queries neste artigo para criar visualizações de dados semelhantes às do Enhanced Analytics.

>[!IMPORTANT]
>
>As consultas produzirão resultados semelhantes aos mostrados no Enhanced Analytics, mas podem não corresponder exatamente.


## Pré-requisitos

Antes de começar, você deve

1. Estabeleça uma conexão com a ferramenta Business Intelligence (BI):
   1. [Criar uma conta ou conexão de leitor para o Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Estabelecer uma conexão com o Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

Depois de estabelecer uma conexão, você pode usar as consultas neste artigo para extrair e visualizar dados.

## Projetos concluídos

O KPI de Projetos concluídos mostra quantos projetos no período filtrado foram concluídos, bem como a porcentagem de aumento ou diminuição desde o período anterior. Abaixo desses números, você pode ver o número de projetos concluídos no período anterior, bem como o número de dias no período anterior.

![Projetos KPI concluídos](assets/kpi-projects-completed-350x182.png)

### Query

```
WITH completedProjectsInRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedProjectsPreviousRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
SELECT (a.PROJECT_COUNT - b.PROJECT_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD FROM completedProjectsInRange a, completedProjectsPreviousRange b 
), percentChange as ( 
SELECT  
CASE 
WHEN a.PROJECT_COUNT = b.PROJECT_COUNT THEN 0.00 
WHEN b.PROJECT_COUNT > 0 THEN ((a.PROJECT_COUNT - b.PROJECT_COUNT) / b.PROJECT_COUNT * 100) 
END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b 
) 
SELECT 
a.PROJECT_COUNT, 
b.PROJECT_COUNT as PREVIOUS_PROJECT_COUNT, 
c.CHANGE_FROM_PREVIOUS_PERIOD, 
d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b, rawChange c, 
percentChange d
```

## Projetos concluídos no prazo

O KPI de Projetos concluídos no prazo mostra a porcentagem de projetos dentro do período filtrado que foram concluídos no prazo, bem como como a porcentagem de aumento ou diminuição em relação ao período anterior. Abaixo desses números, é possível ver a porcentagem de projetos concluídos no prazo no período anterior, bem como o número de dias no período anterior.

![Projetos KPI concluídos no prazo](assets/kpi-projects-completed-on-time-350x180.png)

## Média duração do projeto

A Média KPI de duração do projeto mostra a quantidade média de tempo de conclusão (em dias, semanas ou anos) para projetos com datas de término reais dentro do período filtrado, bem como a porcentagem de aumento ou diminuição desde o período anterior. Abaixo desses números, você pode ver o tempo médio de conclusão de projetos com datas de término reais no período anterior, bem como o número de dias no período anterior.

![Duração média do projeto do KPI](assets/kpi-avg.-project-duration-350x168.png)

## Média de tarefas por projeto

O KPI de Média de Tarefas por Projeto mostra o número médio de tarefas atribuídas a projetos dentro do período filtrado, bem como a porcentagem de aumento ou diminuição desde o período anterior. Abaixo desses números, você pode ver o número médio de tarefas atribuídas a projetos no período anterior, bem como o número de dias no período anterior.

![Média de tarefas de KPI por projeto](assets/kpi-average-tasks-per-project-350x179.png)