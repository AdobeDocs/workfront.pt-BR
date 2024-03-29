---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Enviar uma planilha de horas para aprovação
description: Enviar sua planilha de horas para aprovação oferece ao seu gerente visibilidade sobre suas horas de trabalho. Os aprovadores podem verificar se todo o tempo registrado foi alocado nas áreas corretas e se um número suficiente de horas foi registrado para o período de tempo.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 0%

---

# Enviar uma planilha de horas para aprovação

Enviar sua planilha de horas para aprovação oferece ao seu gerente visibilidade sobre suas horas de trabalho. Os aprovadores podem verificar se todo o tempo registrado foi alocado nas áreas corretas e se um número suficiente de horas foi registrado para o período de tempo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso de visualização ou superior a tarefas e problemas</p> <p>Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir ou aumentar permissões em tarefas e problemas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Enviar uma planilha de horas para aprovação

* [Enviar uma planilha de horas para aprovação](#submit-a-timesheet-for-approval)
* [Exibir o status de uma folha de horas enviada](#view-the-status-of-a-submitted-timesheet)

### Enviar uma planilha de horas para aprovação

Depois que um aprovador de planilha de horas é definido (conforme descrito na seção [Designar aprovadores de planilhas de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) no artigo [Aprovar uma planilha de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), o **Fechar** na parte inferior da folha de horas muda para um **Enviar para aprovação** botão.

Para submeter uma planilha de horas para aprovação:

1. Ir para uma planilha de horas configurada para ter um aprovador.
1. Registrar o tempo, conforme descrito em [Registrar tempo](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Clique em **Enviar para aprovação** para iniciar o processo de aprovação de planilha de horas.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   A variável **Enviar para aprovação** O botão é substituído pelo **Aprovar**, **Rejeitar**, e **Retroceder** botões. O status da folha de horas muda para **Enviado**.

   Quando sua planilha de horas é enviada para aprovação, o aprovador vê a planilha de horas listada no **Aprovações** área na **Início** página. As seguintes situações podem ocorrer:

   * Se o aprovarem, a **Retroceder** botão muda para **Reabrir** e as atualizações de status da folha de horas em **Abertura**.
   * Se o rejeitarem, a **Enviar para aprovação** O botão substitui a **Retroceder** e o status da folha de horas é atualizado para **Rejeitado**.

1. (Opcional) Clique em **Retroceder** se precisar reabrir a folha de horas e atualizar as horas. Para obter informações, consulte a [Cancelar uma planilha de horas](#recall-a-timesheet) neste artigo.

### Exibir o status de uma folha de horas enviada {#view-the-status-of-a-submitted-timesheet}

Você poderá ver o status de uma planilha de horas depois de enviá-la.

Se o administrador do Workfront tiver ativado a Aprovação de folha de horas para o usuário e a Rejeição de folha de horas para os manipuladores de eventos do usuário, você será notificado depois que a folha de horas for aprovada ou rejeitada. Para obter informações sobre como ativar notificações de eventos, consulte [Tipos de notificação de eventos](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Sem essas notificações, você pode saber mais sobre o status de suas folhas de horas enviadas na área Folha de horas do Workfront.

Para exibir o status de uma planilha de horas:

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.
1. Clique em **Planilhas de Horas**. A variável **Todos** é selecionado por padrão.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Siga um destes procedimentos para atualizar o filtro na lista de folhas de horas:

   * Selecionar **Minhas planilhas de horas aprovadas** no canto superior direito da página para exibir somente as folhas de horas que você aprova

     Ou

     Selecionar **Minhas Planilhas de Horas** para exibir apenas suas planilhas de horas.

     Isso aplica os filtros Minhas planilhas de horas ou Minha planilha de horas à lista de planilhas de horas.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Clique no ícone Filtro ![](assets/filter-nwepng.png) para aplicar um filtro diferente ou criar um novo. Para obter informações sobre como criar ou atualizar filtros, consulte [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >As opções Minhas aprovações de folha de horas e Minhas folhas de horas não são exibidas na parte superior da lista de folha de horas ou na lista de filtros se o administrador do Workfront ou um administrador de grupo removeu os filtros Minhas aprovações de folha de horas e Minhas folhas de horas dos Controles de lista na área Configuração ou do Modelo de layout. Para obter mais informações, consulte os seguintes artigos:
   >
   >   
   >   
   >   * [Personalizar filtros, visualizações e agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Condicional) Se você selecionou **Minhas Planilhas de Horas**, assegurar que a **Padrão** for aplicada e observe o **Status** coluna.

   As planilhas de horas podem ter os seguintes status:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aberto</td> 
      <td> <p>Sua planilha de horas está aberta no momento e você pode registrar horas. </p> <p>Uma folha de horas cancelada é exibida com um status de Aberta. Para obter informações, consulte a <a href="#recall-a-timesheet" class="MCXref xref">Cancelar uma planilha de horas</a> neste artigo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviados</td> 
      <td>Você enviou sua planilha de horas para aprovação, mas ela ainda não foi aprovada. Você pode cancelar uma folha de horas enviada para continuar a editá-la. Para obter informações, consulte a <a href="#recall-a-timesheet" class="MCXref xref">Cancelar uma planilha de horas</a> neste artigo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fechado</td> 
      <td> <p>Existem os seguintes cenários:</p> 
       <ul> 
        <li> <p>Se a folha de horas não tiver um aprovador, você salvou seu tempo e a fechou.</p> </li> 
        <li> <p>Se a planilha de horas tiver um aprovador, você a submeteu para aprovação e ela foi aprovada.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rejeitado</td> 
      <td>Você enviou a planilha de horas para aprovação e o aprovador a rejeitou.</td> 
     </tr> 
    </tbody> 
   </table>

## Cancelar uma planilha de horas {#recall-a-timesheet}

Você pode cancelar uma planilha de horas que já foi enviada para aprovação. Somente folhas de horas que não foram aprovadas podem ser recuperadas.

Para chamar novamente uma planilha de horas:

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Planilhas de Horas**.
1. Clique em **Minhas Planilhas de Horas** no canto superior direito da tela ou selecione **Minhas Planilhas de Horas** do **Filtro** ![](assets/filter-nwepng.png) menu suspenso.
1. Clique no intervalo de tempo para uma planilha de horas com status de **Enviado**.
1. Clique em **Retroceder**.

   A folha de horas se torna editável novamente e seu status muda para **Abertura**.
