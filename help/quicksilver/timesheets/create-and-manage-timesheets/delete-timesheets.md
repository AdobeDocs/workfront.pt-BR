---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Excluir planilhas de horas no Adobe Workfront
description: As alterações feitas em um perfil de folha de horas não têm efeito imediatamente para as folhas de horas existentes, como explicado em Criar, editar e atribuir perfis de folha de horas. Para tornar as alterações visíveis em folhas de horas existentes, você deve excluir as folhas de horas que foram geradas e gerar novas. Isso se aplica somente às folhas de horas que foram geradas ao associar perfis de folha de horas a usuários.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Excluir planilhas de horas no Adobe Workfront

As alterações feitas em um perfil de planilha de horas não entrarão em vigor imediatamente para as planilhas existentes, conforme explicado em [Criar, editar e atribuir perfis de planilha de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Para tornar as alterações visíveis em folhas de horas existentes, você deve excluir as folhas de horas que foram geradas e gerar novas. Isso se aplica somente às folhas de horas que foram geradas ao associar perfis de folha de horas a usuários.

>[!NOTE]
>
>Planilhas de horas que foram criadas manualmente não podem ser recriadas regenerando planilhas de horas, a menos que os usuários tenham sido associados a um perfil de planilha de horas desde que a planilha de horas foi criada manualmente. A exclusão de uma folha de horas criada manualmente pode causar perda de dados. Para obter informações sobre como criar uma única folha de horas, consulte [Criar uma folha de horas de uso único](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Os administradores do Adobe Workfront ou de grupo podem gerar folhas de horas para todos no sistema. Para obter mais informações sobre a geração manual de folhas de horas, consulte:

* [Gerar folhas de horas manualmente](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [Criar e gerenciar os perfis de planilha de horas de um grupo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* Não é possível recuperar uma planilha de horas excluída.
>* Recomendamos que você não exclua folhas de horas anteriores, pois elas não são geradas automaticamente com base em perfis de folha de horas. Você pode excluir as folhas de horas atuais e futuras e gerá-las manualmente se quiser que as alterações em seus perfis de folha de horas sejam imediatamente visíveis nas novas folhas de horas.
>* Quando você exclui folhas de horas, as horas registradas em tarefas, problemas e projetos não são excluídas. Somente as Horas gerais são excluídas com a folha de horas. Em um editor de texto separado, anote quais Horas gerais estão associadas à folha de horas. Depois que a folha de horas for excluída, você pode registrá-las na nova folha de horas.
>

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ter acesso administrativo a Planilhas de Horas. </p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p>Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Excluir planilhas de horas em uma lista

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal**, no canto superior direito do Adobe Workfront.

1. Clique em **Folhas de horas**. O filtro **Todos** é selecionado por padrão e exibe todas as planilhas de horas que você tem acesso para visualizar.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Siga um destes procedimentos para atualizar o filtro na lista de folhas de horas:

   * Selecione **Minhas planilhas de horas aprovadas** no canto superior direito da página para exibir somente as planilhas de horas aprovadas por você

     Ou

     Selecione **Minhas Planilhas de Horas** para exibir apenas suas planilhas de horas.

     Isso aplica os filtros Minhas planilhas de horas ou Minha planilha de horas à lista de planilhas de horas.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Clique no ícone Filtro ![](assets/filter-nwepng.png) para aplicar um filtro diferente ou criar um novo. Para obter informações sobre como criar ou atualizar filtros, consulte [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >As opções Minhas aprovações de folha de horas e Minhas folhas de horas não são exibidas na parte superior da lista de folha de horas ou na lista de filtros se o administrador do Workfront ou um administrador de grupo removeu os filtros Minhas aprovações de folha de horas e Minhas folhas de horas dos Controles de lista na área Configuração ou do Modelo de layout. Para obter mais informações, consulte os seguintes artigos:
   >
   >   
   >   
   >   * [Personalizar Filtros, Modos de Exibição e Agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Opcional) Clique nos ícones **Visualização** ![](assets/view-icon.png) ou **Agrupamento** ![](assets/grouping.png) para aplicar uma visualização ou agrupamento diferente ou para criar um novo.

   Para obter informações sobre como criar filtros, visualizações ou agrupamentos, consulte os seguintes artigos:

   * [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Criar ou editar exibições no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Criar agrupamentos no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Selecione uma ou várias planilhas de horas que você deseja excluir e clique no ícone **Excluir** ![](assets/delete.png) na parte superior da lista de planilhas de horas.

1. Clique em **Excluir**.

   As folhas de horas selecionadas são excluídas e não podem ser recuperadas.

   Para gerar novas folhas de horas, verifique se os usuários estão associados a um perfil de folha de horas e peça ao administrador do Workfront ou a um administrador de grupo para gerar novas folhas de horas.

   Para obter mais informações, consulte o seguinte:

   * [Criar, editar e atribuir perfis de planilha de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [Gerar folhas de horas manualmente](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [Criar e gerenciar os perfis de planilha de horas de um grupo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## Excluir uma planilha de horas da página Planilha de horas

1. Clique no ícone ![](assets/main-menu-icon.png) do [!UICONTROL **Menu principal**], no canto superior direito do Adobe Workfront.
1. Clique na folha de horas que deseja excluir para abri-la.
1. Clique no ícone [!UICONTROL **Mais**] ![](assets/more-icon.png) à direita do nome da folha de horas e clique em **Excluir**.

   ![Excluir planilha de horas da página de planilha de horas](assets/delete-timesheet-from-timesheet-page.png)
1. Clique em [!UICONTROL **Excluir**] para confirmar.

   A folha de horas foi excluída e não pode ser recuperada.
