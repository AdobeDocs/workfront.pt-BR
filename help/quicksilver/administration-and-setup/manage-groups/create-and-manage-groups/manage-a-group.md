---
user-type: administrator
product-area: system-administration;user-management
keywords: gerenciar,agrupar,editar,
navigation-topic: create-and-manage-groups
title: Gerenciar um grupo
description: Como administrador de grupo, você pode gerenciar um grupo que administra na área Grupos da Configuração. Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 0afd578ebaa55d911c04a1d08fbcadddc1d05bbc
workflow-type: tm+mt
source-wordcount: '1319'
ht-degree: 0%

---

# Gerenciar um grupo

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

Como administrador de grupo, você pode gerenciar um grupo que administra na área Grupos da Configuração. Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!NOTE]
>
>Quando você é atribuído como administrador de um grupo, você herda a função de administrador de grupo para qualquer subgrupo abaixo dele. Os únicos usuários que podem gerenciar um subgrupo são os administradores do grupo superior acima dele e quaisquer administradores de grupo atribuídos ao subgrupo.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir o tipo de plano ou licença que possui, entre em contato com o administrador do Workfront.

## Gerenciar associações de um grupo

Você pode adicionar e remover usuários e outros grupos de um grupo que administra. Você também pode atribuir membros do grupo como administradores do grupo e gerenciar as informações de perfil do usuário dos membros do grupo.

Para obter instruções, consulte [Exibir e gerenciar associações de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Gerenciar os detalhes de um grupo

Você pode exibir e editar a página Detalhes do Grupo de um grupo ou subgrupo que gerencia. Esta página inclui uma descrição do grupo, os nomes do Líder de negócios e dos administradores de grupo, e uma opção que permite tornar o grupo e todos os seus subgrupos públicos ou privados. E, se o seu nível de acesso permitir gerenciar formulários personalizados, você poderá anexar um formulário personalizado a um grupo.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Para obter instruções, consulte [Exibir e gerenciar os detalhes de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Editar, copiar ou excluir um grupo

Sem sair da página principal de um grupo que você está visualizando, você pode editar, copiar ou excluir o grupo rapidamente.

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Grupos**.

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Selecione o grupo e clique no botão Editar ![](assets/edit-icon.png), Copiar ![](assets/copy-icon.png), ou Excluir ![](assets/delete.png) ícone.

   Se precisar de informações sobre o uso da caixa exibida, consulte uma das seguintes opções:

   * **Editar**: [Exibir e gerenciar os detalhes de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Copiar**: [Criar um grupo de nível superior copiando um grupo ou subgrupo existente](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) no artigo [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **Excluir**: [Excluir um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Configurar as preferências de projeto, tarefa e problema de um grupo

Se você for um administrador de grupo e seu grupo precisar de configurações de preferência de projetos, tarefas e problemas diferentes daquelas definidas no nível do sistema, poderá solicitar que o administrador do Workfront desbloqueie uma preferência para todos os grupos em toda a organização. Depois de desbloqueado, você (e administradores de grupos para todos os outros grupos) pode configurá-lo para os grupos que você gerencia.

Para obter instruções, consulte [Configurar as preferências do projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e  [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Listar, adicionar e configurar subgrupos

Você pode criar, exibir, editar, copiar, renomear, exportar e excluir subgrupos abaixo de um grupo que administra.

## Configurar notificações de eventos para um grupo

Se um administrador do Workfront desbloquear a capacidade de configurar notificações de eventos para os grupos em sua organização, você poderá configurá-los para um grupo que administra. Para obter instruções, consulte [Exibir e configurar notificações de eventos para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Criar e personalizar status para um grupo

Como administrador de grupo, você pode criar status personalizados para um grupo de nível superior gerenciado por você. Isso dá autonomia ao seu grupo e ajuda a eliminar a necessidade de dezenas de status personalizados em toda a empresa. (Um administrador do Workfront também pode fazer isso para qualquer grupo.)

Você também pode personalizar os status do sistema de um grupo de nível superior se um administrador do Workfront os tiver configurado para permitir personalização.

Para obter instruções, consulte [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Trabalhar com projetos de um grupo

Na área Grupos da Configuração, ao visualizar a página principal de um grupo que você administra, é possível fazer o seguinte com projetos:

* Listar e trabalhar com (editar, copiar, excluir e exportar) os projetos associados ao grupo e seus subgrupos e que foram compartilhados com você
* Criar um novo projeto para o grupo

Para obter instruções, consulte [Criar e modificar os projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## Exibir e gerenciar os processos de aprovação de um grupo

Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com os processos de aprovação dos quais os administradores do grupo, ou um de seus subgrupos, têm acesso administrativo.

Para obter instruções, consulte [Processos de aprovação de nível de grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Exibir e gerenciar os modelos de layout de um grupo

Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com o Modelo de layout ao qual os administradores do grupo, ou um de seus subgrupos, têm acesso administrativo.

Para obter instruções, consulte [Criar e modificar os modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Exibir e gerenciar as agendas dos membros do grupo

Um administrador de grupo que cria um agendamento para um grupo deve especificar o grupo cujos administradores gerenciarão o agendamento. Normalmente, esse é o grupo para o qual o agendamento está sendo criado, mas pode ser um grupo diferente se o administrador do grupo gerenciar vários grupos e especificar um dos outros.

Ao visualizar a página principal de um grupo gerenciado, se o grupo for designado como aquele cujos administradores podem editar um agendamento, você poderá visualizar e gerenciar o agendamento na página do grupo.

Para obter instruções, consulte [Criar e modificar as agendas de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Exibir e gerenciar perfis de planilha de horas de membros do grupo

Ao visualizar a página principal de um grupo que você administra, é possível gerenciar os perfis de folha de horas que você e os outros administradores do grupo—ou um de seus subgrupos—têm permissão para editar. Para obter instruções, consulte [Criar e gerenciar os perfis de planilha de horas de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## Exibir e gerenciar os membros de um subgrupo do grupo

Ao visualizar a página principal de um grupo que você administra, é possível visualizar e gerenciar todos os usuários nos subgrupos do grupo. Para obter instruções, consulte [Exibir e gerenciar membros do subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Exibir e gerenciar as equipes de um grupo

Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com equipes associadas ao grupo ou a qualquer um de seus subgrupos.

Para obter instruções, consulte [Criar e modificar as equipes de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## Exibir e gerenciar as empresas de um grupo

Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com empresas associadas ao grupo ou a qualquer um de seus subgrupos. Para obter instruções, consulte [Criar e modificar as empresas de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## Exibir e gerenciar os portfólios e programas de um grupo

Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com portfólios e programas quando ambos os itens a seguir forem verdadeiros:

* Estão associados ao grupo que está a visualizar ou a qualquer um dos seus subgrupos
* Você tem permissão para visualizá-las porque as criou ou porque foram compartilhadas com você

Para obter instruções, consulte [Criar e modificar os projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) e [Criar, modificar e exibir os programas de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Desativar ou reativar um grupo

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

Você pode manter um grupo em seu estado ativo padrão ou desativá-lo.

A desativação de um grupo pode ser útil quando ele não está em uso no momento, pois os usuários não o veem mais em campos de digitação antecipada quando estão procurando um grupo que desejam associar a outro objeto.

Para obter instruções sobre como tornar um grupo inativo ou ativo, consulte [Desativar ou reativar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
