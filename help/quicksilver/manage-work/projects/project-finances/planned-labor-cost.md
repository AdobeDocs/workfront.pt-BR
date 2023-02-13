---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular o custo planejado da mão de obra
description: Conforme você planeja o trabalho em seus projetos, a Adobe Workfront calcula o Custo Planejado da Mão-de-Obra para as funções e usuários atribuídos a esse trabalho com base em seus valores de Custo por Hora.
author: Alina
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Calcular o custo planejado da mão de obra

Conforme você planeja o trabalho em seus projetos, a Adobe Workfront calcula o Custo Planejado da Mão-de-Obra para as funções e usuários atribuídos a esse trabalho com base em seus valores de Custo por Hora.

O Custo Planejado da Mão-de-Obra de um projeto é um cálculo entre o custo associado às funções do job ou os usuários atribuídos para concluir o trabalho no projeto e a quantidade de horas planejadas (Horas Planejadas) que podem levar cada função ou usuário a concluir esse trabalho.

## Visão Geral do Custo Planejado da Mão-de-Obra

O **Custo planejado da mão de obra** de um projeto é calculado adicionando todos os Custos de Mão de obra planejados de todas as tarefas do projeto.

>[!TIP]
>
>Não há Custo Planejado da Mão-de-Obra associado a problemas ou ao próprio projeto.

O Workfront calcula o Custo Planejado da Mão de Obra de um projeto usando a seguinte fórmula:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

O Custo da Mão de Obra Planejada da Tarefa é calculado com base no seguinte:

* O número de recursos na tarefa e sua alocação individual na tarefa
* O Tipo de Custo da tarefa.

O Custo da Mão de Obra Planejada da Tarefa é calculado usando a seguinte fórmula:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Para obter mais informações sobre como o Workfront calcula o Custo da Mão de obra Planejada para tarefas, dependendo das atribuições de tarefa e do Tipo de Custo, consulte a seção &quot;Modificar Tipos de Custo para tarefas individuais&quot; no artigo [Rastrear custos](../../../manage-work/projects/project-finances/track-costs.md).

## Localize o custo planejado da mão de obra

Você pode localizar o Custo planejado da mão de obra de um projeto nas seguintes áreas do Workfront:

* Um relatório de projeto
* Uma lista de projetos
* Um relatório de Linha de base onde você pode rastreá-lo ao longo do tempo
* Por meio da API

Para obter informações sobre como criar relatórios e usar a API do Workfront, consulte os seguintes artigos:

* [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [Noções básicas sobre API](../../../wf-api/general/api-basics.md)
