---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral da data de início prevista do projeto
description: A Data inicial prevista é uma data em tempo real de início do projeto com base na Data inicial prevista da primeira tarefa do projeto.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Visão geral da data de início prevista do projeto

## Visão geral da data inicial projetada para projetos e tarefas

A Data inicial prevista é uma data em tempo real de início do projeto com base na Data inicial prevista da primeira tarefa do projeto. 

Quando você planeja um projeto pela primeira vez, a Data Inicial Planejada e a Data Inicial Projetada das tarefas e do projeto são idênticas. Como os atrasos podem ocorrer ou as tarefas podem ser concluídas anteriormente, a Data inicial projetada pode se tornar diferente da Data inicial planejada. 

As alterações na Data de Início Projetada da primeira tarefa no acionador do projeto são alteradas na Data de Início Projetada do projeto. 

## Modificar a Data Inicial Projetada de uma tarefa

A Data inicial projetada para um projeto ou tarefa é um cálculo feito pela Adobe Workfront e não pode ser modificado manualmente. 

Os seguintes eventos podem acionar uma modificação na Data de início projetada de uma tarefa:

* Quando você começa a trabalhar em uma tarefa, a Data de Início Real da tarefa se torna a Data de Início Projetada.
* Se a Data Inicial Planejada de uma tarefa for aprovada, a Data Inicial Projetada será movida para o futuro, indicando a data mais rápida disponível para a tarefa ser iniciada.\
   O Workfront considera a quantidade de Horas Planejadas na tarefa, bem como o agendamento do projeto ou do usuário atribuído à tarefa ao calcular a data mais antiga disponível para a tarefa iniciar. 
* As tarefas predecessoras que estão sendo executadas anteriormente têm impacto na Data inicial projetada de suas tarefas dependentes. A Data Inicial Projetada das tarefas dependentes é movida de acordo com o Tipo de Dependência da relação do antecessor e de acordo com as Datas Projetadas dos antecessores. 

Se qualquer uma dessas tarefas for a primeira tarefa em um projeto, a Data inicial prevista do projeto será alterada para corresponder à Data inicial projetada dessa tarefa. 

## Localizar a Data Inicial Projetada de um projeto ou tarefa

Você pode localizar a Data inicial projetada de um projeto ou de uma tarefa nas seguintes áreas do Workfront:

* Você pode adicioná-lo a um projeto, a um relatório ou uma visualização de tarefa.

   Para obter mais informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Na seção Detalhes do projeto de um projeto ou na seção Detalhes da tarefa de uma tarefa.
