---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral da data do Slack da tarefa
description: Às vezes, as tarefas podem ser iniciadas e concluídas com atraso sem afetar a Data de conclusão do projeto.
author: Alina
feature: Work Management
exl-id: ccdaa27d-e212-45dc-afca-08539f2b4001
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Visão geral da data do Slack da tarefa

Às vezes, as tarefas podem ser iniciadas e concluídas com atraso sem afetar a Data de conclusão do projeto.

A Data do Slack exibe a data exata em que uma tarefa poderia definitivamente afetar a Data de conclusão do projeto.

## Visão geral da data do Slack

A Data de Slack é diferente da Data de conclusão projetada, já que os relacionamentos do antecessor e as restrições da tarefa aumentam o tempo de folga.

Considere os cenários a seguir, dependendo se uma tarefa está no Caminho Crítico de um projeto ou não:

* Para tarefas que estão no Caminho Crítico do projeto ou que têm sucessores que estão no Caminho Crítico, a Data do Slack corresponde à Data de Conclusão Projetada da tarefa, a menos que o Status do Andamento da tarefa já esteja Atrasado ou Atrasado.

  Para obter informações sobre o Caminho Crítico, consulte [Visão Geral do Caminho Crítico do projeto](../../../manage-work/tasks/manage-tasks/critical-path.md).

  Para obter informações sobre o Status de Progresso das tarefas, consulte [Visão geral do Status de Progresso da Tarefa](../../../manage-work/tasks/task-information/task-progress-status.md).

* Para tarefas que não estão no Caminho Crítico, o tempo de folga aumenta conforme o agendamento da tarefa é antecipado. Para essas tarefas, a Data de Slack permanece no futuro até que as tarefas se tornem tão tardias que comecem a afetar a Data de conclusão do projeto.

## Localizar a data do Slack de uma tarefa

Para exibir a Data de Slack de uma tarefa, você pode adicionar o campo Data de Slack a uma exibição de tarefa ou relatório.

Para obter informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
