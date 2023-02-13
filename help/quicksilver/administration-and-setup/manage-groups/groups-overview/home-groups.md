---
title: Visão geral dos grupos domésticos
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Um Grupo doméstico é atribuído no perfil do usuário. Todos os usuários precisam ter um Grupo doméstico. Um usuário pode pertencer a mais de um grupo, mas só pode ter um Grupo doméstico. Embora qualquer grupo existente no sistema possa ser atribuído como Grupo doméstico de um usuário, recomendamos criar e atribuir novos grupos que representem unidades organizacionais maiores. Ao estabelecer grupos domésticos, considere como sua organização divide os usuários da Adobe Workfront.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Visão geral dos grupos domésticos

Um Grupo doméstico é atribuído no perfil do usuário. Todos os usuários precisam ter um Grupo doméstico. Um usuário pode pertencer a mais de um grupo, mas só pode ter um Grupo doméstico. Para obter mais informações sobre Grupos, consulte [Visão geral dos grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Embora qualquer grupo existente no sistema possa ser atribuído como Grupo doméstico de um usuário, recomendamos criar e atribuir novos grupos que representem unidades organizacionais maiores.

Ao estabelecer grupos domésticos, considere como sua organização divide os usuários da Adobe Workfront. Estas são algumas sugestões para determinar que tipo de grupos deve ser usado como um Grupo doméstico:

* Grupos que representam departamentos, como TI ou Marketing
* Grupos governados por orçamentos diferentes
* Grupos localizados em diferentes áreas ou regiões
* Grupos compostos de várias equipes pertencentes ao mesmo centro de custos

>[!NOTE]
>
>Se você precisar reorganizar seus Grupos iniciais em unidades organizacionais, será necessário
>1. Crie o novo grupo, conforme explicado em [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).
>1. Reatribua o novo grupo como o Grupo doméstico do usuário, conforme explicado em [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>


## Gerenciamento de modelo de layout

Quando você atribui um Modelo de layout a um grupo, todos os usuários que têm o grupo atribuído como Grupo inicial podem ver as configurações especificadas no Modelo de layout.

Se um Modelo de layout for atribuído a um Grupo inicial, ele só será visível para os usuários atribuídos a esse Grupo inicial.

Para obter mais informações, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Gerenciamento de licenças

Cada usuário pode ser atribuído a apenas um Grupo doméstico, o que facilita o gerenciamento das contagens de licença.

Os administradores do Workfront têm a opção de definir contagens máximas de licença para os Grupos Iniciais.

Definir uma contagem máxima de licenças permite que os administradores do Workfront evitem que uma unidade comercial use licenças do Workfront compradas para outras unidades comerciais.

Para obter mais informações, consulte [Gerencie as licenças disponíveis em seu sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
