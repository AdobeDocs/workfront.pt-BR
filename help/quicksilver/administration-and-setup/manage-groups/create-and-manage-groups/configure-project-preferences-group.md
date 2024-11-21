---
title: Configurar preferências do projeto para um grupo
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Se você for um administrador de grupo e um administrador do Adobe Workfront desbloquear uma preferência de projeto para todos os grupos no sistema, poderá configurar essa preferência para que o grupo afete todos os projetos subsequentes criados pelo grupo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '2648'
ht-degree: 2%

---

# Configurar as preferências do projeto para um grupo

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Se você for um administrador de grupo e um administrador do Adobe Workfront desbloquear uma preferência de projeto para todos os grupos no sistema, poderá configurar essa preferência para que o grupo afete todos os projetos subsequentes criados pelo grupo.

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!NOTE]
>
>* Normalmente, uma preferência desbloqueada permanece desbloqueada indefinidamente. Se o administrador do Workfront o bloquear novamente, a configuração do sistema será aplicada novamente e as configurações da preferência feita pelos administradores de grupo serão perdidas.
>* As preferências definidas para o grupo associado a um projeto têm precedência sobre as preferências definidas para o Grupo padrão do usuário que cria o projeto.
>* Algumas preferências de nível de grupo afetam os modelos de projeto criados para o grupo. Para obter mais informações, consulte a seção [Exibir, trabalhar com e criar modelos para seu grupo da área Grupos](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) no artigo [Criar e modificar os modelos de projeto de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Depois que um administrador do Workfront desbloqueia uma preferência no nível do sistema, você pode configurá-la e bloqueá-la para garantir que todos no seu grupo e em seus subgrupos usem a mesma configuração. Isso é paralelo à capacidade que um administrador do Workfront tem de configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Bloquear ou desbloquear uma preferência de projeto, tarefa ou problema para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

A configuração no nível do grupo também é possível para preferências de tarefas e problemas, bem como para preferências de horas e planilhas de horas. Para obter informações, consulte [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) e [Configurar preferências de horas e folha de horas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Para obter informações sobre como um administrador do Workfront desbloqueia uma preferência de projeto, consulte [Bloquear ou desbloquear preferências de projeto para todos os grupos no sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar uma preferência de projeto desbloqueada para um grupo

>[!TIP]
>
>Se você for um administrador do Workfront, poderá ignorar as etapas 1 a 4 em Configuração > Preferências do projeto > Projetos e, em seguida, pesquisará o nome do grupo na caixa na parte superior da página.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo cujas preferências de projeto você deseja configurar.
1. No painel esquerdo, clique em **Preferências do projeto**.
1. Na página exibida, continue com uma das quatro seções listadas abaixo para configurar as preferências de Status do projeto, Linhas do tempo, Casos de negócios e Vida após a morte.

   >[!TIP]
   >
   >Se você passar o mouse sobre uma preferência e uma dica de ferramenta for exibida para informá-lo de que ela está bloqueada, peça ao administrador do Workfront para desbloqueá-la para todos os grupos na organização.

* [Status do projeto](#project-status)
* [Linhas de Tempo](#timelines)
* [Casos de negócio](#business-cases)
* [Vida após a morte](#life-after-death)

### Status do projeto {#project-status}

Configure qualquer uma das seguintes preferências para projetos recém-criados associados ao grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Permitir que os usuários criem projetos sem usar um modelo</td>
<td><p>Esta preferência permite que os usuários criem projetos sem usar um modelo ao criar um projeto das seguintes áreas:</p>
<ul>
<li><p>Usar a opção Novo projeto em uma lista de projetos</p></li>

<li><p>Converter um problema em um projeto a partir da página do problema</p></li>
</ul>

<p>Essa preferência é ativada por padrão no nível do sistema.</p>
<p><b>Nota</b></p>
<p>Quando um usuário pertence a vários grupos com preferências diferentes, ele pode criar um projeto sem um modelo se pelo menos um de seus grupos tiver essa preferência ativada.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Ajustar o status do novo projeto para</td> 
   <td> <p>Determine o status dos novos projetos.</p> <p><b>OBSERVAÇÃO</b>   
     <ul> 
      <li>Se você ou outro administrador do Workfront ocultar o status selecionado aqui, o status padrão será alterado para o primeiro status na lista de status.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">Para preferências de projeto de grupo, você pode selecionar apenas um status bloqueado ou um status obrigatório como o status padrão.</li> 
      <li> <p>Se o status de um sistema ou grupo bloqueado for definido como o status padrão e depois alguém o desbloquear, o sistema tentará substituí-lo por um status bloqueado do mesmo tipo de status.</p> <p>Se não conseguir encontrar um, ele procurará um status obrigatório:</p> 
       <ul> 
        <li>Se houver um status obrigatório igual ao status padrão desbloqueado, o status obrigatório se tornará o status padrão, mesmo se ele estiver desbloqueado.</li> 
        <li>Se nenhum dos status obrigatórios for igual ao status padrão desbloqueado, o primeiro status obrigatório na lista de status se tornará o status padrão.</li> 
       </ul> <p>Para obter informações sobre os status necessários, consulte os artigos <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de projetos do sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de tarefas do sistema</a> e <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de problemas do sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calcular percentual de conclusão com base em</td> 
   <td> <p>O percentual de conclusão de um projeto ou tarefa pai é baseado no progresso geral das tarefas. Essas informações podem ser calculadas com base na Duração ou nas Horas planejadas das tarefas em um projeto.</p> <p>Se você selecionar Duração, a Duração de cada tarefa em um projeto determinará o percentual de conclusão geral do projeto, e a Duração de cada subtarefa determinará o percentual de conclusão geral de sua tarefa pai.</p> <p>Se você selecionar Duração, certifique-se de especificar as horas Típicas por dia de trabalho e os dias de trabalho Típicos por semana na seção Linhas do tempo. O Workfront usa essas informações ao calcular o percentual concluído de uma tarefa com base na Duração. </p> <p>Se você selecionar Horas planejadas, certifique-se de que todas as tarefas em cada projeto tenham a quantidade de Horas planejadas definida e que a quantidade não seja zero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Definir automaticamente a Condição do projeto com base no Status de progresso</td> 
   <td> <p>Essa preferência permite que os usuários definam a Condição de um projeto manualmente (No destino, Em risco, Com problema) ou que o Workfront defina a Condição (Status de progresso) automaticamente com base na progressão do projeto na linha do tempo. Para obter mais informações sobre a Condição de projetos, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Visão Geral da Condição de Projeto e Tipo de Condição</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Criar linhas de base automaticamente</p> </td> 
   <td> <p>Esta preferência cria automaticamente uma linha de base (instantâneo) da tarefa e dos detalhes do projeto quando o status do projeto muda para Atual. Para obter informações sobre como criar linhas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Criar linhas de base do projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Método Índice de desempenho </p> </td> 
   <td> <p>O Método de índice de desempenho (PIM) do projeto controla o método que a Workfront usa para calcular métricas de Valor obtido, como Índice de desempenho de custo (CPI) e Estimar na conclusão (EAC). Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcular Índice de Desempenho de Custo (CPI)</a>e <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular Estimativa na Conclusão (EAC)</a></p> 
    <ul> 
     <li><strong>Baseado em hora</strong>: a Workfront usa o Trabalho em horas para calcular métricas de desempenho como EAC e CPI. Quando o PIM é calculado com base nas horas, o EAC é exibido como um número de horas. Certifique-se de que você tenha um valor para Horas planejadas diferente de zero.</li> 
     <li> <p><strong>Baseado em custo</strong>: a Workfront usa o Custo de Trabalho Planejado para calcular métricas de desempenho como EAC e CPI. Verifique se suas funções de trabalho ou usuários estão associados às taxas de Custo por hora. Quando o PIM é calculado com base nos Custos, o EAC é exibido como um valor de moeda.</p> <p>O gerente de projeto pode modificar essa configuração no nível do projeto, usando a área Finanças em Detalhes do Projeto. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gerenciar informações na área Finanças do projeto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Calcular ao concluir </p> </td> 
   <td> <p>Determine quais dados a Workfront usa para calcular a EAC (Estimativa no término), que representa o custo total projetado de um projeto.</p> 
    <ul> 
     <li><strong>Calcular no nível do projeto</strong>:EAC para a tarefa pai e o projeto é determinado pela inserção de Horas Efetivas ou Custo Efetivo do Trabalho nas Fórmulas EAC. Esse cálculo inclui Horas Reais ou Custos e Despesas adicionados diretamente à tarefa ou ao projeto principal.</li> 
     <li> <p><strong>Acúmulo de tarefas/subtarefas</strong>: a EAC da tarefa pai e do projeto é determinada pela soma da EAC de cada tarefa filho. Esse cálculo exclui Horas Reais ou Custos e Despesas Reais adicionados diretamente à tarefa ou projeto pai.</p> <p>O gerente de projeto pode modificar essa configuração no nível do projeto, usando a área Finanças em Detalhes do Projeto. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gerenciar informações na área Finanças do projeto</a>.</p> </li> 
    </ul> <p>Para obter mais informações sobre como o EAC é calculado, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular EAC (Estimativa no Término)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Linhas de Tempo {#timelines}

Configure qualquer uma das seguintes preferências para projetos recém-criados associados ao grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Cronograma de</td> 
   <td> <p>Determine se os novos projetos estão programados a partir da Data inicial ou da Data de conclusão quando são criados.</p> 
    <ul> 
     <li><strong>Data de Início</strong>: novas tarefas assumem como padrão a Restrição de Tarefa O Mais Breve Possível e os gerentes de projeto são solicitados a fornecer uma Data de Início Planejada para o projeto.</li> 
     <li><strong>Data de conclusão</strong>: novas tarefas assumem como padrão a Restrição de Tarefa o Mais Tarde Possível e os gerentes de projeto são solicitados a fornecer uma Data de conclusão planejada para o projeto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tempo de folga do usuário</td> 
   <td> <p>Determine se o tempo de folga do Principal responsável por uma tarefa ajusta as datas planejadas para essa tarefa em um projeto.</p> 
    <ul> 
     <li> <p><strong>Considere o tempo de folga do usuário nas durações da tarefa</strong>: qualquer tempo de folga agendado para o Destinatário Principal de uma tarefa ajusta as datas planejadas da tarefa se o tempo de folga ocorrer durante a duração da tarefa. Esta é a configuração padrão. </p> <p>Por exemplo, se uma tarefa com uma Restrição o Mais Breve Possível estiver programada para iniciar em 1° de junho e terminar em 3 de junho, e o Destinatário principal tiver o dia 2 de junho marcado para Folga, as datas planejadas da tarefa serão ajustadas de 1º de junho a 4 de junho.</p> <p><b>IMPORTANTE</b>: a duração da tarefa não é alterada quando você seleciona essa configuração. Somente as datas planejadas mudam, dependendo da Restrição da Tarefa.</p> </li> 
     <li><strong>Ignorar o tempo de folga do usuário nas durações de tarefa</strong>: as datas planejadas de cada tarefa em um projeto permanecem como planejadas originalmente, mesmo que o Destinatário Principal de uma tarefa tenha folga durante sua duração.</li> 
    </ul> <p>Considere o seguinte ao selecionar opções para essa configuração:</p> 
    <ul> 
     <li>Quando você altera essa configuração, somente os projetos e modelos criados após a alteração herdam a configuração atualizada. </li> 
     <li> <p>O valor Restrição da Tarefa determina quais datas da tarefa planejada devem ser ajustadas: </p> 
      <ul> 
       <li>A data de início planejada</li> 
       <li>A data de conclusão planejada</li> 
       <li>Ambas as datas</li> 
       <li>Nenhuma data. </li> 
      </ul> <p>Por exemplo, se uma tarefa tiver uma Restrição de datas fixas, as datas não são ajustadas quando o Destinatário principal tem folga, mesmo se a opção Considerar folga do usuário na duração da tarefa estiver selecionada. Para obter informações sobre restrições de tarefa, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Visão geral da Restrição de Tarefa</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>As linhas de tempo do projeto serão recalculadas automaticamente</strong> </p> </td> 
   <td> <p>Determine quando a linha do tempo de um projeto é recalculada. Para obter informações sobre como recalcular a linha de tempo do projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular linhas de tempo do projeto</a>.</p> <p>As opções a seguir são ativadas por padrão. Você pode selecionar uma ou mais das seguintes configurações:</p> 
    <ul> 
     <li> <p><strong>Todas as noites</strong>: selecione esta opção para recalcular as linhas de tempo do projeto todas as noites. Quaisquer alterações feitas no projeto que possam afetar a linha do tempo não ficam visíveis imediatamente. O Workfront​​​ recalcula as linhas do tempo à noite somente para projetos em que ambas as condições a seguir sejam atendidas:</p> <p> 
       <ul> 
        <li>Têm status Atual</li> 
        <li>Teve uma atualização nos últimos 3 meses</li> 
       </ul> </p> </li> 
     <li> <p><strong>Quando o escopo de um projeto for alterado</strong>: selecione esta opção para recalcular as linhas de tempo do projeto imediatamente, à medida que ocorrer uma alteração no escopo do projeto. Para obter informações sobre o que constitui uma alteração de escopo de projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular linhas do tempo do projeto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Quando vários usuários forem atribuídos a uma tarefa, use o agendamento de</strong> </p> </td> 
   <td> <p>Se um projeto não tiver um agendamento atribuído ou se os usuários atribuídos a suas tarefas não tiverem um Agendamento atribuído a eles, o Workfront usará o agendamento padrão do sistema para calcular a linha do tempo das tarefas.</p> <p>Se você atribuir vários usuários à mesma tarefa em um projeto tiver um agendamento atribuído, e os usuários atribuídos às tarefas também tiverem um agendamento atribuído a eles, o Workfront usará os seguintes agendamentos:</p> 
    <ul> 
     <li><strong>Atribuição primária</strong>: a Workfront usa o agendamento da Atribuição primária na tarefa para calcular linhas do tempo.</li> 
     <li><strong>Projeto</strong>: a Workfront usa a agenda do projeto para calcular a linha de tempo de cada tarefa.</li> 
    </ul> <p>Para obter mais informações sobre agendamentos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Criar um agendamento</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Cálculos de linha do tempo </p> </td> 
   <td> 
    <ul> 
     <li><strong>Horas típicas por dia útil</strong>: Defina o número de horas em um dia útil típico para os usuários que trabalharão nos projetos. O padrão é 8 horas.</li> 
    </ul> 
    <ul> 
     <li><strong>Dias úteis típicos por semana</strong>: defina a semana útil padrão para os usuários que trabalharão nos projetos. O padrão é 5 dias.</li> 
    </ul> <p>Essas 2 opções convertem dias em horas ou semanas em dias.</p> <p>Por exemplo, se você tiver uma tarefa com 8 Horas planejadas e a duração for calculada com base nas Horas planejadas, o Workfront converterá essas horas em dias para mostrar a Duração como dias.</p> <p>No campo Typical work days per week, o Workfront calcula o valor de Full Time Equivalent (FTE) para o seu sistema. É o que o Workfront usa ao calcular alocações para usuários.</p> <p>Esses valores são usados quando você está planejando cronogramas de projetos, orçamento de recursos ou registro de tempo em projetos. </p> <p>Elas não são usadas quando você está estabelecendo folhas de horas para usuários no sistema, conforme descrito em <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Configurar folhas de horas e preferências de horas</a>.</p> <p><b>OBSERVAÇÃO</b>: os administradores do Workfront não podem desbloquear as preferências de Cálculos de Linha do Tempo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Trimestres personalizados</strong> </p> </td> 
   <td> <p>Configure trimestres anuais personalizados para os usuários que trabalharão nos projetos. Os trimestres personalizados geralmente são trimestres que não correspondem ao detalhamento tradicional de trimestres durante um ano civil. Você pode adicionar vários trimestres personalizados. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Habilitar trimestres personalizados para projetos</a>.</p> <p><b>OBSERVAÇÃO</b>: os administradores do Workfront não podem desbloquear as preferências de Trimestres personalizados.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--Add this to the table (under the "When multiple users are assigned ..." setting):

When one user is assigned to a task, use the schedule of the...


<p>If a project does not have a schedule assigned or if the users assigned to its tasks do not have a Schedule assigned to them, [!DNL Workfront] uses the system default schedule to calculate the timeline of the tasks.</p> <p>If you assign one user to a task in a project and the project has an assigned schedule and the user assigned to the tasks also has a schedule assigned to them, [!UICONTROL Workfront] uses the following schedules:</p> 
    <ul> 
     <li><strong>[!UICONTROL User]</strong>: The schedule of the assigned user on the task to calculate timelines.</li> 
     <li><strong>[!UICONTROL Project]</strong>: The schedule of the project to calculate the timeline of the task.</li> 
    </ul> <p>For more information about schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Create a schedule</a>.</p>

-->

### Casos de negócio {#business-cases}

Você pode criar um Business Case para projetos recém-criados associados ao grupo para enviar solicitações de projeto. Você pode definir preferências para determinar quais áreas estão visíveis no formulário **Business Case**. Recomendamos ativar essas opções para que outras ferramentas, como o Portfolio Otimizer, sejam atualizadas corretamente. Para obter mais informações sobre o que cada campo exibe, consulte [Definir um Business Case: índice de artigo](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Depois que o administrador do Workfront habilita as seções no Business Case, um Proprietário do projeto pode criar um Business Case no nível do projeto. Para obter informações sobre como criar um Business Case, consulte [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Vida após a morte  {#life-after-death}

Configure qualquer uma das seguintes preferências para projetos recém-criados associados ao grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Depois que um projeto for marcado como Concluído, as pessoas ainda poderão</strong> </p> </td> 
   <td> <p>Determine as regras para sua organização (ou grupo, se estiver configurando preferências de projeto para um grupo) em relação à possibilidade de uma tarefa ou problema ser excluído após o status do projeto ter sido marcado como Concluído.</p> 
    <ul> 
     <li><strong>Excluir Tarefas</strong>: permite que os usuários excluam tarefas de um projeto depois que o projeto for marcado como Concluído.<br></li> 
     <li><strong>Excluir Problemas</strong>: permite que usuários excluam problemas de um projeto depois que o projeto é marcado como Concluído.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Depois que um projeto for marcado como Concluído, Inativo ou com Aprovação Pendente, as pessoas ainda poderão</strong> </p> </td> 
   <td> <p>Determine as regras da sua organização (ou grupo, se estiver configurando preferências de projeto para um grupo) em relação ao que acontece com tarefas, problemas, documentos e outros objetos em um projeto depois que o status do projeto é marcado como <strong>Concluído</strong>, <strong>Desativado</strong> ou com <strong>Aprovação pendente</strong>.</p> 
    <ul> 
     <li><strong>Adicionar e editar tarefas</strong> Permite aos usuários: 
      <ul> 
       <li>Editar tarefas em um projeto depois que ele for marcado como Concluído, Inativo ou com Aprovação pendente. Isso inclui adicionar horas e alterar entradas de despesas em uma tarefa.</li> 
       <li>Adicionar tarefas a um projeto.</li> 
      </ul></li> 
     <li><strong>Adicionar e editar problemas</strong>: permite aos usuários: 
      <ul> 
       <li>Editar problemas em um projeto depois que ele for marcado como Concluído, Inativo ou Com aprovação pendente.</li> 
       <li>Adicione problemas a um projeto depois que o projeto for marcado como Concluído ou Inativo. (Você não pode adicionar problemas a um projeto que está com Aprovação pendente.)</li> 
      </ul></li> 
     <li> <p><strong>Adicionar documentos ao projeto e às suas tarefas e problemas</strong>: permite que os usuários adicionem documentos a um projeto (ou para adicionar documentos a tarefas e problemas dentro do projeto) depois que o projeto for marcado como Concluído ou Inativo.</p> <p>Essa opção não se aplica a projetos com aprovação pendente.</p> </li> 
     <li> <p><strong>Anexar modelos</strong>: permite que os usuários anexem modelos a um projeto depois que o projeto for marcado como Concluído ou Inativo.</p> <p>Essa opção não se aplica a projetos com aprovação pendente.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
