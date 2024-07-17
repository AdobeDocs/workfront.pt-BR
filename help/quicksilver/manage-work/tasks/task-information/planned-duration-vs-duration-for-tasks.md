---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Diferença entre a Duração Planejada e a Duração das tarefas
description: Duração é a quantidade de tempo entre o Início Planejado e a Data de Conclusão Planejada de um item de trabalho. As tarefas têm uma Duração e uma Duração planejada no Adobe Workfront, dependendo do Tipo de duração da tarefa.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Diferença entre a Duração Planejada e a Duração das tarefas

Duração é a quantidade de tempo entre o Início Planejado e a Data de Conclusão Planejada de um item de trabalho. As tarefas têm uma Duração e uma Duração planejada no Adobe Workfront, dependendo do Tipo de duração da tarefa.

Problemas e projetos não podem ser associados a um Tipo de duração e eles têm apenas uma duração.

## Duração da tarefa

Para tarefas, a Duração e a Duração planejada normalmente mostram o mesmo valor: o período de tempo entre a Data inicial planejada e a Data de conclusão planejada de uma tarefa.

Quando o Tipo de duração da tarefa é Orientado pelo Esforço, a Duração planejada diminui à medida que você adiciona recursos à tarefa.

**Exemplo:** Se uma tarefa com um Tipo de Duração de Esforço Orientado tiver uma Duração de 3 dias e você atribuir um recurso com um agendamento de tempo integral à tarefa, a Duração Planejada também será de 3 dias.

Se você atribuir três recursos com um agendamento de tempo integral à mesma tarefa, a Duração permanecerá 3 dias, mas a Duração planejada se tornará 1 dia. A Duração planejada também altera as datas de Início planejado e de Conclusão planejada da tarefa para refletir a nova Duração planejada. Como resultado, a linha do tempo do projeto também é afetada.
Você pode usar o Tipo de Duração Conduzida pelo Esforço ao atribuir uma tarefa a vários recursos. Isso reduz o tempo necessário para que o trabalho seja concluído na tarefa.

Para obter mais informações sobre o Tipo de Duração Conduzido pelo Esforço, consulte [Visão geral do Tipo de Duração: Conduzido pelo Esforço](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Duração do problema e do projeto

Problemas e projetos têm apenas um valor de Duração, que é a diferença entre a Data de início planejada e a Data de conclusão planejada do problema e do projeto, respectivamente.
