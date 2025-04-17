---
title: Visão Geral das Permissões de Compartilhamento no Adobe Workfront Planning
description: Nem todos os usuários na organização têm o mesmo acesso e permissões para usar o Adobe Workfront Planning. Este artigo descreve as informações gerais sobre compartilhamento ou remoção de permissões de um espaço de trabalho ou exibição do Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 5%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Visão geral das permissões de compartilhamento no Adobe Workfront Planning

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>



{{planning-important-intro}}

Você pode compartilhar ou remover permissões de um espaço de trabalho ou exibição do Adobe Workfront Planning.

Este artigo descreve os níveis de permissão para objetos do Workfront Planning.

## Objetos que você pode compartilhar no Adobe Workfront Planning

Você pode compartilhar manualmente os seguintes objetos no Workfront Planning:

* Espaços de trabalho

   * Você pode compartilhar espaços de trabalho com pessoas dentro da organização.
   * Quando você compartilha um espaço de trabalho, todos os tipos de registro, registros e campos associados aos espaços de trabalho também são compartilhados.
   * Quando você compartilha um espaço de trabalho, as exibições não são compartilhadas. As exibições são compartilhadas separadamente.

  Para obter mais informações, consulte [Compartilhar espaços de trabalho](/help/quicksilver/planning/access/share-workspaces.md)

<!--
<div class="preview">

* Record types

    * You can share record types with people inside your organization.
    * The level of permissions granted for the workspace displays as Inherited permissions for the record type. 
    * You cannot share a record type with a higher permission level than the user has on the workspace. 

    For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md). 

</div>
-->

* Visualizações

   * Você deve fornecer aos usuários, incluindo Administradores do sistema, permissões para acessar exibições separadamente de suas permissões para acessar espaços de trabalho.
   * Quando você compartilha uma exibição, todos os elementos da exibição são compartilhados, incluindo filtros, agrupamento, classificação ou Configurações.
   * Quando você compartilha uma exibição, os registros visíveis na exibição não são compartilhados. Os registros devem ser compartilhados por espaços de trabalho de compartilhamento.
   * Você pode compartilhar uma exibição publicamente, com pessoas de fora da organização ao gerar um link público para uma exibição. As pessoas que acessam a página de registro de um link público podem exibir todos os registros e seus campos, incluindo registros e campos conectados.

  Para obter mais informações, consulte [Compartilhar modos de exibição](/help/quicksilver/planning/access/share-views.md).

Internamente, você pode compartilhar um espaço de trabalho ou uma visualização com as seguintes entidades do Workfront:

* Usuários
* Grupos
* Equipes
* Empresas
* Funções de trabalho

<span class="preview"> Quando você compartilha espaços de trabalho e tipos de registro com outras pessoas, o nível de permissão do tipo de registro é automaticamente herdado para os registros e campos associados a eles. </span>

## Considerações sobre o compartilhamento de objetos no Adobe Workfront Planning

* Seu tipo de licença do Adobe Workfront funciona em conjunto com suas permissões do Workfront Planning para fornecer acesso a exibir, contribuir ou gerenciar espaços de trabalho e seus objetos.

  Para obter informações sobre como os tipos de licença afetam os níveis de permissão do Workfront Planning, consulte [Visão geral do tipo de licença ao usar o Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Os administradores do sistema podem gerenciar todos os espaços de trabalho no sistema, inclusive aqueles que não criaram.
* Outros usuários, incluindo Administradores do sistema, só podem acessar as exibições que criaram ou que foram compartilhadas com eles. Os administradores do sistema só podem receber permissões para Gerenciar uma visualização.
* Você pode compartilhar um link com outros usuários para um espaço de trabalho ou uma visualização.

  Existem os seguintes cenários:
   * Os usuários que recebem o link para um espaço de trabalho devem ser usuários ativos e fazer logon no Workfront para acessar o espaço de trabalho.
   * Os usuários que recebem o link para uma visualização podem acessá-la das seguintes maneiras:

      * Deve ser um usuário ativo e fazer logon no Workfront, se o link para a exibição foi compartilhado internamente.
      * Podem ser usuários externos do Workfront e acessar a visualização por meio de um link compartilhado publicamente, sem fazer logon no Workfront.

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


### Permissões do Workspace

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

### Permissões de tipo de registro

No ambiente de Produção, as permissões do Tipo de registro são sempre herdadas ao conceder permissões ao espaço de trabalho.

A seguir estão os níveis de permissões para tipos de registro:


|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Criar | ✓ |            |       |
| Excluir | ✓ |            |       |
| Editar | ✓ |            |       |
| Exibir | ✓ | ✓ | ✓ |

<div class="preview">

No ambiente de Pré-visualização, você pode remover as permissões herdadas do tipo de registro recebidas do espaço de trabalho.

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
>*Quando você remove permissões de um tipo de registro, os usuários ainda retêm permissões de Exibição para o espaço de trabalho e todos os tipos de registro, a menos que você remova as permissões deles do espaço de trabalho.

</div>

### Registrar permissões

As permissões de registro são herdadas de <span class="preview">o tipo de registro</span>, quando você concede permissões ao espaço de trabalho e <span class="preview">ao tipo de registro</span>.

A seguir estão os níveis de permissões para registros:


|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Criar | ✓ | ✓ |       |
| Excluir | ✓ | ✓ |       |
| Editar | ✓ | ✓ |       |
| Exibir | ✓ | ✓ | ✓ |

### Permissões de campo

As permissões de campo são herdadas de <span class="preview">o tipo de registro</span>, quando você concede permissões para o espaço de trabalho e <span class="preview">o tipo de registro</span>.

As permissões a seguir se referem aos próprios campos e não aos valores associados a cada campo. Para editar valores de campo, você deve ter permissões para editar registros.

|        | Gerenciar | Contribuir | Exibir |
|--------|--------|------------|-------|
| Criar | ✓ |            |       |
| Excluir | ✓ |            |       |
| Editar | ✓ |            |       |
| Exibir | ✓ | ✓ | ✓ |


### Exibir permissões

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