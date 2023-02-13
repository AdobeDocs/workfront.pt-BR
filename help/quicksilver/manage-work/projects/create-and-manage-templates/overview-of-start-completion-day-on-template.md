---
product-area: templates
navigation-topic: templates-navigation-topic
title: Visão geral dos Dias de início e conclusão em um modelo
description: Você pode usar modelos de projeto para capturar a maioria dos processos, informações e configurações repetíveis associados aos projetos em sua organização. Embora os projetos tenham datas específicas de início e conclusão, os modelos têm dias genéricos de início e conclusão como indicação para onde essas datas se encaixarão no projeto, com base na linha do tempo geral do projeto.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Visão geral dos Dias de início e conclusão em um modelo

Você pode usar modelos de projeto para capturar a maioria dos processos, informações e configurações repetíveis associados aos projetos em sua organização. Embora os projetos tenham datas específicas de início e conclusão, os modelos têm dias genéricos de início e conclusão como indicação para onde essas datas se encaixarão no projeto, com base na linha do tempo geral do projeto.

**Exemplo:** Se a Data de início de um projeto for 1 de abril e você quiser que uma tarefa seja iniciada em 3 de abril (dois dias após o início do projeto), a tarefa correspondente no modelo que cria o projeto deverá iniciar no Dia 2 do modelo, onde o primeiro dia do modelo será considerado Dia 0.

## Dia de Início

Considere o seguinte ao trabalhar com modelos e tarefas de modelo:

* Por padrão, os modelos têm um Dia de início de 0 e as tarefas do modelo e o modelo mostram um Dia de início de 0. O Dia de início das tarefas do modelo pode ser alterado, mas isso não altera o Dia de início do modelo.
* O dia de início de uma tarefa de modelo representa o número de dias úteis que o Workfront adiciona à Data de início planejada da tarefa quando um projeto é criado a partir do modelo. Por exemplo, você pode ter um template com apenas uma tarefa e o Dia de início da tarefa do template é 4. O Dia de início do modelo ainda é 0. Ao criar um projeto a partir desse modelo, onde o Modo de Programação do projeto é a Data Inicial e a Data Inicial Planejada do projeto é 1º de novembro de 2019, a tarefa recém-criada adiciona 4 dias a essa data e define seu valor da Data Inicial Planejada como 5 de novembro de 2019.

A seguir estão algumas ações que podem alterar o Dia de início das tarefas do modelo:

* Atualizar a Duração das tarefas do modelo predecessor
* Atualizar as Restrições de Tarefa

   Ao usar as Restrições de tarefa baseadas em data, você pode atualizar manualmente o Dia inicial das tarefas do modelo. Alguns exemplos de Restrições de Tarefa com base em data são Datas Fixas, Não Iniciar Antes de, Não Iniciar Mais Tarde do que, Deve Iniciar Em.

* Atualizar os predecessores da tarefa do modelo

## Dia de Término

O Dia de conclusão do modelo é o dia em que a última tarefa do modelo é concluída. Por padrão, todas as tarefas do modelo e o modelo mostram um Dia de conclusão 1, pois o Workfront assume que qualquer tarefa do modelo tem uma Duração de 1 dia. O Dia de conclusão das tarefas do modelo pode ser alterado e isso também altera o Dia de conclusão do modelo. O Dia de conclusão do modelo se torna a Data de conclusão planejada do projeto futuro e os Dias de conclusão das tarefas do modelo se tornam as Datas de conclusão planejadas das tarefas futuras do projeto.

A seguir estão algumas ações que podem alterar o Dia de conclusão das tarefas do modelo:

* Atualizar a duração das tarefas do modelo
* Atualizar as Restrições de Tarefa

   Ao usar Restrições de Tarefa baseadas em data, você pode atualizar manualmente o Dia de conclusão das tarefas do modelo. Alguns exemplos de Restrições de Tarefa com base em data são Datas Fixas, Não Concluir Antes de, Não Terminar Mais Tarde Que, Devem Terminar Em.

* Atualizar os predecessores da tarefa do modelo

## Trabalhar com modelos agendados a partir da conclusão

Você pode agendar um modelo a partir do dia de conclusão. Para obter mais informações, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Considere o seguinte ao trabalhar com modelos agendados a partir da Data de conclusão:

* Alterar o dia de início define a Restrição de tarefa como Deve começar em.
* Alterar o Dia de Conclusão define a Restrição de Tarefa como Deve Concluir.
* Quando o modelo é agendado a partir do dia de conclusão, o Dia da Restrição de Tarefa é calculado a partir do dia de conclusão.

   **Exemplo:** A duração do modelo é de 285 dias e você tem uma tarefa de modelo com duração de 60 dias. Se você definir a Restrição de Tarefa como Deve Iniciar em e Dia de Restrição como 120, você terá um Dia de Início de 165 (285 - 120) e um Dia de Conclusão de 225 (165 + 60). Portanto, ao editar o Dia de início, ele está sendo interpretado como Dia de restrição.
