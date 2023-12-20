---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Visão geral da modificação de atribuições de tarefas
description: É possível atribuir tarefas ou cancelar a atribuição de tarefas de usuários, equipes ou funções de trabalho. Você pode atribuir vários recursos ao mesmo tempo ou apenas um recurso. Você pode atribuir uma tarefa de cada vez ou várias tarefas em massa.
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 0%

---

# Visão geral da modificação de atribuições de tarefas

É possível atribuir tarefas ou cancelar a atribuição de tarefas de usuários, equipes ou funções de trabalho. Você pode atribuir vários recursos ao mesmo tempo ou apenas um recurso. Você pode atribuir uma tarefa de cada vez ou várias tarefas em massa.

>[!TIP]
>
>Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos.
>
>Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
>
>* Reatribuir o item de trabalho aos recursos ativos.
>* Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.
>

Este artigo contém informações gerais sobre o impacto da modificação de atribuições de tarefas. Para obter informações sobre como atribuir tarefas, consulte os seguintes artigos:

* Para obter informações sobre atribuição de tarefas, consulte [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md) e [Modificar atribuições de vários usuários em uma lista de tarefas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Para obter informações sobre como modificar atribuições em várias tarefas na área Programação, consulte &quot;Modificar atribuições de vários usuários a tarefas nas áreas Programação&quot;.
* Para obter informações sobre como atribuir tarefas usando o Balanceador de carga de trabalho, consulte [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Algumas informações neste artigo também se aplicam às atribuições aos problemas. Para obter mais informações sobre a atribuição de problemas e considerações adicionais, consulte [Visão geral da modificação de atribuições de emissão](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Quando modificar atribuições de usuário em tarefas

Talvez você queira modificar as atribuições de usuário para tarefas por vários motivos, incluindo os seguintes:

* Usuários ingressam ou saem da sua equipe
* Um usuário tira férias que se estendem além das datas de vencimento das tarefas

  >[!NOTE]
  >
  >Ao atribuir usuários para trabalhar, sua disponibilidade de acordo com seus agendamentos afetará as Datas Planejadas e Projetadas das tarefas. Para obter informações sobre programações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Uma função ou usuário específico é definido como o destinatário de várias tarefas e você deseja modificar rapidamente todos os itens a serem atribuídos a um usuário ou função diferente

## Considerações para várias atribuições para funções de trabalho, equipes e usuários

Considere o seguinte ao atribuir vários recursos a um item de trabalho:

* Os usuários podem ter mais de uma função de trabalho associada ao seu perfil. Para obter informações sobre como associar usuários a funções de trabalho, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Geralmente, tarefas ou problemas são atribuídos primeiro a uma ou várias funções de trabalho ou a uma equipe. Quando os projetos estiverem prontos para serem iniciados, talvez também seja necessário atribuí-los aos usuários.\
  Se uma tarefa ou um problema for atribuído a uma ou várias funções e você também atribuir um usuário, o Adobe Workfront decide qual função de trabalho deve ser associada ao usuário adicional (se houver) de acordo com as seguintes regras:

   * Se houver apenas uma função de trabalho atribuída e ela corresponder à função principal do usuário, a tarefa ou o problema será atribuído apenas ao usuário que desempenha sua função principal.
   * Se houver várias funções atribuídas e pelo menos uma das funções corresponder às funções secundárias do usuário, a tarefa ou o problema será atribuído ao usuário que desempenha uma de suas Outras funções — que o Workfront seleciona aleatoriamente se houver várias correspondências — bem como quaisquer funções adicionais atribuídas.
   * Se houver uma ou mais funções de trabalho atribuídas e não houver correspondência entre as funções do usuário, a tarefa ou o problema será atribuído à função ou às funções, bem como ao usuário.

* Se uma tarefa ou um problema for atribuído a uma equipe e você também atribuir um usuário, a tarefa ou o problema permanecerá atribuído à equipe e ao usuário.

## Como a remoção de atribuídos afeta as horas da tarefa e as porcentagens de alocação

A remoção de usuários pode afetar as horas de tarefas e as porcentagens de alocação. O efeito que a remoção de um usuário tem na tarefa depende do Tipo de Duração que foi selecionado para a tarefa. Para obter informações sobre o Tipo de duração, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Ao excluir um usuário de uma tarefa com os seguintes Tipos de duração:

* **Simples:** As horas planejadas atribuídas a esse usuário são subtraídas do total de horas planejadas da tarefa.

  >[!IMPORTANT]
  >
  >Isso pode afetar negativamente o plano do projeto, pois altera o total de horas planejadas da tarefa e do projeto.

* **Orientado pelo esforço:** A porcentagem de alocação não é alterada para outros usuários.
* **Atribuição Calculada:** As porcentagens de alocação de outros usuários são ajustadas para que o total seja igual a 100%.
* **Trabalho Calculado:** A porcentagem de alocação não é alterada para outros usuários.

## Considerações sobre o cancelamento da atribuição de tarefas

Você pode remover atribuições de uma tarefa de cada vez ou remover atribuições de várias tarefas em massa.

Para obter mais informações sobre como remover atribuições de tarefas em massa, consulte [Modificar atribuições de vários usuários em uma lista de tarefas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Considere o seguinte ao remover atribuições de tarefas:

* Quando você cancela a atribuição de um usuário de uma tarefa, a tarefa permanece atribuída à função de trabalho que o usuário desempenhou na tarefa.
* Quando você cancela a atribuição de uma função de trabalho ou de uma equipe a uma tarefa, a tarefa permanece sem atribuição se não estiver atribuída a outros recursos.
