---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Criar, editar e atribuir perfis de planilha de horas
description: Você pode criar, editar e atribuir perfis de planilha de horas que geram planilhas de horas recorrentes para seus usuários sem nenhuma intervenção adicional sua. Isso economiza tempo e garante a consistência entre os usuários.
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1472'
ht-degree: 0%

---

# Criar, editar e atribuir perfis de planilha de horas

Você pode criar, editar e atribuir perfis de planilha de horas que geram planilhas de horas recorrentes para seus usuários sem nenhuma intervenção adicional sua. Isso economiza tempo e garante que os itens a seguir sejam consistentes entre os usuários:

* Intervalo de tempo da folha de ponto
* Aprovadores
* Tipos de hora gerais

Para obter mais informações sobre como criar uma folha de horas manualmente, consulte [Criar uma planilha de horas de uso único](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Novo: Padrão </p>
 <p>ou</p> 
<p>Atual: Plano </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ter acesso administrativo a Planilhas de Horas. </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar ou editar um perfil de planilha de horas

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Para habilitar alterações de perfil na planilha de horas atual, você precisa excluir as planilhas existentes e gerar novas. Para obter instruções, consulte [Excluir planilhas de horas no Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) e [Gerar folhas de horas manualmente](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. Se você estiver criando ou editando um perfil de planilha de horas para uso em todo o sistema, clique em **Horas e Planilha de Horas**.

   Ou

   Se você criar ou editar um perfil de planilha de horas para um grupo, clique em **Grupos**, em seguida, clique no nome do grupo.

1. Clique em **Perfis de Planilha de Horas**.
1. Para criar um novo perfil de planilha de horas, clique em **Novo perfil**.

   Ou

   Para editar um perfil de planilha de horas existente, selecione o perfil de planilha de horas que deseja editar e clique em **Editar**.

   O perfil de planilha de horas novo ou existente é exibido.


1. No **Definir detalhes** digite uma **Nome** e **Descrição** para o perfil da folha de horas e forneça as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Grupo com Acesso de Administração</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Se você estiver criando um perfil de planilha de horas no nível do sistema, deixe este campo em branco.</p> <p>Qualquer usuário que possa editar contas de usuário pode anexar uma planilha de horas no nível do sistema a outros usuários.</p> <p>Somente um administrador do Workfront pode editar um perfil de planilha de horas no nível do sistema.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Se você estiver criando um perfil de planilha de horas para um grupo que administra, identifique o grupo aqui.</p> <p>Isso não atribui o perfil da folha de horas aos usuários no grupo; permite apenas que os administradores do grupo modifiquem o perfil da folha de horas. Você atribuirá o perfil aos usuários na Etapa 6.</p>

   <p><b>NOTA</b>: quando usuários fora do grupo anexam perfis de folha de horas a outro usuário, eles não poderão ver ou anexar esse perfil de folha de horas.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Criar planilhas de horas</strong> </td> 
      <td> <p> <p>Especifique quando o perfil de planilha de horas deve gerar as planilhas de horas. Uma folha de horas pode ser definida para ser gerada automaticamente em uma base semanal, bissemanal, semestral ou mensal. Selecione o dia da semana em que você deseja que a folha de horas seja produzida.</p>
      <p>Uma planilha de horas semanal começa na data em que é gerada. Por exemplo, se você criar folhas de horas semanais todas as quintas-feiras, o primeiro dia da semana na folha de horas será quinta-feira.</p>


   <p><b>NOTA</b>: o Workfront sempre cria duas folhas de horas por vez: a primeira folha de horas sempre inclui a data atual e a segunda folha de horas começa quando o período da primeira termina.</p> </p> </td> 
    </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Aprovadores</strong></p> </td> 
      <td> <p> <p>Os aprovadores são usuários que aprovam a folha de horas para os usuários associados à folha de horas. Você pode identificar até 7 usuários como aprovadores em uma folha de horas. Identificar vários usuários é útil para garantir que um aprovador esteja disponível quando alguém estiver fora do escritório. Todos os aprovadores são notificados quando um usuário envia a folha de horas para aprovação. Somente um usuário precisa aprovar a folha de horas para que ela seja aprovada.</p> <p>Somente usuários com direitos administrativos de planilha de horas podem ser definidos como aprovadores. Para obter mais informações sobre direitos administrativos de planilha de horas, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p>Use o menu suspenso para selecionar o aprovador para a folha de horas (se um aprovador for necessário). Você pode selecionar entre as seguintes opções:</p> 
      <ul> 
      <li><strong>Nenhum</strong>: A folha de horas não precisa ser aprovada.</li> 
      <li><strong>O gerente deles</strong>: este é o aprovador padrão, definido pelo sistema. Nesse caso, o usuário designado como gerente aprova a folha de horas quando ela é enviada para aprovação.</li> 
      <li><strong>Pessoas específicas:</strong> Você pode designar usuários específicos, por nome, como aprovadores de folha de horas. Você pode ter múltiplos aprovadores em uma planilha de horas. Nesse caso, depois que um dos aprovadores aprovar a folha de horas, ela será marcada como <strong>Fechado</strong> e desaparecerá da lista de aprovações da folha de horas de todos os aprovadores restantes.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Pode editar as horas </strong> </td> 
      <td> <p> <p>Selecione esta opção para permitir que os aprovadores editem horas na folha de horas.

   Essa opção funciona junto com o **Restringir a edição da folha de horas aos proprietários e administradores** na área Configuração > Horas > Preferências. Para obter mais informações, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurar preferências de horas e planilha de horas</a>.

   Existem os seguintes cenários:

   <ul>
      <li>Quando a variável <b>Restringir a edição da folha de horas aos proprietários e administradores</b> está ativada:</li>
      <ul><li>Os aprovadores só podem aprovar e rejeitar a folha de horas, independentemente da <b>Pode editar as horas</b> está ativado ou não. </li>
      <li>Os gerentes dos proprietários da folha de horas só podem exibir as folhas de horas de seus subordinados diretos.</li></ul>
      <li>Quando a variável <b>Restringir a edição da folha de horas aos proprietários e administradores</b> A opção está desabilitada:</li>
    <ul><li>Quando a variável <b>Pode editar as horas</b> estiver ativado, os aprovadores podem enviar, reabrir ou fechar a folha de horas e editar as horas.</li>
      <li>Quando a variável <b>Pode editar as horas</b> estiver desativado, os aprovadores não poderão enviar, reabrir ou fechar a folha de horas e não poderão editar as horas. Os aprovadores só podem aprovar ou rejeitar a folha de horas. </li>
      <li>Os gerentes dos proprietários da folha de horas podem enviar, retroceder, reabrir e editar as folhas de horas de seus subordinados diretos.</li></ul>
      </ul>

   <p>

   <b>NOTA</b>: depois de enviar uma folha de horas para aprovação, você não poderá mais editar as horas. Para retornar uma folha de horas enviada a um estado editável, cancele a folha de horas ou peça ao aprovador para rejeitar a folha de horas. Para obter mais informações, consulte <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Enviar uma planilha de horas para aprovação</a> e<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Aprovar uma planilha de horas</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipos de Hora Disponíveis</strong> </td> 
      <td><p>Essa configuração se refere somente aos Tipos de horas gerais, e não aos tipos de horas específicos do projeto. </p>
      <p>Por padrão, os usuários veem todas as horas gerais em uma folha de horas. No entanto, se sua organização quiser que apenas as horas gerais específicas sejam mostradas para um conjunto específico de usuários, você pode selecionar as horas gerais que eles precisam ver em suas folhas de horas, selecionando-os no perfil de folha de horas neste campo. Se quiser desativar todas as horas gerais, desmarque todos os tipos de horas para gerar a folha de horas sem uma seção para as horas gerais.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Hora extra</span> </td> 
      <td>Você pode optar por ocultar a caixa Horas extras em folhas de horas. Essa opção está desabilitada por padrão.</td> 
     </tr> 
    </tbody> 
    </table>

1. Clique em **Atribuir pessoas** para associar o perfil da folha de horas a usuários, grupos ou equipes específicos (se você for um administrador do Workfront). Comece a digitar o nome do usuário, grupo ou equipe e clique nele quando ele aparecer na lista suspensa.

   Se você for um administrador de grupo, poderá atribuir o perfil da folha de horas aos grupos que administra, mas não às equipes. Para obter mais informações, consulte [Limitações para um administrador de grupo que atribui um perfil de folha de horas](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) neste artigo.

   >[!NOTE]
   >
   >* Você também pode associar um usuário a um perfil de planilha de horas editando o perfil do usuário. Para obter mais informações, consulte [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Quando você adiciona um grupo, somente o nome do grupo é exibido na guia Atribuir Pessoas, não a lista de membros do grupo. Se quiser ver os membros do grupo listados aqui, clique em Salvar Alterações, em seguida, clique no nome do perfil da planilha de horas que você acabou de criar.
   >* Ao concluir essas etapas, o perfil de folha de horas gera folhas de horas apenas para os usuários atribuídos ou membros do grupo que não têm folhas de horas existentes para o período atual.

1. Clique em **Salvar alterações**.

   Na primeira vez que o perfil de folha de horas gera folhas de horas, duas folhas de horas são criadas para cada usuário. Depois disso, cada vez que gera novas folhas de horas, uma folha de horas é criada por usuário.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Limitações para um administrador de grupo que atribui um perfil de folha de horas {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Se você for um administrador de grupo e a opção de acesso administrativo Folhas de horas e horas estiver desativada no seu nível de acesso, será possível criar perfis de folha de horas, mas você poderá atribuí-los apenas a:

* Grupos que você administra
* Usuários individuais que você tem acesso para editar e que estão em um grupo que você administra

Para esses grupos e usuários, você não terá acesso às folhas de horas geradas pelo perfil da folha de horas.

Além disso, se a opção Administrador de usuários (usuários de grupo) também estiver desativada no seu nível de acesso, você poderá atribuir o perfil de planilha de horas a um grupo que administra, mas isso afetará somente os usuários no grupo que você tem acesso para editar. Se o grupo contiver usuários aos quais você não tem acesso para editar, eles não receberão o perfil da folha de horas junto com o restante do grupo.

Para obter informações sobre a opção Folhas de horas e horas no seu nível de acesso, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obter informações sobre a opção Administrador de usuário (usuários de grupo) no seu nível de acesso, consulte [Conceder acesso aos usuários](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Vários perfis de planilha de horas recorrentes

Você pode ter mais de uma planilha de horas para sua organização se houver:

* Períodos de pagamento exclusivos para diferentes conjuntos de usuários
* Aprovadores únicos para diferentes conjuntos de usuários
* Requisitos exclusivos de horas gerais para diferentes conjuntos de usuários

Um usuário não pode ser associado a mais de um perfil de planilha de horas por vez. 
