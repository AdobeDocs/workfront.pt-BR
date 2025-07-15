---
title: Conceder acesso administrativo a um modelo de layout
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Como administrador do Adobe Workfront, você pode conceder acesso administrativo a um modelo de layout aos administradores de um grupo específico para que eles possam editar o modelo. Isso não atribui o modelo aos usuários no grupo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Conceder acesso administrativo a um modelo de layout

Como administrador do Adobe Workfront, você pode conceder acesso administrativo a um modelo de layout aos administradores de um grupo específico para que eles possam editar o modelo. Isso não atribui o modelo aos usuários no grupo.

Para obter informações sobre como atribuir usuários a um modelo de layout, consulte [Atribuir usuários a um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p>
  <p> Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.
Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conceder acesso administrativo a um modelo de layout

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique em **Conceder acesso a** na seção superior da página.
1. Na caixa exibida, clique em **Adicionar um grupo**, comece a digitar o nome do grupo, clique no nome quando ele aparecer e clique em **Concluído**.

   Todos os usuários designados como administradores do grupo especificado podem administrar o modelo de layout. No entanto, o template não é atribuído ao membro do grupo para uso. Para obter informações sobre como atribuir um modelo de layout a um grupo, consulte [Atribuir um modelo de layout aos usuários](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) neste artigo.

   >[!NOTE]
   >
   >* Quando um administrador de grupo cria um modelo de layout, a atribuição de acesso administrativo é obrigatória. O modelo de layout é designado e visível somente para o grupo especificado. Para obter mais informações, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). Para obter informações sobre administradores de grupo, consulte [Administradores de grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* Se você não conceder acesso administrativo aos administradores de um grupo específico, todos os usuários que podem editar contas de usuários terão acesso administrativo ao modelo de layout. Alguns administradores do Workfront optam intencionalmente por não conceder acesso administrativo a um modelo de layout para transformá-lo em um modelo de layout no nível do sistema.

1. Você pode clicar em **Salvar** a qualquer momento para salvar seu progresso e, em seguida, continuar modificando o modelo mais tarde.
