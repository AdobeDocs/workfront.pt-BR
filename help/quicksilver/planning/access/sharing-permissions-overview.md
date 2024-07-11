---
title: Visão geral das permissões de compartilhamento no Adobe Workfront Planning
description: Você pode compartilhar ou remover permissões de um espaço de trabalho ou exibição do Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 6%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Visão geral das permissões de compartilhamento no Adobe Workfront Planning

{{planning-important-intro}}

Você pode compartilhar ou remover permissões de um espaço de trabalho ou exibição no Adobe Workfront Planning.

Este artigo descreve os níveis de permissão para objetos do Workfront Planning.

Para obter informações sobre como compartilhar espaços de trabalho ou exibições, consulte os seguintes artigos:

* [Compartilhar espaços de trabalho](/help/quicksilver/planning/access/share-workspaces.md)

* [Compartilhar exibições](/help/quicksilver/planning/access/share-views.md)

## Objetos que você pode compartilhar no Adobe Workfront Planning

Você pode compartilhar os seguintes objetos:

* Espaços de trabalho

  Quando você compartilha um espaço de trabalho, todos os tipos de registro, registros e campos associados aos espaços de trabalho também são compartilhados. As exibições não são compartilhadas.

* Visualizações

  Você deve fornecer aos usuários, incluindo administradores do sistema, permissões para acessar exibições separadamente de suas permissões para acessar espaços de trabalho. Para obter informações, consulte [Compartilhar exibições](/help/quicksilver/planning/access/share-views.md).

Você pode compartilhar um espaço de trabalho ou uma exibição com as seguintes entidades:

* Usuários
* Grupos

<!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->

## Considerações sobre o compartilhamento de objetos no Adobe Workfront Planning

* Seu tipo de licença do Adobe Workfront funciona em conjunto com suas permissões do Workfront Planning para fornecer acesso a exibir, contribuir ou gerenciar espaços de trabalho e seus objetos.

  Para obter informações sobre como os tipos de licença afetam os níveis de permissão para o Workfront Planning, consulte [Visão geral do tipo de licença ao usar o Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Os administradores do sistema podem gerenciar todos os espaços de trabalho no sistema, incluindo aqueles que não criaram.
* Outros usuários, incluindo Administradores do sistema, só podem acessar as exibições que criaram ou que foram compartilhadas com eles. Os administradores do sistema só podem receber permissões para Gerenciar uma visualização.
* Você pode compartilhar um link com outros usuários para um espaço de trabalho ou uma visualização.

  Os usuários que recebem o link devem ser usuários ativos e fazer logon no Workfront para acessar o espaço de trabalho ou a página do tipo de registro exibida na exibição selecionada.

## Permissões de compartilhamento para objetos do Adobe Workfront Planning

As tabelas nas seções a seguir ilustram o nível de permissões que você pode selecionar ao compartilhar um espaço de trabalho ou uma exibição e qual funcionalidade cada nível permite.

>[!IMPORTANT]
>
>Nem todos os usuários podem ter os níveis de permissão descritos abaixo. A licença individual dos usuários determina o nível de permissões que eles podem receber para objetos do Workfront Planning.
>
>Somente usuários de licença Padrão (ou Plano) podem ter permissões do Contribute ou Gerenciar para espaços de trabalho e Gerenciar permissões para exibições.
> 
>Os usuários com todos os outros tipos de licença podem ter permissões de Exibição para espaços de trabalho e exibições.
>
>Para obter informações, consulte [Visão geral do tipo de licença ao usar o Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Permissões do Workspace

Você deve conceder aos usuários permissão aos espaços de trabalho para permitir que eles tenham acesso às seguintes entidades:

* Espaços de trabalho
* Tipos de registro
* Registros
* Campos

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

|        | Gerenciar (somente pessoas convidadas podem acessar) | Exibir (somente pessoas convidadas podem acessar) | Todos no espaço de trabalho podem visualizar* |
|--------|--------|-------|------------------------------|
| Editar | ✓ µ |       |                            |
| Excluir | ✓ µ |       |                            |
| Compartilhar | ✓ µ |       |                           |
| Exibir | ✓ µ | ✓ µ | ✓ µ |
| Acessar a visualização | ✓ µ | ✓ µ | ✓ µ |
| Aplicar filtros temporários, agrupamentos, classificar | ✓ µ | ✓ µ | ✓ µ |

*Os usuários devem ter permissões de Visualização ou superiores em um espaço de trabalho para obter esse acesso de visualização.

<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Apply  | ✓      | ✓     | ✓                          |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->


<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |    
-->