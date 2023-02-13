---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Enviar uma folha de ponto para aprovação
description: O envio da folha de ponto para aprovação fornece ao gerente visibilidade sobre o horário de trabalho. Os aprovadores podem verificar se todas as horas registradas foram atribuídas nas áreas corretas e se foi registrado um número suficiente de horas para o período.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Enviar uma folha de ponto para aprovação

O envio da folha de ponto para aprovação fornece ao gerente visibilidade sobre o horário de trabalho. Os aprovadores podem verificar se todas as horas registradas foram atribuídas nas áreas corretas e se foi registrado um número suficiente de horas para o período.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Exibir acesso ou superior a Tarefas e problemas</p> <p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou permissões superiores em tarefas e problemas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Enviar uma folha de ponto para aprovação

* [Enviar uma folha de ponto para aprovação](#submit-a-timesheet-for-approval)
* [Exibir o status de uma folha de ponto enviada](#view-the-status-of-a-submitted-timesheet)

### Enviar uma folha de ponto para aprovação

Depois que um aprovador da folha de ponto é definido (conforme descrito na seção [Designar aprovadores da folha de ponto](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) no artigo [Aprovar uma folha de ponto](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), **Fechar** na parte inferior da folha de ponto, o botão muda para um **Enviar para aprovação** botão.

Para enviar uma folha de ponto para aprovação:

1. Vá para uma folha de ponto que foi configurada para ter um aprovador.
1. Tempo de registro, conforme descrito em [Tempo de registro](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Clique em **Enviar para aprovação** para iniciar o processo de aprovação da folha de ponto.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   O **Enviar para aprovação** é substituído pelo botão **Aprovar**, **Rejeitar** e **Recall** botões. O status da folha de ponto muda para **Enviado**.

   Quando sua folha de horas é enviada para aprovação, o aprovador vê a folha de horas listada na variável **Aprovações** na área **Início** página. Os seguintes itens podem ocorrer:

   * Se o aprovarem, a variável **Recall** botão muda para **Reabrir** e o status da folha de ponto é atualizado para **Abrir**.
   * Se eles rejeitarem, a variável **Enviar para aprovação** substitui o botão **Recall** e o status da folha de ponto é atualizado para **Rejeitada**.

1. (Opcional) Clique em **Recall** se precisar reabrir a folha de ponto e atualizar sua hora. Para obter informações, consulte o [Lembrar uma folha de ponto](#recall-a-timesheet) neste artigo.

### Exibir o status de uma folha de ponto enviada {#view-the-status-of-a-submitted-timesheet}

Você pode visualizar o status de uma folha de ponto depois de enviá-la.

Se o administrador do Workfront tiver ativado a Aprovação de folha de horas para o usuário e a Rejeição de folha de horas para manipuladores de eventos do usuário, você será notificado depois que a folha de horas for aprovada ou rejeitada. Para obter informações sobre como ativar notificações de eventos, consulte [Notificações de evento disponíveis no Adobe Workfront](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Sem essas notificações, você pode saber mais sobre o status das folhas de horas enviadas na área Folha de horas do Workfront.

Para exibir o status de uma folha de ponto:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.
1. Clique em **Folhas de Horas**. O **Todos** filtro é selecionado por padrão.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Siga um destes procedimentos para atualizar o filtro na lista de folhas de horas:

   * Selecionar **Minhas aprovações de folha de ponto** no canto superior direito da página para exibir somente as folhas de horas que você aprovar

      Ou

      Selecionar **Minhas Folhas de Horas** para exibir somente as folhas de horas.

      Isso aplica as aprovações de minha folha de horas ou os filtros Minha folha de horas à lista de folhas de horas.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Clique no ícone Filtro ![](assets/filter-nwepng.png) para aplicar um filtro diferente ou criar um novo. Para obter informações sobre como criar ou atualizar filtros, consulte [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >As opções Minhas Aprovações de Folha de Horas e Minhas Folhas de Horas não são exibidas na parte superior da lista de Folha de Horas ou na lista de filtros se o administrador do Workfront ou um administrador de grupo removeu os filtros Minhas Aprovações de Folha de Horas e Minhas Folhas de Horas dos Controles de Lista na área Configuração ou do Modelo de Layout. Para obter mais informações, consulte os seguintes artigos:
   >
   >   
   >   
   >   * [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Condicional) Se você selecionou **Minhas Folhas de Horas**, assegure que **Padrão** for aplicada e observe a variável **Status** coluna.

   As folhas de horas podem ter os seguintes status:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aberto</td> 
      <td> <p>Sua folha de ponto está aberta no momento e você pode registrar o tempo. </p> <p>Uma folha de ponto recordada é exibida com um status Abrir. Para obter informações, consulte o <a href="#recall-a-timesheet" class="MCXref xref">Lembrar uma folha de ponto</a> neste artigo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviados</td> 
      <td>Você enviou sua folha de ponto para aprovação, mas ela ainda não foi aprovada. Você pode lembrar de uma folha de ponto enviada para continuar a editá-la. Para obter informações, consulte o <a href="#recall-a-timesheet" class="MCXref xref">Lembrar uma folha de ponto</a> neste artigo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fechado</td> 
      <td> <p>Os seguintes cenários existem:</p> 
       <ul> 
        <li> <p>Se a folha de horas não tiver aprovador, você salvou o tempo e o fechou.</p> </li> 
        <li> <p>Se a folha de ponto tiver um aprovador, você a submeteu para aprovação e ela foi aprovada.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rejeitado</td> 
      <td>Você enviou a folha de ponto para aprovação e o aprovador a rejeitou.</td> 
     </tr> 
    </tbody> 
   </table>

## Lembrar uma folha de ponto {#recall-a-timesheet}

Você pode lembrar de uma folha de ponto que já foi enviada para aprovação. Somente as folhas de ponto que não foram aprovadas podem ser recuperadas.

Para lembrar uma folha de ponto:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Folhas de Horas**.
1. Clique em **Minhas Folhas de Horas** no canto superior direito da tela ou selecione **Minhas Folhas de Horas** do **Filtro** ![](assets/filter-nwepng.png) menu suspenso.
1. Clique no período para uma folha de ponto com status de **Enviado**.
1. Clique em **Recall**.

   A folha de ponto torna-se editável novamente e seu status muda para **Abrir**.
