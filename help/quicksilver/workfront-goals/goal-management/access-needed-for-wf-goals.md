---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Requisitos para usar as metas do Workfront
description: O administrador do Adobe Workfront deve garantir que determinadas condições sejam atendidas antes que você possa acessar o Adobe Workfront Goals. Neste artigo, saiba mais sobre os requisitos de acesso, permissões e layout para acessar o Workfront Goals.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---

# Requisitos para usar as metas do Workfront

<!--Audited P&P only: 04/2025-->

O administrador do Adobe Workfront deve garantir que todas as condições a seguir sejam atendidas antes de você acessar o Adobe Workfront Goals:

* Sua organização deve adquirir a licença correta para o Workfront Goals. Para obter informações, consulte a seção [Obter acesso à organização do Workfront Goals](#obtain-workfront-goals-organization-access) neste artigo.

* Atribua o tipo correto de licença da Workfront. Para obter informações sobre como atribuir tipos de licença e níveis de acesso, consulte a seção [Atualizar tipos de licença e configurações de nível de acesso](#update-license-types-and-access-level-settings) neste artigo.

>[!NOTE]
>
>Usuários com um tipo de licença externa não podem acessar o Workfront Goals.

* Conceda acesso às Metas no seu nível de acesso. Para obter informações, consulte [Conceder acesso às Metas do Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* Atribua a você o modelo de layout que inclui a área Metas no menu principal.

  >[!NOTE]
  >
  >Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclui a área Metas no Menu principal.

  Para obter informações, consulte a seção [Adicionar Metas do Workfront a um modelo de layout](#add-workfront-goals-to-a-layout-template) neste artigo.

* Se você precisar modificar metas que não foram criadas por você mesmo, o criador da meta deverá compartilhar as metas com você e fornecer a você permissões de gerenciamento para elas.

  Para obter informações, consulte a seção [Compartilhar metas individuais com outros usuários](#share-individual-goals-with-other-users) neste artigo.

## Obter acesso à organização do Workfront Goals {#obtain-workfront-goals-organization-access}


Dependendo do plano Workfront em que sua empresa está no momento, os seguintes cenários existem:

* **Um novo plano do Workfront**: você deve ter um plano do Ultimate Workfront. As Metas do Workfront estão incluídas somente neste plano.

* **Um plano atual do Workfront**: sua organização deve adquirir uma licença adicional, além da licença da Workfront.

  Depois que sua organização compra a licença adicional, a Workfront ativa o Workfront Goals para sua conta. Para obter informações sobre como adquirir uma licença do Workfront Goals, entre em contato com o gerente de conta da Workfront.

Para obter informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Atualizar tipos de licença e configurações de nível de acesso  {#update-license-types-and-access-level-settings}

Dependendo do plano Workfront em que sua empresa está no momento, os seguintes cenários existem:

* **Novo modelo de nível de acesso**: o administrador do Workfront deve conceder a você um dos seguintes tipos de licença da Workfront para acessar o Workfront Goals:

   * Colaborador
   * Leve
   * Padrão

* **Modelo de nível de acesso atual**: o administrador do Workfront deve conceder a você um dos seguintes tipos de licença da Workfront para acessar o Workfront Goals:

   * Plano
   * Trabalho
   * Revisar
   * Solicitar

Depois que o administrador do Workfront conceder um desses tipos de licença, ele também deverá conceder acesso às Metas no seu nível de acesso. Para obter informações sobre acesso a Metas, consulte [Conceder acesso às Metas do Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

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
