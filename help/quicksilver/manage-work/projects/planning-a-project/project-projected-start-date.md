---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão Geral da Data de Início Projetada do projeto
description: A Data de Início Projetada é uma data em tempo real em que o projeto vai iniciar com base na Data de Início Projetada da primeira tarefa do projeto.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Visão Geral da Data de Início Projetada do projeto

## Visão geral da Data de Início Projetada para projetos e tarefas

A Data de Início Projetada é uma data em tempo real em que o projeto vai iniciar com base na Data de Início Projetada da primeira tarefa do projeto.

Quando você planeja um projeto pela primeira vez, a Data Inicial Planejada e a Data Inicial Projetada das tarefas e do projeto são idênticas. Como podem ocorrer atrasos ou as tarefas serem concluídas anteriormente, a Data de Início Projetada pode se tornar diferente da Data de Início Planejada.

Alterações na Data Inicial Projetada da primeira tarefa no projeto acionam alterações na Data Inicial Projetada do projeto.

## Modificar a Data de Início Projetada de uma tarefa

A Data de Início Projetada para um projeto ou uma tarefa é um cálculo feito pela Adobe Workfront e não pode ser modificada manualmente.

Os seguintes eventos podem acionar uma modificação na Data inicial projetada de uma tarefa:

* Quando você começa a trabalhar em uma tarefa, a Data Inicial Real da tarefa se torna a Data Inicial Projetada.
* Se a Data Inicial Planejada de uma tarefa for aprovada, a Data Inicial Projetada será movida para o futuro, indicando a data mais próxima disponível para o início da tarefa.\
  O Workfront leva em conta a quantidade de Horas planejadas na tarefa, bem como a programação do projeto ou do usuário atribuído à tarefa ao calcular a data mais próxima disponível para o início da tarefa.
* As tarefas predecessoras que estão atrasadas têm um impacto na Data de início projetada de suas tarefas dependentes. A Data Inicial Projetada das tarefas dependentes é movida de acordo com o Tipo de Dependência do relacionamento antecessor e de acordo com as Datas Projetadas dos predecessores.

Se qualquer uma dessas tarefas for a primeira tarefa de um projeto, a Data Inicial Projetada do projeto será alterada para corresponder à Data Inicial Projetada dessa tarefa.

## Localize a Data Inicial Projetada de um projeto ou tarefa

Você pode localizar a Data de início projetada de um projeto ou tarefa nas seguintes áreas do Workfront:

* Você pode adicioná-lo a um projeto ou a um relatório ou visualização de tarefa.

  Para obter mais informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Na seção Detalhes de um projeto ou na seção Detalhes de uma tarefa.
