---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''Visão geral da restrição de tarefa: Logo Que Possível"'
description: Assim que possível é uma restrição de tarefa que coloca a hora de início da tarefa o mais próximo possível do início do projeto.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Visão geral da restrição de tarefa: Logo Que Possível

Assim que possível é uma restrição de tarefa que coloca a hora de início da tarefa o mais próximo possível do início do projeto.

## Considerações para usar a restrição Assim que Possível

* Assim que possível é a restrição padrão se um projeto usar um Modo de Programação a partir da Data inicial e se a data de início padrão do sistema para uma nova tarefa for definida como Baseado na Data Planejada do Projeto.

* Se um projeto usar um modo de agendamento da Data Inicial e se a Data Inicial padrão do sistema ou grupo para uma nova tarefa estiver definida como Hoje, a Restrição de tarefa padrão será Iniciar não antes de uma.

   Para obter informações sobre onde definir a Restrição padrão para uma nova tarefa, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

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

## A diferença entre o horário disponível mais cedo e o mais rápido possível

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

A restrição de Tempo Disponível Mais Antiga difere da restrição Assim que Possível quando todos os seguintes critérios existem:

* O projeto é agendado a partir da conclusão.
* As tarefas no projeto têm uma relação predecessora.
* A tarefa predecessora tem uma restrição de tarefa flexível.

Nesta situação:

* **Hora Disponível Mais Antiga:** Usar a restrição de Tempo Disponível Mais Antiga na tarefa sucessora dá prioridade à restrição flexível do antecessor.

   Por exemplo, suponha que a Tarefa A seja um antecessor da Tarefa B. A Tarefa B tem a Restrição de Tempo Disponível Mais Antiga e a Tarefa A tem a restrição O Mais Tarde Possível. Nessa situação, a tarefa é agendada o mais próximo possível da conclusão do projeto.

* **Assim Que Possível:** Nesse cenário, o uso da restrição Assim que Possível na tarefa sucessora dá prioridade à tarefa sucessora.

   Por exemplo, suponha que a Tarefa A seja um antecessor da Tarefa B. A Tarefa B tem a restrição Assim que Possível e a Tarefa A tem a restrição O Mais Tarde Possível. Nessa situação, a tarefa é agendada o mais próximo possível do início do projeto.
