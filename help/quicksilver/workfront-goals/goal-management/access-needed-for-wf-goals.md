---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Requisitos para usar as metas do Workfront
description: O administrador do Adobe Workfront deve garantir que determinadas condições sejam atendidas antes que você possa acessar o Adobe Workfront Goals. Neste artigo, saiba mais sobre os requisitos de acesso, permissões e layout para acessar o Workfront Goals.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: dacfd8ef7475b197ac6ce5dd598c99df97037479
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Requisitos para usar as metas do Workfront

<!--Audited P&P only: 04/2025-->

O administrador do Adobe Workfront deve garantir que todas as condições a seguir sejam atendidas antes de você acessar o Adobe Workfront Goals:

* Sua organização adquiriu um pacote do Adobe Workfront Goals no passado. O Adobe Workfront Goals não está mais disponível para compra.

  Para obter mais informações, consulte a seção [Obter acesso à organização do Workfront Goals](#obtain-workfront-goals-organization-access) neste artigo.

* Atribua o tipo correto de licença da Workfront. Para obter informações sobre como atribuir tipos de licença e níveis de acesso, consulte a seção [Atualizar tipos de licença e configurações de nível de acesso](#update-license-types-and-access-level-settings) neste artigo.

  >[!NOTE]
  >
  >Usuários com um tipo de licença externa não podem acessar o Workfront Goals.

* Conceda acesso às Metas no seu nível de acesso. Para obter informações, consulte [Conceder acesso às Metas do Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

  >[!NOTE]
  >
  >Por padrão, os usuários não têm acesso às metas em seus níveis de acesso.


* Atribua a você o modelo de layout que inclui a área Metas no menu principal.

  >[!NOTE]
  >
  >Todos os usuários, incluindo Administradores do sistema, devem receber um modelo de layout que inclua a área Metas no Menu principal.

  Para obter informações, consulte a seção [Adicionar Metas do Workfront a um modelo de layout](#add-workfront-goals-to-a-layout-template) neste artigo.

* Se você precisar modificar metas que não foram criadas por você mesmo, o criador da meta deverá compartilhar as metas com você e fornecer a você permissões de gerenciamento para elas.

  Para obter informações, consulte a seção [Compartilhar metas individuais com outros usuários](#share-individual-goals-with-other-users) neste artigo.

## Obter acesso à organização do Workfront Goals {#obtain-workfront-goals-organization-access}

O último pacote do Adobe Workfront que incluiu o Workfront Goals foi o Adobe Workfront Ultimate.
O Workfront Goals não está mais disponível para compra de pacotes mais recentes.
Fale com o seu representante de conta para saber mais sobre os Objetivos do Workfront.

<!--Old: >
Depending on which Workfront plan your company is currently on, the following scenarios exist: 

* **A new Workfront plan**: You must have an Ultimate Workfront plan. Workfront Goals are included only in this plan. 

* **A current Workfront plan**: Your organization must purchase an additional license, in addition to the Workfront license.

  After your organization purchases the additional license, Workfront enables Workfront Goals for your account. For information about purchasing a license for Workfront Goals contact your Workfront account manager.

For information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Atualizar tipos de licença e configurações de nível de acesso  {#update-license-types-and-access-level-settings}

Se sua empresa tiver acesso ao Workfront Goals a partir de uma compra anterior, o administrador do Workfront deverá conceder a você o seguinte para acessar o Workfront Goals:

1. Uma das seguintes licenças:

   * Colaborador ou superior
   * Solicitação ou superior

<!--Old: 
* **The new access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

  * Contributor
  * Light
  * Standard

* **The current access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals:

  * Plan
  * Work 
  * Review
  * Request
-->

1. O seguinte nível de acesso:

   * Acesso igual ou superior a Metas no seu nível de acesso.

   Para obter informações sobre acesso a Metas, consulte [Conceder acesso às Metas do Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Como administrador do Workfront, você pode revisar o número de licenças do Workfront Goals em seu sistema e entender quantas estão habilitadas no momento. Para obter mais informações, consulte [Gerenciar licenças disponíveis em seu sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>O Workfront permite atribuir mais licenças do Workfront Goals que você adquiriu. No entanto, quando você atribuir mais licenças do que o permitido pelo contrato do Workfront Goals, um gerente de conta da Workfront entrará em contato com você para informar que você excedeu o número contratual.

## Adicionar Metas do Workfront a um modelo de layout {#add-workfront-goals-to-a-layout-template}

O administrador do Workfront ou do Grupo deve atribuir um Modelo de layout que inclua a área Metas no Menu principal para que você possa acessar as Metas do Workfront.

![Modelo de layout](assets/layout-template-align-highlighted-350x220.png)

O administrador do Workfront ou do Grupo também pode adicionar o seguinte ao modelo de layout para que você possa acessar facilmente o Workfront Goals:

* Uma guia fixada
* Transforme a área Metas em sua página inicial

Para obter informações sobre como atualizar o Modelo de layout, consulte os seguintes artigos:

* [Criar e gerenciar modelos de layout](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [Personalizar o Menu Principal usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [Personalizar páginas fixadas usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [Personalizar a página de aterrissagem usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [Atribuir usuários a um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## Compartilhar metas individuais com outros usuários {#share-individual-goals-with-other-users}

Por padrão, todos os usuários que têm pelo menos o acesso de Visualização a Metas em seus níveis de acesso podem visualizar todas as metas no Workfront.

Qualquer usuário com acesso para Editar metas pode criar metas e automaticamente obtém acesso para Gerenciar as metas que cria. Se precisarem editar as metas de outros usuários, alguém com permissões para Gerenciar essas metas deverá compartilhar com eles as metas que não criaram.

Para obter informações sobre como compartilhar metas com usuários e conceder a eles permissões de Gerenciamento, consulte [Compartilhar uma meta no Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
