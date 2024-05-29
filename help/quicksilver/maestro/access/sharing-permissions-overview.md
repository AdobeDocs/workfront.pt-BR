---
title: Visão geral das permissões de compartilhamento no Adobe Workfront Planning
description: Você pode compartilhar ou remover permissões de um espaço de trabalho ou exibição do Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 44073ea242803e28ca00c82811ae2865747d11c3
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 7%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Visão geral das permissões de compartilhamento no Adobe Workfront Planning

{{maestro-important-intro}}

Você pode compartilhar ou remover permissões de um espaço de trabalho ou exibição no Adobe Workfront Planning.

Este artigo descreve os níveis de permissão para objetos do Workfront Planning.

Para obter informações sobre como compartilhar espaços de trabalho ou exibições, consulte os seguintes artigos:

* [Compartilhar espaços de trabalho](/help/quicksilver/maestro/access/share-workspaces.md)

* [Compartilhar exibições](/help/quicksilver/maestro/access/share-views.md)

## Objetos que você pode compartilhar no Adobe Workfront Planning

Você pode compartilhar os seguintes objetos:

* Espaços de trabalho

  Quando você compartilha um espaço de trabalho, todos os tipos de registro, registros e campos associados aos espaços de trabalho também são compartilhados. As exibições não são compartilhadas.

* Visualizações

## Considerações sobre o compartilhamento de objetos no Adobe Workfront Planning

* Seu tipo de licença do Adobe Workfront funciona em conjunto com suas permissões do Workfront Planning para fornecer acesso a visualização, contribuição ou gerenciamento de objetos ao usar o Workfront Planning.

  Para obter informações sobre como os tipos de licença afetam os níveis de permissão para o Workfront Planning, consulte [Visão geral do tipo de licença ao usar o Adobe Workfront Planning](/help/quicksilver/maestro/access/license-type-overview.md).
* Os administradores do sistema podem gerenciar e compartilhar espaços de trabalho criados por outros usuários.
* Se você não for um Administrador do sistema, poderá contribuir com espaços de trabalho criados por outros se eles forem compartilhados com você.
* Não é possível compartilhar espaços de trabalho ou exibições em massa.
* Você pode compartilhar um espaço de trabalho ou uma exibição com as seguintes entidades:
   * Usuários
   * Grupos
     <!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->
* Outros usuários, incluindo Administradores do sistema, só podem acessar as exibições que criaram ou que foram compartilhadas com eles. Os administradores do sistema só podem receber permissões para Gerenciar uma exibição.
* É possível compartilhar um link para um espaço de trabalho ou para uma exibição de uma página do tipo record com outras pessoas. Os usuários que recebem o link devem ser usuários ativos e fazer logon no Workfront para acessar o espaço de trabalho ou a página do tipo de registro exibida na exibição selecionada.

## Permissões de compartilhamento para objetos do Adobe Workfront Planning

As tabelas nas seções a seguir ilustram o nível de permissões que você pode selecionar ao compartilhar um espaço de trabalho ou uma exibição e qual funcionalidade cada nível permite.

>[!IMPORTANT]
>
>Nem todos os usuários podem ter os níveis de permissão descritos abaixo. A licença individual dos usuários determina o nível de permissões que eles podem receber para objetos do Workfront Planning.
>
>Para obter informações, consulte [Visão geral do tipo de licença ao usar o Adobe Workfront Planning](/help/quicksilver/maestro/access/license-type-overview.md).


### Permissões do Workspace

Você deve conceder aos usuários permissão aos espaços de trabalho para permitir que eles tenham acesso às seguintes entidades:

* Espaços de trabalho
* Tipos de registro
* Registros
* Campos
<!--* Views*
    
    *You can allow all users with View or higher permissions to a workspace to also access a view. This is an additional permission that you must enable when sharing a view. For information, see [Share views](/help/quicksilver/maestro/access/share-views.md). -->

A seguir estão os níveis de permissões para espaços de trabalho:

|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Editar | ✓ µ |            |       |
| Compartilhar | ✓ µ |            |       |
| Excluir | ✓ µ |            |       |
| Exibir | ✓ µ | ✓ µ | ✓ µ |

### Permissões de tipo de registro

As permissões de Tipo de registro são herdadas ao conceder permissões ao espaço de trabalho.

A seguir estão os níveis de permissões para tipos de registro:


|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Criar | ✓ µ |            |       |
| Excluir | ✓ µ |            |       |
| Editar | ✓ µ |            |       |
| Exibir | ✓ µ | ✓ µ | ✓ µ |

### Registrar permissões

As permissões de registro são herdadas ao conceder permissões ao espaço de trabalho.

A seguir estão os níveis de permissões para registros:


|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Criar | ✓ µ |            |       |
| Excluir | ✓ µ | ✓ µ |       |
| Editar | ✓ µ | ✓ µ |       |
| Exibir | ✓ µ | ✓ µ | ✓ µ |

### Permissões de campo

As permissões de campo são herdadas ao conceder permissões ao espaço de trabalho.
As permissões a seguir se referem aos próprios campos e não aos valores associados a cada campo. Para editar valores de campo, você deve ter permissões para editar registros.

|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Criar | ✓ µ |            |       |
| Excluir | ✓ µ |            |       |
| Editar | ✓ µ |            |       |
| Exibir | ✓ µ | ✓ µ | ✓ µ |


### Exibir permissões

Você deve conceder permissões separadas para exibições de registros. A concessão de permissões para o espaço de trabalho não concede permissões para as exibições de registros no espaço de trabalho.

Você deve conceder aos usuários permissão para exibições para permitir que eles tenham acesso aos seguintes elementos de exibição:

* Filtros
* Visibilidade do campo
* Ordenar
* Agrupamento
* Altura da linha
* Configurações


<!--You can share views internally or publicly. -->

A seguir estão os níveis de permissões para exibições e elementos de exibição:

|        | Gerenciar | Exibir |
|--------|--------|-------|
| Editar | ✓ µ |       |
| Excluir | ✓ µ |       |
| Compartilhar | ✓ µ |       |
| Exibir | ✓ µ | ✓ µ |
| Aplicar | ✓ µ | ✓ µ |

<!--Replace the above with this when global sharing is released: 

|        | Manage | View  |View permissions to a workspace*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Apply  | ✓      | ✓     | ✓                          |

*Users must have View or higher permissions on a workspace to gain this view access.-->

<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |
| Delete | ✓      |       |
| Share  | ✓       |       |
| View   | ✓      | ✓     |
| Apply  | ✓      | ✓     |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->