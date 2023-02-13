---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Criar uma folha de ponto de uso único
description: Você pode criar manualmente uma folha de ponto de uso único se quiser uma folha de ponto que não seja recorrente. Quando a data de término da folha de ponto for atingida e você precisar de mais folhas de ponto, é necessário criar novas.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 1%

---

# Criar uma folha de ponto de uso único

Você pode criar manualmente uma folha de ponto de uso único se quiser uma folha de ponto que não seja recorrente. Quando a data de término da folha de ponto for atingida e você precisar de mais folhas de ponto, é necessário criar novas.

Para obter informações sobre como criar um perfil de folha de ponto que gera folhas de ponto recorrentes para seus usuários sem nenhuma intervenção adicional de você (recomendado), consulte [Criar, editar e atribuir perfis de folha de ponto](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* As folhas de horas de uso único não podem ser criadas para grupos.

>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Ao criar uma folha de ponto de uso único, você não pode selecionar tipos específicos de hora geral para incluir na folha de horas. Todos os tipos de horas gerais ativados no sistema são exibidos nas folhas de horas criadas manualmente.
>
>  Se quiser selecionar apenas determinados tipos de hora gerais a serem exibidos em suas folhas de horas, use um perfil de folha de horas. Para obter mais informações sobre perfis de folha de ponto, consulte [Criar, editar e atribuir perfis de folha de ponto](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

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
   <td> <p>Você deve ter acesso administrativo às Folhas de Horas. </p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p><b> Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar uma folha de ponto de uso único

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Folhas de Horas**. O **Todos** filtro é selecionado por padrão. Isso exibe todas as folhas de horas que você tem acesso para visualizar.

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
   >   * [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)



1. (Opcional) Clique no botão **Pesquisar** ícone ![](assets/search-icon.png) para digitar uma palavra-chave e procurar uma folha de ponto específica. Por exemplo, você pode procurar por um período de folha de ponto do nome do proprietário.

1. (Opcional) Clique no botão **Exibir** ![](assets/view-icon.png) ou **Agrupamento** ![](assets/grouping.png) para aplicar uma exibição ou agrupamento diferente ou para criar um novo.

   Para obter informações sobre a criação de filtros, exibições ou agrupamentos, consulte os seguintes artigos:

   * [Criar ou editar filtros no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Criar ou editar exibições no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Criar agrupamentos no Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Clique em **Nova Folha de Horas** na parte superior da lista de folhas de horas.

   Especifique as seguintes informações:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Criar planilha de horas para</strong> </td> 
      <td>Comece a inserir o nome do usuário, uma função de trabalho ou uma equipe para a qual você está criando a folha de ponto e clique neles quando eles forem exibidos na lista.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Data de início</strong> </td> 
      <td>Esta é a data de início da folha de ponto.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Data Final</strong> </td> 
      <td> Esta é a data final da folha de ponto.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Aprovadores</strong> </td> 
      <td>Aprovadores são usuários que aprovam a folha de ponto para os usuários associados à folha de ponto. Somente usuários com direitos administrativos de folha de ponto podem ser definidos como aprovadores. Para obter mais informações sobre os direitos administrativos da folha de ponto, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.<br>Comece a inserir os nomes dos aprovadores da folha de ponto e clique neles quando eles forem exibidos na lista.<br>Você pode ter vários aprovadores em uma folha de ponto. Nesse caso, depois que um dos aprovadores aprovar a folha de ponto, a folha de ponto é marcada como <strong>Fechado</strong> e desaparece da lista de aprovações da folha de ponto de todos os aprovadores restantes.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Pode editar as horas</strong> </td>

   <td> <p>Selecione essa opção se desejar permitir que aprovadores editem horas na folha de ponto.</p>

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

   Depois de enviar uma folha de horas para aprovação, você não pode mais editar as horas. Para retornar uma folha de ponto enviada a um estado editável, recupere a folha de ponto ou peça para o aprovador rejeitar a folha de ponto. Para obter mais informações, consulte <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Enviar uma folha de ponto para aprovação</a> e <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Aprovar uma folha de ponto</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Hora extra</span> </td> 
      <td>Você pode optar por ocultar a caixa Hora extra na folha de ponto. Essa opção é desativada por padrão.</td> 
      </tr> 
      </tbody> 
   </table>

1. Clique em **Criar folha de ponto**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Quando tarefas e problemas aparecem nas folhas de ponto dos usuários

Uma tarefa ou problema atribuído a um usuário é exibido automaticamente na folha de ponto de um usuário se a tarefa ou problema atender a qualquer um dos seguintes critérios:

* O usuário registrou horas na tarefa ou no problema
* As datas planejadas da tarefa ou emissão estão dentro das datas da folha de ponto
* A tarefa ou o problema tem uma Data Inicial Real (O status da tarefa ou do problema está Em Andamento)
* A tarefa ou o problema é fixado à folha de ponto
* A Data de Conclusão Planejada fica dentro do intervalo de datas da folha de ponto e o status é Em Andamento

Se a variável **Preencha previamente as folhas de ponto com ...** as preferências (localizadas nas preferências de Folhas de data e hora) estiverem desmarcadas, a folha de horas mostrará problemas e tarefas que têm um status Em andamento. Para obter mais informações sobre as Folhas de Horas e Preferências de Hora, consulte [Configurar preferências de hora e folha de ponto](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
