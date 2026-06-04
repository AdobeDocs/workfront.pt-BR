---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral da duração do projeto
description: O Adobe Workfront calcula a Duração de um projeto levando em conta a Data inicial da tarefa mais antiga e a Data de conclusão da tarefa mais recente, além de contar o número de dias entre as duas datas.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
TQID: https://experienceleague.adobe.com/1j0nj2W5f7FtgIk46G3ePFA-zwt7VAyV9fQWKm2kZJ4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 2%

---

# Visão geral da duração do projeto

O Adobe Workfront calcula a Duração de um projeto levando em conta a Data inicial da tarefa mais antiga e a Data de conclusão da tarefa mais recente, além de contar o número de dias entre as duas datas.

## Duração de Projeto

A duração do projeto é calculada pela seguinte fórmula:

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>A duração dos problemas no projeto não afeta a duração do projeto.

A duração do projeto conta o número de dias entre as duas datas de tarefa com base no Agendamento associado ao projeto ou aos usuários atribuídos às tarefas. Para obter informações sobre qual agendamento a Workfront usa para calcular a duração, consulte [Visão geral dos agendamentos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## Tipos de duração do projeto

Há dois tipos de Duração do projeto e as fórmulas pelas quais o Workfront os calcula:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **Duração planejada**:

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **Duração real**:

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## Localizar a duração do projeto

Você pode localizar o Planejado do projeto e as Durações reais nas seguintes áreas do Workfront:

* . Na área Detalhes do projeto, na seção Visão geral.

  Para obter mais informações sobre a subguia Visão Geral de um projeto, consulte o artigo [Gerenciar informações na área Visão Geral do projeto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* Em um relatório de Projeto, incluindo os campos Duração ou Duração real no relatório.

  Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
