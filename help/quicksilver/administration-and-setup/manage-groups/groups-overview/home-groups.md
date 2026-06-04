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
TQID: https://experienceleague.adobe.com/S44kvUMrEV6C3K2BcqJZnKVqTRfT16xxhyDmG-P2J0c
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d83a421c-ecb9-4757-b609-c531392f90eb
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 333
ht-degree: 0%

---

# Visão geral de grupos da página inicial

Um Grupo padrão é atribuído no perfil do usuário. Todos os usuários precisam ter um Grupo padrão. Um usuário pode pertencer a mais de um grupo, mas pode ter apenas um Grupo padrão. Para obter mais informações sobre Grupos, consulte [Visão geral sobre Grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Embora qualquer grupo existente no sistema possa ser atribuído como o Grupo inicial de um usuário, recomendamos criar e atribuir novos grupos que representem unidades organizacionais maiores.

Ao estabelecer Grupos padrão, considere como sua organização divide os usuários da Adobe Workfront. Estas são algumas sugestões para determinar que tipo de grupos deve ser usado como Grupo padrão:

* Grupos que representam departamentos, como TI ou Marketing
* Grupos regidos por orçamentos diferentes
* Grupos localizados em diferentes áreas ou regiões
* Grupos compostos de várias equipes que pertencem ao mesmo centro de custo

>[!NOTE]
>
>Se você precisar reorganizar seus Grupos padrão em unidades organizacionais, será necessário
>
>1. Crie o novo grupo, conforme explicado em [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).
>1. Reatribua o novo grupo como o Grupo Inicial do usuário, conforme explicado em [Editar perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Gerenciamento de modelos de layout

Quando você atribui um Modelo de layout a um grupo, todos os usuários aos quais o grupo foi atribuído como Grupo inicial podem ver as configurações especificadas no Modelo de layout.

Se um Modelo de layout for atribuído a um Grupo padrão, ele só será visível para os usuários atribuídos a esse Grupo padrão.

Para obter mais informações, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Gerenciamento de licenças

Cada usuário pode ser atribuído a apenas um Grupo inicial, o que facilita o gerenciamento de contagens de licença.

Os administradores do Workfront têm a opção de definir contagens máximas de licença para os Grupos padrão.

Definir uma contagem máxima de licenças permite que os administradores do Workfront impeçam uma unidade de negócios de usar licenças da Workfront adquiridas para outras unidades de negócios.

Para obter mais informações, consulte [Gerenciar licenças disponíveis em seu sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
