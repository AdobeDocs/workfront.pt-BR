---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Consultas de atividade do projeto
description: Consultas do Enhanced Analytics
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: b7155160-4537-4919-bebf-72056b181bb6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Consultas de atividade do projeto

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

## Eventos de logon de usuários de projetos

Mostra o número de pessoas atribuídas ao projeto que fizeram logon em um determinado dia.

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    tds.projectid, 
    ads.calendardate, 
    count(1) 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN userlogins ul ON ads.assignedtoid = ul.userid and TO_DATE(ul.lastlogindate) = ads.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### Eventos de logon de usuários de projetos: detalhar

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 

SELECT 
    tds.projectid, 
    ul.userid, 
    ads.calendardate, 
    count(1) 
FROM assignments_daily_history ads 
INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
INNER JOIN userlogins ul ON ads.assignedtoid = ul.userid AND TO_DATE(ul.lastlogindate) = ads.calendardate 
group by tds.projectid, ul.userid, ads.calendardate
 
```

## Eventos de alteração de status de tarefa de usuários de projetos

Mostra o número de pessoas que alteraram o status de uma tarefa para o projeto em um determinado dia.

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event 
        WHERE status != 'CPL' 
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    count(tds.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid and TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### Eventos de alteração de status de tarefa de usuários de projetos: detalhar

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        lastupdatedbyid, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lastupdatedbyid, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status != 'CPL'  
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    tsc.lastupdatedbyid, 
    count(tsc.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid AND TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, tsc.lastupdatedbyid, ads.calendardate
```

## Eventos de conclusão de tarefas de usuários de projetos

Mostrar o número de pessoas que concluíram uma tarefa para o projeto em um determinado dia.

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status = 'CPL'  
    )  
    WHERE status != previous_status  
) 
 
SELECT 
    tds.projectid, 
    count(tds.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid and tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid and tsc.taskid = tds.taskid and TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### Eventos de conclusão de tarefas de usuários de projetos: detalhar

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        lastupdatedbyid, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lastupdatedbyid, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status = 'CPL'  
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    tsc.lastupdatedbyid, 
    count(tsc.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid AND TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, tsc.lastupdatedbyid, ads.calendardate
```
