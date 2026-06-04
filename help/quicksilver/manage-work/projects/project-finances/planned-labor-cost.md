---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular o custo do trabalho planejado
description: À medida que você planeja o trabalho em seus projetos, a Adobe Workfront calcula o Custo de mão de obra planejado para as funções e usuários atribuídos a esse trabalho com base em seus valores de Custo por hora.
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
TQID: https://experienceleague.adobe.com/xzjI7jrIuUBcwF7MpZ8fcWGuFgDrY-V2OUlAq95lDAw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 3%

---

# Calcular o custo do trabalho planejado

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
