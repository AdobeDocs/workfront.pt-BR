---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão geral da restrição de tarefa: Hora Disponível Mais Antiga'
description: Hora Disponível Mais Antiga é uma Restrição de Tarefa que agenda uma tarefa para começar o mais cedo possível após considerar qualquer relação de antecessor.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Visão geral da restrição de tarefa: Hora Disponível Anterior

Hora Disponível Mais Antiga é uma Restrição de Tarefa que agenda uma tarefa para começar o mais cedo possível após considerar qualquer relação de antecessor.

Para obter informações sobre como atualizar a Restrição de Tarefa em uma tarefa, consulte [Atualizar a Restrição de Tarefa de uma tarefa](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## A diferença entre o horário disponível mais cedo e o mais rápido possível

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

A restrição de Tempo Disponível Mais Antiga difere da restrição Assim que Possível quando todos os seguintes critérios existem:

* O projeto está programado desde a conclusão
* As tarefas no projeto têm uma relação predecessora
* A tarefa predecessora tem uma restrição de tarefa flexível

Nesta situação:

* **Hora Disponível Mais Antiga:** Usar a restrição de Tempo Disponível Mais Antiga na tarefa sucessora dá prioridade à restrição flexível do antecessor.

   **Exemplo:** A Tarefa A é um antecessor da Tarefa B. A Tarefa B tem a Restrição de Tempo Disponível Mais Antiga e a Tarefa A tem a restrição O Mais Tarde Possível. Nesta situação, a Tarefa B é agendada o mais próximo possível da conclusão do projeto.

   ![Primeira restrição de Tempo Disponível quando a tarefa tiver as datas próximas à Data de Conclusão do projeto](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **Assim Que Possível:** Nesse cenário, o uso da restrição Assim que Possível na tarefa sucessora dá prioridade à tarefa sucessora.

   **Exemplo:**  A Tarefa A é antecessora da Tarefa B. A Tarefa B tem a restrição Logo que Possível e a Tarefa A tem a restrição O Mais Tarde Possível. Nessa situação, a Tarefa B é agendada o mais próximo possível do início do projeto.

   ![Assim que possível, a restrição quando a tarefa tiver as datas próximas à Data inicial do projeto](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
