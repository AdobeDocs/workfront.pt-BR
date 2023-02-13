---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral da Data Slack da tarefa
description: Às vezes, as tarefas podem iniciar e concluir tarde sem afetar a Data de conclusão do projeto.
author: Alina
feature: Work Management
exl-id: ccdaa27d-e212-45dc-afca-08539f2b4001
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Visão geral da Data Slack da tarefa

Às vezes, as tarefas podem iniciar e concluir tarde sem afetar a Data de conclusão do projeto.

A Data de Slack exibe a data exata em que uma tarefa pode definitivamente afetar a Data de conclusão do projeto.

## Visão geral da data Slack

A Data de Slack é diferente da Data de Conclusão Projetada, já que as relações do antecessor e as restrições de tarefa aumentam o tempo de folga.

Considere os seguintes cenários, dependendo se uma tarefa está ou não no Caminho Crítico de um projeto:

* Para tarefas que estão no Caminho Crítico do projeto ou que têm sucessores que estejam no Caminho Crítico, a Data de Slack corresponde à Data de Conclusão Projetada da tarefa, a menos que o Status de Andamento da tarefa já esteja Atrasado ou Atrasado.

   Para obter informações sobre o Caminho Crítico, consulte [Visão geral do caminho crítico do projeto](../../../manage-work/tasks/manage-tasks/critical-path.md).

   Para obter informações sobre o Status de Andamento de tarefas, consulte [Visão geral do status de progresso da tarefa](../../../manage-work/tasks/task-information/task-progress-status.md).

* Para tarefas que não estão no Caminho Crítico, o tempo de folga aumenta quanto antes a tarefa for agendada. Para essas tarefas, a Data de Slack permanece no futuro até que as tarefas se tornem tão atrasadas que comecem a afetar a Data de conclusão do projeto.

## Localize a Data de Slack de uma tarefa

Para exibir a Data de Slack de uma tarefa, é possível adicionar o campo Data de Slack a uma visualização de tarefa ou relatório.

Para obter informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
