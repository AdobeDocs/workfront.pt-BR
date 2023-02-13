---
user-type: administrator
product-area: system-administration;user-management
keywords: gerenciar,agrupar,editar,
navigation-topic: create-and-manage-groups
title: Gerenciar um grupo
description: Como administrador de grupo, você pode gerenciar um grupo que você administra na área Grupos em Configurar. Se houver algum grupo acima do grupo que você gerencia, os administradores também poderão fazer isso para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 0%

---

# Gerenciar um grupo

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

Como administrador de grupo, você pode gerenciar um grupo que você administra na área Grupos em Configurar. Se houver algum grupo acima do grupo que você gerencia, os administradores também poderão fazer isso para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!NOTE]
>
>Ao ser atribuído como administrador para um grupo, você herda a função de administrador do grupo para qualquer subgrupo que esteja abaixo dele. Os únicos usuários que podem gerenciar um subgrupo são os administradores de grupo do grupo superior acima dele e os administradores de grupo atribuídos ao subgrupo.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Gerenciar as associações de um grupo

Você pode adicionar e remover usuários e outros grupos de um grupo que você administra. Também é possível atribuir membros do grupo como administradores do grupo e gerenciar as informações de perfil do usuário dos membros do grupo.

Para obter instruções, consulte [Exibir e gerenciar as associações de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Gerenciar os detalhes de um grupo

Você pode exibir e editar a página Detalhes do grupo para um grupo ou subgrupo que gerencia. Esta página inclui uma descrição do grupo, os nomes do Líder da empresa e dos administradores do grupo e uma opção que permite tornar o grupo e todos os seus subgrupos públicos ou privados. E, se o nível de acesso permitir gerenciar formulários personalizados, é possível anexar um formulário personalizado a um grupo.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Para obter instruções, consulte [Exibir e gerenciar os detalhes de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Editar, copiar ou excluir um grupo

Sem sair da página principal de um grupo que esteja visualizando, é possível editar, copiar ou excluir rapidamente

<!--
DRAFTED IN FLARE:
or deactivate

-->

o grupo.

<!--
DRAFTED IN FLARE:
Make this change when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Grupos**.

   Na lista que é exibida, é possível ver os grupos gerenciados, juntamente com os subgrupos que eles possuem. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Selecione o grupo e clique no botão Editar ![](assets/edit-icon.png), Copiar ![](assets/copy-icon.png)ou Excluir ![](assets/delete.png) ícone .

   Se você precisar de informações sobre o uso da caixa exibida, consulte um dos seguintes:

   * **Editar**: [Exibir e gerenciar os detalhes de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Copiar**: [Criar um grupo de nível superior copiando um grupo ou subgrupo existente](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) no artigo [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **Excluir**: [Excluir um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Configurar projeto, tarefa e emitir preferências para um grupo

Se você for um administrador de grupo e o seu grupo precisar de diferentes configurações de projeto, tarefa e preferência daquelas definidas no nível do sistema, poderá solicitar ao administrador do Workfront que desbloqueie uma preferência para todos os grupos em toda a organização. Após desbloqueá-lo, você (e os administradores de grupo para todos os outros grupos) poderá configurá-lo para os grupos que você gerencia.

Para obter instruções, consulte [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e  [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Listar, adicionar e configurar subgrupos

É possível criar, exibir, editar, copiar, renomear, exportar e excluir subgrupos abaixo de um grupo que você administra.

## Configurar notificações de evento para um grupo

Se um administrador do Workfront desbloquear a capacidade de configurar notificações de eventos para os grupos em sua organização, você poderá configurá-las para um grupo que você administra. Para obter instruções, consulte [Exibir e configurar notificações de evento para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Criar e personalizar status para um grupo

Como administrador de grupo, você pode criar status personalizados para um grupo de nível superior que gerencia. Isso dá autonomia ao seu grupo e ajuda a eliminar a necessidade de dezenas de status personalizados em toda a empresa. (Um administrador do Workfront também pode fazer isso para qualquer grupo.)

Você também pode personalizar os status do sistema para um grupo de nível superior se um administrador do Workfront os tiver configurado para permitir a personalização.

Para obter instruções, consulte [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Trabalhar com projetos de um grupo

Na área Grupos da Configuração, ao visualizar a página principal de um grupo que você administra, você pode fazer o seguinte com projetos:

* Listar e trabalhar com (editar, copiar, excluir e exportar) os projetos que estão associados ao grupo e seus subgrupos e que foram compartilhados com você
* Criar um novo projeto para o grupo

Para obter instruções, consulte [Criar e modificar projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## Exibir e gerenciar os processos de aprovação de um grupo

Ao visualizar um grupo que você gerencia na área Grupos , é possível visualizar e trabalhar com os processos de aprovação para os quais os administradores do grupo, ou um de seus subgrupos, têm acesso administrativo.

Para obter instruções, consulte [Processos de aprovação no nível do grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Exibir e gerenciar os modelos de layout de um grupo

Ao visualizar um grupo que você gerencia na área Grupos , é possível visualizar e trabalhar com o Modelo de layout para o qual os administradores do grupo, ou um de seus subgrupos, têm acesso administrativo.

Para obter instruções, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Exibir e gerenciar programações de membros do grupo

Um administrador de grupo que crie um agendamento para um grupo deve especificar o grupo cujos administradores gerenciarão o agendamento. Normalmente, esse é o grupo para o qual o agendamento está sendo criado, mas pode ser um grupo diferente se o administrador do grupo gerencia vários grupos e especifica um dos outros em vez disso.

Ao visualizar a página principal de um grupo que você gerencia, se o grupo for designado como aquele cujos administradores podem editar um agendamento, você poderá visualizar e gerenciar o agendamento na página do grupo.

Para obter instruções, consulte [Criar e modificar agendamentos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Exibir e gerenciar os perfis da folha de ponto dos membros do grupo

Ao visualizar a página principal de um grupo administrado, é possível gerenciar os perfis da folha de ponto que você e os outros administradores do grupo, ou um de seus subgrupos, têm permissão para editar. Para obter instruções, consulte [Criar e gerenciar os perfis de folha de ponto de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## Exibir e gerenciar membros de subgrupo de um grupo

Ao visualizar a página principal de um grupo administrado, é possível visualizar e gerenciar todos os usuários dos subgrupos do grupo. Para obter instruções, consulte [Exibir e gerenciar membros do subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Exibir e gerenciar as equipes de um grupo

Ao visualizar um grupo que você gerencia na área Grupos , é possível visualizar e trabalhar com equipes associadas ao grupo ou a qualquer um de seus subgrupos.

Para obter instruções, consulte [Criar e modificar as equipes de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## Exibir e gerenciar as empresas de um grupo

Ao visualizar um grupo que você gerencia na área Grupos , é possível visualizar e trabalhar com empresas associadas ao grupo ou a qualquer um de seus subgrupos. Para obter instruções, consulte [Criar e modificar empresas de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## Exibir e gerenciar portfólios e programas de um grupo

Ao visualizar um grupo que você gerencia na área Grupos , é possível visualizar e trabalhar com portfólios e programas quando ambas as opções a seguir forem verdadeiras:

* Eles estão associados ao grupo que você está visualizando ou a qualquer um de seus subgrupos
* Você tem permissões para visualizá-los porque os criou ou eles foram compartilhados com você

Para obter instruções, consulte [Criar e modificar projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) e [Criar, modificar e exibir os programas de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Desativar ou reativar um grupo

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

Você pode manter um grupo no seu estado ativo padrão ou desativá-lo.

A desativação de um grupo pode ser útil quando ele não está em uso no momento, pois os usuários não o veem mais em campos do tipo forward ao pesquisarem um grupo que desejam associar a outro objeto.

Para obter instruções sobre como tornar um grupo inativo ou ativo, consulte [Desativar ou reativar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
