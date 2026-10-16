---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Criar uma planilha de horas de uso único
description: Você pode criar manualmente uma folha de horas de uso único se quiser uma folha de horas que não seja recorrente. Quando a data de término da folha de horas é atingida e você precisa de mais folhas de horas, você deve criar novas.
author: Lisa
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
TQID: https://experienceleague.adobe.com/6ngmKzkpxxHYM7L9Z16JsJKcEW7CdFjJcdp6B6hgTtc
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
source-wordcount: '1048'
ht-degree: 7%
---
# Criar uma folha de horas de uso único

<!--Audited: 6/2025-->

Você pode criar manualmente uma folha de horas de uso único se quiser uma folha de horas que não seja recorrente. Quando a data de término da folha de horas é atingida e você precisa de mais folhas de horas, você deve criar novas.

Para obter informações sobre como criar um perfil de folha de horas que gere folhas de horas recorrentes para seus usuários sem nenhuma intervenção adicional (recomendado), consulte [Criar, editar e atribuir perfis de folha de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Para obter informações sobre como gerar folhas de horas manualmente para todos os usuários no sistema associados a um perfil de folha de horas, consulte [Gerar folhas de horas manualmente](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

>[!NOTE]
>
>* Planilha de horas de uso único não pode ser criada para grupos.
>* Ao criar uma folha de horas de uso único, você não pode selecionar tipos de horas gerais específicos para incluir em sua folha de horas. Todos os tipos de horas gerais ativados no seu sistema são exibidos em folhas de horas criadas manualmente.
>
>Se você quiser selecionar apenas determinados tipos de horas gerais para exibir em suas folhas de horas, use um perfil de folha de horas. Para obter mais informações sobre perfis de folha de horas, consulte [Criar, editar e atribuir perfis de folha de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

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

## Criar uma folha de horas de uso único

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
   >As opções Minhas aprovações de folha de horas e Minhas folhas de horas não são exibidas na parte superior da lista de folha de horas ou na lista de filtros se o administrador do Workfront ou um administrador de grupo removeu os filtros Minhas aprovações de folha de horas e Minhas folhas de horas dos Controles de lista na área Configuração ou do Modelo de layout. Para obter mais informações, consulte [Personalizar Filtros, Exibições e Agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Opcional) Clique no ícone **Pesquisar** ![Ícone Pesquisar](assets/search-icon.png) para digitar uma palavra-chave e procurar uma folha de horas específica. Por exemplo, você pode procurar um intervalo de tempo de planilha de horas do nome do proprietário.

1. (Opcional) Clique nos ícones **Exibir** ![Exibir](assets/view-icon.png) ou **Agrupamento** ![Agrupamento](assets/grouping.png) para aplicar um modo de exibição ou agrupamento ou para criar um novo.

   Para obter informações sobre como criar filtros, visualizações ou agrupamentos, consulte os seguintes artigos:

   * [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Criar ou editar exibições no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Criar agrupamentos no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Clique em **Nova Planilha de Horas** na parte superior da lista de planilhas de horas.

   Insira a seguinte informação:

   | Nome do Campo | Descrição |
   | --------- | ---------- |
   | Criar planilha de horas para | Comece a inserir o nome do usuário, uma função de trabalho ou uma equipe para a qual você está criando a folha de horas e clique neles quando eles forem exibidos na lista. |
   | Data de início | Esta é a data de início da folha de horas. |
   | Data final | Esta é a data de término da folha de horas. |
   | Aprovadores | <p>Os aprovadores são usuários que aprovam a folha de horas para os usuários associados à folha de horas. Somente usuários com direitos administrativos de planilha de horas podem ser definidos como aprovadores. Para obter mais informações sobre direitos administrativos de planilha de horas, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).</p> <p>Comece a inserir os nomes dos aprovadores de folha de horas e selecione-os quando eles aparecerem na lista.</p> <p>Você pode ter múltiplos aprovadores em uma planilha de horas. Nesse caso, depois que um dos aprovadores aprovar a folha de horas, ela será marcada como **Fechada** e desaparecerá da lista de aprovações da folha de horas de todos os aprovadores restantes.</p> |
   | Pode editar as horas | <p>Selecione esta opção se quiser permitir que os aprovadores editem horas na folha de horas.</p><p>Esta opção funciona junto com a configuração **Restringir edição da folha de horas a proprietários e administradores** na área Configuração > Folhas de horas e horas > Preferências. Para obter mais informações, consulte [Configurar preferências de horas e folha de horas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).</p><p>Existem os seguintes cenários:</p><p>Quando a opção **Restringir edição da folha de horas a proprietários e administradores** está habilitada:</p><ul><li>Os aprovadores só podem aprovar e rejeitar a folha de horas, independentemente de **Poder editar as horas** estar habilitada ou não.</li><li>Os gerentes dos proprietários da folha de horas só podem exibir as folhas de horas de seus subordinados diretos.</li></ul><p>Quando a opção **Restringir edição da folha de horas a proprietários e administradores** está desabilitada:</p><ul><li>Quando **Pode editar as horas** estiver habilitado, os aprovadores poderão enviar, reabrir ou fechar a folha de horas e editar as horas.</li><li>Quando a opção **Pode editar as horas** está desabilitada, os aprovadores não podem enviar, reabrir ou fechar a folha de horas e não podem editar as horas. Os aprovadores só podem aprovar ou rejeitar a folha de horas.</li><li>Os gerentes dos proprietários da folha de horas podem enviar, retroceder, reabrir e editar as folhas de horas de seus subordinados diretos.</li></ul><p>**OBSERVAÇÃO**</br> Depois que você enviar uma folha de horas para aprovação, não poderá mais editar as horas. Para retornar uma folha de horas enviada a um estado editável, cancele a folha de horas ou peça ao aprovador para rejeitar a folha de horas. Para obter mais informações, consulte [Enviar uma folha de horas para aprovação](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) e [Aprovar uma folha de horas](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md). |
   | Hora extra | Você pode optar por ocultar a caixa **Horas extras** na folha de horas. Essa opção está desabilitada por padrão. |

1. Clique em **Criar planilha de horas**.

## Quando tarefas e problemas aparecem na planilha de horas dos usuários

Uma tarefa ou problema atribuído a um usuário aparece automaticamente na folha de horas de um usuário se a tarefa ou problema atender a qualquer um dos seguintes critérios:

* O usuário registrou horas na tarefa ou problema
* As datas planejadas da tarefa ou problema estão dentro das datas da folha de horas
* A tarefa ou problema tem uma Data de Início Real (o status da tarefa ou problema é Em Andamento)
* A tarefa ou problema está fixado à folha de horas
* A data de conclusão planejada está no intervalo de datas da folha de horas e o status é Em andamento

Se as **Preencher folhas de horas previamente com ...** preferências (localizadas nas preferências de Horas e Folhas de horas) estiverem desmarcadas, a folha de horas mostrará problemas e tarefas com o status Em andamento. Para obter mais informações sobre as Preferências de Horas e Planilha de Horas, consulte [Configurar preferências de horas e planilha de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
