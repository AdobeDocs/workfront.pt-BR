---
title: Visão Geral Do Tipo De Licença Ao Usar O Adobe Workfront Planning
description: Seu acesso ao Adobe Workfront Planning depende do tipo de licença, além das permissões para objetos. Nem todos os usuários na organização têm o mesmo acesso e permissões para usar o Adobe Workfront Planning. Este artigo descreve os níveis de acesso que os usuários podem ter ao Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: cf3b5d3f8e3a8a1922da757a41b4c5e0ee84e6fd
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---


# Visão geral do tipo de licença ao usar o Adobe Workfront Planning

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Seu tipo de licença do Adobe Workfront funciona em conjunto com suas permissões do Adobe Workfront Planning para conceder o seguinte acesso:

* Exibir, contribuir ou gerenciar espaços de trabalho
* Exibir ou gerenciar exibições.

Para obter informações sobre permissões para objetos no Workfront Planning, consulte [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Para obter informações sobre o acesso ao Workfront Planning, consulte [Visão geral do acesso ao Adobe](/help/quicksilver/planning/access/access-overview.md).

## O relacionamento entre os tipos de licença do Workfront e as permissões do Workfront Planning

A tabela abaixo descreve a relação entre o tipo de licença de um usuário no Adobe Workfront e o nível de permissões que você pode conceder a ele para objetos do Adobe Workfront Planning com base nessa licença.

Conceder permissões de usuário a um espaço de trabalho também concede a eles permissões para tipos de registro, registros e campos.

Você deve conceder aos usuários permissões separadas para exibições, além daquelas que eles têm para espaços de trabalho, para acessar e gerenciar exibições.

| Tipo de licença da Adobe Workfront* | Permissões mais altas permitidas no Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Padrão | <p>Os usuários podem gerenciar espaços de trabalho e visualizações. Eles podem criar, editar ou excluir espaços de trabalho, tipos de registro, registros, campos e exibições.</p> <br> <p>Os administradores do sistema têm permissões de gerenciamento para todos os espaços de trabalho, incluindo aqueles que não criaram.</p> |
| Leve ou Colaborador | <p>Os usuários podem exibir os espaços de trabalho compartilhados com eles, bem como os tipos de registro, registros e campos desses espaços de trabalho.</p> <br> <p>Os usuários podem exibir as visualizações compartilhadas com eles, mas não podem criar as suas próprias visualizações. </p><br> <p>Os usuários não podem criar, editar ou excluir espaços de trabalho, tipos de registro, registros ou campos.</p> |

*O Workfront Planning não está disponível para licenças herdadas do Workfront.
Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


<!--OLD 

| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

### Tipos de licença e permissões de espaço de trabalho

Somente os usuários com uma licença Standard podem ter permissões do Contribute ou Gerenciar para espaços de trabalho. Os usuários com todos os outros tipos de licença podem ter permissões de Exibição para espaços de trabalho compartilhados com eles.

Os administradores do sistema podem exibir todos os espaços de trabalho no sistema, mesmo aqueles que não criaram.

>[!INFO]
>
>**EXEMPLO:**
>
>Colaboradores ou usuários com licenças leves não podem contribuir para espaços de trabalho e seus objetos, nem gerenciá-los.
>
>Há uma indicação na caixa de compartilhamento de que os usuários não podem receber permissões para contribuir ou gerenciar um espaço de trabalho quando possuem uma licença de nível inferior, pois esses níveis de permissões estão esmaecidos.
>
><span class="preview">![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)</span>


### Tipos de licença e permissões de exibição

Somente os usuários com uma licença Standard podem ter permissões de gerenciamento para exibições. Os usuários com todos os outros tipos de licença podem ter permissões de Exibição para exibições compartilhadas com eles.

>[!INFO]
>
>**EXEMPLO:**
>
>Colaboradores ou usuários com licenças leves não podem gerenciar exibições. Eles podem aplicar filtros, classificações ou agrupamentos temporários a visualizações que podem acessar.
>
>Há uma indicação na caixa de compartilhamento de que os usuários não podem receber permissões para gerenciar uma exibição quando têm uma licença de nível inferior, pois esses níveis de permissão estão esmaecidos.
>
><span class="preview">![](assets/permissions-grayed-out-for-light-user.png)</span>
