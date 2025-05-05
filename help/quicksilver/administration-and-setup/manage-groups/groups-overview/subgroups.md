---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Visão geral de subgrupos
description: Você pode criar até 14 níveis de subgrupos em um grupo. Em qualquer um desses níveis, você pode criar um número ilimitado de subgrupos paralelos.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Visão geral dos subgrupos

Você pode criar até 14 níveis de subgrupos em um grupo. Em qualquer um desses níveis, você pode criar um número ilimitado de subgrupos paralelos. Para obter instruções, consulte [Criar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

Para obter informações sobre grupos, consulte [Visão geral sobre grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## O que os subgrupos herdam?

Os subgrupos herdam a associação do grupo pai. Portanto, os usuários e grupos em um subgrupo têm a mesma visibilidade, permissões e acesso a todos os objetos que os usuários e grupos que pertencem ao grupo pai que compartilham.

Além disso, um subgrupo herda automaticamente os administradores de grupo de seu grupo de nível superior, mas você também pode atribuir membros de um subgrupo para atuar como administradores de grupo.

>[!TIP]
>
>Às vezes, você pode querer usar subgrupos para adicionar vários usuários a um grupo existente para dar a eles acesso a um objeto que precisam.
>
>Por exemplo, suponha que você tenha um grupo de técnicos de suporte e um grupo separado de diretores de TI. O grupo de help desk tem permissões para uma determinada Fila de solicitações. Você deseja adicionar os diretores de TI ao grupo de suporte técnico para que eles também tenham permissões para a Fila de solicitações. Sem a funcionalidade de subgrupo, seria necessário adicionar os diretores de TI ao grupo de suporte técnico manualmente, o que poderia ser ineficiente e difícil de gerenciar. Se você adicionar o grupo Diretores de TI ao grupo de suporte técnico como um subgrupo, você realizará essa tarefa mais rapidamente com apenas uma alteração.

>[!NOTE]
>
>Se um usuário foi adicionado separadamente a um subgrupo e a seu grupo principal, remover o usuário de um não remove o usuário do outro. Se você não quiser que o usuário tenha o acesso permitido para o grupo pai, remova o usuário do subgrupo e do grupo pai.

## Subgrupos públicos e privados

Para um grupo público, qualquer usuário (dentro ou fora do grupo) que tenha acesso de usuário de edição pode adicionar o grupo ao perfil de outros usuários. Eles não podem fazer isso para um grupo privado.

Você pode editar essa opção somente no grupo pai superior em uma hierarquia de grupos que tenha mais de um nível. Todos os subgrupos do grupo pai herdam sua configuração.

Se você criar um subgrupo em um grupo público, o subgrupo também será público, por padrão. Para obter mais informações sobre como criar e tornar público um grupo, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). Para obter mais informações sobre o acesso necessário para editar usuários, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Qualquer grupo adicionado a um grupo existente torna-se automaticamente um subgrupo e não é mais um grupo principal. No entanto, o subgrupo retém seus usuários existentes, bem como quaisquer associações com projetos, problemas e tarefas, além de todos os status de projeto, tarefa e problema que pertençam ao novo grupo pai.

## Administradores de grupo para subgrupos

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

Você pode atribuir membros do subgrupo como administradores do grupo ao subgrupo ao criá-lo ou editá-lo. Para obter instruções, consulte [&#128279;](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) no artigo [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Como alternativa, você pode deixar a administração do subgrupo para os administradores de grupo atribuídos aos grupos acima dele. Ao criar um subgrupo, os administradores de grupo nos grupos acima têm acesso automático para gerenciar o subgrupo.

>[!NOTE]
>
>Se você adicionar um usuário a um subgrupo e esse usuário for um administrador de grupo de um grupo em qualquer lugar acima do subgrupo, esse usuário terá direitos administrativos para gerenciar o subgrupo, mesmo sem ser atribuído a ele como um administrador de grupo.

Para saber quais ações estão disponíveis para um administrador do Adobe Workfront que gerencia o sistema do Workfront, um administrador de grupo que gerencia um grupo de nível superior e um administrador de grupo que gerencia um subgrupo, consulte [Ações permitidas para diferentes tipos de administradores](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
