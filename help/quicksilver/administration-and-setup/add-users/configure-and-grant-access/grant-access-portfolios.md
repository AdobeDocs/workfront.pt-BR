---
title: Conceder acesso a portfólios
user-type: administrator
product-area: system-administration;portfolios
navigation-topic: configure-access-to-workfront
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário a portfólios no Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f4a9c4f3-8ed4-4629-aced-9cc09b8acd3f
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Conceder acesso a portfólios

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário a portfólios, como explicado em [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar o acesso de usuários a portfólios usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, como explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no **Exibir** ou **Editar** à direita do Portfolio, em seguida, selecione as capacidades que deseja conceder **Ajustar as configurações**.

   ![](assets/fine-tune-portfolios.png)

   >[!NOTE]
   >
   >Quando você configura uma configuração de nível de acesso para um determinado tipo de objeto, essa configuração não afeta o acesso dos usuários a objetos com uma classificação menor. Por exemplo, você pode impedir que os usuários excluam portfólios em seu nível de acesso, mas isso não os restringe de excluir projetos, que são de classificação inferior à dos portfólios.Para obter mais informações sobre a hierarquia de objetos, consulte a seção [Interdependência e hierarquia de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) no artigo [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configuração do acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

   Depois que o nível de acesso é criado, você pode atribuí-lo a um usuário. Para obter mais informações, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acesso a carteiras por tipo de licença

Para obter informações sobre o que os usuários em cada nível de acesso podem fazer com portfólios, consulte a seção [Portfolio](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#portfoli) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acesso a portfólios compartilhados

Como proprietário ou criador de um portfólio, você pode compartilhar com outros usuários, concedendo a eles permissões, como explicado em [Compartilhar um portfólio](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Quando você compartilha qualquer objeto com outro usuário, os direitos do recipient são determinados por uma combinação de dois itens:

* As permissões concedidas ao destinatário para o objeto
* As configurações de nível de acesso do recipient para o tipo do objeto

Para obter informações sobre permissões que os usuários podem conceder em um portfólio ao compartilhá-lo, consulte [Compartilhar um portfólio](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).
