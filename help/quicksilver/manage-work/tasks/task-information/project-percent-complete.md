---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão Geral do Percentual de Término do Projeto
description: O valor do Percentual concluído de um projeto é calculado com base na Duração planejada ou nas Horas planejadas das tarefas no projeto. O administrador do Adobe Workfront ou um administrador de grupo define qual valor é levado em conta ao calcular o percentual concluído no sistema quando configuram informações na área Preferências do projeto. Para obter informações sobre como configurar as preferências do projeto, consulte Configurar preferências do projeto do sistema.
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# Visão geral do Percentual de Término do Projeto

<!-- Audited 01/2024 -->

O valor do Percentual concluído de um projeto é calculado com base na Duração ou nas Horas planejadas das tarefas no projeto. O administrador do Adobe Workfront ou um administrador de grupo define qual valor é levado em conta ao calcular o percentual concluído no sistema quando configuram informações na área Preferências do projeto.

Para obter informações sobre como configurar preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

O Percentual de Término de uma tarefa pai é baseado na Duração ou nas Horas Planejadas de cada uma de suas subtarefas.

Da mesma forma, o Percentual concluído de um projeto se baseia nas durações ou nas horas planejadas de cada tarefa principal do projeto.

As tarefas principais são as tarefas pai e as tarefas autônomas que não têm filhos.

>[!TIP]
>
>As tarefas principais não são recuadas em um plano de projeto.

## Como o Workfront calcula a porcentagem concluída

### Atualizar o Percentual de Término em uma tarefa {#update-the-percent-complete-on-a-task}

Você pode modificar o percentual concluído de uma tarefa manualmente. Isso não é um cálculo.

O Workfront usa o percentual concluído de uma tarefa individual para calcular o percentual concluído de sua tarefa pai ou o percentual concluído do projeto.

Para obter informações sobre como atualizar o percentual concluído de uma tarefa, consulte [Exibir e atualizar o Percentual concluído das tarefas](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Como o Workfront calcula a porcentagem concluída em uma tarefa pai {#how-workfront-calculates-percent-complete-on-a-parent-task}

Dependendo do que o administrador do Workfront ou do grupo selecionou nas Preferências do projeto no nível do sistema ou do grupo, o percentual concluído de uma tarefa pai é calculado com base na Duração ou nas Horas planejadas das tarefas.

Considere os seguintes cenários:

* Se o sistema calcular o percentual de conclusão com base nas Horas Planejadas, o percentual de conclusão da tarefa pai será calculado usando a seguinte fórmula:

  `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

  O Total de Horas Planejadas do pai representa a soma de todas as Horas Planejadas de cada filho.

  ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* Se o sistema calcular o percentual concluído com base na Duração, o percentual concluído da tarefa pai será calculado usando a seguinte fórmula:

  `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

  ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!IMPORTANT]
  >
  >A Duração Total da Tarefa Pai é o total de todas as durações das tarefas filho. Por exemplo, uma tarefa pai com dois filhos que têm uma Duração de 1 dia e 2 dias respectivamente tem uma Duração total de 3 dias, mesmo quando os dois filhos podem começar no mesmo dia.


### Como o Workfront calcula a porcentagem concluída em um projeto {#how-workfront-calculates-percent-complete-on-a-project}

Dependendo do que o administrador do Workfront ou do grupo selecionou nas Preferências do projeto no nível do sistema ou do grupo, o percentual concluído de um projeto é calculado com base na Duração ou no Trabalho Planejado das principais tarefas do projeto.

* Se o sistema calcular o percentual concluído com base nas Horas Planejadas, o percentual concluído do projeto será calculado usando a seguinte fórmula:

  `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

  O Total de Horas Planejadas do projeto é a soma das Horas Planejadas de todas as tarefas principais do projeto.

  ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

  >[!NOTE]
  >
  >A Tarefa 1 ou a Tarefa 2 só podem ser tarefas pai ou tarefas independentes. As tarefas de Horas Planejadas e Percentual Concluído dos filhos não são usadas neste cálculo.

* Se o sistema calcular o percentual concluído com base na Duração, o percentual concluído do projeto será calculado usando a seguinte fórmula:

  `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

  >[!IMPORTANT]
  >
  >A Duração do Projeto é o total de todas as durações das tarefas principais que exibem uma porcentagem concluída. Por exemplo, um projeto com uma tarefa independente com uma Duração de 2 dias e uma tarefa pai com uma Duração de 5 dias que tiveram trabalho concluído neles terá uma Duração total de 7 dias, mesmo que as duas tarefas possam começar no mesmo dia.

  ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!NOTE]
  >
  >A Tarefa 1 ou a Tarefa 2 só podem ser tarefas pai ou tarefas independentes. As tarefas Duração e Percentual Concluído dos filhos não são usadas neste cálculo.

## Exemplo de Porcentagem Concluída em um projeto usando a Duração

Ao usar a Duração das tarefas para calcular o percentual concluído de um projeto, considere o seguinte exemplo:

![](assets/project-with-tasks-percent-complete-duration-calculation.png)

As informações a seguir são usadas para calcular o percentual concluído do projeto

* O percentual de conclusão da tarefa independente (Tarefa 1 - 20%)
* O percentual de Término da tarefa pai (Tarefa 2 - 25%)
* A Duração da Tarefa 1 (5 Dias)
* A Duração da Tarefa 2 (2 Dias)
* A duração do projeto (7 dias)


Para calcular o percentual concluído do projeto usando a Duração:

`Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

Ou

`(((5*0.2)+(2*0.25))/7)*100= 21.43%`


<!--drafted, this was the old example:

When using the Planned Duration of the tasks to calculate the percent complete of a project, consider the following example:

percent_complete_on_project_example.png

Only the parent task (Task 1) and the standalone task (Task 8) are used to calculate the percent complete of the project.

The secondary parents of Task 1 are used to calculate the percent complete of the main parent (Task 1).

To calculate the percent complete of the main parent (Task 1), first calculate the percent complete of its secondary parents:

Task 5 Percent Complete = ((14 * 0.75 + 12 * 0.25)/(12 + 14))*100 = 51.92%

Task 2 Percent Complete = ((5 * 0.7 + 2 * 0.5)/(5 + 2))*100 = 64.29 %

Then, to calculate the percent complete of the main parent (Task 1), use the following formula:

Task 1 Percent Complete =((56 * 0.5192 + 7 * 0.6429)/63)*100 = 53.29%

To calculate the percent complete of the project, you will need to have the following numbers ready:

Task 1 Duration (63 hours) and Percent Complete (53.29%)
Task 8 Duration (100 hours) and Percent Complete (4%)
Now, to calculate the percent complete of the project, use the following formula:

Project Percent Complete =((100 * 0.04 + 63 * 0.5329))/163)*100 = 23.05%
-->
