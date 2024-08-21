---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Criar e gerenciar perfis de planilha de horas de um grupo
description: Quando você está visualizando um grupo gerenciado na área Grupos, é possível visualizar e trabalhar com os perfis de folha de horas para os quais os administradores do grupo, ou um de seus subgrupos, têm acesso administrativo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Criar e gerenciar os perfis de planilha de horas de um grupo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

Quando você está visualizando um grupo gerenciado na área Grupos, é possível visualizar e trabalhar com os perfis de folha de horas para os quais os administradores do grupo, ou um de seus subgrupos, têm acesso administrativo.

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

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
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador de grupo do grupo.</p>  <p>Você também deve ter acesso administrativo às Folhas de horas. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p>  <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

+++

## Criar e editar perfis de planilha de horas no nível do grupo

Você pode criar e editar perfis de planilha de horas para uso em um grupo gerenciado por você. Para obter instruções, consulte [Criar, editar e atribuir perfis de folha de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Excluir perfis de planilha de horas no nível de grupo

Você pode excluir perfis de planilhas de horas em uso por um grupo gerenciado por você. Para obter instruções, consulte [Excluir perfis de folha de horas](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Gerar folhas de horas de grupo manualmente

Para permitir que as alterações feitas nos perfis de folha de horas do grupo sejam refletidas nas folhas de horas do grupo atual, primeiro exclua as folhas de horas existentes e gere manualmente as novas. Para obter instruções, consulte [Gerar folhas de horas manualmente na área Folhas de horas e Horas](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) em [Gerar folhas de horas manualmente](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

Para obter informações sobre como excluir folhas de horas de grupo, consulte [Excluir folhas de horas no Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Exportar perfis de planilhas de horas de nível de grupo

{{step-1-to-setup}}

1. Clique em **Grupos**.

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo com os perfis de planilha de horas que deseja exportar.
1. Clique em **Perfis de Planilha de Horas**.
1. Clique em **Exportar** para exportar a lista de perfis de folha de horas do grupo.
