---
title: Conceder acesso ao Adobe Maestro
description: Saiba como conceder acesso e compartilhar informações no Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 937498a68a994d19b0005d518d7e313c48961672
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Conceder acesso ao Adobe Maestro

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para ter acesso ao Maestro
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Todos os usuários em sua organização podem ter acesso ao Maestro, se os seguintes pré-requisitos estiverem em vigor:

<!--the first requisite will be removed when we go to GA-->

* Sua organização está inscrita no programa beta fechado do Adobe Maestro.
* Como administrador do sistema, você deve adicionar a área Maestro ao Menu principal usando um modelo de layout.

  O Maestri não é exibido no Menu principal por padrão para nenhum usuário, incluindo administradores de sistema.

  Para obter informações, consulte [Personalizar o menu principal usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

<!-- take out the note below when we release permissions-->

>[!NOTE]
>
>Não há níveis de acesso ou permissões associados aos usuários ou às informações no Maestro. Todos os usuários que têm o Maestro habilitado em seus ambientes podem exibir, editar e excluir todas as informações que qualquer outro usuário adiciona ao Maestro.

## Compartilhar a área Maestro no Menu Principal com outras pessoas

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

Depois que sua organização tiver sido inscrita no programa Maestro beta, você poderá adicionar a área Maestro ao Menu principal de todos os usuários usando um modelo de layout.

1. Efetue logon no **Workfront** como administrador do Workfront.

1. Adicione o **Maestro** ícone ![](assets/maestro-icon.png) para o **Menu principal** usando um **Modelo de layout**.

   Para obter informações, consulte [Personalizar o menu principal usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Atribua o modelo de layout aos usuários que você deseja que tenham acesso ao Maestro.

   Para obter informações, consulte [Atribuir usuários a um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Todos os usuários atribuídos ao modelo agora podem acessar o Maestro no menu principal.

   Os usuários podem começar a criar espaços de trabalho, tipos de registros, registros e campos.

<!--

## Share permissions to a workspace

Only system administrators can access all workspaces in Maestro. As a system administrator, you must share a workspace with other users for them to view, manage, or contribute to it. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu at the right of a user or group name, then click **Remove**. 
    
    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 
1. Click **Save**.

-->