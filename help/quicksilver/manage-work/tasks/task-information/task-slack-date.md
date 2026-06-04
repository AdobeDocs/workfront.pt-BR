---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão Geral da Data de Slack da Tarefa
description: Às vezes, as tarefas podem ser iniciadas e concluídas com atraso sem afetar a Data de conclusão do projeto. A Data do Slack exibe a data exata em que uma tarefa poderia definitivamente afetar a Data de conclusão do projeto.
author: Alina
feature: Work Management
exl-id: ccdaa27d-e212-45dc-afca-08539f2b4001
TQID: https://experienceleague.adobe.com/p2lKXWr-25jYKmV38ifdEJcyJf72FZMYRccaNiD5gTw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 273
ht-degree: 1%

---

# Visão geral da Data do Slack da tarefa

Às vezes, as tarefas podem ser iniciadas e concluídas com atraso sem afetar a Data de conclusão do projeto.

A Data do Slack exibe a data exata em que uma tarefa poderia definitivamente afetar a Data de conclusão do projeto.

## Visão geral da data do Slack

A Data de Slack é diferente da Data de conclusão projetada, já que os relacionamentos do antecessor e as restrições de tarefa aumentam o tempo de folga.

Considere os cenários a seguir, dependendo se uma tarefa está no Caminho Crítico de um projeto ou não:

* Para tarefas que estão no Caminho Crítico do projeto ou que têm sucessores que estão no Caminho Crítico, a Data do Slack corresponde à Data de conclusão projetada da tarefa, a menos que o Status do Andamento da tarefa já esteja Atrasado ou Atrasado.

  Para obter informações sobre o Caminho Crítico, consulte [Visão Geral do Caminho Crítico do projeto](../../../manage-work/tasks/manage-tasks/critical-path.md).

  Para obter informações sobre o Status de Progresso das tarefas, consulte [Visão geral do Status de Progresso da Tarefa](../../../manage-work/tasks/task-information/task-progress-status.md).

* Para tarefas que não estão no Caminho Crítico, o tempo de folga aumenta conforme o agendamento da tarefa é antecipado. Para essas tarefas, a Data de Slack permanece no futuro até que as tarefas se tornem tão tardias que comecem a afetar a Data de conclusão do projeto.

## Localizar a data de Slack de uma tarefa

Para exibir a Data Slack de uma tarefa, você pode adicionar o campo Data Slack a uma exibição de tarefa ou relatório.

Para obter informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
