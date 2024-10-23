---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral de "Pode iniciar" para tarefas"
description: Quando uma tarefa está pronta para ser iniciada, o Adobe Workfront adiciona um indicador Pode iniciar à tarefa para identificar facilmente que é seguro começar a trabalhar nela. Você pode exibir esse indicador na exibição de uma lista de tarefas ou relatório.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Visão geral &quot;Pode iniciar&quot; para tarefas

Quando uma tarefa está pronta para ser iniciada, o Adobe Workfront adiciona um indicador Pode iniciar à tarefa para identificar facilmente que é seguro começar a trabalhar nela. Você pode exibir esse indicador na exibição de uma lista de tarefas ou relatório.

Quando a tarefa está pronta para ser trabalhada, o campo Pode Iniciar na tarefa é definido como Verdadeiro.

## Como o Workfront marca uma tarefa como &quot;Pode iniciar&quot;

O Workfront verifica os seguintes itens antes de marcar uma tarefa como Verdadeira para o campo Pode iniciar:

* Se o valor Pode Iniciar para o pai definido como Verdadeiro, se a tarefa tiver um pai. Se o valor do pai for Falso, todas as subtarefas terão o valor Pode Iniciar definido como Falso.
* Se os predecessores da tarefa e os predecessores de seus pais estão concluídos. Se estiverem concluídos, o valor Pode iniciar da tarefa será definido como Verdadeiro. Se qualquer um dos predecessores da tarefa ou os predecessores de seus pais não estiverem completos ou tiverem um status de Concluído-Pendente de Aprovação, o valor Pode Iniciar da tarefa será definido como Falso.
* Se o tipo de dependência da tarefa é Início-Início ou Início-Término. Se o tipo de dependência for Início-Início ou Início-Término, a tarefa dependente terá o sinalizador &quot;Pode iniciar&quot; definido como Verdadeiro depois que a tarefa predecessora estiver em andamento (ou depois que o percentual concluído da tarefa predecessora for maior que 1%).

  Para obter informações sobre predecessores de tarefas, consulte [Visão geral dos predecessores da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Considerações sobre a identificação de tarefas que estão prontas para serem iniciadas

* Se o Tipo de Dependência entre uma tarefa e suas predecessoras for Início-Início, a predecessora deverá iniciar antes que a relação predecessora seja considerada resolvida e as tarefas sucessoras possam iniciar. Para obter informações sobre tipos de dependência, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Se uma tarefa tiver uma predecessora entre projetos, a conclusão da predecessora não acionará o indicador Pode iniciar para ser aplicado automaticamente à sucessora. Você deve recalcular manualmente a linha do tempo do projeto do sucessor ou o Workfront deve recalculá-la automaticamente, antes que a tarefa sucessora seja exibida como uma tarefa Pode iniciar. Para obter mais informações sobre o recálculo das linhas de tempo do projeto, consulte [Recalcular linhas de tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

  Para obter informações sobre predecessores entre projetos, consulte [Criar predecessores entre projetos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
