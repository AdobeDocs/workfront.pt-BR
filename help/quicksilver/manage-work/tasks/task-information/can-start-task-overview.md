---
content-type: overview
product-area: projects
navigation-topic: task-information
title: '`Can Start` overview for tasks'
description: Quando uma tarefa está pronta para iniciar, o Adobe Workfront adiciona um indicador Pode iniciar à tarefa para identificar facilmente se é seguro começar a trabalhar na tarefa. Você pode exibir esse indicador na exibição de uma lista de tarefas ou relatório.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Visão geral de &quot;Pode iniciar&quot; para tarefas

Quando uma tarefa está pronta para iniciar, o Adobe Workfront adiciona um indicador Pode iniciar à tarefa para identificar facilmente se é seguro começar a trabalhar na tarefa. Você pode exibir esse indicador na exibição de uma lista de tarefas ou relatório.

Quando a tarefa está pronta para ser trabalhada, o campo Pode iniciar da tarefa é definido como Verdadeiro.

## Como o Workfront marca uma tarefa como &quot;Pode iniciar&quot;

O Workfront verifica os seguintes itens antes de marcar uma tarefa como True para o campo Can Start :

* Se a tarefa tiver um pai, ela verificará se o valor de Pode Iniciar do pai está definido como True. Se o valor para o pai for False, todas as subtarefas também terão o valor Pode Iniciar definido como False. 
* Verifica também se os antecessores da tarefa, bem como os antecessores dos seus pais, estão completos. Se estiverem concluídos, o valor Pode iniciar da tarefa será definido como Verdadeiro. Se algum antecessor da tarefa ou antecessor de seus pais não estiver concluído ou tiver um status de Aprovação Concluído Pendente, o valor Pode Iniciar da tarefa será definido como Falso. 

   Para obter informações sobre predecessores de tarefas, consulte [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Considerações sobre a identificação de tarefas prontas para iniciar

* Se o Tipo de Dependência entre uma tarefa e seus antecessores for Início, o antecessor deverá iniciar antes que o relacionamento do antecessor seja considerado resolvido e as tarefas sucessoras possam ser iniciadas. Para obter informações sobre tipos de dependência, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Se uma tarefa tiver um antecessor entre projetos, a conclusão do antecessor não acionará o indicador Pode Iniciar para ser aplicado automaticamente ao sucessor. Você deve recalcular manualmente a linha do tempo do projeto do sucessor ou o Workfront deve recalcular automaticamente, antes que a tarefa do sucessor seja exibida como uma tarefa Pode iniciar . Para obter mais informações sobre o recálculo de linhas do tempo do projeto, consulte [Recalcular linhas do tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

   Para obter informações sobre predecessores entre projetos, consulte [Criar antecessores entre projetos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
