---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Classificação dos resultados da consulta na API
description: Classificação dos resultados da consulta na API
author: John
feature: Workfront API
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Classificação dos resultados da consulta na API

Você pode classificar os resultados por qualquer campo se anexar o seguinte à chamada de API:

```
&entryDate_Sort=asc
```

Por exemplo, se você deseja classificar por tarefa Data de início planejada, remova `entryDate` e substitua por `plannedCompletionDate`.

Isso funciona para a maioria dos campos no Adobe Workfront.
