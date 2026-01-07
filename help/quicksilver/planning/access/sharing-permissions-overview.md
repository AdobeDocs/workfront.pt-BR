---
title: Visão Geral das Permissões de Compartilhamento no Adobe Workfront Planning
description: Nem todos os usuários na organização têm o mesmo acesso e permissões para usar o Adobe Workfront Planning. Este artigo descreve as informações gerais sobre compartilhamento ou remoção de permissões de um espaço de trabalho ou exibição do Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 5%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Visão geral das permissões de compartilhamento no Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

Você pode compartilhar ou remover permissões de um espaço de trabalho, tipo de registro ou exibição do Adobe Workfront Planning.

Também é possível compartilhar formulários de solicitação do Planning. Para obter informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Este artigo descreve os níveis de permissão para espaços de trabalho do Workfront Planning, tipos de registro, registros, campos e exibições.

## Objetos que você pode compartilhar no Adobe Workfront Planning

Você pode compartilhar manualmente alguns objetos do Workfront Planning, enquanto outros objetos herdam essas permissões de outros objetos.

Você pode compartilhar manualmente os seguintes objetos no Workfront Planning:

* Espaços de trabalho

   * Você pode compartilhar espaços de trabalho com pessoas dentro da organização.
   * Quando você compartilha um espaço de trabalho, todos os tipos de registro, registros e campos associados aos espaços de trabalho também são compartilhados.
   * Quando você compartilha um espaço de trabalho, as exibições não são compartilhadas. As exibições são compartilhadas separadamente.

  Para obter mais informações, consulte [Compartilhar espaços de trabalho](/help/quicksilver/planning/access/share-workspaces.md)

* Tipos de registro

   * Você pode compartilhar tipos de registro com pessoas dentro da organização.
   * O nível de permissões concedidas para o espaço de trabalho é exibido como Permissões herdadas para o tipo de registro.
   * Não é possível compartilhar um tipo de registro com um nível de permissão superior ao do usuário no espaço de trabalho.

  Para obter mais informações, consulte [Compartilhar tipos de registros](/help/quicksilver/planning/access/share-record-types.md).


* Exibições

   * Você deve fornecer aos usuários, incluindo Administradores do sistema, permissões para acessar exibições separadamente de suas permissões para acessar espaços de trabalho.
   * Quando você compartilha uma exibição, todos os elementos da exibição são compartilhados, incluindo filtros, agrupamento, classificação ou Configurações.
   * Quando você compartilha uma exibição, os registros visíveis na exibição não são compartilhados. Os registros devem ser compartilhados por espaços de trabalho de compartilhamento.
   * Você pode compartilhar uma exibição publicamente, com pessoas de fora da organização ao gerar um link público para uma exibição. As pessoas que acessam a página de registro de um link público podem exibir todos os registros e seus campos, incluindo registros e campos conectados.

  Para obter mais informações, consulte [Compartilhar modos de exibição](/help/quicksilver/planning/access/share-views.md).

## Considerações sobre o compartilhamento de objetos no Adobe Workfront Planning

* Seu tipo de licença do Adobe Workfront funciona em conjunto com suas permissões do Workfront Planning para fornecer acesso a exibir, contribuir ou gerenciar espaços de trabalho e seus objetos.

  Para obter informações sobre como os tipos de licença afetam os níveis de permissão do Workfront Planning, consulte [Visão geral do tipo de licença ao usar o Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Os administradores do sistema podem gerenciar todos os espaços de trabalho no sistema, inclusive aqueles que não criaram.
* Outros usuários, incluindo Administradores do sistema, só podem acessar as exibições que criaram ou que foram compartilhadas com eles. Os administradores do sistema só podem receber permissões para Gerenciar uma visualização.

* Quando você compartilha espaços de trabalho e tipos de registro com outras pessoas, o nível de permissão do tipo de registro é automaticamente herdado para os registros e campos associados a eles.

  >[!IMPORTANT]
  >
  >Se a instância do Workfront da sua organização tiver sido integrada à Adobe Unified Experience, os usuários com os quais você deseja compartilhar objetos do Planning deverão ser adicionados à Adobe Admin Console. Não é possível compartilhar objetos do Planning com usuários do Workfront que não foram adicionados ao Adobe Admin Console.

* Você pode compartilhar objetos do Planning das seguintes maneiras:

   * Internamente, você pode compartilhar um espaço de trabalho, uma exibição ou um tipo de registro com as seguintes entidades do Workfront:

      * Usuários
      * Grupos
      * Equipes
      * Empresas
      * Funções de trabalho

     É possível compartilhar um objeto do Planning com até 100 entidades por objeto.

   * Internamente, compartilhando um link para um espaço de trabalho ou para uma exibição com outros usuários do Planning. Existem os seguintes cenários:

      * Os usuários que recebem o link para um espaço de trabalho devem ser usuários ativos e fazer logon no Workfront para acessar o espaço de trabalho.
      * Os usuários que recebem um link Compartilhamento interno para uma exibição devem ser usuários ativos e fazer logon no Workfront para acessar a exibição.
   * Externamente, compartilhando um link de compartilhamento Público com uma visualização com usuários externos que não têm uma conta do Workfront.

## Permissões de compartilhamento para objetos do Adobe Workfront Planning

As tabelas nas seções a seguir ilustram o nível de permissões que você pode selecionar ao compartilhar um espaço de trabalho ou uma exibição e qual funcionalidade cada nível permite.

>[!IMPORTANT]
>
>Nem todos os usuários podem ter os níveis de permissão descritos abaixo. A licença individual dos usuários determina o nível de permissões que eles podem receber para objetos do Workfront Planning.
>
>Somente os usuários com licença Padrão (ou Plano) podem ter permissões de Contribute ou Gerenciar para espaços de trabalho e Gerenciar permissões para exibições.
> 
>Os usuários com todos os outros tipos de licença podem ter permissões de Exibição para espaços de trabalho e exibições.
>
>Para obter informações, consulte [Visão geral do tipo de licença ao usar o Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Permissões para espaços de trabalho

Você deve conceder aos usuários permissão aos espaços de trabalho para permitir que eles tenham acesso às seguintes entidades:

* Espaços de trabalho
* Tipos de registro
* Registros
* Campos

A seguir estão os níveis de permissões para espaços de trabalho:

|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Editar | ✓ |            |       |
| Compartilhar | ✓ |            |       |
| Excluir | ✓ |            |       |
| Exibir | ✓ | ✓ | ✓ |

### Permissões para tipos de registro

<!-- old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

As permissões de Tipo de registro são sempre herdadas ao conceder permissões ao espaço de trabalho.

Você pode remover as permissões herdadas do tipo de registro recebidas do espaço de trabalho.

Você pode conceder aos usuários permissões mais baixas no tipo de registro do que no espaço de trabalho.

No entanto, você não pode fazer o seguinte:

* Conceda permissões mais altas para o tipo de registro do que os usuários têm no espaço de trabalho.
* Conceda aos gerentes de espaço de trabalho permissões mais baixas em um tipo de registro.
* Remova as permissões de Exibição ao tipo de registro ou ao espaço de trabalho removendo usuários das permissões de tipo de registro.

Existem os seguintes cenários:

| Permissões do Workspace | Permissões herdadas automáticas para um Tipo de Registro | Possíveis permissões de Tipo de registro quando Permissões herdadas estão desativadas (concedidas manualmente) |
|--------|--------|-------------|
| Gerenciar | Gerenciar | Gerenciar, remover permissões* |
| Contribuir | Contribuir | Permissões para Colaborar, Exibir, Remover* |
| Exibir | Exibir | Exibir, remover permissões* |

>[!NOTE]
>
>Ao remover permissões de um tipo de registro, os usuários ainda retêm permissões de Exibição para o espaço de trabalho e todos os tipos de registro, a menos que você remova as permissões deles do espaço de trabalho.

### Permissões para registros

As permissões de registro são herdadas do tipo de registro quando você concede permissões ao espaço de trabalho e ao tipo de registro.

A seguir estão os níveis de permissões para registros:


|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Criar | ✓ | ✓ |       |
| Excluir | ✓ | ✓ |       |
| Editar | ✓ | ✓ |       |
| Exibir | ✓ | ✓ | ✓ |

### Permissões para registrar campos

As permissões de campo são herdadas do tipo de registro, ao conceder permissões ao espaço de trabalho e ao tipo de registro.

As permissões a seguir se referem aos próprios campos e não aos valores associados a cada campo. Para editar valores de campo, você deve ter permissões para editar registros.

|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Criar | ✓ |            |       |
| Excluir | ✓ |            |       |
| Editar | ✓ |            |       |
| Exibir | ✓ | ✓ | ✓ |


### Permissões para visualizações

Você deve conceder permissões separadas para exibições de registros. A concessão de permissões para o espaço de trabalho não concede permissões para as exibições de registros no espaço de trabalho.

Você deve conceder aos usuários permissão para exibições para permitir que eles tenham acesso aos seguintes elementos de exibição:

* Filtros
* Visibilidade do campo
* Ordenar
* Agrupamento
* Altura da linha
* Configurações

Você pode compartilhar visualizações interna ou publicamente.

A seguir estão os níveis de permissões para exibições e elementos de exibição:

| Compartilhamento interno | Gerenciar (somente pessoas convidadas podem acessar) | Exibir (somente pessoas convidadas podem acessar) | Todos no espaço de trabalho podem visualizar* |
|--------|--------|-------|------------------------------|
| Editar | ✓ |       |                            |
| Excluir | ✓ |       |                            |
| Compartilhar | ✓ |       |                           |
| Exibir | ✓ | ✓ | ✓ |
| Aplicar | ✓ | ✓ | ✓ |

| Compartilhamento público | Exibir |
|--------|-------|
| Exibir | ✓ |
| Aplicar | ✓ |

*Os usuários devem ter permissões de Visualização ou superiores em um espaço de trabalho para obter esse acesso de visualização.

<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->
