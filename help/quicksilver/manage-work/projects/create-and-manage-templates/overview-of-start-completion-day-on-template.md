---
product-area: templates
navigation-topic: templates-navigation-topic
title: Visão Geral dos Dias de Início e Término em um modelo
description: Você pode usar modelos de projeto para capturar a maioria dos processos, informações e configurações repetíveis associados aos projetos em sua organização. Embora os projetos tenham datas de início e conclusão específicas, os modelos têm dias de início e conclusão genéricos como uma indicação de onde essas datas estarão no projeto, com base na linha do tempo geral do projeto.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Visão Geral dos Dias de Início e Término em um modelo

Você pode usar modelos de projeto para capturar a maioria dos processos, informações e configurações repetíveis associados aos projetos em sua organização. Embora os projetos tenham datas de início e conclusão específicas, os modelos têm dias de início e conclusão genéricos como uma indicação de onde essas datas estarão no projeto, com base na linha do tempo geral do projeto.

**Exemplo:** Se a Data de Início de um projeto for 1º de abril e você quiser que uma tarefa inicie em 3º de abril (dois dias após o início do projeto), a tarefa correspondente no modelo que cria o projeto deverá iniciar no Dia 2 do modelo, onde o primeiro dia do modelo é considerado Dia 0.

## Dia de Início

Considere o seguinte ao trabalhar com modelos e tarefas de modelo:

* Por padrão, os modelos têm um Dia de início de 0 e as tarefas do modelo e o modelo mostram um Dia de início de 0. O dia de início das tarefas do modelo pode mudar, mas isso não altera o dia de início do modelo.
* O dia de início de uma tarefa de modelo representa o número de dias úteis que o Workfront adiciona à Data de início planejada da tarefa quando um projeto é criado a partir do modelo. Por exemplo, você pode ter um modelo com apenas uma tarefa e o dia de início da tarefa de modelo é 4. O dia de início do modelo ainda é 0. Ao criar um projeto a partir desse modelo, onde o Modo de programação do projeto é Data inicial, e a Data inicial planejada do projeto é 1º de novembro de 2019, a tarefa recém-criada adiciona 4 dias a essa data e define o valor Data inicial planejada como 5 de novembro de 2019.

Veja a seguir algumas ações que podem alterar o Dia de início das tarefas do modelo:

* Atualizar a Duração das tarefas de modelo predecessoras
* Atualizar as Restrições da Tarefa

  Ao usar Restrições de Tarefa com base em data, você pode atualizar manualmente o Dia de Início das tarefas do modelo. Alguns exemplos de restrições de tarefas baseadas em datas são Datas fixas, Não iniciar antes de, Não iniciar depois de, Deve começar em.

* Atualizar as predecessoras da tarefa de modelo

## Dia de Término

O Dia de conclusão do modelo é o dia em que a última tarefa do modelo é concluída. Por padrão, todas as tarefas de modelo e o modelo mostram um Dia de conclusão de 1, porque a Workfront presume que qualquer tarefa de modelo tem uma Duração de 1 dia. O Dia de conclusão das tarefas do modelo pode mudar e isso também altera o Dia de conclusão do modelo. O Dia de Término do modelo se torna a Data de Término Planejada do projeto futuro e os Dias de Término das tarefas do modelo se tornam as Datas de Término Planejadas das tarefas do projeto futuras.

A seguir estão algumas ações que podem alterar o Dia de conclusão das tarefas do modelo:

* Atualizar a Duração das tarefas do modelo
* Atualizar as Restrições da Tarefa

  Ao usar Restrições de Tarefa com base em data, você pode atualizar manualmente o Dia de Conclusão das tarefas do modelo. Alguns exemplos de Restrições de Tarefas baseadas em datas são Datas Fixas, Não Terminar Antes De, Não Terminar Depois De, Deve Terminar Em.

* Atualizar as predecessoras da tarefa de modelo

## Trabalhar com modelos agendados a partir da conclusão

Você pode programar um modelo a partir do Dia de conclusão. Para obter mais informações, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Considere o seguinte ao trabalhar com modelos agendados a partir da Data de conclusão:

* Alterar o Dia de Início define a Restrição da Tarefa como Deve Iniciar em.
* Alterar o Dia de conclusão define a restrição da tarefa como Deve ser concluída em.
* Quando o modelo é programado a partir do Dia de Conclusão, o Dia de Restrição da Tarefa é calculado a partir do Dia de Conclusão.

  **Exemplo:** a duração do modelo é de 285 dias e você tem uma tarefa de modelo com duração de 60 dias. Se você definir a Restrição de Tarefa como Deve Iniciar em e o Dia de Restrição como 120, você terá um Dia de Início de 165 (285 - 120) e um Dia de Conclusão de 225 (165 + 60). Portanto, ao editar o Dia de início, ele é interpretado como um Dia de restrição.
