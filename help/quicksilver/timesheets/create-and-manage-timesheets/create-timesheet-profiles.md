---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Criar, editar e atribuir perfis de folha de horas
description: Você pode criar, editar e atribuir perfis de planilha de horas que geram planilhas de horas recorrentes para seus usuários sem nenhuma intervenção adicional sua. Isso economiza tempo e garante a consistência entre os usuários.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 395a7788ddfda71264b7b964953435affd7761e9
workflow-type: tm+mt
source-wordcount: '1597'
ht-degree: 2%

---

# Criar, editar e atribuir perfis de folha de horas

<!--Audited: 06/2025-->

Você pode criar, editar e atribuir perfis de planilha de horas que geram planilhas de horas recorrentes para seus usuários sem nenhuma intervenção adicional sua. Isso economiza tempo e garante que os itens a seguir sejam consistentes entre os usuários:

* Intervalo de tempo da folha de ponto
* Aprovadores
* Tipos de hora gerais

Para obter mais informações sobre como criar uma folha de horas manualmente, consulte [Criar uma folha de horas de uso único](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Novo: Padrão </p>
 <p>ou</p> 
<p>Atual: Plano </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ter acesso administrativo a Planilhas de Horas. </p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação da Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar ou editar um perfil de planilha de horas

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Para habilitar alterações de perfil na folha de horas atual, você precisa excluir as folhas de horas existentes antes de fazer as alterações nos perfis de folha de horas e gerar novas folhas de horas. Para obter instruções, consulte [Excluir folhas de horas no Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) e [Gerar folhas de horas manualmente](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. Se você criar ou editar um perfil de planilha de horas para uso em todo o sistema, clique em **Planilha de horas e horas**.

   Ou

   Se você criar ou editar um perfil de planilha de horas para um grupo, clique em **Grupos** e, em seguida, clique no nome do grupo.

1. Clique em **Perfis de Planilha de Horas**.
1. Para criar um perfil de planilha de horas, clique em **Novo Perfil**.

   Ou

   Para editar um perfil de planilha de horas existente, selecione o perfil de planilha de horas que deseja editar e clique em **Editar**.

   A página de perfil da folha de horas nova ou existente é exibida.

1. Atualize as seguintes informações:

   * **Nome**: adicione um nome ao perfil da folha de horas. Pode ser o nome de uma equipe ou grupo cujas pessoas compartilham o mesmo período de suas folhas de horas. Este campo é obrigatório.
   * **Descrição**: adicione mais informações sobre o perfil da folha de horas.
   * **Grupo com Acesso de Administração**: se você estiver criando um perfil de planilha de horas no nível do sistema, deixe este campo em branco.

     Qualquer usuário que possa editar contas de usuário pode anexar uma planilha de horas no nível do sistema a outros usuários.

     Somente um administrador do Workfront pode editar um perfil de planilha de horas no nível do sistema.

     Se você estiver criando um perfil de planilha de horas para um grupo que administra, identifique o grupo aqui.

     Isso não atribui o perfil da folha de horas aos usuários no grupo; permite apenas que os administradores do grupo modifiquem o perfil da folha de horas. Você atribuirá o perfil aos usuários na Etapa 6.

     >[!NOTE]
     >
     >Quando usuários fora do grupo estão anexando perfis de folha de horas a outros usuários, eles não poderão ver ou anexar esse perfil de folha de horas.

   * **Criar folhas de horas**: especifique quando o perfil da folha de horas deve gerar as folhas de horas. Uma folha de horas pode ser definida para ser gerada automaticamente em uma base semanal, bissemanal, semestral ou mensal. Selecione o dia da semana em que você deseja que a folha de horas seja produzida.

     Uma planilha de horas semanal começa na data em que é gerada. Por exemplo, se você criar folhas de horas semanais todas as quintas-feiras, o primeiro dia da semana na folha de horas será quinta-feira.

     >[!NOTE]
     >
     >O Workfront sempre cria duas folhas de horas por vez: a primeira folha de horas sempre inclui a data atual e a segunda folha de horas começa quando o período da primeira termina.

   * **Aprovadores**: aprovadores são usuários que aprovam a folha de horas dos usuários associados à folha de horas. Você pode identificar até 7 usuários como aprovadores em uma folha de horas. Identificar vários usuários é útil para garantir que um aprovador esteja disponível quando alguém estiver fora do escritório. Todos os aprovadores são notificados quando um usuário envia a folha de horas para aprovação. Somente um usuário precisa aprovar a folha de horas para que ela seja aprovada.

     Somente usuários com direitos administrativos de planilha de horas podem ser definidos como aprovadores. Para obter mais informações sobre direitos administrativos de planilha de horas, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Use o menu suspenso para selecionar o aprovador para a folha de horas (se um aprovador for necessário). Você pode selecionar entre as opções a seguir:

      * **Nenhuma**: a folha de horas não precisa ser aprovada.
      * **Gerente**: este é o aprovador padrão, definido pelo sistema. Nesse caso, o usuário designado como gerente aprova a folha de horas quando ela é enviada para aprovação.
      * **Pessoas Específicas**: você pode designar usuários específicos, por nome, como aprovadores de planilhas de horas. Você pode ter múltiplos aprovadores em uma planilha de horas. Nesse caso, depois que um dos aprovadores aprovar a folha de horas, ela será marcada como **Fechada** e desaparecerá da lista de aprovações da folha de horas de todos os aprovadores restantes.

   * **Pode editar as horas**: selecione esta opção para permitir que os aprovadores editem as horas na folha de horas.

     Esta opção funciona junto com a configuração **Restringir edição da folha de horas a proprietários e administradores** na área Configuração > Folhas de horas e horas > Preferências. Para obter mais informações, consulte [Configurar preferências de horas e folha de horas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     Existem os seguintes cenários:

     Quando a opção **Restringir edição da folha de horas a proprietários e administradores** está habilitada:

      * Os aprovadores só podem aprovar e rejeitar a folha de horas, independentemente de o horário Pode editar estar ativado ou não.
      * Os gerentes dos proprietários da folha de horas só podem exibir as folhas de horas de seus subordinados diretos.

     Quando a opção **Restringir edição da folha de horas a proprietários e administradores** está desabilitada:

      * Quando **Pode editar as horas** estiver habilitado, os aprovadores poderão enviar, reabrir ou fechar a folha de horas e editar as horas.
      * Quando a opção **Pode editar as horas** está desabilitada, os aprovadores não podem enviar, reabrir ou fechar a folha de horas e não podem editar as horas. Os aprovadores só podem aprovar ou rejeitar a folha de horas.
      * Os gerentes dos proprietários da folha de horas podem enviar, retroceder, reabrir e editar as folhas de horas de seus subordinados diretos.

     >[!NOTE]
     >
     >Depois que você enviar uma folha de horas para aprovação, não poderá mais editar as horas. Para retornar uma folha de horas enviada a um estado editável, cancele a folha de horas ou peça ao aprovador para rejeitar a folha de horas. Para obter mais informações, consulte [Enviar uma folha de horas para aprovação](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) e [Aprovar uma folha de horas](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md).

   * **Horas Extras**: você pode optar por ocultar a caixa Horas Extras na planilha de horas. Essa opção está desabilitada por padrão.
   * **Tipos de Hora Disponíveis**: esta configuração se refere apenas aos Tipos de Hora Gerais, e não aos tipos de hora específicos do projeto.

     Por padrão, os usuários veem todas as horas gerais em uma folha de horas. No entanto, se sua organização quiser que apenas as horas gerais específicas sejam mostradas para um conjunto específico de usuários, você pode selecionar as horas gerais que eles precisam ver em suas folhas de horas, selecionando-os no perfil de folha de horas neste campo. Se quiser desativar todas as horas gerais, desmarque todos os tipos de horas para gerar a folha de horas sem uma seção para as horas gerais.

   * **Notificações de lembrete**: adicione uma notificação de lembrete. O Workfront enviará lembretes aos usuários para que eles concluam ou aprovem suas folhas de horas. Você deve criar notificações de lembrete antes de associá-las a um perfil de planilha de horas.

1. Para associar o perfil da folha de horas a usuários, grupos ou equipes específicos (se você for um administrador do Workfront), role em direção à parte inferior da página e localize a seção **Atribuir pessoas**.

   Comece a digitar o nome do usuário, grupo ou equipe e clique nele quando ele aparecer na lista suspensa.

   <!--To associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams, scroll towards the bottom of the page and find the **Assign People** section.-->

   Se você for um administrador de grupo, poderá atribuir o perfil da folha de horas aos grupos que administra, mas não às equipes. Para obter mais informações, consulte [Limitações para um administrador de grupo atribuir um perfil de folha de horas](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) neste artigo.

   >[!NOTE]
   >
   >* Você também pode associar um usuário a um perfil de planilha de horas editando o perfil do usuário. Para obter mais informações, consulte [Editar perfil de usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Quando você adiciona um grupo, somente o nome do grupo é exibido na guia Atribuir Pessoas, não a lista de membros do grupo. Se quiser ver os membros do grupo listados aqui, clique em Salvar Alterações, em seguida, clique no nome do perfil da planilha de horas que você acabou de criar.
   >* Ao concluir essas etapas, o perfil de folha de horas gera folhas de horas apenas para os usuários atribuídos ou membros do grupo que não têm folhas de horas existentes para o período atual.

1. Clique em **Salvar**.

1. Na parte superior da lista de perfis de folha de horas, clique no ícone **Mais** ícone ![Mais](assets/more-icon.png) e clique em **Gerar folhas de horas**.

   Uma confirmação é exibida na parte inferior da tela de que as folhas de horas foram geradas com sucesso. Novas planilhas de horas são geradas com base nos novos perfis que você criou.

   Para obter mais informações, consulte [Gerar folhas de horas manualmente](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

   Na primeira vez que o perfil de folha de horas gera folhas de horas, duas folhas de horas são criadas para cada usuário, tanto para o período que inclui o tempo atual quanto para o período seguinte.

   Depois disso, cada vez que ele gera novas folhas de horas, uma folha de horas é criada por usuário.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Limitações para um administrador de grupo que atribui um perfil de folha de horas {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Se você for um administrador de grupo e a opção de acesso administrativo Folhas de horas e horas estiver desativada no seu nível de acesso, será possível criar perfis de folha de horas, mas você poderá atribuí-los apenas a:

* Grupos que você administra
* Usuários individuais que você tem acesso para editar e que estão em um grupo que você administra

Para esses grupos e usuários, você não terá acesso às folhas de horas geradas pelo perfil da folha de horas.

Além disso, se a opção Administrador de usuários (usuários de grupo) também estiver desativada no seu nível de acesso, você poderá atribuir o perfil de planilha de horas a um grupo que administra, mas isso afetará somente os usuários no grupo que você tem acesso para editar. Se o grupo contiver usuários aos quais você não tem acesso para editar, eles não receberão o perfil da folha de horas junto com o restante do grupo.

Para obter informações sobre a opção Folhas de horas e horas no seu nível de acesso, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obter informações sobre a opção Administrador de Usuários (Usuários de Grupo) no seu nível de acesso, consulte [Conceder acesso aos usuários](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Vários perfis de planilha de horas recorrentes

Você pode ter mais de uma planilha de horas para sua organização se houver:

* Períodos de pagamento exclusivos para diferentes conjuntos de usuários
* Aprovadores únicos para diferentes conjuntos de usuários
* Requisitos exclusivos de horas gerais para diferentes conjuntos de usuários

Um usuário não pode ser associado a mais de um perfil de planilha de horas por vez.

<!--
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Add a name for the timesheet profile. It could be the name of a team or a group whose people share the same timeframe for their timesheets. </p> <p>This ia a required field.</p> </td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Add more information about the timesheet profile.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group's administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p>

   <p><b>NOTE</b>: When users outside the group are attaching timesheet profiles to other users, they won't be able to see or attach this timesheet profile.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p>
      <p>A weekly timesheet begins on the date it is generated. For example, if you create weekly timesheets every Thursday, the first day of the week on the timesheet is Thursday.</p>
    
      
   <p><b>NOTE</b>: Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet starts when the time frame of the first one ends.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvers</strong></p> </td> 
      <td> <p> <p>Approvers are users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
      <ul> 
      <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time </strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. 

   <p>This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.</p>

   <p>The following scenarios exist: </p>

   <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
      <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
      <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
    <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
      <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
      <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
      </ul>

   <p>

   <b>NOTE</b>: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Overtime</strong> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td><p>This setting refers only to General Hour Types, and not to project-specific hour types. </p>
      <p>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect all hour types to generate the timesheet without a section for general hours.</p></td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Reminder notifications</strong> </td> 
      <td> <p> Add a reminder notification. Workfront will send reminders to users to ask them to complete or approve their timesheets. You must create reminder notifications before you can associate them with a timesheet profile.  </p> </td> 
     </tr>
    </tbody> 
   </table>
-->