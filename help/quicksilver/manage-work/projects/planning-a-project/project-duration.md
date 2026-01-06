---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral da duração do projeto
description: O Adobe Workfront calcula a Duração de um projeto levando em conta a Data inicial da tarefa mais antiga e a Data de conclusão da tarefa mais recente, além de contar o número de dias entre as duas datas.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

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
