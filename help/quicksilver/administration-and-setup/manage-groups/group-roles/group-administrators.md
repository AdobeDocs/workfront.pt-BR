---
title: Administradores de Grupos
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Os administradores do Adobe Workfront em uma grande organização com muitos departamentos podem não querer gerenciar todos os departamentos e grupos da organização nesses departamentos. Em vez disso, eles podem criar um grupo para cada departamento e subgrupos dentro desse grupo, cada um gerenciado por um administrador de grupo.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 1%

---

# Admins de grupo

<!-- Audited: 12/2023 -->

Os administradores do Adobe Workfront em uma grande organização com muitos departamentos podem não querer gerenciar todos os departamentos e grupos da organização nesses departamentos. Em vez disso, eles podem criar um grupo para cada departamento e subgrupos dentro desse grupo, cada um gerenciado por um administrador de grupo.

Um administrador de grupo pode gerenciar as necessidades de um grupo, como associação de usuário, modelos de layout, dados personalizados, status e preferências.

Até 14 níveis de subgrupos podem existir em um grupo.

>[!NOTE]
>
>Todos os administradores de grupo na hierarquia acima de um subgrupo têm direitos administrativos para gerenciar esse subgrupo.

Para obter informações sobre como criar e gerenciar grupos, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Gerenciar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Além disso, consulte [Visão geral dos subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Designar administradores de grupo

Todos os grupos de nível superior devem ter pelo menos um administrador de grupo. Um administrador do Workfront ou de um grupo pode atribuir administradores de grupo aos subgrupos do grupo, mas isso não é necessário. Para obter mais informações, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Se você for um administrador do Workfront, recomendamos fazer o seguinte antes de designar usuários como administradores de grupo:

* Anote o número atual de administradores do Workfront em seu sistema.
* Anote o número de grupos que você tem em seu sistema.
* Determine se você pode alterar o nível de acesso de alguns dos administradores do Workfront e designá-los como administradores de grupo.

  Para obter mais informações sobre os recursos de administradores de grupo, consulte [Tarefas feitas por administradores de grupo](#tasks-done-by-group-administrators) neste artigo.

* Determine se você deseja que os administradores de grupo façam logon como outros usuários ou redefinam senhas para os usuários nos grupos que você administra. É necessário acesso adicional para executar essas tarefas, conforme explicado abaixo em [Acesso necessário para administradores de grupo](#access-needed-for-group-administrators).
* Para melhorar o gerenciamento de usuários, considere atribuir grupos ou subgrupos em vez de usuários aos seguintes objetos:

   * Modelos de layout
   * Cronogramas
   * Planilhas de horas recorrentes

## Acesso necessário para administradores de grupo {#access-needed-for-group-administrators}

Todos os administradores de grupo precisam ter

* Uma licença de plano no modelo atual de preços e pacotes
* Uma licença Standard no novo modelo de preços e pacotes

Recomendamos que os administradores de grupo tenham acesso de edição aos usuários para que possam executar as seguintes tarefas:

* Faça logon como outros usuários nos grupos e subgrupos que eles gerenciam.
* Redefina a senha de outro usuário nos grupos que ele gerencia.

>[!IMPORTANT]
>
>Os administradores de grupo devem ter acesso maior do que aqueles que gerenciam; caso contrário, não poderão visualizar ou modificar níveis de acesso mais baixos.
>&#x200B;>Para obter instruções sobre como conceder esse acesso, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Para um administrador de grupo que precisa atribuir perfis de folha de horas a usuários em seus grupos e subgrupos, também recomendamos Acesso administrativo a folhas de horas e horas. Para obter instruções sobre como conceder esse acesso, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Tarefas feitas por administradores de grupo {#tasks-done-by-group-administrators}

Como administrador de grupo, você pode realizar as tarefas descritas abaixo para gerenciar os grupos que supervisiona. Alguns deles são o mesmo que as habilidades oferecidas a um administrador do Workfront.

>[!NOTE]
>
>No novo modelo de preços e pacotes, você deve ter um plano do Prime ou superior para executar o seguinte:
>
> * Criar notificações de evento de grupo
> * Configurar preferências do projeto do grupo
> * Configurar preferências de tarefas de grupo e problemas
> * Desbloquear a configuração de preferências de subgrupo
> * Preferências de Horas e Planilha de Horas do Grupo
> * Desbloquear a preferência de horas e planilhas de horas

### Gerenciar membros do grupo {#manage-group-members}

* Crie, edite e exclua subgrupos dentro dos grupos e subgrupos que você gerencia. Para obter instruções, consulte [Criar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Adicione todos os usuários para os quais você tem acesso de Edição aos seus grupos e subgrupos. Ou adicione usuários a grupos e subgrupos editando seus perfis.

  Você também pode atualizar os campos no perfil de um membro do grupo se tiver a permissão Administrador de usuário (usuários do grupo) ativada em seu nível de acesso.

  Para obter mais informações, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Os administradores do Workfront podem substituir alterações feitas em associações de grupo por um administrador de grupo.

* Redefina senhas para os usuários que são membros dos grupos que você gerencia. Para obter mais informações, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Efetue login como usuários membros dos grupos que você gerencia. Para obter mais informações, consulte [Fazer logon como outro usuário](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Exiba o número de licenças disponíveis disponíveis para o seu grupo e os subgrupos abaixo dele. Para obter mais informações, consulte [Gerenciar licenças disponíveis em seu sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Gerenciar objetos de grupo {#manage-group-objects}

* Crie Modelos de layout de nível de grupo e associe-os aos grupos e subgrupos que você gerencia. Para obter mais informações, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Crie perfis de planilhas de horas no nível do grupo, associe-os a usuários e grupos que você gerencia, e gere planilhas de horas manualmente. Para obter mais informações, consulte [Criar, editar e atribuir perfis de folha de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Sem acesso administrativo aos processos de aprovação, crie e edite processos de aprovação para os grupos e subgrupos que você gerencia. Para obter mais informações, consulte [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Para obter informações sobre acesso administrativo a processos de aprovação, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Crie agendamentos e associe-os a um grupo gerenciado por você. Para obter mais informações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Gerenciar uma equipe atribuída a um grupo gerenciado por você, sem ser um membro da equipe. Além disso, crie um relatório de equipe com base no campo Grupo para identificar a qual grupo uma determinada equipe está atribuída. Para obter mais informações, consulte [Criar uma equipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Restaure um projeto que esteja associado a um grupo que você gerencia, juntamente com qualquer tarefa, problema ou documento associado ao projeto. Para obter mais informações, consulte [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Gerenciar preferências e ferramentas do grupo {#manage-group-preferences-and-tools}

* Quando uma preferência de projeto, de tarefa ou de problema, ou uma preferência de planilhas de horas e horas for desbloqueada para grupos em todo o sistema, edite essa preferência para os grupos que você gerencia. Essas preferências afetam o comportamento do projeto, tarefa e problema. Para obter mais informações, consulte:

   * [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Crie e edite status de grupos para grupos que você gerencia. Para obter mais informações, consulte [Criar ou editar o status de um grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Configure uma notificação de evento para grupos que você gerencia. Você pode fazer isso somente depois que um administrador do Workfront desbloqueia a capacidade de configurar notificações de eventos para grupos em todo o sistema. Para obter mais informações, consulte [Exibir e configurar notificações de eventos para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
