---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Visão Geral do Loop de Dependência de Tarefa
description: Ao adicionar relações de predecessoras a tarefas, você pode encontrar loops de dependência. Para obter informações sobre predecessores, consulte Visão geral dos predecessores da tarefa.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
TQID: https://experienceleague.adobe.com/cQbPOUES-tmSgZTpXrft8lQby-ubPmI-TZ1PjdGURMc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 1%

---

# Visão geral do loop de dependência da tarefa

Ao adicionar relações de predecessoras a tarefas, você pode encontrar loops de dependência. Para obter informações sobre predecessores, consulte [Visão geral dos predecessores da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Visão geral do loop de dependência

Os loops de dependência ocorrem quando você tem duas ou mais tarefas que dependem umas das outras para serem concluídas. O Adobe Workfront não permite criar uma relação de predecessora entre tarefas se criar um loop de dependência.

**Exemplo:** a Tarefa 2 é predecessora da Tarefa 1, o que significa que você deve concluir a Tarefa 2 antes de começar a trabalhar na Tarefa 1.

Se você tentar tornar a Tarefa 1 uma predecessora da Tarefa 2, receberá um erro de loop de dependência porque não poderá iniciar a Tarefa 1 até que a Tarefa 2 tenha sido concluída, mas a tarefa 2 não poderá ser iniciada até que a Tarefa 1 seja concluída.

![Mensagem de erro do loop de dependência](assets/dependency-loop-error-message-350x209.png)

![Loop de dependência na lista de tarefas](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Considerações sobre loops de dependência

* Os loops de dependência podem envolver mais de duas tarefas. Às vezes, qualquer número de pais das tarefas que você está conectando a um relacionamento de predecessor é o que cria o loop de dependência.
* Um loop de dependência também pode ocorrer se você tentar tornar um pai o predecessor de um filho.
* No caso de um loop de dependência, não é possível salvar as tarefas ou o projeto. Para corrigir o loop de dependência, você deve reavaliar a relação de predecessora entre as tarefas listadas na mensagem de erro e remover os conflitos antes de salvar as tarefas ou o projeto.


