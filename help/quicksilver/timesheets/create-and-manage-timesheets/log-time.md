---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Tempo de registro
description: Você pode registrar o tempo dos itens de trabalho no &Adobe Workfront para indicar o número de horas que você gastou trabalhando neles. Você também pode registrar tempo que não esteja relacionado ao trabalho, como férias, tempo de doença ou tempo gasto em reuniões. A hora em que você registra é exibida na sua folha de horas.
author: Alina
feature: Timesheets
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: e148126102d30ef061a89edae83980ebe81e9810
workflow-type: tm+mt
source-wordcount: '3016'
ht-degree: 0%

---

# Tempo de registro

Você pode registrar o tempo para itens de trabalho no Adobe Workfront para indicar o número de horas que você gastou trabalhando neles. Você também pode registrar tempo que não esteja relacionado ao trabalho, como férias, tempo de doença ou tempo gasto em reuniões. A hora em que você registra é exibida na sua folha de horas.

Para obter mais informações sobre o tipo de horas em que você pode fazer logon no Workfront, consulte [Gerenciar tipos de hora](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

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

Você deve ter o seguinte acesso para executar as etapas neste artigo e registrar as Horas específicas do projeto:

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
   <td> <ul><li>Revisar ou superior para registrar Horas Gerais em uma folha de ponto</li>
   <li> Trabalhe ou superior para registrar horas em um projeto, tarefa ou problema</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Edite o acesso ao tipo de item de trabalho para o qual você registra o tempo </p> <p>Por exemplo, é necessário Editar acesso a Problemas para registrar o tempo dos problemas</p> <p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribua com permissões mais altas no item de trabalho para o qual você registra no tempo, incluindo permissões para as Horas de registro.</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações ao registrar o tempo no Workfront

* Você pode registrar tempo para projetos, tarefas ou problemas, ou pode registrar tempo diretamente na sua folha de horas.

   Para obter informações sobre como criar folhas de horas, consulte [Criar uma folha de ponto de uso único](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* Todas as ferramentas logadas durante o período correspondente, exceto a folha de ponto, são exibidas na folha de ponto.
* Tarefas e problemas em um projeto que não é atual não são preenchidos previamente em uma folha de ponto.
* O tempo registrado na folha de ponto é aplicado imediatamente à tarefa, ocorrência ou projeto.
* As folhas de horas incluem o tempo total para todas as datas registradas. Os finais de semana são sempre incluídos, mesmo quando os cálculos de linha do tempo foram configurados para excluí-los (conforme descrito em [Configurar preferências de projeto em todo o sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)).
* O número máximo de itens exibidos em uma folha de ponto é 45. Se houver mais de 45 itens cujas datas correspondam ao período da folha de ponto, somente os itens atualizados mais recentemente serão exibidos.
* As entradas de hora incluídas nos registros de faturamento faturados estão esmaecidas e não podem ser editadas na folha de horas. Para obter mais informações, consulte [Criar registros de faturamento](../../manage-work/projects/project-finances/create-billing-records.md).

## Tempo de registro

Você pode registrar o tempo nas seguintes áreas no Workfront:

* [Planilha de horas](#timesheet)
* [Página inicial](#home)
* [Projeto, tarefa ou problema](#project-task-or-issue)
* [Painel Resumo](#summary-panel)
* [Quadros](#boards)
* [Aplicativo móvel](#mobile-app)

### Planilha de horas {#timesheet}

Você pode registrar horas gerais ou horas específicas do projeto em uma folha de ponto.

>[!NOTE]
>
>Os usuários de revisão atribuídos a um Perfil de Folha de Horas podem ver a guia Folhas de Horas e registrar horas gerais. No entanto, eles não podem registrar horas em nenhuma tarefa ou problema atribuído a eles que apareça na folha de ponto.

1. Clique no botão [!UICONTROL **Menu principal**] ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em [!UICONTROL **Folhas de Horas**]. Sua folha de ponto atual é exibida por padrão.
   ![Planilha de horas](assets/timesheet-redesigned-nwe.png)

   A folha de ponto é pré-preenchida com itens atribuídos a você durante o período da folha de ponto. Para obter informações sobre como as folhas de horas são pré-preenchidas, consulte [Configurar preferências de hora e folha de ponto](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md). Se você não vir um item na folha de ponto, é possível adicioná-lo.

   >[!NOTE]
   >
   >A folha de ponto é preenchida automaticamente somente com itens atribuídos a você. Ele não preenche com itens atribuídos às suas equipes ou funções de trabalho.
   >
   >Clicar em Trabalhar nele em um item atribuído às suas equipes atribui o item a você e o item será exibido na sua folha de horas.


1. (Opcional) Clique no botão **tela cheia** ícone ![](assets/full-screen.png) para exibir a folha de ponto no modo de tela cheia, clique no botão **tela cheia de saída** ![](assets/exit-full-screen.png) ícone para retornar à folha de ponto.

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (Opcional) Para adicionar um projeto, tarefa ou problema à folha de ponto, clique no botão **Adicionar item** menu suspenso no canto superior esquerdo da folha de ponto e clique em **Adicionar projetos**, **Adicionar Tarefas** ou **Adicionar problemas**.

   Uma lista de projetos, tarefas ou problemas é exibida.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (Opcional) Clique no ícone de pesquisa ![Procurar um item](assets/search-icon.png) para procurar um item específico usando uma palavra-chave para adicionar à folha de ponto.

1. (Opcional) Expanda os menus suspensos filtro, visualização ou agrupamento para aplicar ou personalizar um e para exibir as informações do item que deseja.

1. Selecione um ou vários itens na lista e clique em **Adicionar**.

   >[!NOTE]
   >
   >Quando você adiciona tarefas ou problemas à folha de ponto, o projeto também é adicionado.


1. (Condicional) Se você adicionar 50 ou mais itens de uma vez, uma mensagem de confirmação exibindo o número de itens adicionados à sua folha de horas será exibida.

   Clique em **Adicionar tudo** para adicionar todos os itens Ou clique em **Cancelar** para interromper a adição dos itens selecionados, em seguida **Cancelar** para fechar a lista de itens.

   Tarefas e problemas são listados com o nome do projeto.

   >[!NOTE]
   >
   >Os itens que você adiciona manualmente à folha de ponto são fixados e permanecerão nas folhas de ponto atuais e futuras até que você os desmarque manualmente para removê-los. Para obter informações sobre como desmarcar itens para removê-los da folha de ponto, continue com a Etapa 10.

   <!--(ensure this stays accurate)-->

1. (Opcional) Clique no botão **Recolher** ![](assets/collapse-icon.png) ou **Expandir** ![](assets/expand-icon.png) ícones ao lado do nome do projeto para exibir ou ocultar a lista de tarefas e problemas do projeto.


   >[!TIP]
   >
   >   Ao usar um teclado QWERTY padrão e depois de clicar no nome de um projeto na folha de ponto, pressione o seguinte conjunto de teclas para recolher ou expandir o projeto:
   >   * Para expandir o projeto e exibir seus itens de trabalho:
      >     * Shift + Alt + seta para cima para computadores Windows
      >     * Shift + Option + seta para cima para computadores Mac
   >   * Para recolher o projeto e ocultar seus itens de trabalho:
      >     * Shift + Alt + seta para baixo para computadores Windows
      >     * Shift + Option + seta para baixo para computadores Mac.



1. (Opcional) Para fixar manualmente um item que é exibido na folha de ponto automaticamente, passe o mouse sobre o nome do item e clique no botão **pino** ícone ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   Ao usar um teclado QWERTY padrão depois de clicar em um item na folha de ponto, pressione o seguinte conjunto de teclas para fixar um item:
   >   * Opção + P para computadores Windows e Mac.



1. (Opcional) Clique no ícone de pesquisa ![](assets/search-icon.png) e comece a digitar uma palavra-chave para localizar um projeto, uma tarefa ou um problema na folha de ponto.

1. (Opcional) É possível remover um item (projeto, tarefa ou problema) da folha de ponto se você tiver adicionado manualmente o item (conforme descrito nas Etapas 3 a 6) e se ainda não tiver registrado tempo em relação a ele, removendo-o. <!--ensure this stays accurate-->

   Não é possível remover itens incluídos na folha de ponto automaticamente de acordo com as preferências da folha de ponto no seu sistema ou grupo do Workfront que estão configurados para preencher previamente as folhas de ponto (conforme descrito em [Configurar preferências de hora e folha de ponto](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   Para remover um item da folha de ponto que foi adicionado manualmente:

   1. Certifique-se de que não haja registro de hora no item.
   1. Clique no botão **remover** ícone ![Fixar um item](assets/pin-icon.png) ao lado do item para desprender o item da folha de ponto.

   >[!TIP]
   >
   >   Ao usar um teclado QWERTY padrão depois de clicar em um item na folha de ponto, pressione o seguinte conjunto de teclas para desafixar um item:
   >   * Opção + P para computadores Windows e Mac.



   O item é removido da folha de ponto depois que você atualiza a página.

1. (Condicional) Se o administrador da Workfront ou do grupo ativou a variável **Atribuir funções de tarefa a entradas de hora manualmente** , selecione uma função de trabalho no menu suspenso. A função especificada quando você é atribuída ao item de trabalho é exibida por padrão. Se você não tiver uma função atribuída ao objeto, sua Função primária será exibida como padrão. Para obter mais informações sobre essa configuração, consulte o artigo [Configurar preferências de hora e folha de ponto](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![Tempo de registro para várias funções na folha de horas](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. (Opcional) Clique no botão **+** ícone para adicionar outra linha, em seguida, selecione um novo tipo de hora no menu suspenso na [!UICONTROL Tipo de hora] coluna para registrar o tempo para um tipo de hora diferente.

   ![Menu suspenso Tipo de hora](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Dependendo do seu sistema operacional ou navegador e ao usar um teclado QWERTY padrão, pressione o seguinte conjunto de teclas para adicionar outra linha:
   >   * Ctrl + Option + + para computadores Windows
   >   * Cmd + Opção + + para computadores Mac


   Os tipos de horas estão disponíveis, dependendo do que foi definido nos níveis do sistema, projeto e usuário, conforme descrito em [Definir os tipos de hora e a disponibilidade das folhas de horas](define-hour-types-and-availability.md).

   O tipo de hora não pode ser alterado depois que uma folha de ponto é fechada.

   >[!TIP]
   >
   >Se você tiver registrado log antes e o tipo de hora selecionado for desativado, a linha inteira para o tempo registrado ficará esmaecida. Selecionar outro tipo de hora e atualizar a página remove a opção de tipo de hora desativada da lista suspensa, de modo que não é possível adicionar mais horas a esse tipo de hora.
   >
   >Considere adicionar uma nova linha para o item de trabalho que deseja registrar mais tempo e selecionar um novo tipo de hora, se desejar manter o tipo de hora desativado associado ao tempo registrado anterior.

1. Clique no botão **excluir** ícone  ![](assets/delete.png) ao lado da função de trabalho para removê-la. Qualquer vez registrada para a função também é removida.

   >[!TIP]
   >
   >   Dependendo do seu sistema operacional ou navegador e ao usar um teclado QWERTY padrão, pressione o seguinte conjunto de teclas para excluir uma linha:
   >   * Ctrl + Opção + - para computadores Windows
   >   * Cmd + Opção + - para computadores Mac



1. Especifique a quantidade de tempo que deseja fazer logon em qualquer dia na seção da linha do tempo da folha de horas e clique fora da caixa de hora para salvar a entrada de hora. As horas são salvas automaticamente. A linha em que a hora de registro é realçada em azul claro e a caixa de entrada da hora é contornada em azul escuro.

   ![Caixa de hora do registro na folha de horas](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   Você registra o tempo em horas ou dias. Essa configuração é configurada pelos usuários com uma licença do Plano ou pelo administrador do sistema, conforme descrito em [Configurar se a hora é registrada em horas ou dias](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >Você deve salvar a folha de ponto manualmente se qualquer um dos seguintes cenários ocorrer:
   >
   >* A função de trabalho associada ao tempo que você fez logon anteriormente foi alterada e a função **Atribuir funções de tarefa a entradas de hora manualmente** foi desativada. O tempo de registro de novas datas o associará a uma função de trabalho diferente.
      >   
      >   Se a função tiver sido alterada e a função **Atribuir funções de tarefa a entradas de hora manualmente** estiver ativada, você poderá registrar o tempo ou atualizar a função e suas alterações serão salvas automaticamente.
   >
   >* A função de trabalho atribuída a uma tarefa ou problema é diferente da função de trabalho com a qual o proprietário da folha de ponto está registrando tempo <!--or assigned to them_ this last  piece came from a Support note but but sure what role it's referring to. Leaving it out for now.-->.
   >
   >A folha de ponto salvará novamente o tempo automaticamente quando não houver mais entradas conflitantes entre as duas funções.

1. (Opcional) Especifique a quantidade de horas extras no campo Hora extra no cabeçalho da folha de horas.

   >[!TIP]
   >
   >Não é possível registrar um número maior de horas extras do que o total de horas atual na folha de horas. Por exemplo, se você fez logon por 7 horas na folha de ponto até o momento, não é possível registrar 8 horas extras.

1. (Opcional) Clique em **Comentário** para adicionar um comentário para a entrada de hora.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Ao usar um teclado QWERTY padrão depois de clicar na caixa de entrada de hora, pressione o seguinte conjunto de teclas para abrir a caixa de comentários:
   >   * Shift + F2 para computadores Windows e Mac.


1. Clique em **Concluído** para salvar o comentário.

   >[!TIP]
   >
   >   Ao usar um teclado QWERTY padrão, de dentro da caixa de comentários, pressione o seguinte conjunto de teclas para salvar o comentário:
   >   * Ctrl + Enter para computadores Windows.
   >   * Cmd + Retorno para computadores Mac.



1. (Opcional) Clique em **Mostrar comentários** na barra de ferramentas para exibir comentários de entrada de hora no item de trabalho.

   ![Comentários listados no item da folha de ponto](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Todas as alterações feitas na folha de ponto são salvas automaticamente.

1. (Opcional) Clique na linha de uma tarefa ou problema e, em seguida, clique em **Abrir resumo** no canto superior direito da folha de ponto para adicionar uma atualização ou atualizar informações sobre a tarefa ou problema. O painel Resumo é aberto à direita.

   ![resumo-painel-para-tarefa-aberta-no-horário](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   Sua atualização é exibida na área Atualizações do item de trabalho associado ao tempo registrado.

   >[!TIP]
   >
   >Não é possível comentar projetos ou entradas de Hora Geral.

1. Clique em [!UICONTROL **Fechar resumo**] para fechar o painel Resumo e retornar à folha de ponto.

1. (Opcional) Clique em [!UICONTROL **Atualizações**] no painel à esquerda, adicione uma atualização à folha de horas. Para obter mais informações sobre atualizações do Workfront, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-recreated-timesheet-left-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

   * **Fechar**: Feche a folha de ponto quando terminar de atualizá-la. Essa opção só está disponível quando a folha de horas não está associada a um aprovador.

   * **Enviar para aprovação:** Essa opção só estará disponível se houver um aprovador na folha de ponto. Salve as alterações e envie para aprovação. Você pode abrir a folha de ponto depois de fechá-la clicando em **Recall**, se uma aprovação ainda não tiver sido concedida. Para obter mais informações, consulte [Enviar uma folha de ponto para aprovação](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **Rejeitar**: Essa opção é exibida quando você é um aprovador de folha de ponto e a folha de ponto foi enviada a você para aprovação. Clicar nele altera o status da folha de ponto para Rejeitada e a folha de ponto permanece aberta.

   * **Aprovar**: Essa opção é exibida quando você é um aprovador de folha de ponto e a folha de ponto foi enviada a você para aprovação. Clicar nele altera o status da folha de ponto para Aprovado e fecha a folha de ponto.
   >[!TIP]
   >
   >As opções Rejeitar e Aprovar também são exibidas na folha de ponto quando você é um administrador do sistema e a folha de ponto está associada a um aprovador.

1. (Condicional) Se tiver fechado ou enviado sua folha de horas para aprovação, clique em uma das seguintes opções:

   * **Reabrir**: Essa opção está disponível para folhas de horas que você já fechou e que não têm aprovadores ou folhas de horas que já foram aprovadas. Reabra a folha de ponto para modificar as entradas de hora.
   * **Recall**: Essa opção está disponível para folhas de horas que foram enviadas para aprovação, mas ainda não foram aprovadas ou rejeitadas. Clique em **Recall** para reabrir a folha de ponto e modificar entradas de hora.

### Página inicial {#home}

Você pode registrar o tempo específico do projeto na página inicial.

Para obter informações gerais sobre o uso da área inicial, consulte [Usar a área Início](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

Para registrar o tempo em um item de trabalho da área inicial:

1. No **Lista de Trabalho** selecione o item em que deseja registrar o tempo.
1. No painel direito, clique em **Hora de registro**.

   ![](assets/log-time-home-350x181.png)

1. No **Inserir Horas** selecione o tipo de hora apropriado.\
   Os tipos de horas estão disponíveis, dependendo do que foi definido nos níveis do sistema, projeto e usuário, conforme descrito em [Definir os tipos de hora e a disponibilidade das folhas de horas](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (Condicional) Se o administrador da Workfront ou do grupo ativou a variável **Atribuir funções de tarefa a entradas de hora manualmente** , selecione uma função de trabalho no menu suspenso. A função especificada quando você é atribuída ao item de trabalho é exibida por padrão. Se você não tiver uma função atribuída ao objeto, sua Função primária será exibida como padrão. Para obter mais informações sobre essa configuração, consulte o artigo [Configurar preferências de hora e folha de ponto](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. Especifique o horário que deseja registrar e clique em **Hora de registro**.

### Projeto, tarefa ou problema {#project-task-or-issue}

Você pode registrar o tempo específico do projeto em um projeto, tarefa ou problema.

#### Permissões necessárias para o tempo de registro

Para registrar horas em um projeto, tarefa ou problema, você precisa ter permissões específicas. Você pode registrar o tempo em dois locais em um projeto, tarefa ou problema:

* [Guia Atualizações](#updates-tab)
* [Guia Hours](#hours-tab)

##### Guia Atualizações{#updates-tab}

Os itens a seguir são necessários antes que você possa registrar horas na guia Atualizações de um projeto, tarefa ou problema:

* Você deve ter uma licença de Trabalho ou Plano.
* Você deve ter pelo menos permissões do Contribute para o projeto, tarefa ou problema com acesso às Horas de Log.\
   Para obter mais informações sobre a concessão de permissões em projetos, consulte [Compartilhar um projeto no Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* Se você quiser registrar o tempo diretamente em um projeto, o administrador do Workfront deve ativar a configuração Log time directly on projects em [!UICONTROL **Folha de Horas e Horas** ]> [!UICONTROL **Preferências**].\
   Para obter mais informações sobre como permitir que os usuários façam logon horas diretamente em projetos, consulte [Configurar preferências de hora e folha de ponto](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

##### Guia Hours{#hours-tab}

Os itens a seguir são necessários para que você possa registrar horas na guia Horas de um projeto, tarefa ou problema:

* Você deve ser o administrador do sistema.

Ou você deve ter todos os itens a seguir:

* Você deve ter uma licença do Plano com acesso administrativo a Folhas de horas e horas. Para obter mais informações sobre a concessão de acesso administrativo a Folhas de horas e horas, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* Você deve ter pelo menos permissões do Contribute para o projeto com acesso às Horas de registro. Para obter mais informações sobre a concessão de permissões em projetos, consulte [Compartilhar um projeto no Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* Se você deseja registrar o tempo diretamente em um projeto, o administrador do Workfront deve ativar a configuração Log time directly on projects , em Timesheet &amp; Hours > Preferences (Tempo de registro diretamente em projetos). Para obter mais informações sobre como permitir que os usuários façam logon horas diretamente em projetos, consulte [Configurar preferências de hora e folha de ponto](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para fazer logon em um projeto, tarefa ou problema:

1. Navegue até um projeto, tarefa ou ocorrência.
1. No painel esquerdo, selecione **Horas**.
1. Clique em **Hora de registro**.

   A caixa de diálogo Horas de registro é exibida.

1. Especifique as seguintes informações:

   * **Proprietário:** Seu nome é exibido neste campo, por padrão.\
      Se você estiver registrando as horas para outro usuário, especifique seu nome.

   * **Horas**: Insira o número de horas para o projeto, tarefa ou emissão.
   * **Tipo de hora**: Selecione um Tipo de hora no menu suspenso, se ele for diferente daquele exibido por padrão.

      Dependendo dos tipos de hora configurados no sistema, as opções aqui podem variar. Para obter mais informações sobre como configurar tipos de hora, consulte [Definir os tipos de hora e a disponibilidade das folhas de horas](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Função da Tarefa**: (Condicional) Se o administrador da Workfront ou do grupo ativou a variável **Atribuir funções de tarefa a entradas de hora manualmente** selecione uma **Função da Tarefa** no menu suspenso. A Função especificada quando é atribuída ao objeto é exibida por padrão. Se você não tiver atribuído uma Função no objeto, sua Função primária será exibida como padrão. Para obter mais informações sobre essa configuração, consulte o artigo [Configurar preferências de hora e folha de ponto](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

      ![Screen_Shot_2017-05-03_at_10.16.52_AM.png](assets/screen-shot-2017-05-03-at-10.16.52-am-350x346.png)

1. Clique em **Horas de Log**.

### Painel Resumo

Você pode registrar o tempo das tarefas e problemas no painel Resumo.
Para obter mais informações, consulte [Visão geral do resumo](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### Quadros {#boards}

Você pode registrar o tempo em placas conectadas em um quadro do Workfront. Esse é o mesmo processo que registrar o tempo em uma tarefa ou problema, e as horas registradas no cartão são salvas na tarefa ou problema conectado.
Para obter mais informações, consulte [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### Aplicativo móvel {#mobile-app}

Você pode registrar o tempo no aplicativo móvel do Workfront.
Para obter mais informações, consulte [Adobe Workfront para Android](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) ou [Adobe Workfront para iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
