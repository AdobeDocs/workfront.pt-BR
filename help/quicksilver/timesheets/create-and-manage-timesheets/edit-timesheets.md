---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Editar informações da folha de horas
description: Como um usuário com acesso administrativo a Folhas de horas, você pode editar informações em folhas de horas existentes no Adobe Workfront. Por exemplo, você pode editar o Proprietário, os Aprovadores ou o intervalo de tempo da folha de horas.
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
TQID: https://experienceleague.adobe.com/--QshuygnTfcEJtt6-Tx-2QtNT-5p9TrTWaQTMBZNAg
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
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a3c1ab8fc8012199d9863fc978cca7418fa0a2f5
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 9%
---
# Editar informações da folha de horas

Como um usuário com acesso administrativo a Folhas de horas, você pode editar informações em folhas de horas existentes no Adobe Workfront. Por exemplo, você pode editar o Proprietário, os Aprovadores ou o intervalo de tempo da folha de horas.

Você pode editar informações em uma única folha de horas ou pode editar várias folhas de horas em massa.

>[!IMPORTANT]
>
>Se os usuários estiverem associados a Perfis de Planilha de Horas e as planilhas de horas forem geradas automaticamente, as alterações feitas nas planilhas existentes não serão refletidas nas planilhas de horas que serão geradas para datas futuras. Todas as folhas de horas geradas automaticamente têm as configurações estabelecidas nos Perfis de folha de horas. Para obter mais informações, consulte [Criar perfis de planilha de horas](../create-and-manage-timesheets/create-timesheet-profiles.md)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>
   <p>Padrão</p>
   <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td><p>Acesso administrativo a planilhas de horas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar planilhas de horas

{{step1-to-timesheets}}

Todas as planilhas de horas que você tem acesso para visualizar são exibidas por padrão.

![Lista de planilhas de horas](assets/list-of-all-timesheets.png)

1. (Opcional) Clique no ícone **pesquisar** ![ícone Pesquisar](assets/search-icon.png) e digite uma palavra-chave para procurar uma folha de horas específica. Por exemplo, você pode procurar um intervalo de tempo de planilha de horas ou nome de proprietário.

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

1. Selecione uma ou várias planilhas de horas e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png) na parte superior da lista de planilhas de horas.
1. Exibir ou inserir as seguintes informações:

   | Nome do Campo | Descrição |
   | --------- | ---------- |
   | Proprietário | <p>Esse é o nome do usuário para o qual a folha de horas foi criada. Não é possível editar esse campo.</p><p>Esse campo não é exibido quando você seleciona várias folhas de horas.</p> |
   | Data de início | Esta é a data de início da folha de horas. |
   | Data final | Esta é a data de término da folha de horas. |
   | Status | <p>Este é o status da folha de horas. A seguir estão opções possíveis de status da folha de horas:</p><ul><li>**Abrir**: a folha de horas está aberta e as entradas de horas podem ser editadas.</li><li>**Enviado**: a planilha de horas é enviada para aprovação dos aprovadores designados.</li><li>**Rejeitada**: a folha de horas não foi aprovada pelos aprovadores e agora está disponível novamente para o usuário editar as entradas de horas.</li><li>**Fechado**: a folha de horas foi fechada pelo usuário ou aprovada pelo aprovador e, como resultado, agora está fechada. Não é possível adicionar horas a uma folha de horas fechada.</li></ul> |
   | Aprovadores | <p>Os aprovadores são usuários que aprovam a folha de horas para os usuários associados à folha de horas. Somente usuários com direitos administrativos de planilha de horas podem ser definidos como aprovadores. Para obter mais informações sobre direitos administrativos de planilha de horas, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).</p> <p>Comece a inserir os nomes dos aprovadores de folha de horas e selecione-os quando eles aparecerem na lista.</p> <p>Você pode ter múltiplos aprovadores em uma planilha de horas. Nesse caso, depois que um dos aprovadores aprovar a folha de horas, ela será marcada como **Fechada** e desaparecerá da lista de aprovações da folha de horas de todos os aprovadores restantes.</p> |
   | Pode editar as horas | <p>Selecione esta opção se quiser permitir que os aprovadores editem horas na folha de horas.</p><p>Essa opção não está disponível quando você seleciona várias folhas de horas.</p> |
   | Hora extra | <p>Você pode optar por ocultar a caixa Horas extras na folha de horas.</p><p>Essa opção está desabilitada por padrão.</p> |

1. Clique em **Salvar**.
