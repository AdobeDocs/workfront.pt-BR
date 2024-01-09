---
title: Visão geral das permissões de compartilhamento no Adobe Maestro
description: Você pode compartilhar ou remover permissões de um espaço de trabalho ou visualização do Adobe Maestri.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 3c49657c929c414888e6678022ef61b1bba1a420
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 8%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!-- *********add to TOC****************-->

# Visão geral das permissões de compartilhamento no Adobe Maestro

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para ter acesso ao Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Você pode compartilhar ou remover permissões de um espaço de trabalho ou visualização do Adobe Maestri.

Este artigo descreve os níveis de permissão para objetos Maestro.

Para obter informações sobre como compartilhar espaços de trabalho ou exibições, consulte os seguintes artigos:

* [Compartilhar um espaço de trabalho](/help/quicksilver/maestro/access/share-workspaces.md)

* [Compartilhar uma exibição](/help/quicksilver/maestro/access/share-views.md)

## Objetos que você pode compartilhar no Adobe Maestro

Você pode compartilhar os seguintes objetos no Maestro:

* Espaços de trabalho

  Quando você compartilha um espaço de trabalho, todos os tipos de registro, registros e campos associados aos espaços de trabalho também são compartilhados. As exibições não são compartilhadas.

* Visualizações

## Considerações sobre o compartilhamento de objetos no Maestro

* Você deve ter a seguinte licença para criar espaços de trabalho no Maestro:

   * Novo modelo de preços: Licença padrão
   * Modelo de preço atual: licença de trabalho ou superior

  Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)
* Os administradores do sistema podem gerenciar e compartilhar espaços de trabalho criados por outros usuários.
* Se você não for um Administrador do sistema, poderá contribuir com espaços de trabalho criados por outros se eles forem compartilhados com você.
* Não é possível compartilhar espaços de trabalho em massa.
* Você pode compartilhar um espaço de trabalho com as seguintes entidades:
   * Usuários
   * Grupos
* Outros usuários, incluindo Administradores do sistema, só podem acessar as exibições que criaram ou que foram compartilhadas com eles.

## Permissões de compartilhamento para objetos do Maestro

As tabelas nas seções a seguir ilustram o nível de permissões que você pode selecionar ao compartilhar um espaço de trabalho ou view Maestri e qual funcionalidade cada nível permite.

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




<!--
<table>
  <tr>
   

   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td><p><b>New: Standard license</b></p> <p><b>Current: Worker or higher license</b></p></strong>
   </td>
   <td><strong>Manage permissions</strong>
   </td>
   <td><strong>Contribute permissions</strong>
   </td>
   <td><strong>View permissions</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Create</strong>
   </td>
   <td rowspan="5" ><strong>Workspace</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Delete</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Share</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Edit</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <td><strong>Create/delete</strong>
   </td>
   <td rowspan="3" ><strong>Record Type*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Edit</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <td><strong>Create/delete</strong>
   </td>
   <td rowspan="3" ><strong>Record*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Edit</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <tr>
   <td><strong>Create</strong>
   </td>
   <td rowspan="5" ><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Delete</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Share</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Edit</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>✓
   </td>
  </tr>

<tr>
   <td><strong>Create/delete</strong>
   </td>
   <td rowspan="3" ><strong>Fields*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Edit</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>



</table>

*Record types, records, and fields inherit permissions from the Workspace. -->



