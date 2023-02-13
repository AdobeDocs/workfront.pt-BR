---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Editar informações da folha de ponto
description: Como usuário com acesso administrativo às Folhas de horas, você pode editar informações nas Folhas de horas existentes no Adobe Workfront . Por exemplo, você pode editar o Proprietário, os Aprovadores ou o período da folha de ponto.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 2%

---

# Editar informações da folha de ponto

Como usuário com acesso administrativo às Folhas de horas, você pode editar informações nas Folhas de horas existentes no Adobe Workfront . Por exemplo, você pode editar o Proprietário, os Aprovadores ou o período da folha de ponto.

Você pode editar informações em uma única folha de ponto ou pode editar várias folhas de ponto em massa.

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
   <td> <p>Você deve ter acesso administrativo às Folhas de Horas. </p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Editar folhas de horas

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Folhas de Horas**.

   O **Todos** O filtro é selecionado por padrão, exibindo todas as folhas de horas que você tem acesso para visualizar.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Clique no botão **pesquisa** ícone ![](assets/search-icon.png) e digite uma palavra-chave e procure por uma folha de ponto específica. Por exemplo, você pode pesquisar por um período da folha de ponto ou nome do proprietário.

1. (Opcional) Siga um destes procedimentos para atualizar o filtro na lista de folhas de horas:

   * Selecionar **Minhas aprovações de folha de ponto** no canto superior direito da página para exibir somente as folhas de horas que você aprovar

      Ou

      Selecionar **Minhas Folhas de Horas** para exibir somente as folhas de horas.

      Isso aplica as aprovações de minha folha de horas ou os filtros Minha folha de horas à lista de folhas de horas.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Clique no ícone Filtro ![](assets/filter-nwepng.png) para aplicar um filtro diferente ou criar um novo. Para obter informações sobre como criar ou atualizar filtros, consulte [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >As opções Minhas Aprovações de Folha de Horas e Minhas Folhas de Horas não são exibidas na parte superior da lista de Folha de Horas ou na lista de filtros se o administrador do Workfront ou um administrador de grupo removeu os filtros Minhas Aprovações de Folha de Horas e Minhas Folhas de Horas dos Controles de Lista na área Configuração ou do Modelo de Layout. Para obter mais informações, consulte os seguintes artigos:
   * [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Opcional) Clique no botão **Exibir** ![](assets/view-icon.png) ou **Agrupamento** ![](assets/grouping.png) para aplicar uma exibição ou agrupamento diferente ou para criar um novo.

   Para obter informações sobre a criação de filtros, exibições ou agrupamentos, consulte os seguintes artigos:

   * [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Criar ou editar exibições no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Criar agrupamentos no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Selecione uma ou várias folhas de horas e clique no botão **Editar** ícone ![](assets/edit-icon.png) na parte superior da lista de folha de ponto.
1. Exibir ou especificar as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Proprietário</strong> </td> 
      <td> <p>Esse é o nome do usuário para o qual a folha de ponto foi criada. Não é possível editar esse campo. </p> <p>O campo não é exibido quando você seleciona várias folhas de horas. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data de início</strong> </td> 
      <td>Esta é a data de início da folha de ponto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data Final</strong> </td> 
      <td> Esta é a data final da folha de ponto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aprovadores</strong> </td> 
      <td> <p>Aprovadores são usuários que aprovam a folha de ponto para os usuários associados à folha de ponto. Somente os usuários com acesso administrativo às Folhas de Horas podem ser definidos como aprovadores. </p> <p>Para obter mais informações sobre os direitos administrativos da folha de ponto, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p>Comece a inserir os nomes dos aprovadores da folha de ponto e selecione-os quando eles forem exibidos na lista.</p> <p>Você pode ter vários aprovadores em uma folha de ponto. Nesse caso, depois que um dos aprovadores aprovar a folha de ponto, a folha de ponto é marcada como <strong>Fechado</strong> e desaparece da lista de aprovações da folha de ponto de todos os aprovadores restantes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Pode editar as horas</strong> </td> 
      <td> <p>Selecione essa opção se desejar permitir que aprovadores editem horas na folha de ponto.</p> <p>Essa opção não está disponível ao selecionar várias folhas de horas. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Hora extra</span> </td> 
      <td> <p>Você pode optar por ocultar a caixa Hora extra na folha de ponto.</p> <p>Essa opção é desativada por padrão.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em Salvar.
