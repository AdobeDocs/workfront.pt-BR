---
title: Grupos
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Um administrador do Workfront pode criar grupos de usuários que coincidem com a estrutura departamental. Grupos são semelhantes, mas distintos, de equipes e empresas. O administrador do Workfront concede aos grupos o acesso às áreas do Workfront onde precisam trabalhar e se comunicar. Cada grupo pode, então, manter suas informações do Workfront, como usuários, modelos e formulários personalizados, além de projetos separados das de outros departamentos. Pelo menos um administrador de grupo é necessário para cada grupo. Os administradores de grupo podem usar a página Grupos para gerenciar seus grupos em um único local. É possível criar até 14 níveis de subgrupos em um grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# Visão geral dos grupos

Um administrador do Workfront pode criar grupos de usuários que coincidem com a estrutura departamental. Grupos são semelhantes, mas distintos, de equipes e empresas.

O administrador do Workfront concede aos grupos o acesso às áreas do Workfront onde precisam trabalhar e se comunicar. Cada grupo pode, então, manter suas informações do Workfront, como usuários, modelos e formulários personalizados, além de projetos separados das de outros departamentos.

Pelo menos um administrador de grupo é necessário para cada grupo. Os administradores de grupo podem usar a página Grupos para gerenciar seus grupos em um único local. Para obter mais informações, consulte [Administradores do grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

É possível criar até 14 níveis de subgrupos em um grupo. Para obter mais informações, consulte [Visão geral de subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) e [Criar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Usar grupos para organizar usuários

Como administrador do Workfront ou administrador de grupo, você pode associar usuários a grupos e subgrupos. Se você tornar um grupo público, os usuários com uma licença do Planejador poderão associar usuários a ele. Para obter mais informações sobre administradores de grupos e grupos públicos, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Ao criar um usuário, recomendamos que você o adicione ao Grupo doméstico apropriado e a outros grupos nos quais o usuário deve trabalhar. Um usuário pode ter apenas um Grupo doméstico, mas pode estar em vários outros grupos.

Fazer parte de um grupo dá ao usuário acesso a objetos que são compartilhados com o grupo e os subgrupos. Por exemplo, se você compartilhar um projeto com um grupo, os usuários do grupo e dos subgrupos do grupo terão acesso a ele.

>[!TIP]
>
>Se os departamentos da sua organização geralmente trabalharem juntos para gerenciar projetos e os recursos nesses projetos, talvez não seja necessário dividir os departamentos em muitos grupos menores. Alguns grupos de alto nível podem funcionar melhor.

Um grupo pode ter um número ilimitado de usuários.

Para obter mais informações sobre como criar novos usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/add-users.md).

## Concessão de acesso de grupo a objetos

Ao compartilhar um objeto com um grupo, todos os membros desse grupo (incluindo membros de quaisquer subgrupos) têm acesso ao objeto. Para obter mais informações sobre compartilhamento no Workfront, consulte [Visão geral do compartilhamento de permissões em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Associar um grupo a um objeto

Ao criar ou editar um dos seguintes objetos Workfront, você pode associá-lo a um grupo:

* **Projeto**: Você pode associar um único grupo a um projeto para indicar a propriedade do projeto.

   Isso não concede implicitamente a cada membro do grupo direitos ao projeto. Para ter direitos no projeto, os usuários devem receber direitos compartilhando o projeto com eles.

   Embora os usuários possam ser membros de vários grupos, um projeto pode ter um único grupo associado a ele. Usuários de outros grupos ainda podem trabalhar no mesmo projeto, se os projetos tiverem sido compartilhados com eles ou com seus grupos. O grupo associado ao projeto é geralmente o responsável pela conclusão do projeto ou o grupo para o qual o projeto é entregue.

   Para obter instruções sobre como associar um projeto a um grupo, consulte [Gerenciar informações na área Visão geral do projeto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, programa ou empresa**: Ao criar ou editar um portfólio, programa ou empresa, você pode atribuir um único grupo a ele para indicar que o grupo é proprietário ou tem responsabilidade por ele. Com essa associação feita, os administradores e usuários podem identificar facilmente em quais portfólios, programas e empresas seus grupos estão trabalhando.

   Por exemplo, um administrador de grupo pode listar todos os portfólios na organização usando uma lista ou relatório e anotar na coluna Grupo quais portfólios recebem o grupo.

   >[!NOTE]
   >
   >Atribuir um grupo a um portfólio, programa ou empresa com um grupo não significa automaticamente que as informações nesse grupo tenham acesso aos seus dados. Você precisa compartilhar manualmente o acesso aos dados com o grupo antes que eles possam visualizá-los.

   Para obter instruções, consulte [Criar um portfólio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Criar um programa](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)e [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Processo de aprovação**: Você pode disponibilizar um processo de aprovação para projetos, tarefas e problemas pertencentes a um determinado grupo. Para obter mais informações, consulte [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Caminho do marco**: Você pode permitir que usuários em determinados grupos usem um caminho de marco com seus projetos. Para obter mais informações, consulte [Criar um caminho de marco](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Modelo de layout**: Você pode conceder permissões aos administradores de um grupo para modificar um Modelo de layout. Para obter instruções, consulte [Conceder acesso administrativo a um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Perfil da folha de horas**: Você pode conceder permissões aos administradores de um grupo para modificar um perfil de folha de ponto. Para obter mais informações, consulte [Criar, editar e atribuir perfis de folha de ponto](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Agendamentos**: Você pode conceder permissão aos administradores de um grupo para modificar um agendamento. Para obter mais informações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Equipes**: Você pode associar um grupo a uma equipe para que os administradores dos grupos e seus subgrupos possam visualizar e trabalhar com essas equipes na área Grupos . Para obter mais informações, consulte [Criar um grupo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) ou [Editar configurações do grupo](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Modelo**: Você pode atribuir um grupo a um modelo de projeto. Isso pode ajudá-lo a simplificar o processo de criação do projeto e ajudá-lo a identificar e relatar mais facilmente quais grupos possuem quais modelos de projeto. Para obter mais informações, consulte a seção [Visão geral](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) no artigo [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Itens excluídos e restaurados recentemente**: Você pode visualizar e gerenciar os grupos com itens excluídos recentemente. Para obter mais informações, consulte [Exibir e gerenciar os itens excluídos recentemente de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) e [Exibir e gerenciar os itens restaurados recentemente de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
