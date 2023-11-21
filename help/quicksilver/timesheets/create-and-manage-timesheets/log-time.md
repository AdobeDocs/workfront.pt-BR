---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Registrar de tempo
description: Você pode registrar horas para itens de trabalho no &Adobe Workfront para indicar o número de horas que você gasta trabalhando neles. Você também pode registrar horas que não estejam relacionadas ao trabalho, como férias, licença médica ou tempo gasto em reuniões. O horário registrado é exibido em sua folha de horas.
author: Alina
feature: Timesheets
role: User
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: edd4aa9556b624de3634af26d6d9efd59f5d2e44
workflow-type: tm+mt
source-wordcount: '3491'
ht-degree: 0%

---

# Registrar de tempo

<!--remove all preview and production references from this article with 23.3 release-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). 

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 
-->

Você pode registrar o tempo para itens de trabalho no Adobe Workfront para indicar o número de horas que você gasta trabalhando neles. Você também pode registrar horas que não estejam relacionadas ao trabalho, como férias, licença médica ou tempo gasto em reuniões. O horário registrado é exibido em sua folha de horas.

Para obter mais informações sobre o tipo de horas em que você pode fazer logon no Workfront, consulte [Gerenciar tipos de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Requisitos de acesso

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p>
   <p>Legacy license: 
   <ul><li>Review or higher to log General Hours in a timesheet</li>
   <li>Work or higher to log hours on a project, task, or issue</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the type of work item you log time for </p> <p>For example, you need Edit access to Issues, to log time for issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions on the work item you log time for that includes permissions to Log Hours</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas deste artigo e registrar as horas específicas do projeto:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <ul><li>Revise ou registre horas gerais em uma planilha de horas</li>
   <li> Trabalhar ou mais para registrar horas em um projeto, tarefa ou problema</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar o acesso ao tipo de item de trabalho para o qual você registra horas </p> <p>Por exemplo, você precisa ter acesso de Edição a Problemas para registrar o tempo de ocorrências</p> <p>Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribute ou tenha permissões mais altas no item de trabalho para o qual você registra horas, que incluem permissões para Registrar horas.</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Considerações ao registrar tempo no Workfront

* Você pode registrar horas para projetos, tarefas ou problemas, ou pode registrar horas diretamente em sua folha de horas.

  Para obter informações sobre como criar planilhas de horas, consulte [Criar uma planilha de horas de uso único](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* Todo o tempo registrado em ferramentas diferentes da folha de horas aparece na folha de horas para o período correspondente.
* Tarefas e problemas em um projeto que não é atual não são pré-preenchidos em uma folha de horas.
* As horas registradas na folha de horas são aplicadas imediatamente à tarefa, problema ou projeto.
* As planilhas de horas incluem o tempo total para todas as datas registradas. Os finais de semana são sempre incluídos, mesmo quando os cálculos de linha do tempo foram configurados para excluí-los (conforme descrito em [Configurar preferências de projeto em todo o sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)).
* O número máximo de itens exibidos em uma folha de horas é 45. Se houver mais de 45 itens cujas datas correspondam ao período da folha de horas, apenas os itens atualizados mais recentemente serão exibidos.
* As entradas de horas incluídas nos registros de cobrança são esmaecidas e não podem ser editadas na folha de horas. Para obter mais informações, consulte [Criar registros de cobrança](../../manage-work/projects/project-finances/create-billing-records.md).
* Por padrão, as tarefas pessoais não são exibidas na folha de horas. As tarefas pessoais são exibidas na folha de horas somente quando têm tempo registrado. Depois de registrar as horas em uma tarefa pessoal, você pode fixar a tarefa na folha de horas e ela permanecerá na folha de horas se permanecer fixada. Para obter mais informações, consulte [Criar itens de trabalho a partir da Área da página inicial](../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Registrar de tempo

Você pode registrar horas nas seguintes áreas no Workfront:

* [Planilha de horas](#timesheet)
* [Página inicial](#home)
* [Projeto, tarefa ou problema](#project-task-or-issue)
* [Painel Resumo](#summary-panel)
* [Quadros](#boards)
* [Aplicativo móvel](#mobile-app)

### Planilha de horas {#timesheet}

#### Registrar horas em uma folha de horas {#log-time-on-a-timesheet}

Você pode registrar horas nos seguintes itens da folha de horas:

* Tarefas, problemas e projetos pré-preenchidos são exibidos automaticamente com base em como o administrador do Workfront define as preferências da folha de horas. Para obter informações sobre como as folhas de horas são pré-preenchidas, consulte [Configurar preferências de horas e planilha de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  Somente as tarefas e problemas atribuídos a você são preenchidas previamente em sua planilha de horas. Tarefas e problemas atribuídos às suas equipes ou funções de trabalho não preenchem sua folha de horas automaticamente.

  Clicar em Trabalhar nisso em um item atribuído às suas equipes atribui o item a você e o item será exibido em sua folha de horas.

* Tarefas, problemas ou projetos adicionados manualmente.
* Tarefas, problemas ou projetos para os quais você já fez logon em outro lugar na Workfront.
* Tempo geral (férias, treinamento, horas extras).

>[!NOTE]
>
>Revise os usuários atribuídos a um Perfil de folha de horas. Você pode ver a área Folhas de horas e registrar as horas gerais. No entanto, eles não podem registrar horas em nenhuma tarefa ou problema atribuído a eles que apareçam na folha de horas.

Para registrar horas em uma folha de horas:

1. Clique em [!UICONTROL **Menu principal**] ícone ![](assets/main-menu-icon.png) no canto superior direito, ou na guia **Menu principal** ícone ![](assets/lines-main-menu.png) no canto superior esquerdo do Workfront, se disponível.

1. Clique em [!UICONTROL **Planilhas de Horas**]. Sua Planilha de Horas atual é exibida por padrão.
   ![Planilha de horas](assets/timesheet-redesigned-nwe.png)


1. (Opcional) Clique no link **tela cheia** ícone ![](assets/full-screen.png) para exibir a folha de horas no modo de tela cheia, clique no link **exit-full-screen** ![](assets/exit-full-screen.png) ícone para retornar à folha de horas.

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (Opcional) Para adicionar um projeto, tarefa ou problema à folha de horas, clique no link **Adicionar item** no canto superior esquerdo da folha de horas e, em seguida, clique em **Adicionar Projetos**, **Adicionar tarefas** ou **Adicionar Problemas**.

   Uma lista de projetos, tarefas ou problemas é exibida.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (Opcional) Clique no ícone de pesquisa ![Pesquisar um item](assets/search-icon.png) para procurar um item específico usando uma palavra-chave para adicionar à folha de horas.

1. (Opcional) Expanda os menus suspensos filtro, exibição ou agrupamento para aplicar ou personalizar um e exibir as informações de item desejadas.

1. Selecione um ou vários itens na lista e clique em **Adicionar**.

   >[!NOTE]
   >
   >Quando você adiciona tarefas ou problemas à folha de horas, o projeto também é adicionado.


1. (Condicional) Se você adicionar 50 ou mais itens de uma vez, uma mensagem de confirmação exibindo o número de itens adicionados à sua folha de horas será exibida.

   Clique em **Adicionar tudo** para adicionar todos os itens ou clique em **Cancelar** para interromper a adição dos itens selecionados, **Cancelar** para fechar a lista de itens.

   Tarefas e problemas são listados sob o nome do projeto.

   >[!NOTE]
   >
   >Os itens adicionados manualmente à folha de horas são fixados e permanecerão na folha de horas atual e futura até que você os desafixe manualmente para removê-los. Para obter informações sobre como desafixar itens para removê-los da folha de horas, continue com a Etapa 10.

   <!--(ensure this stays accurate)-->

1. (Opcional) Clique no link **Recolher** ![](assets/collapse-icon.png) ou **Expandir** ![](assets/expand-icon.png) ícones ao lado do nome do projeto para exibir ou ocultar a lista de tarefas e problemas do projeto.


   >[!TIP]
   >
   >   Ao usar um teclado QWERTY padrão e depois de clicar no nome de um projeto na folha de horas, pressione o seguinte conjunto de teclas para recolher ou expandir o projeto:
   >   * Para expandir o projeto e exibir seus itens de trabalho:
   >     * Shift + Alt + seta para cima para computadores com Windows
   >     * Shift + Option + seta para cima para computadores Mac
   >   * Para recolher o projeto e ocultar seus itens de trabalho:
   >     * Shift + Alt + seta para baixo para computadores com Windows
   >     * Shift + Option + seta para baixo para computadores Mac.


1. (Opcional) Para fixar manualmente um item que é exibido automaticamente na folha de horas, passe o mouse sobre o nome do item e clique no link **fixar** ícone ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   Ao usar um teclado QWERTY padrão depois de clicar em um item na folha de horas, pressione o seguinte conjunto de teclas para fixar um item:
   >   * Option + P para computadores com Windows e Mac.


1. (Opcional) Clique no ícone de pesquisa ![](assets/search-icon.png) e comece a digitar uma palavra-chave para localizar um projeto, tarefa ou um problema na folha de horas.

1. (Condicional) Se o administrador do Workfront ou do grupo tiver ativado o **Atribuir funções de trabalho a entradas de horas manualmente** selecione uma função de trabalho no menu suspenso. A função especificada quando você está atribuído ao item de trabalho é exibida por padrão. Se uma função não for atribuída a você no objeto, sua função principal será exibida como padrão. Para obter mais informações sobre essa configuração, consulte o artigo [Configurar preferências de horas e planilha de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![Registrar horas de várias funções na folha de horas](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. (Opcional) Clique no link **+** para adicionar outra linha, selecione um novo tipo de hora no menu suspenso na [!UICONTROL Tipo de Hora] coluna para registrar horas para um tipo de hora diferente.

   ![Menu suspenso de tipo de hora](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Dependendo do seu sistema operacional ou navegador e ao usar um teclado QWERTY padrão, pressione o seguinte conjunto de teclas para adicionar outra linha:
   >   * Ctrl + Option + + para computadores com Windows
   >   * Cmd + Option + + para computadores Mac

   Os tipos de horas estão disponíveis dependendo do que foi definido nos níveis de sistema, projeto e usuário, conforme descrito em [Definir tipos de horas e disponibilidade para folhas de horas](define-hour-types-and-availability.md).

   O tipo de hora não pode ser alterado depois que uma folha de horas é fechada.

   >[!TIP]
   >
   >Se você tiver registrado o tempo anteriormente e o tipo de hora selecionado estiver desativado, a linha inteira para o tempo registrado ficará esmaecida. Selecionar outro tipo de hora e atualizar a página remove a opção de tipo de hora desativado da lista suspensa para que você não possa adicionar horas extras a esse tipo de hora.
   >
   >Considere adicionar uma nova linha para o item de trabalho para o qual você deseja registrar mais tempo e selecione um novo tipo de hora se desejar manter o tipo de hora desativado associado ao tempo registrado passado.

1. Clique em **excluir** ícone  ![](assets/delete.png) ao lado da função de trabalho para removê-la. As horas registradas para a função também são removidas.

   >[!TIP]
   >
   >   Dependendo do seu sistema operacional ou navegador e ao usar um teclado QWERTY padrão, pressione o seguinte conjunto de teclas para excluir uma linha:
   >   * Ctrl + Option + - para computadores Windows
   >   * Cmd + Option + - para computadores Mac


1. Especifique por quanto tempo você deseja fazer logon em um determinado dia na seção linha do tempo da folha de horas e, em seguida, clique fora da caixa horas para salvar a entrada de horas. As horas são salvas automaticamente. A linha para a qual você registra horas é destacada em azul claro e a caixa de entrada de horas é contornada em azul escuro.

   ![Registrar caixa de horas na folha de horas](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   Você registra horas em horas ou dias. Essa configuração é definida por usuários com uma licença de Plano ou pelo administrador do sistema, conforme descrito em [Configurar se a hora está conectada em horas ou dias](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >Você deve salvar a folha de horas manualmente se qualquer um dos seguintes cenários ocorrer:
   >
   >* A função de trabalho associada a tempo que você registrou anteriormente foi alterada e o **Atribuir funções de trabalho a entradas de horas manualmente** foi desabilitada. O registro de tempo para novas datas associará esse tempo a uma função de trabalho diferente.
   >   
   >   Se a função tiver sido alterada e a variável **Atribuir funções de trabalho a entradas de horas manualmente** estiver ativada, você poderá registrar horas ou atualizar a função e suas alterações serão salvas automaticamente.
   >
   >* A função de trabalho atribuída a uma tarefa ou problema é diferente da função de trabalho com a qual o proprietário da folha de horas está registrando horas <!--or assigned to them_ this last  piece came from a Support note but but sure what role it's referring to. Leaving it out for now.-->.
   >
   >A folha de horas salvará novamente o tempo automaticamente quando não houver mais entradas conflitantes entre as duas funções.
   >

1. (Opcional) Especifique a quantidade de horas extras no campo Horas extras no cabeçalho da folha de horas.

   >[!TIP]
   >
   >Você não pode registrar um número de horas extras maior que o total de horas atual na folha de horas. Por exemplo, se você registrou 7 horas na folha de horas até agora, não é possível registrar 8 horas extras.

1. (Opcional) Clique em **Comentário** para adicionar um comentário à sua entrada de hora.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Ao usar um teclado QWERTY padrão depois de clicar na caixa de entrada de hora, pressione o seguinte conjunto de teclas para abrir a caixa de comentário:
   >   * Shift + F2 para computadores Windows e Mac.

1. Clique em **Concluído** para salvar o comentário.

   >[!TIP]
   >
   >   Ao usar um teclado QWERTY padrão, de dentro da caixa de comentário, pressione o seguinte conjunto de teclas para salvar o comentário:
   >   * Ctrl + Enter para computadores Windows.
   >   * Cmd + Return para computadores Mac.


1. (Opcional) Clique em **Mostrar comentários** na barra de ferramentas para exibir comentários de entrada de horas sob o item de trabalho.

   ![Comentários listados no item na folha de horas](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Todas as alterações feitas na folha de horas são salvas automaticamente.

1. (Opcional) Clique na linha de uma tarefa ou problema e clique em **Abrir resumo** no canto superior direito da folha de horas para adicionar uma atualização ou atualizar informações sobre a tarefa ou problema. O painel Resumo é aberto à direita.

   ![resumo-painel-para-tarefa-aberto-na-folha de horas](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   A atualização é exibida na área Atualizações do item de trabalho associado ao tempo registrado.

   >[!TIP]
   >
   >Não é possível comentar em projetos ou entradas de horas em Tempo geral.

1. Clique em [!UICONTROL **Fechar resumo**] para fechar o painel Resumo e retornar à folha de horas.

1. (Opcional) Clique em [!UICONTROL **Atualizações**] no painel esquerdo, adicione uma atualização à folha de horas. Para obter mais informações sobre atualizações do Workfront, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-reDesigned-timesheet-left-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

   * **Fechar**: feche a folha de horas quando terminar de atualizá-la. Essa opção só está disponível quando sua folha de horas não está associada a um aprovador.

   * **Enviar para aprovação:** Esta opção está disponível somente se houver um aprovador na planilha de horas. Salve as alterações e envie para aprovação. Você pode abrir a folha de horas depois de fechá-la clicando em **Retroceder**, se uma aprovação ainda não tiver sido concedida. Para obter mais informações, consulte [Enviar uma planilha de horas para aprovação](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **Rejeitar**: esta opção é exibida quando você é um aprovador de folha de horas e a folha de horas foi enviada a você para aprovação. Clicar nela altera o status da folha de horas para Rejeitada e a folha de horas permanece aberta.

   * **Aprovar**: esta opção é exibida quando você é um aprovador de folha de horas e a folha de horas foi enviada a você para aprovação. Clicar nela altera o status da folha de horas para Aprovado e fecha a folha de horas.

   >[!TIP]
   >
   >As opções Rejeitar e Aprovar também são exibidas em sua folha de horas quando você é um administrador do sistema e a folha de horas é associada a um aprovador.

1. (Condicional) Se tiver fechado ou enviado sua planilha de horas para aprovação, clique em uma das seguintes opções:

   * **Reabrir**: esta opção está disponível para folhas de horas que você já fechou e que não têm aprovadores ou folhas de horas que já foram aprovadas. Reabra a folha de horas para modificar entradas de horas.
   * **Retroceder**: essa opção está disponível para folhas de horas que foram enviadas para aprovação, mas ainda não foram aprovadas ou rejeitadas. Clique em **Retroceder** para reabrir a folha de horas e modificar as entradas de horas.

#### Remover um item da folha de horas

Você pode remover uma entrada de horas ou um item (projeto, tarefa ou problema) de uma planilha de horas.

Para remover uma entrada de horas de uma folha de horas:

1. Vá para a folha de horas e localize a entrada de horas que deseja remover.
1. Substitua as horas inseridas por 0 ou Remova as horas e substitua-as por 0 e pressione Enter.

   As horas são removidas e a folha de horas é salva automaticamente.

Você pode remover um item (projeto, tarefa ou problema) da folha de horas desfixando-o, se ainda não tiver registrado tempo para ele e se tiver adicionado manualmente o item (conforme descrito nas Etapas 4 a 8 no [Registrar horas em uma folha de horas](#log-time-on-a-timesheet) neste artigo). <!--ensure this stays accurate-->

Não é possível remover automaticamente os itens incluídos na folha de horas de acordo com as preferências da folha de horas no sistema ou grupo do Workfront que estão configuradas para preencher previamente as folhas de horas (conforme descrito em [Configurar preferências de horas e planilha de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)). Os itens param de preencher previamente a folha de horas quando as datas dos itens estão fora do período da folha de horas.

Para remover um item da folha de horas que foi adicionado manualmente:

1. Certifique-se de que nenhuma hora seja registrada em relação ao item.
1. Clique em **desafixar** ícone ![Fixar um item](assets/pin-icon.png) ao lado do item para desafixar o item da folha de horas.

   >[!TIP]
   >
   >   Ao usar um teclado QWERTY padrão depois de clicar em um item na folha de horas, pressione o seguinte conjunto de teclas para desafixar um item:
   > * Option + P para computadores com Windows e Mac.

   O item é removido da folha de horas após você atualizar a página.

### Página inicial {#home}

Você pode registrar horas específicas do projeto na Página inicial.

Para obter informações gerais sobre o uso da área Início, consulte as seguintes seções:

* Para obter informações sobre como usar a área inicial herdada, consulte [Usar a área Início](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).
* Para obter informações sobre como usar a nova área Página inicial, consulte [Introdução à nova página inicial no Adobe Workfront](../../workfront-basics/using-home/new-home/get-started-with-new-home.md).

#### Registrar horas em um item de trabalho na nova área Página inicial

1. Chegou ao **Início** área.
1. Adicione qualquer um dos seguintes widgets:

   * Minhas tarefas
   * Meus problemas
   * Meu trabalho
   * Minhas solicitações
1. Selecione uma tarefa, problema ou solicitação em uma lista e clique em **Resumo**

   Ou

   Clique em **Resumo** ícone ![](assets/open-summary-icon-in-home.png) de uma tarefa ou um problema no widget Meu trabalho.

   O painel Resumo é aberto à direita.

   ![](assets/log-time-new-home-my-work-widget.png)
1. Continue a registrar o tempo no painel Resumo, conforme descrito em [Visão geral do resumo](../../workfront-basics/the-new-workfront-experience/summary-overview.md).


#### Registrar o tempo em um item de trabalho na área inicial herdada

1. No **Lista de trabalho** selecione o item onde deseja registrar o tempo.
1. No painel direito, clique em **Registro de tempo**.

   ![](assets/log-time-home-350x181.png)

1. No **Digite horas** selecione o tipo de hora apropriado.\
   Os tipos de horas estão disponíveis dependendo do que foi definido nos níveis de sistema, projeto e usuário, conforme descrito em [Definir tipos de horas e disponibilidade para folhas de horas](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (Condicional) Se o administrador do Workfront ou do grupo tiver ativado o **Atribuir funções de trabalho a entradas de horas manualmente** selecione uma função de trabalho no menu suspenso. A função especificada quando você está atribuído ao item de trabalho é exibida por padrão. Se uma função não for atribuída a você no objeto, sua função principal será exibida como padrão. Para obter mais informações sobre essa configuração, consulte o artigo [Configurar preferências de horas e planilha de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. Especifique a hora que deseja registrar e clique em **Registro de tempo**.

### Projeto, tarefa ou problema {#project-task-or-issue}

Você pode registrar o tempo específico do projeto em um projeto, tarefa ou problema nas seguintes seções:

* [Atualiza a seção](#updates-section)
* [seção Horas](#hours-section)

#### Atualiza a seção{#updates-section}

Para registrar horas na seção Atualizações de um projeto, tarefa ou problema, você deve ter o seguinte:

* Uma licença de Trabalho ou Plano.
* Contribute ou tenha permissões mais altas para o projeto, tarefa ou problema com acesso a Registrar horas.\
  Para obter mais informações sobre a concessão de permissões em projetos, consulte [Compartilhar um projeto no Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* O administrador do Workfront deve ativar a configuração Registrar tempo diretamente nos projetos em [!UICONTROL **Horas e Planilha de Horas**]> [!UICONTROL **Preferências**], se quiser registrar horas diretamente em um projeto.

  Para obter mais informações sobre como permitir que os usuários registrem horas diretamente nos projetos, consulte [Configurar preferências de horas e planilha de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para registrar horas na seção Atualizações de um projeto, tarefa ou problema:

1. Ir para um projeto, tarefa ou problema.
1. No painel esquerdo, selecione **Atualizações**.
1. Clique em **Registro de tempo**. <!-- did Anna B change the casing for this button? If yes and if she changed it for the other areas, update screen shot too-->

   A caixa de diálogo Log time é exibida.

   >[!TIP]
   >
   >   Se a preferência do seu perfil estiver definida para registrar horas em dias, a caixa Inserir dias será exibida.
   >   
   >   Há uma indicação no canto superior direito da caixa Inserir dias de quantas horas são incluídas em um dia.

   ![](assets/log-time-box-in-updates-stream.png)

1. Especifique as seguintes informações:

   * **Tipo de Hora**: selecione um Tipo de hora no menu suspenso, se ele for diferente do exibido por padrão.

     Dependendo dos tipos de horas configurados em seu sistema, as opções aqui podem variar. Para obter mais informações sobre a configuração de tipos de horas, consulte [Definir tipos de horas e disponibilidade para folhas de horas](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Função de trabalho**: (Condicional) Se o administrador do Workfront ou do grupo tiver ativado o **Atribuir funções de trabalho a entradas de horas manualmente** , selecione uma **Função de trabalho** no menu suspenso. A Função especificada quando você está atribuído ao objeto é exibida por padrão. Se uma Função não for atribuída a você, sua Função principal é exibida como padrão. Para obter mais informações sobre essa configuração, consulte o artigo [Configurar preferências de horas e planilha de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   * **Horas**: insira o número de horas do projeto, tarefa ou problema.

1. Clique em **Registrar tempo**.

#### seção Horas{#hours-section}

Você deve ser um administrador do Workfront para registrar horas para projetos, tarefas e problemas na seção Horas,

Ou

Você deve ter todos os itens a seguir:

* Uma licença de Plano com acesso administrativo a Planilhas de Horas e horas. Para obter mais informações sobre como conceder acesso administrativo a Folhas de horas e horas, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* Contribute ou tenha permissões mais altas para o projeto com acesso a Registrar horas. Para obter mais informações sobre a concessão de permissões em projetos, consulte [Compartilhar um projeto no Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* O administrador do Workfront deve ativar a configuração Registrar tempo diretamente nos projetos em Planilha de horas e Horas > Preferências, se quiser registrar tempo diretamente em um projeto. Para obter mais informações sobre como permitir que os usuários registrem horas diretamente nos projetos, consulte [Configurar preferências de horas e planilha de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para registrar horas na seção Horas de um projeto, tarefa ou problema:

1. Ir para um projeto, tarefa ou problema.
1. No painel esquerdo, clique em **Horas**.
1. Clique em **Registro de tempo**.

   A caixa de diálogo Log Hours é exibida.

1. Especifique as seguintes informações:

   * **Proprietário:** Seu nome é exibido nesse campo, por padrão.\
     Se você estiver registrando as horas de outro usuário, especifique o nome dele.

   * **Tipo de Hora**: selecione um Tipo de hora no menu suspenso, se ele for diferente do exibido por padrão.

     Dependendo dos tipos de horas configurados em seu sistema, as opções aqui podem variar. Para obter mais informações sobre a configuração de tipos de horas, consulte [Definir tipos de horas e disponibilidade para folhas de horas](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Função de trabalho**: (Condicional) Se o administrador do Workfront ou do grupo tiver ativado o **Atribuir funções de trabalho a entradas de horas manualmente** , selecione uma **Função de trabalho** no menu suspenso. A Função especificada quando você está atribuído ao objeto é exibida por padrão. Se uma Função não for atribuída a você, sua Função principal é exibida como padrão. Para obter mais informações sobre essa configuração, consulte o artigo [Configurar preferências de horas e planilha de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     ![](assets/log-time-box-in-hours-section-on-task.png)
   * **Horas**: insira o número de horas do projeto, tarefa ou problema.

1. Clique em **Registro de tempo**.

### Painel Resumo

Você pode registrar o tempo para tarefas e problemas no painel Resumo.
Para obter mais informações, consulte [Visão geral do resumo](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### Quadros {#boards}

É possível registrar o tempo em cartões conectados em uma placa Workfront. Esse é o mesmo processo que registrar o tempo em uma tarefa ou problema, e as horas registradas no cartão são salvas na tarefa ou problema conectado.
Para obter mais informações, consulte [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### Aplicativo móvel {#mobile-app}

Você pode registrar horas no aplicativo móvel do Workfront.
Para obter mais informações, consulte [Adobe Workfront para Android](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) ou [Adobe Workfront para iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
