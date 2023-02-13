---
title: Administradores do grupo
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Os administradores da Adobe Workfront em uma grande organização com muitos departamentos talvez não queiram gerenciar todos os departamentos e grupos da organização nesses departamentos. Em vez disso, eles podem criar um grupo para cada departamento e subgrupos dentro desse grupo, cada um gerenciado por um administrador de grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 03667fbdd1b0d68b9ad2d2db4a1ed85b8136062b
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---

# Administradores do grupo

Os administradores da Adobe Workfront em uma grande organização com muitos departamentos talvez não queiram gerenciar todos os departamentos e grupos da organização nesses departamentos. Em vez disso, eles podem criar um grupo para cada departamento e subgrupos dentro desse grupo, cada um gerenciado por um administrador de grupo.

Um administrador de grupo pode gerenciar as necessidades de um grupo, como associação de usuário, modelos de layout, dados personalizados, status e preferências.

Podem existir até 14 níveis de subgrupos em um grupo.

>[!NOTE]
>
>Todos os administradores de grupo na hierarquia acima de um subgrupo têm direitos administrativos para gerenciar esse subgrupo.

Para obter informações sobre como criar e gerenciar grupos, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Gerenciar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Além disso, consulte [Visão geral de subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Designando administradores de grupo

Cada grupo de nível superior deve ter pelo menos um administrador de grupo. Um administrador ou administrador do Workfront de um grupo pode atribuir administradores de grupo aos subgrupos do grupo, mas isso não é necessário. Para obter mais informações, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Se você for um administrador do Workfront, recomendamos que faça o seguinte antes de designar usuários como administradores de grupo:

* Anote o número atual de administradores do Workfront em seu sistema.
* Anote o número de grupos que você tem em seu sistema.
* Determine se é possível alterar o nível de acesso de alguns administradores do Workfront e designá-los como administradores de grupo.

   Para obter mais informações sobre os recursos dos administradores de grupo, consulte [Tarefas realizadas pelos administradores do grupo](#tasks-done-by-group-administrators).

* Determine se você deseja que os administradores de grupo possam fazer logon como outros usuários ou redefinir senhas para usuários nos grupos que você administra. É necessário acesso adicional para executar essas tarefas, como explicado em [Acesso necessário para administradores de grupo](#access-needed-for-group-administrators).
* Para um melhor gerenciamento de usuários, considere atribuir grupos ou subgrupos em vez de usuários aos seguintes objetos:

   * Modelos de layout
   * Cronogramas
   * Planilhas de horas recorrentes

## Acesso necessário para administradores de grupo {#access-needed-for-group-administrators}

Todos os administradores de grupo precisam ter uma licença Plan .

Recomendamos que os administradores de grupo tenham acesso ao Edit para que possam executar as seguintes tarefas:

* Faça logon como outros usuários nos grupos e subgrupos gerenciados.
* Redefina a senha de outro usuário nos grupos que ele gerencia.

>[!IMPORTANT]
>
>Os administradores de grupo devem ter um acesso mais elevado do que os que gerem; caso contrário, eles não poderão visualizar ou modificar níveis de acesso mais baixos.
>Para obter instruções sobre como conceder esse acesso, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Para um administrador de grupo que precisa atribuir perfis de folha de ponto aos usuários em seus grupos e subgrupos, também recomendamos acesso Administrativo a folhas de ponto e horas. Para obter instruções sobre como conceder esse acesso, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Tarefas realizadas pelos administradores do grupo {#tasks-done-by-group-administrators}

Como administrador de grupo, você pode realizar as tarefas abaixo para gerenciar os grupos que você supervisiona. Alguns deles são as mesmas capacidades oferecidas a um administrador do Workfront.

* [Gerenciar membros do grupo](#manage-group-members)
* [Gerenciar objetos de grupo](#manage-group-objects)
* [Gerenciar preferências de grupo e ferramentas](#manage-group-preferences-and-tools)

### Gerenciar membros do grupo {#manage-group-members}

* Crie, edite e exclua subgrupos dentro dos grupos e subgrupos que você gerencia. Para obter instruções, consulte [Criar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Adicione usuários para os quais você tiver o acesso Editar a seus grupos e subgrupos. Ou adicione usuários a grupos e subgrupos editando seus perfis.

   Você também pode atualizar os campos no perfil de um membro do grupo se tiver a permissão Administrador de usuário (usuários do grupo) ativada em seu nível de acesso.

   Para obter mais informações, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >Os administradores do Workfront podem substituir as alterações nas associações de grupo feitas por um administrador de grupo.

* Redefina senhas para usuários que são membros dos grupos que você gerencia. Para obter mais informações, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Faça logon como usuários membros dos grupos que você gerencia. Para obter mais informações, consulte [Fazer logon como outro usuário](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Exiba o número de licenças disponíveis para seu grupo e os subgrupos abaixo dele. Para obter mais informações, consulte [Gerencie as licenças disponíveis em seu sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Gerenciar objetos de grupo {#manage-group-objects}

* Crie Modelos de layout de nível de grupo e associe-os aos grupos e subgrupos que você gerencia. Para obter mais informações, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Crie perfis de folha de ponto em nível de grupo, associe-os a usuários e grupos que você gerencia e gere manualmente as folhas de ponto. Para obter mais informações, consulte [Criar, editar e atribuir perfis de folha de ponto](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Sem acesso administrativo aos processos de aprovação, crie e edite processos de aprovação para os grupos e subgrupos que você gerencia. Para obter mais informações, consulte [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   Para obter informações sobre o acesso administrativo aos processos de aprovação, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Crie agendamentos e associe-os a um grupo que você gerencia. Para obter mais informações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Gerencie uma equipe atribuída a um grupo que você gerencia, sem ser membro da equipe. Além disso, crie um relatório de equipe com base no campo Grupo para identificar a qual grupo uma determinada equipe está atribuída. Para obter mais informações, consulte [Criar um grupo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Restaure um projeto associado a um grupo que você gerencia, juntamente com quaisquer tarefas, problemas ou documentos associados ao projeto. Para obter mais informações, consulte [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Gerenciar preferências de grupo e ferramentas {#manage-group-preferences-and-tools}

* Quando uma preferência de projeto, de tarefa ou de emissão, ou de folha de horas e de horas estiver desbloqueada para grupos em todo o sistema, edite essa preferência para grupos que você gerencia. Essas preferências afetam o comportamento do projeto, da tarefa e da ocorrência. Para obter mais informações, consulte:

   * [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Crie e edite os status do grupo para grupos que você gerencia. Para obter mais informações, consulte [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Configure uma notificação de evento para grupos que você gerencia. Você pode fazer isso somente depois que um administrador do Workfront desbloquear a capacidade de configurar notificações de eventos para grupos através do sistema. Para obter mais informações, consulte [Exibir e configurar notificações de evento para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
