---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Enviar planilha de horas para aprovação
description: Enviar sua planilha de horas para aprovação oferece ao seu gerente visibilidade sobre suas horas de trabalho. Os aprovadores podem verificar se todo o tempo registrado foi alocado nas áreas corretas e se um número suficiente de horas foi registrado para o período de tempo.
author: Lisa
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
TQID: https://experienceleague.adobe.com/uxfkWowkcyC9zeX1vNaZaY-i3AFCHMngvflZ8-REnac
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
source-git-commit: 64bb9e6dba8976ba413ec9b58e926da931bba1c5
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 6%
---
# Enviar uma folha de horas para aprovação

<!--Audited: 8/2024-->

Enviar sua planilha de horas para aprovação oferece ao seu gerente visibilidade sobre suas horas de trabalho. Os aprovadores podem verificar se todo o tempo registrado foi alocado nas áreas corretas e se um número suficiente de horas foi registrado para o período de tempo.

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
   <p>Revisar ou superior </p>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Visualize ou aumente o acesso a tarefas e problemas </p> </td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Exibir permissões ou mais altas para a folha de horas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Enviar uma folha de horas para aprovação

* [Enviar uma planilha de horas para aprovação](#submit-a-timesheet-for-approval)
* [Exibir o status de uma folha de horas enviada](#view-the-status-of-a-submitted-timesheet)

### Enviar uma folha de horas para aprovação

Depois que um aprovador de folha de horas é definido (conforme descrito na seção [Designar aprovadores de folha de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) no artigo [Aprovar uma folha de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), o botão **Fechar** na parte inferior da folha de horas muda para um botão **Enviar para aprovação**.

Para submeter uma planilha de horas para aprovação:

1. Ir para uma planilha de horas configurada para ter um aprovador.
1. Registrar hora, conforme descrito em [Registrar hora](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Clique em **Enviar para aprovação** para iniciar o processo de aprovação da folha de horas.

   ![Botão Enviar para aprovação](assets/submit-for-approval-button-on-timesheet.png)

   O botão **Enviar para aprovação** foi substituído pelos botões **Aprovar**, **Rejeitar** e **Cancelar**. O status da planilha de horas muda para **Enviado**.

   Quando sua planilha de horas é enviada para aprovação, o aprovador vê a planilha de horas listada no widget **Minhas aprovações** na área **Página inicial**. As seguintes situações podem ocorrer:

   * Se eles aprovarem, o botão **Cancelar** será alterado para **Reabrir** e o status da folha de horas será atualizado para **Abrir**.
   * Se ele rejeitar, o botão **Enviar para aprovação** substituirá o botão **Cancelar** e o status da folha de horas será atualizado para **Rejeitado**.

1. (Opcional) Clique em **Cancelar** se precisar reabrir a folha de horas e atualizar suas horas. Para obter informações, consulte a seção [Cancelar uma folha de horas](#recall-a-timesheet) neste artigo.

### Exibir o status de uma folha de horas enviada {#view-the-status-of-a-submitted-timesheet}

Você poderá ver o status de uma planilha de horas depois de enviá-la.

Se o administrador do Workfront tiver ativado a Aprovação de folha de horas para o usuário e a Rejeição de folha de horas para os manipuladores de eventos do usuário, você será notificado depois que a folha de horas for aprovada ou rejeitada. Para obter informações sobre como habilitar notificações de eventos, consulte [Tipos de notificação de eventos](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Sem essas notificações, você pode saber mais sobre o status de suas folhas de horas enviadas na área Folha de horas do Workfront.

Para exibir o status de uma planilha de horas:

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

1. (Condicional) Se você selecionou **Minhas Planilhas de Horas**, verifique se a exibição **Padrão** foi aplicada e observe a coluna **Status**.

   As folhas de horas podem ter os seguintes status:

   | Status | Descrição |
   | --------- | ---------- |
   | Abrir | <p>Sua planilha de horas está aberta no momento e você pode registrar horas.</p><p>Uma folha de horas cancelada é exibida com um status de Aberta. Para obter informações, consulte a seção [Cancelar uma folha de horas](#recall-a-timesheet) neste artigo.</p> |
   | Enviado | Você enviou sua planilha de horas para aprovação, mas ela ainda não foi aprovada. Você pode cancelar uma folha de horas enviada para continuar a editá-la. Para obter informações, consulte a seção [Cancelar uma folha de horas](#recall-a-timesheet) neste artigo. |
   | Fechado | <p>Existem os seguintes cenários:</p><ul><li>Se a folha de horas não tiver um aprovador, você salvou seu tempo e a fechou.</li><li>Se a planilha de horas tiver um aprovador, você a submeteu para aprovação e ela foi aprovada.</li></ul> |
   | Rejeitado | Você enviou a planilha de horas para aprovação e o aprovador a rejeitou. |

## Cancelar uma planilha de horas {#recall-a-timesheet}

Você pode cancelar uma planilha de horas que já foi enviada para aprovação. Somente folhas de horas que não foram aprovadas podem ser recuperadas.

Para chamar novamente uma planilha de horas:

{{step1-to-timesheets}}

1. Clique em **Minhas Planilhas de Horas** no canto superior direito da tela ou selecione **Minhas Planilhas de Horas** no menu suspenso **Filtro** ![Ícone Filtro](assets/filter-nwepng.png).
1. Clique no intervalo de tempo de uma planilha de horas com o status **Enviado**.
1. Clique em **Cancelar**.

   A folha de horas se torna editável novamente e seu status muda para **Abrir**.
