---
title: Visão geral do tipo de licença ao usar o Adobe Workfront Planning
description: Seu acesso ao Adobe Workfront Planning depende do tipo de licença, além das permissões para objetos.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Visão geral do tipo de licença ao usar o Adobe Workfront Planning

{{planning-important-intro}}

Seu tipo de licença do Adobe Workfront funciona em conjunto com suas permissões do Adobe Workfront Planning para conceder o seguinte acesso:

* Exibir, contribuir ou gerenciar espaços de trabalho
* Exibir ou gerenciar exibições.

Para obter informações sobre permissões para objetos no Workfront Planning, consulte [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## O relacionamento entre os tipos de licença do Workfront e as permissões do Workfront Planning

A tabela abaixo descreve a relação entre o tipo de licença de um usuário no Adobe Workfront e o nível de permissões que você pode conceder a ele para objetos do Adobe Workfront Planning com base nessa licença.

Conceder permissões de usuário a um espaço de trabalho também concede a eles permissões para tipos de registro, registros e campos.


| Tipo de licença da Adobe Workfront* | Permissões mais altas permitidas no Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Novo: Padrão <br> ou <br>Atual: Plano | Os usuários podem gerenciar espaços de trabalho. Eles podem criar, editar ou excluir espaços de trabalho, tipos de registro, registros e campos. <br> Os administradores do sistema têm permissões de gerenciamento para todos os espaços de trabalho, incluindo aqueles que não criaram. |
| Novo: Claro, Colaborador <br> ou <br>Atual: Trabalho, Solicitante, Revisor | Os usuários podem exibir os espaços de trabalho compartilhados com eles, bem como os tipos de registro, registros e campos desses espaços de trabalho. <br> Usuários não podem criar, editar ou excluir espaços de trabalho, tipos de registro, registros ou campos. |

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

### Tipos de licença e permissões de espaço de trabalho

Somente usuários com uma licença Padrão (ou Plano) podem ter permissões do Contribute ou Manage para espaços de trabalho. Os usuários com todos os outros tipos de licença podem ter permissões de Exibição para espaços de trabalho compartilhados com eles.

Os administradores do sistema podem exibir todos os espaços de trabalho no sistema, mesmo aqueles que não criaram.

>[!INFO]
>
>**EXEMPLO:**
>
>Os solicitantes (ou colaboradores, de acordo com o novo modelo de licença) não podem contribuir para espaços de trabalho e seus objetos, nem gerenciá-los.
>
>Há uma indicação na caixa de compartilhamento de que os usuários não podem receber permissões para contribuir ou gerenciar um espaço de trabalho quando possuem uma licença de nível inferior, pois esses níveis de permissões estão esmaecidos.
>
>![](assets/permissions-grayed-out-for-requestor-user.png)

### Tipos de licença e permissões de exibição

Somente usuários com uma licença Padrão (ou Plano) podem ter permissões de Gerenciamento para exibições. Os usuários com todos os outros tipos de licença podem ter permissões de Exibição para exibições compartilhadas com eles.

>[!INFO]
>
>**EXEMPLO:**
>
>Colaboradores (ou Solicitantes e Revisores) não podem gerenciar exibições. Eles podem aplicar filtros, classificações ou agrupamentos temporários a visualizações que podem acessar.
>
>Há uma indicação na caixa de compartilhamento de que os usuários não podem receber permissões para gerenciar uma exibição quando têm uma licença de nível inferior, pois esses níveis de permissão estão esmaecidos.
>
>![](assets/permissions-grayed-out-for-reviewer-user-on-a-view.png)


<!--Replace all of the above with this:

The table below describes the relationship between the license type of a user in Adobe Workfront and the level of permissions you can grant to them to Adobe Workfront Planning objects based on that license. 

Granting a user permissions to a workspace also grants them permissions to record types, records, and fields. 

You must grant view permissions separately from workspace permissions. 


| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | <ul><li>Users can contribute to or manage workspaces and they can manage views. They can create, edit, or delete workspaces, record types, records, fields, and views.</li> <li> System administrators have Manage permissions to all workspaces, including the ones they did not create.</li> <li> System administrators can only access views they created.</li></ul>                                                                                                                     |
|New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | <ul><li>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</li> <li>Users can access views shared with them and apply temporary filters, sorts, or groupings, but they cannot modify the views. </li><li> Users cannot create, edit, or delete workspaces, record types, records, fields, or views.</li></ul>|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->