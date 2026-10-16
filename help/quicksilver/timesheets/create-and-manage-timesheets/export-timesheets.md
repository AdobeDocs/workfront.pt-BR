---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Exportar uma lista de folhas de horas
description: Como gerente de pessoas ou aprovador de planilhas de horas, você pode precisar baixar uma lista de planilhas de horas para visualizar rapidamente as informações sobre as planilhas de horas das pessoas pelas quais você é responsável. Você pode fazer isso exportando uma lista de folhas de horas.
author: Lisa
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-bihpKoVoPCwTpAj-SK-RPPFpaCubsyLAfnfSmpTnyI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 64bb9e6dba8976ba413ec9b58e926da931bba1c5
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 14%
---
# Exportar uma lista de folhas de horas

<!--Audited: 8/2024-->

Como gerente de pessoas ou aprovador de planilhas de horas, você pode precisar baixar uma lista de planilhas de horas para visualizar rapidamente as informações sobre as planilhas de horas das pessoas pelas quais você é responsável. Você pode fazer isso exportando uma lista de folhas de horas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td> <p>Leve ou superior </p>
   <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td>Configuração do nível de acesso</td> 
   <td> <p>Acesso maior ou igual a tarefas e problemas</p> </td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Exibir ou aumentar permissões em tarefas e problemas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exportar uma lista de folhas de horas

{{step1-to-timesheets}}

Todas as planilhas de horas que você tem acesso para visualizar são exibidas por padrão.

![Lista de planilhas de horas](assets/list-of-all-timesheets.png)

1. (Opcional) Siga um destes procedimentos para atualizar o filtro na lista de folhas de horas:

   * Selecione **Minhas planilhas de horas aprovadas** no canto superior direito da página para exibir somente as planilhas de horas aprovadas por você,

     Ou

     Selecione **Minhas Planilhas de Horas** para exibir apenas suas planilhas de horas.

     Isso aplica os filtros **Minhas Aprovações de Planilha de Horas** ou **Minha Planilha de Horas** à lista de planilhas de horas.

   * Clique no ícone **Filtro** ![Ícone Filtro](assets/filter-nwepng.png) para aplicar um filtro ou criar um novo filtro. Para obter informações sobre como criar ou atualizar filtros, consulte [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >As opções Minhas aprovações de folha de horas e Minhas folhas de horas não são exibidas na parte superior da lista de folha de horas ou na lista de filtros se o administrador do Workfront ou um administrador de grupo removeu esses filtros dos Controles de lista na área Configuração ou do Modelo de layout. Para obter mais informações, consulte [Personalizar Filtros, Exibições e Agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Opcional) Clique nos ícones **Exibir** ![Exibir](assets/view-icon.png) ou **Agrupamento** ![Agrupamento](assets/grouping.png) para aplicar um modo de exibição ou agrupamento ou para criar um novo.

   Para obter informações sobre como criar filtros, visualizações ou agrupamentos, consulte os seguintes artigos:

   * [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Criar ou editar exibições no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Criar agrupamentos no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Selecione as planilhas de horas que deseja exportar e clique no ícone **Exportar** ![Exportar](assets/export-38x15.png).

   ![Clique no ícone Exportar](assets/export-timesheets.png)

1. Selecione o tipo de arquivo para o qual deseja exportar a lista de planilhas de horas a partir das seguintes opções:

   * PDF Ladscape
   * PDF Portrait
   * PDF de outros tamanhos
   * Excel
   * Excel (xlsx)
   * Delimitado por tabulação

   Uma lista de folhas de horas é baixada para o computador no formato selecionado e inclui as seguintes informações de folha de horas:

   * Date Range
   * Nome do proprietário
   * Horas totais
   * Valor de horas extras
   * Nomes dos aprovadores
   * Status
