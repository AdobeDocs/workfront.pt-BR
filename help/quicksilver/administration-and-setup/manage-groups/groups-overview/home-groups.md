---
title: Visão Geral dos Grupos Padrão
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Um Grupo padrão é atribuído no perfil do usuário. Todos os usuários precisam ter um Grupo padrão.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Visão geral dos Grupos padrão

Um Grupo padrão é atribuído no perfil do usuário. Todos os usuários precisam ter um Grupo padrão. Um usuário pode pertencer a mais de um grupo, mas pode ter apenas um Grupo padrão. Para obter mais informações sobre Grupos, consulte [Visão geral sobre Grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Embora qualquer grupo existente no sistema possa ser atribuído como o Grupo inicial de um usuário, recomendamos criar e atribuir novos grupos que representem unidades organizacionais maiores.

Ao estabelecer Grupos padrão, considere como sua organização divide os usuários da Adobe Workfront. Estas são algumas sugestões para determinar que tipo de grupos deve ser usado como Grupo padrão:

* Grupos que representam departamentos, como TI ou Marketing
* Grupos regidos por orçamentos diferentes
* Grupos localizados em diferentes áreas ou regiões
* Grupos compostos de várias equipes que pertencem ao mesmo centro de custo

>[!NOTE]
>
>Se você precisar reorganizar seus Grupos padrão em unidades organizacionais, será necessário>
>1. Crie o novo grupo, conforme explicado em [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).
>1. Reatribua o novo grupo como o Grupo Inicial do usuário, conforme explicado em [Editar perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>

## Gerenciamento de modelos de layout

Quando você atribui um Modelo de layout a um grupo, todos os usuários aos quais o grupo foi atribuído como Grupo inicial podem ver as configurações especificadas no Modelo de layout.

Se um Modelo de layout for atribuído a um Grupo padrão, ele só será visível para os usuários atribuídos a esse Grupo padrão.

Para obter mais informações, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Gerenciamento de licenças

Cada usuário pode ser atribuído a apenas um Grupo inicial, o que facilita o gerenciamento de contagens de licença.

Os administradores do Workfront têm a opção de definir contagens máximas de licença para os Grupos padrão.

Definir uma contagem máxima de licenças permite que os administradores do Workfront impeçam uma unidade de negócios de usar licenças da Workfront adquiridas para outras unidades de negócios.

Para obter mais informações, consulte [Gerenciar licenças disponíveis em seu sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
