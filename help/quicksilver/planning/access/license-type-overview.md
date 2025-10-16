---
title: Visão Geral Do Tipo De Licença Ao Usar O Adobe Workfront Planning
description: Seu acesso ao Adobe Workfront Planning depende do tipo de licença, além das permissões para objetos. Nem todos os usuários na organização têm o mesmo acesso e permissões para usar o Adobe Workfront Planning. Este artigo descreve os níveis de acesso que os usuários podem ter ao Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: c879d06cfe7ba76df3e974c160a7349f1503f17f
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---


# Visão geral do tipo de licença ao usar o Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Seu tipo de licença do Adobe Workfront funciona em conjunto com suas permissões do Adobe Workfront Planning para conceder o seguinte acesso:

* Exibir, contribuir ou gerenciar espaços de trabalho ou tipos de registro
* Exibir ou gerenciar exibições.

Para obter informações sobre permissões para objetos no Workfront Planning, consulte [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Para obter informações sobre o acesso ao Workfront Planning, consulte [Visão geral do acesso ao Adobe Planning](/help/quicksilver/planning/access/access-overview.md).

## O relacionamento entre os tipos de licença do Workfront e as permissões do Workfront Planning

A tabela abaixo descreve a relação entre o tipo de licença de um usuário no Adobe Workfront e o nível de permissões que você pode conceder a ele para objetos do Adobe Workfront Planning com base nessa licença.

Conceder permissões de usuário a um espaço de trabalho também concede a eles permissões para tipos de registro, registros e campos.

Você deve conceder aos usuários permissões separadas para exibições, além daquelas que eles têm para espaços de trabalho, para acessar e gerenciar exibições.

Considere o seguinte ao trabalhar com permissões de tipo de registro:

* Os usuários herdam automaticamente permissões de tipo de registro de espaços de trabalho.
* Quando um usuário tem Permissões de gerenciamento em um espaço de trabalho, ele não pode ter um acesso menor a um tipo de registro.
* Os usuários não podem ter mais permissões para um tipo de registro do que têm para o espaço de trabalho ao qual o tipo de registro pertence.
* Remover as permissões dos usuários para um tipo de registro não remove o acesso de Exibição para todos os tipos de registros no espaço de trabalho, pois isso não remove as permissões deles para o espaço de trabalho.

| Tipo de licença do Adobe Workfront | Permissões mais altas permitidas no Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standard | <p>Os usuários podem gerenciar espaços de trabalho, tipos de registro e visualizações. Eles podem criar, editar ou excluir espaços de trabalho, tipos de registro, registros, campos e exibições.</p> <br> <p>Os administradores do sistema têm permissões de gerenciamento para todos os espaços de trabalho, incluindo aqueles que não criaram.</p> |
| Leve ou Colaborador | <p>Os usuários podem exibir os espaços de trabalho compartilhados com eles, bem como os tipos de registro, registros e campos desses espaços de trabalho.</p> <br> <p>Os usuários podem exibir as visualizações compartilhadas com eles, mas não podem criar as suas próprias visualizações. </p><br> <p>Os usuários não podem criar, editar ou excluir espaços de trabalho, tipos de registro, registros ou campos.</p> |

<!--Old: 
*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->


### Tipos de licença e permissões para espaços de trabalho e tipos de registro

Somente os usuários com uma licença Standard podem ter permissões do Contribute ou do Manage para espaços de trabalho e tipos de registros. As permissões do Contribute e do Manage para espaços de trabalho e tipos de registros também são transferidas para registros e campos.

Os administradores do sistema podem exibir todos os espaços de trabalho no sistema, incluindo aqueles que não criaram.

Os usuários com todos os outros tipos de licença podem ter permissões de Exibição para espaços de trabalho e tipos de registro compartilhados com eles, bem como para seus registros e campos.


>[!INFO]
>
>**EXEMPLO:**
>
>Colaboradores ou usuários com licenças leves não podem contribuir para espaços de trabalho e seus objetos, nem gerenciá-los.
>
>Há uma indicação na caixa de compartilhamento de que os usuários não podem receber permissões para contribuir ou gerenciar um espaço de trabalho quando possuem uma licença de nível inferior, pois esses níveis de permissões estão esmaecidos.
>
>![Permissões esmaecidas para o usuário colaborador no espaço de trabalho](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Tipos de licença e permissões para exibições

Somente os usuários com uma licença Standard podem ter permissões de gerenciamento para exibições.

Os administradores do sistema não podem acessar as exibições que não criaram. Eles devem ser compartilhados com eles.

Os usuários com todos os outros tipos de licença podem ter permissões de Exibição para exibições compartilhadas com eles.

>[!INFO]
>
>**EXEMPLO:**
>
>Colaboradores ou usuários com licenças leves não podem gerenciar exibições. Eles podem aplicar filtros, classificações ou agrupamentos temporários a visualizações que podem acessar.
>
>Há uma indicação na caixa de compartilhamento de que os usuários não podem receber permissões para gerenciar uma exibição quando têm uma licença de nível inferior, pois esses níveis de permissão estão esmaecidos.
>
>![Permissões esmaecidas para usuário light no compartilhamento de exibição](assets/permissions-grayed-out-for-light-user.png)
