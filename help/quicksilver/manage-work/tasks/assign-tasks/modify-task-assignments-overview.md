---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Visão geral da modificação de atribuições de tarefa
description: Você pode atribuir tarefas ou cancelar a atribuição de tarefas de usuários, equipes ou funções de trabalho. Você pode atribuir vários recursos ao mesmo tempo ou apenas um recurso. É possível atribuir uma tarefa de cada vez ou várias tarefas em massa.
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: f4cc5ae89c8746ec4c40ece88bfdb21dc1996575
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Visão geral da modificação de atribuições de tarefa

Você pode atribuir tarefas ou cancelar a atribuição de tarefas de usuários, equipes ou funções de trabalho. Você pode atribuir vários recursos ao mesmo tempo ou apenas um recurso. É possível atribuir uma tarefa de cada vez ou várias tarefas em massa.

>[!TIP]
>
>Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários ativos, funções de trabalho e equipes.
>
>Se um usuário, uma função de trabalho ou uma equipe tiver sido atribuída antes de ser desativada, ela permanecerá atribuída ao item de trabalho. Nesse caso, recomendamos o seguinte:
>
>* Atribua novamente o item de trabalho aos recursos ativos.
>* Associe os usuários em uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.
>


Este artigo contém informações gerais sobre o impacto da modificação de atribuições de tarefa. Para obter informações sobre como atribuir tarefas, consulte os seguintes artigos:

* Para obter informações sobre atribuição de tarefas, consulte [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md) e [Modificar várias atribuições de usuário em uma lista de tarefas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Para obter informações sobre a modificação de atribuições em várias tarefas na área Agendamento, consulte &quot;Modificar várias atribuições de usuários para tarefas nas áreas de Agendamento&quot;.
* Para obter informações sobre a atribuição de tarefas usando o Balanceador de Carga de Trabalho, consulte [Visão Geral da atribuição de trabalho no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Algumas informações neste artigo também se aplicam a atribuições para problemas. Para obter mais informações sobre atribuição de problemas e considerações adicionais, consulte [Modificar visão geral de atribuições de emissão](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Quando modificar atribuições de usuários em tarefas

Talvez você queira modificar as atribuições de usuários para tarefas por uma variedade de motivos, incluindo o seguinte:

* Os usuários se associam ou saem da equipe
* Um usuário tira férias que se estendem além das datas de vencimento das tarefas

   >[!NOTE]
   >
   >Ao atribuir usuários ao trabalho, sua disponibilidade de acordo com suas programações afeta as Datas Planejadas e Projetadas das tarefas. Para obter informações sobre programações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Uma função ou usuário específico é definido como o destinatário para várias tarefas e você deseja modificar rapidamente todos os itens a serem atribuídos a um usuário ou função diferente

## Considerações para várias atribuições em funções, equipes e usuários

Considere o seguinte ao atribuir vários recursos a um item de trabalho:

* Os usuários podem ter mais de uma função de trabalho associada ao perfil. Para obter informações sobre como associar usuários a funções de jobs, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Tarefas ou problemas normalmente são atribuídas pela primeira vez a uma ou várias funções de trabalho ou a uma equipe. Quando os projetos estiverem prontos para o início, eles também poderão precisar ser atribuídos aos usuários.\
   Se uma tarefa ou um problema for atribuído a uma ou várias funções e você também atribuir um usuário, o Adobe Workfront decide qual função de trabalho associar ao usuário adicional (se houver) de acordo com as seguintes regras:

   * Se houver apenas uma função de trabalho atribuída e ela corresponder à Função Principal do usuário, a tarefa ou problema será atribuído somente ao usuário que cumpre sua Função Principal.
   * Se houver várias funções atribuídas e pelo menos uma delas corresponder às funções secundárias do usuário, a tarefa ou problema será atribuído ao usuário que cumpre uma de suas Outras funções — que o Workfront seleciona aleatoriamente se houver várias correspondências — bem como quaisquer funções adicionais atribuídas.
   * Se houver uma ou mais funções de trabalho atribuídas e não houver correspondências com as funções do usuário, a tarefa ou problema será atribuído tanto à função ou às funções como ao usuário.

* Se uma tarefa ou um problema for atribuído a uma equipe e você também atribuir um usuário, a tarefa ou o problema permanecerá atribuído à equipe e ao usuário.

## Como a remoção de destinatários afeta as horas da tarefa e as porcentagens de alocação

A remoção de usuários pode afetar as horas da tarefa e as porcentagens de alocação. O efeito que a remoção de um usuário tem na tarefa depende do Tipo de duração que foi selecionado para a tarefa. Para obter informações sobre Tipo de duração, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Ao excluir um usuário de uma tarefa com os seguintes Tipos de duração:

* **Simples:** As horas planejadas atribuídas a esse usuário são subtraídas do total de horas planejadas da tarefa.

   >[!IMPORTANT]
   >
   >Isso pode afetar negativamente seu plano de projeto, pois altera o total de horas planejadas para a tarefa e o projeto.

* **Impulsionado pelo esforço:** A porcentagem de alocação não é alterada para outros usuários.
* **Atribuição calculada:** As porcentagens de alocação de outros usuários são ajustadas para que o total seja igual a 100%.
* **Trabalho calculado:** A porcentagem de alocação não é alterada para outros usuários.

## Considerações sobre o cancelamento da atribuição de tarefas

Você pode remover atribuições de uma tarefa de cada vez, ou pode remover atribuições de várias tarefas em massa.

Para obter mais informações sobre como remover atribuições de tarefas em massa, consulte [Modificar várias atribuições de usuário em uma lista de tarefas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Considere o seguinte ao remover atribuições de tarefas:

* Quando você cancela a atribuição de um usuário de uma tarefa, a tarefa permanece atribuída à função de trabalho que o usuário realizou na tarefa.
* Ao cancelar a atribuição de uma função de trabalho ou de uma equipe de uma tarefa, a tarefa permanece não atribuída se não estiver atribuída a nenhum outro recurso.
