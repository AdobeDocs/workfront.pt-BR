---
title: Visão geral das permissões de compartilhamento nos recursos de planejamento do Adobe Workfront
description: Você pode compartilhar ou remover permissões de um espaço de trabalho ou visualização do Adobe Maestri.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: c50ff48bbc492199b39db17b8c445207209bb6a5
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 7%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Visão geral das permissões de compartilhamento nos recursos de planejamento do Adobe Workfront

{{maestro-important-intro}}

Você pode compartilhar ou remover permissões de um espaço de trabalho ou exibição ao usar os recursos de planejamento no Adobe Workfront.

Este artigo descreve os níveis de permissão para objetos de recursos de planejamento.

Para obter informações sobre como compartilhar espaços de trabalho ou exibições, consulte os seguintes artigos:

* [Compartilhar espaços de trabalho](/help/quicksilver/maestro/access/share-workspaces.md)

* [Compartilhar exibições](/help/quicksilver/maestro/access/share-views.md)

## Objetos que você pode compartilhar nos recursos de planejamento do Adobe Workfront

Você pode compartilhar os seguintes objetos:

* Espaços de trabalho

  Quando você compartilha um espaço de trabalho, todos os tipos de registro, registros e campos associados aos espaços de trabalho também são compartilhados. As exibições não são compartilhadas.

* Visualizações

## Considerações sobre o compartilhamento de objetos nos recursos de planejamento do Adobe Workfront

* Seu tipo de licença do Adobe Workfront funciona em conjunto com suas permissões para fornecer acesso a visualização, contribuição ou gerenciamento de objetos ao usar os recursos do Planning.

  Para obter informações sobre como os tipos de licença afetam os níveis de permissão para objetos de recursos do Planning, consulte [Visão geral do tipo de licença ao usar os recursos de planejamento do Adobe Workfront](/help/quicksilver/maestro/access/license-type-overview.md).
* Os administradores do sistema podem gerenciar e compartilhar espaços de trabalho criados por outros usuários.
* Se você não for um Administrador do sistema, poderá contribuir com espaços de trabalho criados por outros se eles forem compartilhados com você.
* Não é possível compartilhar espaços de trabalho em massa.
* Você pode compartilhar um espaço de trabalho ou uma exibição com as seguintes entidades:
   * Usuários
   * Grupos
* Outros usuários, incluindo Administradores do sistema, só podem acessar as exibições que criaram ou que foram compartilhadas com eles. Os administradores do sistema só podem receber permissões para Gerenciar uma exibição.
* É possível compartilhar um link para um espaço de trabalho ou para uma exibição de uma página do tipo record com outras pessoas. Os usuários que recebem o link devem ser usuários ativos e fazer logon no Workfront para acessar o espaço de trabalho ou a página do tipo de registro exibida na exibição selecionada.

## Permissões de compartilhamento para objetos de recursos de planejamento do Adobe Workfront

As tabelas nas seções a seguir ilustram o nível de permissões que você pode selecionar ao compartilhar um espaço de trabalho ou uma exibição e qual funcionalidade cada nível permite.

>[!IMPORTANT]
>
>Nem todos os usuários podem ter os níveis de permissão descritos abaixo. A licença individual dos usuários determina o nível de permissões que eles podem receber para objetos de recursos de planejamento.
>
>Para obter informações, consulte [Visão geral do tipo de licença ao usar os recursos de planejamento do Adobe Workfront](/help/quicksilver/maestro/access/license-type-overview.md).


### Permissões do Workspace

|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Editar | ✓ µ |            |       |
| Compartilhar | ✓ µ |            |       |
| Excluir | ✓ µ |            |       |
| Exibir | ✓ µ | ✓ µ | ✓ µ |

### Permissões de tipo de registro

As permissões de Tipo de registro são herdadas ao conceder permissões ao espaço de trabalho.

|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Criar | ✓ µ |            |       |
| Excluir | ✓ µ |            |       |
| Editar | ✓ µ |            |       |
| Exibir | ✓ µ | ✓ µ | ✓ µ |

### Registrar permissões

As permissões de registro são herdadas ao conceder permissões ao espaço de trabalho.

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

|        | Gerenciar | Exibir |
|--------|--------|-------|
| Editar | ✓ µ |       |
| Excluir | ✓ µ |       |
| Exibir | ✓ µ | ✓ µ |
| Aplicar | ✓ µ | ✓ µ |






