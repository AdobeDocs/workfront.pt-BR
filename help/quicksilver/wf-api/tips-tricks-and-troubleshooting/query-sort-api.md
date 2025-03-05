---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Classificação dos resultados da consulta na API
description: Classificação dos resultados da consulta na API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 5936982217adc6cfcaf9e400bfff67a1496d3a78
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Classificação dos resultados da consulta na API

Você pode classificar os resultados por qualquer campo se anexar o seguinte à chamada de API:

```
&entryDate_Sort=asc
```

Por exemplo, se você deseja classificar por Data de conclusão planejada da tarefa, remova `entryDate` e substitua-a por `plannedCompletionDate`.

```
&plannedCompletionDate_Sort=asc
```

Isso funciona para a maioria dos campos no Adobe Workfront.
