---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Diferença entre Duração planejada e Duração das tarefas
description: Duração é o tempo entre o Início Planejado e a Data de Conclusão Planejada de um item de trabalho. As tarefas têm uma Duração e uma Duração planejada no Adobe Workfront, dependendo do Tipo de duração da tarefa.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Diferença entre Duração planejada e Duração das tarefas

Duração é o tempo entre o Início Planejado e a Data de Conclusão Planejada de um item de trabalho. As tarefas têm uma Duração e uma Duração planejada no Adobe Workfront, dependendo do Tipo de duração da tarefa.

Problemas e projetos não podem ser associados a um Tipo de duração e eles têm apenas uma Duração.

## Duração da tarefa

Para tarefas, a Duração e a Duração planejada normalmente mostram o mesmo valor: o período de tempo entre a Data Inicial Planejada e a Data de Conclusão Planejada de uma tarefa.

Quando o Tipo de duração da tarefa é Orientada ao Esforço, a Duração Planejada diminui à medida que você adiciona recursos à tarefa.

**Exemplo:** Se uma tarefa com um Tipo de duração de esforço determinado tiver uma Duração de 3 dias e você atribuir um recurso com uma programação de tempo completo à tarefa, a Duração planejada também será de 3 dias.

Se você atribuir três recursos com uma programação de tempo integral para a mesma tarefa, a Duração fica em 3 dias, mas a Duração Planejada se torna 1 dia. A Duração Planejada também altera as datas Inicial Planejada e Conclusão Planejada da tarefa para refletir a nova Duração Planejada. Como resultado, a linha do tempo do projeto também é afetada.
Você pode usar o Tipo de duração orientada por esforço ao atribuir uma tarefa a vários recursos. Isso reduz o tempo necessário para concluir o trabalho na tarefa.

Para obter mais informações sobre o Tipo de Duração Orientada pelo Esforço, consulte [Visão geral do Tipo de duração: Esforço orientado](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Emissão e duração do projeto

As emissões e os projetos têm apenas um valor de Duração, que é a diferença entre a Data Inicial Planejada e a Data de Conclusão Planejada da emissão e do projeto, respectivamente.
