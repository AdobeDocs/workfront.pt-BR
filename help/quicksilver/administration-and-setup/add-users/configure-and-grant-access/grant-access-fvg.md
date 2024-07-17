---
title: Conceder acesso a filtros, visualizações e agrupamentos
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário aos controles de filtro, visualização e agrupamento para listas e relatórios.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 1%

---

# Conceder acesso a filtros, visualizações e agrupamentos

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário aos controles de filtro, exibição e agrupamento para listas e relatórios, conforme explicado na [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Para obter informações sobre os controles de filtro, exibição e agrupamento, consulte [Elementos de relatório: filtros, exibições e agrupamentos](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Requisitos de acesso

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure o acesso do usuário a filtros, visualizações e agrupamentos usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, conforme explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no botão **Exibir** ou **Editar** à direita de Filtros e selecione as capacidades que deseja conceder em **Ajustar suas configurações**.

   ![](assets/gear-icon-filters-dashboards-groupings.jpg)

   Por padrão, os usuários com uma licença de Plano, Trabalho, Revisor ou Solicitação têm capacidades totais de Exibição e Edição. Os usuários com uma licença de Usuário externo não acessam filtros, visualizações e agrupamentos.

   <!--If this changes, undraft section with table below
   -->

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configurar acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

   Após criar o nível de acesso, você pode atribuí-lo a um usuário. Para obter mais informações, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--## Access to filters, views, and groupings by license type

Drafting out this section for now because the table is redundant since all four license types can do everything.</span>-->

Esta tabela lista o que um administrador do Workfront pode permitir que usuários com cada tipo de licença façam com filtros, visualizações e agrupamentos. Para obter informações sobre os tipos de licença da Workfront, consulte [visão geral das licenças da Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<thead>
<tr>
<th> Ação </th>
<th> Planejador </th>
<th> Trabalhador </th>
<th> Revisor </th>
<th> Solicitante </th>
</tr>
</thead>
<tbody>
<tr>
<td>Editar filtros, visualizações e agrupamentos</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
</tr>
<tr>
<td>Criar filtros, visualizações e agrupamentos</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
</tr>
<tr>
<td>Exibir filtros, visualizações e agrupamentos</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
</tr>
<tr>
<td>Excluir filtros, visualizações e agrupamentos</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
</tr>
<tr>
<td>Compartilhar filtros, visualizações e agrupamentos</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
</tr>
<tr>
<td>Compartilhar filtros, visualizações e agrupamentos em todo o sistema</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
<td>✓ µ</td>
</tr>
</tbody>
</table>
