---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral de "Pode iniciar" para tarefas
description: Quando uma tarefa está pronta para ser iniciada, o Adobe Workfront adiciona um indicador Pode iniciar à tarefa para identificar facilmente que é seguro começar a trabalhar nela. Você pode exibir esse indicador na exibição de uma lista de tarefas ou relatório.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
TQID: https://experienceleague.adobe.com/jb8Vj9wMNCQj31cgjHMIm6M0RH3VusK5jBdNx233yjw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 440
ht-degree: 1%

---

# Visão geral de tarefas “Prontas para iniciar”

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
