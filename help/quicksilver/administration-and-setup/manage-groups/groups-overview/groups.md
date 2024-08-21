---
title: Visão geral dos grupos
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Um administrador do Workfront pode criar grupos de usuários que coincidam com a estrutura departamental. Os grupos são semelhantes a, mas distintos de equipes e empresas.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Visão geral dos grupos

<!-- Audited: 01/2024 -->

Um administrador do Workfront pode criar grupos de usuários que coincidam com a estrutura departamental. Os grupos são semelhantes a, mas distintos de equipes e empresas.

O administrador do Workfront concede aos grupos acesso às áreas do Workfront onde precisam trabalhar e se comunicar. Cada grupo pode manter suas informações do Workfront, como usuários, modelos, formulários personalizados e projetos, separadas das de outros departamentos.

Pelo menos um administrador de grupo é necessário para cada grupo. Os administradores de grupo podem usar a página Grupos para gerenciar seus grupos em um único local. Para obter mais informações, consulte [Administradores de grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

Você pode criar até 14 níveis de subgrupos em um grupo. Para obter mais informações, consulte [Visão geral dos subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) e [Criar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Utilização de grupos para organizar usuários

Como administrador do Workfront ou administrador de grupo, você pode associar usuários a grupos e subgrupos. Se você tornar um grupo público, os usuários com uma licença Padrão (nova) ou de Plano (atual) poderão associar usuários a ele. Para obter mais informações sobre administradores de grupo e grupos públicos, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Ao criar um usuário, recomendamos que você o adicione ao Grupo padrão apropriado e a outros grupos nos quais o usuário deve trabalhar. Um usuário pode ter somente um Grupo padrão, mas pode estar em vários outros grupos.

Fazer parte de um grupo dá ao usuário acesso aos objetos compartilhados com o grupo e os subgrupos. Por exemplo, se você compartilhar um projeto com um grupo, os usuários no grupo e os subgrupos do grupo terão acesso a ele.

>[!TIP]
>
>Se os departamentos da sua organização geralmente trabalham juntos para gerenciar projetos e os recursos nesses projetos, talvez não seja necessário dividir os departamentos em muitos grupos menores. Alguns grupos de alto nível podem funcionar melhor.

Um grupo pode ter um número ilimitado de usuários.

Para obter mais informações sobre como criar novos usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/add-users.md).

## Concedendo a um grupo acesso a objetos

Quando você compartilha um objeto com um grupo, todos os membros desse grupo (incluindo membros de quaisquer subgrupos) têm acesso ao objeto. Para obter mais informações sobre compartilhamento no Workfront, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Associando um grupo a um objeto

Ao criar ou editar um dos seguintes objetos do Workfront, você pode associá-lo a um grupo:

* **Projeto**: você pode associar um único grupo a um projeto para indicar a propriedade do projeto.

  Isso não concede implicitamente direitos ao projeto a cada membro do grupo. Para ter direitos ao projeto, os usuários devem ter o projeto compartilhado com eles.

  Embora os usuários possam ser membros de vários grupos, um projeto pode ter um único grupo associado a ele. Usuários de outros grupos ainda podem trabalhar no mesmo projeto, se o projeto tiver sido compartilhado com eles ou seus grupos. O grupo associado ao projeto geralmente é o grupo responsável por concluir o projeto ou o grupo para o qual o projeto é entregue.

  Para obter instruções sobre como associar um projeto a um grupo, consulte [Gerenciar informações na área Visão Geral do projeto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, programa ou empresa**: ao criar ou editar um portfólio, programa ou empresa, você pode atribuir um único grupo a ele para indicar que o grupo é proprietário ou tem responsabilidade por ele. Com essa associação feita, administradores e usuários podem identificar facilmente em quais portfólios, programas e empresas seus grupos estão trabalhando.

  Por exemplo, um administrador de grupo pode listar todos os portfólios na organização usando uma lista ou relatório e anotar na coluna Grupo quais portfólios são atribuídos a seu grupo.

  >[!NOTE]
  >
  >Atribuir um grupo a um portfólio, programa ou empresa com um grupo não significa automaticamente que as informações no tenham acesso aos dados do grupo. Você precisa compartilhar manualmente o acesso aos dados com o grupo antes que ele possa vê-los.

  Para obter instruções, consulte [Criar um portfólio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Criar um programa](../../../manage-work/portfolios/create-and-manage-programs/create-program.md) e [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Processo de aprovação**: você pode disponibilizar um processo de aprovação para projetos, tarefas e problemas que pertençam a um determinado grupo. Para obter mais informações, consulte [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Caminho de Etapas**: você pode permitir que usuários de determinados grupos usem um caminho de etapas com seus projetos. Para obter mais informações, consulte [Criar um caminho de etapas](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Modelo de layout**: você pode conceder permissão aos administradores de um grupo para modificar um Modelo de layout. Para obter instruções, consulte [Conceder acesso administrativo a um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Perfil de Planilha de Horas**: você pode dar permissão aos administradores de um grupo para modificar um perfil de planilha de horas. Para obter mais informações, consulte [Criar, editar e atribuir perfis de folha de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Agendamentos**: você pode dar permissão aos administradores de um grupo para modificar um agendamento. Para obter mais informações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Equipes**: você pode associar um grupo a uma equipe para que os administradores dos grupos e seus subgrupos possam exibir e trabalhar com essas equipes da área Grupos. Para obter mais informações, consulte [Criar uma equipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) ou [Editar configurações da equipe](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Modelo**: você pode atribuir um grupo a um modelo de projeto. Isso pode ajudá-lo a simplificar o processo de criação de projetos e a identificar e relatar com mais facilidade quais grupos são proprietários de cada modelo de projeto. Para obter mais informações, consulte a seção [Visão geral](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) no artigo [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Itens excluídos e restaurados recentemente**: você pode exibir e gerenciar os grupos de itens excluídos recentemente. Para obter mais informações, consulte [Exibir e gerenciar os itens excluídos recentemente de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) e [Exibir e gerenciar os itens restaurados recentemente de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
