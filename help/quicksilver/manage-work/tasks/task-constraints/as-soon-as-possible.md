---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visão Geral Da Restrição De Tarefa: O Mais Breve Possível'
description: Assim que possível é uma restrição de tarefa que coloca a hora de início da tarefa o mais próximo possível do início do projeto.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Visão geral da restrição de tarefas: o mais rápido possível

Assim que possível é uma restrição de tarefa que coloca a hora de início da tarefa o mais próximo possível do início do projeto.

## Considerações para usar a restrição O Mais Breve Possível

* Assim que Possível é a restrição padrão se um projeto usar um Modo de Agendamento de Agendamento a partir da Data Inicial e se a data inicial padrão do sistema para uma nova tarefa for definida como Baseado na Data Planejada do Projeto.

* Se um projeto usar um modo de programação Programação a partir da Data Inicial e se a Data Inicial padrão do sistema ou grupo para uma nova tarefa estiver definida como Hoje, a Restrição de Tarefa padrão será Não Iniciar Antes de.

  Para obter informações sobre onde definir a Restrição padrão para uma nova tarefa, consulte [Configurar preferências de tarefas e problemas do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Para obter informações sobre como atualizar a Restrição de Tarefa em uma tarefa, consulte [Atualizar a Restrição de Tarefa de uma tarefa](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Soon As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Soon As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## A diferença entre o Horário Mais Antigo Disponível e o Mais Breve Possível

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

A restrição Primeiro Horário Disponível difere da restrição O Mais Breve Possível quando todos os critérios a seguir existem:

* A conclusão do projeto está programada.
* As tarefas no projeto têm um relacionamento predecessor.
* A tarefa predecessora tem uma restrição de tarefa flexível.

Nesta situação:

* **Primeiro Horário Disponível:** Usar a restrição Primeiro Horário Disponível na tarefa sucessora dá prioridade à restrição flexível da predecessora.

  Por exemplo, suponha que a Tarefa A seja predecessora da Tarefa B. A Tarefa B tem a restrição Momento Mais Cedo Disponível e a Tarefa A tem a restrição O Mais Tarde Possível. Nessa situação, a tarefa é agendada o mais próximo possível da conclusão do projeto.

* **O Mais Breve Possível:** Neste cenário, usar a restrição O Mais Breve Possível na tarefa sucessora dá prioridade à tarefa sucessora.

  Por exemplo, suponha que a Tarefa A seja predecessora da Tarefa B. A Tarefa B tem a restrição O Mais Breve Possível e a Tarefa A tem a restrição O Mais Tarde Possível. Nessa situação, a tarefa é agendada o mais próximo possível do início do projeto.
