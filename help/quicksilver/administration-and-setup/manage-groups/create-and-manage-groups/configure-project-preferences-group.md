---
title: Configurar preferências de projeto para um grupo
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Se você for um administrador de grupo e um administrador da Adobe Workfront desbloquear uma preferência de projeto para todos os grupos no sistema, será possível configurar essa preferência para que o grupo afete todos os projetos subsequentes criados pelo grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: 11c4028038fe3d410ee0d4f238d2138435d9a3fa
workflow-type: tm+mt
source-wordcount: '2643'
ht-degree: 3%

---

# Configurar preferências de projeto para um grupo

Se você for um administrador de grupo e um administrador da Adobe Workfront desbloquear uma preferência de projeto para todos os grupos no sistema, será possível configurar essa preferência para que o grupo afete todos os projetos subsequentes criados pelo grupo.

Se houver algum grupo acima do grupo que você gerencia, os administradores também poderão fazer isso para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!NOTE]
>
>* Normalmente, uma preferência desbloqueada permanece desbloqueada indefinidamente. Se o administrador do Workfront rebloquear, a configuração do sistema entrará em vigor novamente e as configurações da preferência feitas pelos administradores do grupo serão perdidas.
>* As preferências definidas para o grupo associado a um projeto têm prioridade sobre as preferências definidas para o Grupo inicial do usuário que cria o projeto.
>* Algumas preferências de nível de grupo afetam os modelos de projeto criados para o grupo. Para obter mais informações, consulte a seção [Exibir, trabalhar e criar modelos para seu grupo na área Grupos](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) no artigo [Criar e modificar modelos de projeto de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Depois que um administrador do Workfront desbloquear uma preferência no nível do sistema, você pode configurá-la e bloqueá-la para garantir que todos no seu grupo e em seus subgrupos estejam usando a mesma configuração. Isso é paralelo à capacidade de um administrador do Workfront configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Bloquear ou desbloquear um projeto, tarefa ou emitir preferência para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


A configuração em nível de grupo também é possível para preferências de tarefa e emissão e para o folha de ponto e preferências de hora. Para obter mais informações, consulte [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) e [Configurar as preferências de hora e folha de ponto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Para obter informações sobre como um administrador do Workfront desbloqueia uma preferência de projeto, consulte [Bloquear ou desbloquear preferências de projeto para todos os grupos no sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Configurar uma preferência de projeto desbloqueado para um grupo

>[!TIP]
>
>Se você for um administrador do Workfront, poderá ignorar as etapas 1 a 4 acessando Configurar > Preferências do projeto > Projetos e, em seguida, pesquisando o nome do grupo na caixa na parte superior da página.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo cujas preferências de projeto você deseja configurar.
1. No painel esquerdo, clique em **Preferências do projeto**.
1. Na página exibida, continue com uma das 4 seções listadas abaixo para configurar as preferências para Status do projeto, Linhas do tempo, Casos de negócios e Vida após a morte.

   >[!TIP]
   >
   >Se você passar o mouse sobre uma preferência e uma dica de ferramenta for exibida para informá-lo que está bloqueada, você pode solicitar que o administrador do Workfront a desbloqueie para todos os grupos na organização.

* [Status do projeto](#project-status)
* [Linhas de Tempo](#timelines)
* [Casos de negócio](#business-cases)
* [Vida após a morte](#life-after-death)

### Status do projeto {#project-status}

Configure qualquer uma das preferências a seguir para projetos recém-criados associados ao grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Permitir que os usuários criem projetos sem usar um modelo</td>
<td><p>Essa preferência permite que os usuários criem projetos sem usar um modelo ao criar um projeto a partir das seguintes áreas:</p>
<ul>
<li><p>Usar a opção Novo projeto em uma lista de projetos</p></li>

<li><p>Converter um problema em um projeto a partir da página do problema</p></li>
</ul>

<p>Essa preferência é ativada por padrão no nível do sistema.</p>
<p><b>Nota</b></p>
<p>Quando um usuário pertence a vários grupos com preferências diferentes, ele pode criar um projeto sem um modelo se pelo menos um de seus grupos tiver essa preferência ativada.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Definir o status do novo projeto como</td> 
   <td> <p>Determine o status de novos projetos.</p> <p><b>Nota</b>   
     <ul> 
      <li>Se você ou outro administrador do Workfront ocultar o status selecionado aqui, o status padrão será alterado para o primeiro status na lista de status.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">Para preferências de projeto de grupo, você pode selecionar apenas um status bloqueado ou um status obrigatório como status padrão.</li> 
      <li> <p>Se um sistema bloqueado ou um status de grupo for definido como o status padrão e depois alguém o desbloquear, o sistema tentará substituí-lo por um status bloqueado do mesmo tipo de status.</p> <p>Se não encontrar um, ele procura um status obrigatório:</p> 
       <ul> 
        <li>Se houver um status obrigatório que seja igual ao status padrão desbloqueado, o status necessário se tornará o status padrão, mesmo se estiver desbloqueado.</li> 
        <li>Se nenhum dos status necessários for igual ao status padrão desbloqueado, o primeiro status necessário na lista de status se tornará o status padrão.</li> 
       </ul> <p>Para obter informações sobre os status necessários, consulte os artigos <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de projeto do sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de tarefas do sistema</a>e <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Acesse a lista de status de problemas do sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calcular percentual de conclusão com base em</td> 
   <td> <p>A porcentagem de conclusão de um projeto ou tarefa pai é baseada no progresso geral das tarefas. Essas informações podem ser calculadas com base na Duração ou nas Horas Planejadas das tarefas em um projeto.</p> <p>Se você selecionar Duração, a Duração de cada tarefa em um projeto determinará a porcentagem total concluída para o projeto e a Duração de cada subtarefa determinará a porcentagem total concluída para sua tarefa pai.</p> <p>Se você selecionar Duração, especifique as Horas típicas por dia de trabalho e os Dias de trabalho típicos por semana na seção Linhas do tempo . O Workfront usa essas informações ao calcular a porcentagem de conclusão de uma tarefa com base na Duração. </p> <p>Se você selecionar Horas Planejadas, verifique se todas as tarefas em cada projeto têm a quantidade de Horas Planejadas definida e se a quantidade não é zero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Definir automaticamente a Condição do projeto com base no Status de progresso</td> 
   <td> <p>Essa preferência permite que os usuários definam a Condição de um projeto manualmente (No Target, Em risco, Em problema) ou que o Workfront defina a Condição (Status de progresso) automaticamente com base na progressão do projeto na linha do tempo. Para obter mais informações sobre a Condição dos projetos, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Visão geral da condição do projeto e do tipo de condição</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Criar linhas de base automaticamente</p> </td> 
   <td> <p>Essa preferência cria automaticamente uma linha de base (instantâneo) da tarefa e detalhes do projeto quando o status do projeto é alterado para Atual. Para obter informações sobre como criar linhas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Criar linhas de base do projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Método Índice de desempenho </p> </td> 
   <td> <p>O PIM (Performance Index Method) do projeto controla o método que a Workfront usa para calcular métricas de Valor Ganho, como CPI (Cost Performance Index) e EAC (Estimate At Completion). Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcular Índice de Desempenho de Custo (CPI)</a>e <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular Estimativa na Conclusão (EAC)</a></p> 
    <ul> 
     <li><strong>Baseado em hora</strong>: O Workfront usa Horas Planejadas para calcular métricas de desempenho como EAC e CPI. Quando o PIM é calculado com base em horas, o EAC é exibido como um número de horas. Certifique-se de ter um valor para Horas Planejadas, diferente de zero.</li> 
     <li> <p><strong>Baseado em custos</strong>: O Workfront usa o Custo planejado da mão de obra para calcular métricas de desempenho como EAC e CPI. Certifique-se de que suas funções ou usuários estejam associados às taxas de Custo por Hora. Quando o PIM é calculado com base em Custos, o EAC é exibido como um valor de moeda.</p> <p>O gerente de projeto pode modificar essa configuração no nível do projeto, usando a área Finanças em Detalhes do projeto . Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gerenciar informações na área de finanças do projeto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Calcular ao concluir </p> </td> 
   <td> <p>Determine quais dados o Workfront usa para calcular a Estimativa na Conclusão (EAC) que representa o custo total projetado de um projeto.</p> 
    <ul> 
     <li><strong>Calcular no nível do projeto</strong>:EAC para a tarefa pai e o projeto são determinados informando Horas Reais ou Custo Real da Mão de Obra nas Fórmulas EAC. Esse cálculo inclui Horas reais ou Custos e Despesas adicionados diretamente à tarefa pai ou ao projeto.</li> 
     <li> <p><strong>Rolar de tarefas/subtarefas</strong>: EAC para a tarefa pai e o projeto são determinados pela soma do EAC para cada tarefa filho. Esse cálculo exclui Horas Reais ou Custos e Despesas Reais adicionados diretamente à tarefa pai ou ao projeto.</p> <p>O gerente de projeto pode modificar essa configuração no nível do projeto, usando a área Finanças em Detalhes do projeto . Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gerenciar informações na área de finanças do projeto</a>.</p> </li> 
    </ul> <p>Para obter mais informações sobre como o EAC calcula, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular Estimativa na Conclusão (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Linhas de Tempo {#timelines}

Configure qualquer uma das preferências a seguir para projetos recém-criados associados ao grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Cronograma de</td> 
   <td> <p>Determine se os novos projetos são agendados a partir da Data inicial ou da Data de conclusão quando são criados.</p> 
    <ul> 
     <li><strong>Data inicial</strong>: Novas tarefas são padronizadas para a Restrição de Tarefa Assim que Possível e os gerentes de projeto são solicitados a fornecer uma Data Inicial Planejada para o projeto.</li> 
     <li><strong>Data de conclusão</strong>: Novas tarefas são padronizadas para a Restrição de Tarefas o Mais Tarde Possível e os gerentes de projeto são solicitados a fornecer uma Data de Conclusão Planejada para o projeto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tempo de folga do usuário</td> 
   <td> <p>Determine se a hora do Destinatário Principal de uma tarefa ajusta as datas planejadas para essa tarefa em um projeto.</p> 
    <ul> 
     <li> <p><strong>Considere o tempo limite do usuário nas durações da tarefa</strong>: Qualquer hora de agendamento para o Destinatário Principal de uma tarefa ajusta as datas planejadas da tarefa se o tempo limite ocorrer durante a duração da tarefa. Esta é a configuração padrão. </p> <p>Por exemplo, se uma tarefa com uma Restrição do Mais Rápido Possível estiver programada para iniciar em 1º de junho e ser concluída em 3 de junho, e o Destinatário Principal tiver 2 de junho marcado para Tempo Limite, as datas planejadas da tarefa serão ajustadas para 1 de junho a 4 de junho.</p> <p><b>IMPORTANTE</b>: A Duração da tarefa não é alterada ao selecionar essa configuração. Somente as datas planejadas são alteradas, dependendo da Restrição de Tarefa.</p> </li> 
     <li><strong>Ignorar tempo limite do usuário nas durações da tarefa</strong>: As datas planejadas de cada tarefa em um projeto permanecem como originalmente planejadas, mesmo se o Destinatário Principal de uma tarefa tiver tempo livre durante sua duração.</li> 
    </ul> <p>Considere o seguinte ao selecionar as opções para esta configuração:</p> 
    <ul> 
     <li>Ao alterar essa configuração, somente os projetos e modelos criados após a alteração herdam a configuração atualizada. </li> 
     <li> <p>O valor de Restrição de Tarefa da tarefa determina quais datas de tarefa planejada ajustar: </p> 
      <ul> 
       <li>A data de início planejada</li> 
       <li>A data de conclusão planejada</li> 
       <li>Ambas as datas</li> 
       <li>Nenhuma data. </li> 
      </ul> <p>Por exemplo, se uma tarefa tiver uma Restrição de Datas Fixas, as datas não se ajustarão quando o Destinatário Principal tiver tempo de folga, mesmo se a opção Considere que o tempo do usuário off na duração da tarefa estiver selecionada. Para obter informações sobre restrições de tarefa, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Visão geral da restrição de tarefa</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>As linhas do tempo do projeto serão recalculadas automaticamente</strong> </p> </td> 
   <td> <p>Determine quando a linha do tempo de um projeto é recalculada. Para obter informações sobre como recalcular a linha do tempo do projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular linhas do tempo do projeto</a>.</p> <p>As opções a seguir são ativadas por padrão. É possível selecionar uma ou mais das seguintes configurações:</p> 
    <ul> 
     <li> <p><strong>Todas as noites</strong>: Selecione essa opção para recalcular as linhas do tempo do projeto todas as noites. Quaisquer alterações feitas no projeto que possam afetar a linha do tempo não estarão imediatamente visíveis. O Workfront ​ ​ recalcula as linhas do tempo da noite somente para projetos em que ambas as condições a seguir são atendidas:</p> <p> 
       <ul> 
        <li>Ter um status de Atual</li> 
        <li>Tiveram uma atualização nos últimos 3 meses</li> 
       </ul> </p> </li> 
     <li> <p><strong>Quando o escopo de um projeto é alterado</strong>: Selecione essa opção para recalcular as linhas do tempo do projeto imediatamente, conforme ocorre uma alteração no escopo do projeto. Para obter informações sobre o que constitui uma alteração no escopo do projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular linhas do tempo do projeto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Quando vários usuários forem atribuídos a uma tarefa, use o agendamento da variável</strong> </p> </td> 
   <td> <p>Se um projeto não tiver um agendamento atribuído ou se os usuários atribuídos a suas tarefas não tiverem um Agendamento atribuído a eles, o Workfront usará o agendamento padrão do sistema para calcular a linha do tempo das tarefas.</p> <p>Se você atribuir vários usuários à mesma tarefa em um projeto tiver um agendamento atribuído, e os usuários atribuídos às tarefas também tiverem um agendamento atribuído a eles, o Workfront usará os seguintes agendamentos:</p> 
    <ul> 
     <li><strong>Atribuição principal</strong>: O Workfront usa o agendamento da Atribuição primária na tarefa para calcular linhas do tempo.</li> 
     <li><strong>Projeto</strong>: O Workfront usa o agendamento do projeto para calcular a linha do tempo de cada tarefa.</li> 
    </ul> <p>Para obter mais informações sobre programações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Criar um agendamento</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Cálculos de linha do tempo </p> </td> 
   <td> 
    <ul> 
     <li><strong>Horas típicas por dia de trabalho</strong>: Defina o número de horas em um dia de trabalho típico para os usuários que trabalharão em projetos. O padrão é 8 horas.</li> 
    </ul> 
    <ul> 
     <li><strong>Dias normais de trabalho por semana</strong>: Defina a semana de trabalho padrão para os usuários que trabalharão em projetos. O padrão é 5 dias.</li> 
    </ul> <p>Essas 2 opções convertem dias em horas ou semanas em dias.</p> <p>Por exemplo, se você tiver uma tarefa com 8 Horas Planejadas e a duração for calculada com base nas Horas Planejadas, o Workfront converterá essas horas em dias para mostrar a Duração como dias.</p> <p>No campo Typical work days per week , a Workfront calcula o valor Full Time Equivalent (FTE) para seu sistema. É o que o Workfront usa ao calcular alocações para usuários.</p> <p>Esses valores são usados quando você está planejando linhas do tempo dos projetos, orçando recursos ou registrando tempo em projetos. </p> <p>Eles não são usados ao estabelecer folhas de horas para usuários no sistema, conforme descrito em <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Configurar preferências de hora e folha de ponto</a>.</p> <p><b>OBSERVAÇÃO</b>: Os administradores do Workfront não podem desbloquear as preferências de Cálculos de Linha do Tempo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Trimestres personalizados</strong> </p> </td> 
   <td> <p>Configure trimestres anuais personalizados para os usuários que trabalharão em projetos. Os trimestres personalizados são normalmente trimestres que não correspondem à discriminação tradicional de trimestres durante um ano civil. Você pode adicionar vários trimestres personalizados. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Habilitar trimestres personalizados para projetos</a>.</p> <p><b>OBSERVAÇÃO</b>: Os administradores do Workfront não podem desbloquear as preferências de Trimestres personalizados.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Casos de negócio {#business-cases}

Você pode criar um Caso de negócios para projetos recém-criados associados ao grupo para enviar solicitações de projeto. É possível definir preferências para determinar quais áreas estão visíveis na variável **Caso de negócios** formulário. Recomendamos que você ative essas opções para que outras ferramentas, como o Portfolio Otimizer, sejam atualizadas corretamente. Para obter mais informações sobre o que cada campo exibe, consulte [Definir um caso de negócios](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Depois que o administrador do Workfront ativar as seções no Caso de negócios, um Proprietário do projeto poderá criar um Caso de negócios no nível do projeto. Para obter informações sobre como criar um Caso de Negócios, consulte [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Vida após a morte  {#life-after-death}

Configure qualquer uma das preferências a seguir para projetos recém-criados associados ao grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Depois que um projeto é marcado como Concluído, as pessoas ainda podem</strong> </p> </td> 
   <td> <p>Determine as regras para sua organização (ou grupo, se estiver configurando preferências de projeto para um grupo) sobre se uma tarefa ou um problema pode ser excluído depois que o status do projeto for marcado como Concluído.</p> 
    <ul> 
     <li><strong>Excluir Tarefas</strong>: Permite que os usuários excluam tarefas de um projeto depois que ele é marcado como Concluído.<br></li> 
     <li><strong>Excluir problemas</strong>: Permite que os usuários excluam problemas de um projeto depois que ele é marcado como Concluído.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Depois que um projeto é marcado como Concluído, Inativo ou Pendente na aprovação, as pessoas ainda podem</strong> </p> </td> 
   <td> <p>Determine as regras de sua organização (ou grupo, se estiver configurando as preferências do projeto para um grupo) em relação ao que acontece com tarefas, problemas, documentos e outros objetos em um projeto após o status do projeto ter sido marcado <strong>Concluído</strong>, <strong>Morto</strong>ou é <strong>Aprovação pendente</strong>.</p> 
    <ul> 
     <li><strong>Adicionar e editar tarefas</strong> Permite aos usuários: 
      <ul> 
       <li>Edite as tarefas em um projeto depois que ele tiver sido marcado como Concluído, Adiado ou Pendente na aprovação. Isso inclui adicionar horas e alterar entradas de despesas em uma tarefa.</li> 
       <li>Adicionar tarefas a um projeto.</li> 
      </ul></li> 
     <li><strong>Adicionar e editar problemas</strong>: Permite aos usuários: 
      <ul> 
       <li>Edite problemas em um projeto depois que o projeto for marcado como Concluído, Adiado ou Aprovação pendente.</li> 
       <li>Adicione problemas a um projeto depois que ele for marcado como Concluído ou Inativo. (Não é possível adicionar problemas a um projeto que esteja com Aprovação pendente.)</li> 
      </ul></li> 
     <li> <p><strong>Adicionar documentos ao projeto e às suas tarefas e problemas</strong>: Permite que os usuários adicionem documentos a um projeto (ou adicionem documentos a tarefas e problemas dentro do projeto) após o projeto ter sido marcado como Concluído ou Inativo.</p> <p>Essa opção não se aplica a projetos que estão pendentes de aprovação.</p> </li> 
     <li> <p><strong>Anexar modelos</strong>: Permite que os usuários anexem modelos a um projeto depois que o projeto é marcado como Concluído ou Inativo.</p> <p>Essa opção não se aplica a projetos que estão pendentes de aprovação.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
