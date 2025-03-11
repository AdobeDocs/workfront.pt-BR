---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Consultas de mapa de árvore do projeto
description: Consultas do Enhanced Analytics
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 3943703a-0d0b-46d3-a708-52987d330523
source-git-commit: da5c7197b3826855bae5dd3d3bf2ba9d07d7f188
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 0%

---

# Consultas de mapa de árvore do projeto

Você pode usar as queries neste artigo para criar visualizações de dados semelhantes às do Enhanced Analytics.

>[!IMPORTANT]
>
>As consultas produzirão resultados semelhantes aos mostrados no Enhanced Analytics, mas podem não corresponder exatamente.


## Pré-requisitos

Antes de começar, você deve

1. Estabeleça uma conexão com a ferramenta Business Intelligence (BI):
   1. [Criar uma conta ou conexão de leitor para o Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Estabelecer uma conexão com o Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

Depois de estabelecer uma conexão, você poderá usar as consultas neste artigo para extrair e visualizar dados.

## Horas planejadas de projetos retiradas

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### Horas planejadas de projetos desativadas: burndown

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

## Duração planejada dos projetos removida 

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### Duração planejada dos projetos desativada: burndown

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```
