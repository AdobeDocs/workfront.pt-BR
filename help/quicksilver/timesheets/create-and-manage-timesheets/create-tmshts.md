---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Criar uma planilha de horas de uso único
description: Você pode criar manualmente uma folha de horas de uso único se quiser uma folha de horas que não seja recorrente. Quando a data de término da folha de horas é atingida e você precisa de mais folhas de horas, você deve criar novas.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---

# Criar uma planilha de horas de uso único

Você pode criar manualmente uma folha de horas de uso único se quiser uma folha de horas que não seja recorrente. Quando a data de término da folha de horas é atingida e você precisa de mais folhas de horas, você deve criar novas.

Para obter informações sobre como criar um perfil de folha de horas que gere folhas de horas recorrentes para seus usuários sem nenhuma intervenção adicional (recomendado), consulte [Criar, editar e atribuir perfis de folha de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* Planilha de horas de uso único não pode ser criada para grupos.
>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Ao criar uma folha de horas de uso único, você não pode selecionar tipos de horas gerais específicos para incluir em sua folha de horas. Todos os tipos de horas gerais ativados no seu sistema são exibidos em folhas de horas criadas manualmente.
>
>  Se você quiser selecionar apenas determinados tipos de horas gerais para exibir em suas folhas de horas, use um perfil de folha de horas. Para obter mais informações sobre perfis de folha de horas, consulte [Criar, editar e atribuir perfis de folha de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
>

## Requisitos de acesso

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
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ter acesso administrativo a Planilhas de Horas. </p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p><b> Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Criar uma planilha de horas de uso único

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal**, no canto superior direito do Adobe Workfront.

1. Clique em **Folhas de horas**. O filtro **Todos** é selecionado por padrão. Isso exibe todas as planilhas de horas que você tem acesso para visualizar.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Siga um destes procedimentos para atualizar o filtro na lista de folhas de horas:

   * Selecione **Minhas planilhas de horas aprovadas** no canto superior direito da página para exibir somente as planilhas de horas aprovadas por você

     Ou

     Selecione **Minhas Planilhas de Horas** para exibir apenas suas planilhas de horas.

     Isso aplica os filtros Minhas planilhas de horas ou Minha planilha de horas à lista de planilhas de horas.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Clique no ícone Filtro ![](assets/filter-nwepng.png) para aplicar um filtro diferente ou criar um novo. Para obter informações sobre como criar ou atualizar filtros, consulte [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >As opções Minhas aprovações de folha de horas e Minhas folhas de horas não são exibidas na parte superior da lista de folha de horas ou na lista de filtros se o administrador do Workfront ou um administrador de grupo removeu os filtros Minhas aprovações de folha de horas e Minhas folhas de horas dos Controles de lista na área Configuração ou do Modelo de layout. Para obter mais informações, consulte os seguintes artigos:
   > 
   >   * [Personalizar Filtros, Modos de Exibição e Agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Opcional) Clique no ícone ![](assets/search-icon.png) da **Pesquisa** para digitar uma palavra-chave e procurar uma folha de horas específica. Por exemplo, você pode procurar um intervalo de tempo de planilha de horas do nome do proprietário.

1. (Opcional) Clique nos ícones **Visualização** ![](assets/view-icon.png) ou **Agrupamento** ![](assets/grouping.png) para aplicar uma visualização ou agrupamento diferente ou para criar um novo.

   Para obter informações sobre como criar filtros, visualizações ou agrupamentos, consulte os seguintes artigos:

   * [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Criar ou editar exibições no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Criar agrupamentos no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Clique em **Nova Planilha de Horas** na parte superior da lista de planilhas de horas.

   Especifique as seguintes informações:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Criar planilha de horas para</strong> </td> 
      <td>Comece a inserir o nome do usuário, uma função de trabalho ou uma equipe para a qual você está criando a folha de horas e clique neles quando eles forem exibidos na lista.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Data de Início</strong> </td> 
      <td>Esta é a data de início da folha de horas.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Data de término</strong> </td> 
      <td> Esta é a data de término da folha de horas.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Aprovadores</strong> </td> 
      <td>Os aprovadores são usuários que aprovam a folha de horas para os usuários associados à folha de horas. Somente usuários com direitos administrativos de planilha de horas podem ser definidos como aprovadores. Para obter mais informações sobre direitos administrativos de planilha de horas, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.<br>Comece a inserir os nomes dos aprovadores de planilhas de horas e clique neles quando eles aparecerem na lista.<br>Você pode ter vários aprovadores em uma planilha de horas. Nesse caso, depois que um dos aprovadores aprovar a folha de horas, ela será marcada como <strong>Fechada</strong> e desaparecerá da lista de aprovações da folha de horas de todos os aprovadores restantes.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Pode editar as horas</strong> </td>

   <td> <p>Selecione esta opção se quiser permitir que os aprovadores editem horas na folha de horas.</p>

   Esta opção funciona junto com a configuração **Restringir edição da folha de horas a proprietários e administradores** na área Configuração > Folhas de horas e horas > Preferências. Para obter mais informações, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurar preferências de horas e folha de horas</a>.

   Existem os seguintes cenários:

   <ul>
      <li>Quando a opção <b>Restringir edição da folha de horas a proprietários e administradores</b> está habilitada:</li>
   <ul><li>Os aprovadores só podem aprovar e rejeitar a folha de horas, independentemente de o <b>Pode editar as horas</b> estar habilitado ou não. </li>
   <li>Os gerentes dos proprietários da folha de horas só podem exibir as folhas de horas de seus subordinados diretos.</li></ul>
   <li>Quando a opção <b>Restringir edição da folha de horas a proprietários e administradores</b> está desabilitada:</li>
   <ul><li>Quando a <b>Pode editar as horas</b> estiver habilitada, os aprovadores poderão enviar, reabrir ou fechar a folha de horas e editar as horas.</li>
   <li>Quando a <b>Pode editar as horas</b> está desabilitada, os aprovadores não podem enviar, reabrir ou fechar a folha de horas e não podem editar as horas. Os aprovadores só podem aprovar ou rejeitar a folha de horas. </li>
   <li>Os gerentes dos proprietários da folha de horas podem enviar, retroceder, reabrir e editar as folhas de horas de seus subordinados diretos.</li></ul>
   </ul>

   <p><b>Nota</b>

   Depois que você enviar uma folha de horas para aprovação, não poderá mais editar as horas. Para retornar uma folha de horas enviada a um estado editável, cancele a folha de horas ou peça ao aprovador para rejeitar a folha de horas. Para obter mais informações, consulte <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Enviar uma folha de horas para aprovação</a> e <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Aprovar uma folha de horas</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Hora extra</span> </td> 
      <td>Você pode optar por ocultar a caixa Horas extras na folha de horas. Essa opção está desabilitada por padrão.</td> 
      </tr> 
      </tbody> 
   </table>

1. Clique em **Criar planilha de horas**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Quando tarefas e problemas aparecem na planilha de horas dos usuários

Uma tarefa ou problema atribuído a um usuário aparece automaticamente na folha de horas de um usuário se a tarefa ou problema atender a qualquer um dos seguintes critérios:

* O usuário registrou horas na tarefa ou problema
* As datas planejadas da tarefa ou problema estão dentro das datas da folha de horas
* A tarefa ou problema tem uma Data de Início Real (o status da tarefa ou problema é Em Andamento)
* A tarefa ou problema está fixado à folha de horas
* A data de conclusão planejada está no intervalo de datas da folha de horas e o status é Em andamento

Se as **Preencher folhas de horas previamente com ...** preferências (localizadas nas preferências de Horas e Folhas de horas) estiverem desmarcadas, a folha de horas mostrará problemas e tarefas com o status Em andamento. Para obter mais informações sobre as Preferências de Horas e Planilha de Horas, consulte [Configurar preferências de horas e planilha de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
