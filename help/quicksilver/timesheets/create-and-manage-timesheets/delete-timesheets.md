---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Excluir folhas de ponto no Adobe Workfront
description: As alterações feitas em um perfil de folha de ponto não são efetivas imediatamente para as folhas de ponto existentes no momento, conforme explicado em Criar, editar e atribuir perfis de folha de ponto. Para tornar as alterações visíveis nas folhas de horas existentes, você deve excluir as folhas de horas que foram geradas e gerar novas. Isso se aplica somente às folhas de ponto que foram geradas pela associação de perfis de folha de ponto aos usuários.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Excluir folhas de ponto no Adobe Workfront

As alterações feitas em um perfil de folha de ponto não são efetivas imediatamente para as folhas de ponto existentes no momento, conforme explicado em [Criar, editar e atribuir perfis de folha de ponto](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Para tornar as alterações visíveis nas folhas de horas existentes, você deve excluir as folhas de horas que foram geradas e gerar novas. Isso se aplica somente às folhas de ponto que foram geradas pela associação de perfis de folha de ponto aos usuários.

>[!NOTE]
>
>As folhas de horas que foram criadas manualmente não podem ser recriadas com a regeneração das folhas de horas, a menos que os usuários tenham sido associados a um perfil de folha de ponto desde que a folha de ponto foi criada manualmente. A exclusão de uma folha de ponto criada manualmente pode causar perda de dados. Para obter informações sobre como criar uma única folha de ponto, consulte [Criar uma folha de ponto de uso único](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Os administradores de Adobe Workfront ou administradores de grupo podem gerar folhas de horas para todos no sistema. Para obter mais informações sobre a geração manual de folhas de horas, consulte:

* [Gerar manualmente folhas de ponto](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [Criar e gerenciar os perfis de folha de ponto de um grupo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* Não é possível recuperar uma folha de ponto excluída.
>* Recomendamos que você não exclua folhas de horas antigas, pois elas não são geradas automaticamente com base nos perfis da folha de horas. É possível excluir as folhas de horas atuais e futuras e gerá-las manualmente se desejar que as alterações nos perfis da folha de horas sejam imediatamente visíveis nas novas folhas de horas.
>* Ao excluir folhas de ponto, as horas registradas em relação a tarefas, problemas e projetos não são excluídas. Somente as Horas Gerais são excluídas com a folha de ponto. Em um editor de texto separado, anote o que as Horas Gerais estão associadas à folha de ponto. Depois que a folha de ponto é excluída, você pode registrá-las na nova folha de ponto.
>


## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ter acesso administrativo às Folhas de Horas. </p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Excluir folhas de horas em uma lista

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Folhas de Horas**. O **Todos** O filtro é selecionado por padrão e exibe todas as folhas de horas que você tem acesso para visualizar.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Siga um destes procedimentos para atualizar o filtro na lista de folhas de horas:

   * Selecionar **Minhas aprovações de folha de ponto** no canto superior direito da página para exibir somente as folhas de horas que você aprovar

      Ou

      Selecionar **Minhas Folhas de Horas** para exibir somente as folhas de horas.

      Isso aplica as aprovações de minha folha de horas ou os filtros Minha folha de horas à lista de folhas de horas.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Clique no ícone Filtro ![](assets/filter-nwepng.png) para aplicar um filtro diferente ou criar um novo. Para obter informações sobre como criar ou atualizar filtros, consulte [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   As opções Minhas Aprovações de Folha de Horas e Minhas Folhas de Horas não são exibidas na parte superior da lista de Folha de Horas ou na lista de filtros se o administrador do Workfront ou um administrador de grupo removeu os filtros Minhas Aprovações de Folha de Horas e Minhas Folhas de Horas dos Controles de Lista na área Configuração ou do Modelo de Layout. Para obter mais informações, consulte os seguintes artigos:
   * [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Opcional) Clique no botão **Exibir** ![](assets/view-icon.png) ou **Agrupamento** ![](assets/grouping.png) para aplicar uma exibição ou agrupamento diferente ou para criar um novo.

   Para obter informações sobre a criação de filtros, exibições ou agrupamentos, consulte os seguintes artigos:

   * [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Criar ou editar exibições no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Criar agrupamentos no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Selecione uma ou várias folhas de horas que você deseja excluir e clique no botão **Excluir**  ![](assets/delete.png) ícone na parte superior da lista de folhas de horas.

1. Clique em **Excluir**.

   As folhas de horas selecionadas são excluídas e não podem ser recuperadas.

   Para gerar novas folhas de ponto, verifique se os usuários estão associados a um perfil de folha de ponto e peça ao administrador do Workfront ou a um administrador de grupo para gerar novas folhas de ponto.

   Para obter mais informações, consulte:

   * [Criar, editar e atribuir perfis de folha de ponto](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [Gerar manualmente folhas de ponto](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [Criar e gerenciar os perfis de folha de ponto de um grupo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## Excluir uma folha de ponto da página de folha de ponto

1. Clique no botão [!UICONTROL **Menu principal**] ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.
1. Clique na folha de ponto que deseja excluir para abri-la.
1. Clique no botão [!UICONTROL **Mais**] ícone ![](assets/more-icon.png) à direita do nome da folha de ponto e clique em **Excluir**.

   ![Excluir folha de ponto da página de folha de ponto](assets/delete-timesheet-from-timesheet-page.png)
1. Clique em [!UICONTROL **Excluir**] para confirmar.

   A folha de ponto é excluída e não pode ser recuperada.
