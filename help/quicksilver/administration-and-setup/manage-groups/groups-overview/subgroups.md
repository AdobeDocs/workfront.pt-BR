---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Visão geral de subgrupos
description: É possível criar até 14 níveis de subgrupos em um grupo. Em qualquer um desses níveis, é possível criar um número ilimitado de subgrupos paralelos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Visão geral de subgrupos

É possível criar até 14 níveis de subgrupos em um grupo. Em qualquer um desses níveis, é possível criar um número ilimitado de subgrupos paralelos. Para obter instruções, consulte [Criar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

Para obter informações sobre grupos, consulte [Visão geral dos grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## O que os subgrupos herdam?

Os subgrupos herdam a associação do grupo pai. Assim, os usuários e grupos em um subgrupo têm a mesma visibilidade, permissões e acesso a todos os objetos que os usuários e grupos que pertencem ao grupo pai que eles compartilham.

Além disso, um subgrupo herda automaticamente os administradores de grupo de seu grupo de nível superior, mas também é possível atribuir membros de um subgrupo para agir como seus administradores de grupo.

>[!TIP]
>
>Às vezes, é possível usar subgrupos para adicionar vários usuários a um grupo existente, a fim de conceder a eles acesso a um objeto necessário.
>
>Por exemplo, suponha que você tenha um grupo de técnicos de suporte técnico e um grupo separado de diretores de TI. O grupo de suporte técnico tem permissões para uma fila de solicitações específica. Você deseja adicionar os diretores de TI ao grupo do suporte técnico para que eles também tenham permissões para a fila de solicitações. Sem a funcionalidade do subgrupo, você teria que adicionar manualmente os diretores de TI ao grupo de suporte técnico, o que poderia ser ineficiente e difícil de gerenciar. Se você adicionar o grupo de diretores de TI ao grupo de suporte técnico como um subgrupo, conclua essa tarefa mais rapidamente com apenas uma alteração.

>[!NOTE]
>
>Se um usuário tiver sido adicionado a um subgrupo e a seu grupo pai separadamente, a remoção do usuário de um não removerá o usuário do outro. Se você não quiser que o usuário tenha o acesso permitido para o grupo pai, remova o usuário do subgrupo e do grupo pai.

## Subgrupos públicos e privados

Para um grupo público, qualquer usuário (dentro ou fora do grupo) que tenha acesso de usuário de edição pode adicionar o grupo ao perfil de outros usuários. Eles não podem fazer isso por um grupo privado.

Você pode editar essa opção somente no grupo principal superior em uma hierarquia de grupos que tenha mais de um nível. Todos os subgrupos do grupo pai herdam sua configuração.

Se você criar um subgrupo em um grupo que é público, o subgrupo também será público, por padrão. Para obter mais informações sobre como criar um grupo e torná-lo público, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). Para obter mais informações sobre o acesso necessário para editar usuários, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Qualquer grupo adicionado a um grupo existente torna-se automaticamente um subgrupo e não é mais um grupo principal. No entanto, o subgrupo retém seus usuários existentes, bem como quaisquer associações com projetos, problemas e tarefas, além de todos os status de projeto, tarefa e emissão que pertencem ao novo grupo pai.

## Administradores de grupo para subgrupos

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

É possível atribuir membros do subgrupo como administradores de grupo ao subgrupo ao criá-lo ou editá-lo. Para obter instruções, consulte [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) no artigo [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Como alternativa, você pode deixar a administração do subgrupo para os administradores do grupo que estão atribuídos aos grupos acima dele. Ao criar um subgrupo, os administradores de grupo nos grupos acima dele têm acesso automático para gerenciar o subgrupo.

>[!NOTE]
>
>Se você adicionar um usuário a um subgrupo e ele for um administrador de grupo para um grupo em qualquer lugar acima do subgrupo, ele terá direitos administrativos para gerenciar o subgrupo, mesmo sem ter sido atribuído como administrador de grupo para ele.

Para saber quais ações estão disponíveis para um administrador do Adobe Workfront gerenciando o sistema Workfront, um administrador de grupo gerenciando um grupo de nível superior e um administrador de grupo gerenciando um subgrupo, consulte [Ações permitidas para diferentes tipos de administradores](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
