---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Criar, editar e atribuir perfis de folha de ponto
description: Você pode criar, editar e atribuir perfis de folha de ponto que geram folhas de ponto recorrentes para seus usuários sem nenhuma outra intervenção sua. Isso economiza tempo e garante que os seguintes itens sejam consistentes entre os usuários - EDITE-ME.
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 7e2a4b02277e8b82ac6ee92a7994250fcdebb0b0
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 1%

---

# Criar, editar e atribuir perfis de folha de ponto

Você pode criar, editar e atribuir perfis de folha de ponto que geram folhas de ponto recorrentes para seus usuários sem nenhuma outra intervenção sua. Isso economiza tempo e garante que os seguintes itens sejam consistentes entre os usuários:

* Intervalo de tempo da folha de ponto
* Aprovadores
* Tipos de hora gerais

Para obter mais informações sobre como criar uma folha de ponto manualmente, consulte [Criar uma folha de ponto de uso único](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

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
   <td> <p>Você deve ter acesso administrativo às Folhas de Horas. </p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p>  <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar ou editar um perfil de folha de ponto

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Para ativar as alterações de perfil da folha de horas nas folhas de horas atuais, é necessário excluir as folhas de horas existentes e gerar novas. Para obter instruções, consulte [Excluir folhas de ponto no Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) e [Gerar manualmente folhas de ponto](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Se você estiver criando ou editando um perfil de folha de ponto para uso em todo o sistema, clique em **Folha de Horas e Horas**.

   Ou

   Se você estiver criando ou editando um perfil de folha de ponto para um grupo, clique em **Grupos** e clique no nome do grupo.

1. Clique em **Perfis de Folha de Horas**.
1. Para criar um novo perfil de folha de horas, clique em **Novo perfil**.

   Ou

   Para editar um perfil de folha de ponto existente, selecione o perfil de folha de ponto que deseja editar e clique em **Editar**.

   O perfil de folha de ponto novo ou existente é exibido.


1. No **Definir detalhes** guia , digite um **Nome** e **Descrição** para o perfil da folha de ponto e forneça as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Grupo com Acesso de Administração</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Se estiver criando um perfil de folha de ponto no nível do sistema, deixe este campo em branco.</p> <p>Qualquer usuário que possa editar contas de usuário pode anexar uma folha de ponto no nível do sistema a outros usuários.</p> <p>Somente um administrador do Workfront pode editar um perfil de folha de ponto no nível do sistema.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Se estiver criando um perfil de folha de ponto para um grupo que você administra, identifique o grupo aqui.</p> <p>Isso não atribui o perfil da folha de ponto aos usuários do grupo; ela permite somente que os administradores do grupo modifiquem o perfil da folha de ponto. Você atribuirá o perfil aos usuários na Etapa 6.</p> <p><b>Nota</b>

   Quando usuários fora do grupo estão anexando perfis de folha de ponto a outros usuários, eles não poderão ver ou anexar esse perfil de folha de ponto.</p> </li>
   </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Criar planilhas de horas</strong> </td> 
      <td> <p> <p>Especifique quando o perfil de folha de ponto deve gerar as folhas de ponto. Uma folha de ponto pode ser configurada para gerar automaticamente em uma base semanal, quinzenal, semimensal ou mensal. Selecione o dia da semana em que deseja que a folha de horas seja produzida.</p> <p><b>Nota</b>

   Se você configurar um perfil de folha de ponto para criar folhas de ponto em uma sexta-feira, os usuários não poderão gravar horas na sexta, sábado e domingo para a semana atual.</p> <p>O Workfront sempre cria duas folhas de ponto por vez: a primeira folha de ponto sempre inclui a data atual e a segunda folha de ponto começa quando o período da primeira termina.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Aprovadores</strong></p> </td> 
      <td> <p> <p>Aprovadores são usuários que aprovam a folha de ponto para os usuários associados à folha de ponto. Você pode identificar até 7 usuários como aprovadores em uma folha de ponto. Identificar vários usuários é útil para garantir que um aprovador esteja disponível quando alguém estiver fora do escritório. Todos os aprovadores são notificados quando um usuário envia a folha de ponto para aprovação. Somente um usuário é necessário aprovar a folha de ponto para que ela seja aprovada.</p> <p>Somente usuários com direitos administrativos de folha de ponto podem ser definidos como aprovadores. Para obter mais informações sobre os direitos administrativos da folha de ponto, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p>Use o menu suspenso para selecionar o aprovador da folha de ponto (se um aprovador for necessário). Você pode selecionar entre as seguintes opções:</p> 
      <ul> 
      <li><strong>Nenhum</strong>: A folha de ponto não precisa ser aprovada.</li> 
      <li><strong>Gerente</strong>: Este é o aprovador padrão, definido pelo sistema. Nesse caso, o usuário designado como gerente aprova a folha de ponto quando é enviada para aprovação.</li> 
      <li><strong>Pessoas específicas:</strong> Você pode designar usuários específicos, por nome, como aprovadores da folha de ponto. Você pode ter vários aprovadores em uma folha de ponto. Nesse caso, depois que um dos aprovadores aprovar a folha de ponto, a folha de ponto é marcada como <strong>Fechado</strong> e desaparece da lista de aprovações da folha de ponto de todos os aprovadores restantes.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Pode editar as horas </strong> </td> 
      <td> <p> <p>Selecione essa opção para permitir que os aprovadores editem horas na folha de ponto.

   Essa opção funciona juntamente com o **Restringir edição de folha de ponto a proprietários e administradores** na área Configuração > Folha de horas > Preferências . Para obter mais informações, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurar preferências de hora e folha de ponto</a>.

   Os seguintes cenários existem:

   <ul>
      <li>Quando a variável <b>Restringir edição de folha de ponto a proprietários e administradores</b> está ativada:</li>
      <ul><li>Os aprovadores só podem aprovar e rejeitar a folha de ponto, independentemente de a variável <b>Pode editar tempo</b> está ativado ou não. </li>
      <li>Os gerentes dos proprietários da folha de ponto só podem exibir as folhas de ponto de seus relatórios diretos.</li></ul>
      <li>Quando a variável <b>Restringir edição de folha de ponto a proprietários e administradores</b> está desativada:</li>
    <ul><li>Quando a variável <b>Pode editar tempo</b> estiver ativado, os aprovadores podem enviar, reabrir ou fechar a folha de ponto e podem editar a hora.</li>
      <li>Quando a variável <b>Pode editar tempo</b> estiver desativado, os aprovadores não poderão enviar, reabrir ou fechar a folha de ponto e não poderão editar a hora. Os aprovadores só podem aprovar ou rejeitar a folha de ponto. </li>
      <li>Os gerentes dos proprietários da folha de ponto podem enviar, cancelar, reabrir e editar as folhas de ponto de seus relatórios diretos.</li></ul>
      </ul>

   <p><b>Nota</b>

   Depois de enviar uma folha de horas para aprovação, você não pode mais editar as horas. Para retornar uma folha de ponto enviada a um estado editável, recupere a folha de ponto ou peça para o aprovador rejeitar a folha de ponto. Para obter mais informações, consulte <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Enviar uma folha de ponto para aprovação</a> e<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Aprovar uma folha de ponto</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipos de horas disponíveis</strong> </td> 
      <td>Por padrão, os usuários visualizam todas as horas gerais em uma folha de ponto. No entanto, se sua organização quiser que apenas horas gerais específicas sejam mostradas para um conjunto específico de usuários, você poderá selecionar as horas gerais que eles precisam ver em suas folhas de horas selecionando-as no perfil da folha de horas nesse campo. Se quiser desativar todas as horas gerais, desmarque todos os tipos de hora para gerar a folha de horas sem uma seção para horas gerais.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Hora extra</span> </td> 
      <td>Você pode optar por ocultar a caixa Hora extra nas folhas de horas. Essa opção é desativada por padrão.</td> 
     </tr> 
    </tbody> 
    </table>

1. Clique no botão **Atribuir Pessoas** para associar o perfil da folha de ponto a usuários, grupos ou equipes específicas (se você for um administrador do Workfront). Comece digitando o nome do usuário, grupo ou equipe e clique nele quando ele for exibido na lista suspensa.

   Se você for um administrador de grupo, poderá atribuir o perfil da folha de ponto aos grupos que administra, mas não às equipes. Para obter mais informações, consulte [Limitações para um administrador de grupo que atribui um perfil de folha de ponto](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) neste artigo.

   >[!NOTE]
   >
   >* Também é possível associar um usuário a um perfil de folha de ponto editando o perfil do usuário. Para obter mais informações, consulte [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Quando você adiciona um grupo, somente o nome do grupo é exibido na guia Atribuir pessoas , não na lista de membros do grupo. Se quiser ver os membros do grupo listados aqui, clique em Salvar alterações e clique no nome do perfil da folha de ponto que acabou de criar.
   >* Quando você conclui essas etapas, o perfil de folha de ponto gera folhas de ponto somente para os usuários atribuídos ou membros do grupo que não têm folhas de ponto existentes para o período atual.


1. Clique em **Salvar alterações**.

   Na primeira vez que o perfil da folha de ponto gera folhas de ponto, 2 folhas de ponto são criadas para cada usuário. Depois disso, sempre que gerar novas folhas de ponto, uma folha de ponto será criada por usuário.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Limitações para um administrador de grupo que atribui um perfil de folha de ponto {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Se você for um administrador de grupo e a opção de acesso administrativo Folhas de horas e horas estiver desativada em seu nível de acesso, você poderá criar perfis de folha de horas, mas somente atribuí-los a:

* Grupos que você administra
* Usuários individuais que você tem acesso para editar e que estão em um grupo que você administra

Para esses grupos e usuários, você não terá acesso às folhas de horas geradas pelo perfil da folha de horas.

Além disso, se a opção Administrador do usuário (Usuários do grupo) também estiver desativada em seu nível de acesso, você poderá atribuir o perfil da folha de ponto a um grupo que você administra, mas afetará apenas os usuários do grupo que você tem acesso para editar. Se o grupo contiver usuários que você não tem acesso para editar, eles não receberão o perfil da folha de ponto juntamente com o restante do grupo.

Para obter informações sobre a opção Folhas de horas e horas no nível de acesso, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obter informações sobre a opção Administrador de usuário (usuários do grupo) em seu nível de acesso, consulte [Conceder acesso aos usuários](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Vários perfis recorrentes de folha de ponto

Você pode ter mais de um perfil de folha de ponto para sua organização se houver:

* Períodos de pagamento únicos para diferentes conjuntos de usuários
* Aprovadores únicos para diferentes conjuntos de usuários
* Requisitos gerais de horas únicos para diferentes conjuntos de usuários

Um usuário não pode ser associado a mais de um perfil de folha de ponto por vez. 
