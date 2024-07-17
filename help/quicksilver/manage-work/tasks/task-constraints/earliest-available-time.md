---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Visão geral da Restrição da Tarefa: Primeiro Horário Disponível"
description: Primeiro Horário Disponível é uma Restrição de Tarefa que programa uma tarefa para iniciar no primeiro horário disponível depois de considerar quaisquer relacionamentos com predecessores.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Visão geral de Restrição de Tarefa: Horário Mais Cedo Disponível

Primeiro Horário Disponível é uma Restrição de Tarefa que programa uma tarefa para iniciar no primeiro horário disponível depois de considerar quaisquer relacionamentos com predecessores.

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

## A diferença entre o Horário Mais Antigo Disponível e o Mais Breve Possível

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

A restrição Primeiro Horário Disponível difere da restrição O Mais Breve Possível quando todos os critérios a seguir existem:

* O projeto está agendado a partir da conclusão
* As tarefas no projeto têm um relacionamento predecessor
* A tarefa predecessora tem uma restrição de tarefa flexível

Nesta situação:

* **Primeiro Horário Disponível:** Usar a restrição Primeiro Horário Disponível na tarefa sucessora dá prioridade à restrição flexível da predecessora.

  **EXEMPLO**

  A Tarefa A é antecessora da Tarefa B. A Tarefa B tem a restrição Tempo Mais Cedo Disponível e a Tarefa A tem a restrição O Mais Tarde Possível. Nessa situação, a Tarefa B é agendada o mais próximo possível da conclusão do projeto.

  ![Restrição de Tempo Mais Cedo Disponível quando a tarefa tem datas próximas à Data de Término do projeto](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **O Mais Breve Possível:** Neste cenário, usar a restrição O Mais Breve Possível na tarefa sucessora dá prioridade à tarefa sucessora.

  **EXEMPLO**

  A Tarefa A é antecessora da Tarefa B. A Tarefa B tem a restrição O Mais Breve Possível e a Tarefa A tem a restrição O Mais Tarde Possível. Nessa situação, a Tarefa B é agendada o mais próximo possível do início do projeto.

  ![Restrição o Mais Breve Possível quando a tarefa tiver datas próximas à Data de Início do projeto](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
