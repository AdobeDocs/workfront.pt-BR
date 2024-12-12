---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular Custo de Trabalho Planejado
description: À medida que você planeja o trabalho em seus projetos, a Adobe Workfront calcula o Custo de mão de obra planejado para as funções e usuários atribuídos a esse trabalho com base em seus valores de Custo por hora.
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Calcular Custo de Trabalho Planejado

À medida que você planeja o trabalho em seus projetos, a Adobe Workfront calcula o Custo de mão de obra planejado para as funções e usuários atribuídos a esse trabalho com base em seus valores de Custo por hora.

O Custo de Trabalho Planejado de um projeto é um cálculo entre o custo associado às funções de trabalho ou aos usuários atribuídos para concluir o trabalho no projeto e a quantidade de horas planejadas (Horas Planejadas) que podem levar cada função ou usuário para concluir esse trabalho.

## Visão Geral do Custo de Trabalho Planejado

O **Custo de Trabalho Planejado** de um projeto é calculado adicionando todos os Custos de Trabalho Planejados de todas as tarefas do projeto.

>[!TIP]
>
>Não há Custo de Trabalho Planejado associado a problemas ou ao próprio projeto.

O Workfront calcula o Custo de Trabalho Planejado de um projeto usando a seguinte fórmula:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

O Custo de Trabalho Planejado da Tarefa é calculado com base no seguinte:

* O número de recursos na tarefa e sua alocação individual para a tarefa
* O Tipo de Custo da tarefa.

O Custo de Trabalho Planejado da Tarefa é calculado usando a seguinte fórmula:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Para obter mais informações sobre como a Workfront calcula o Custo de Trabalho Planejado para tarefas, dependendo das atribuições de tarefa e do Tipo de Custo, consulte a seção &quot;Modificar Tipos de Custo para tarefas individuais&quot; no artigo [Rastrear custos](../../../manage-work/projects/project-finances/track-costs.md).

## Localize o Custo de Trabalho Planejado

Você pode localizar o Custo de mão de obra planejado de um projeto nas seguintes áreas do Workfront:

* Um relatório de Projeto
* Uma lista de projetos
* Um relatório de Linha de Base onde você pode rastreá-lo ao longo do tempo
* Por meio da API

Para obter informações sobre como criar relatórios e usar a API do Workfront, consulte os seguintes artigos:

* [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [Noções básicas sobre API](../../../wf-api/general/api-basics.md)
