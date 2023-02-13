---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Visão geral do loop de dependência de tarefa
description: Ao adicionar relações do antecessor às tarefas, você pode encontrar loops de dependência. Para obter informações sobre antecessores, consulte Visão geral dos antecessores de tarefa.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Visão geral do loop de dependência de tarefa

Ao adicionar relações do antecessor às tarefas, você pode encontrar loops de dependência. Para obter informações sobre predecessores, consulte [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Visão geral do loop de dependências

Os loops de dependência ocorrem quando você tem duas ou mais tarefas que dependem umas das outras para serem concluídas. O Adobe Workfront não permite que você crie uma relação de antecessor entre tarefas se criar um loop de dependência.

**Exemplo:** A Tarefa 2 é um antecessor da Tarefa 1, o que significa que você deve concluir a Tarefa 2 antes de começar a trabalhar na Tarefa 1.

Se você tentar fazer da Tarefa 1 um antecessor da Tarefa 2, você receberá um erro de loop de dependência porque não poderá iniciar a Tarefa 1 até que a Tarefa 2 tenha sido concluída, mas a tarefa 2 não poderá ser iniciada até que a Tarefa 1 seja concluída.

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Considerações sobre loops de dependência

* Os loops de dependência podem envolver mais de duas tarefas. Às vezes, qualquer número de pais das tarefas que você está conectando com um relacionamento antecessor é aquele que está criando o ciclo de dependência.
* Um loop de dependência também pode ocorrer se você tentar fazer de um pai o antecessor de um filho.
* No caso de um loop de dependência, não é possível salvar as tarefas ou o projeto. Para corrigir o loop de dependência, é necessário reavaliar o relacionamento do antecessor entre as tarefas listadas na mensagem de erro e remover os conflitos antes de salvar as tarefas ou o projeto.

 
