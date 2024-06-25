---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurar preferências de projeto em todo o sistema
description: Como um [!DNL Adobe Workfront] administrador, você pode configurar as preferências padrão para todos os projetos criados no sistema. Essas preferências afetam o comportamento do projeto, tarefa e problema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 93a2630ec5c21f03643a29a8730046c8458c795f
workflow-type: tm+mt
source-wordcount: '2561'
ht-degree: 0%

---

# Configurar preferências de projeto em todo o sistema

<!--Audited: 12/2023-->

Como um [!DNL Adobe Workfront] administrador, você pode configurar as preferências padrão para todos os projetos criados no sistema. Essas preferências afetam o comportamento do projeto, tarefa e problema.

>[!NOTE]
>
>Por padrão, essas preferências estão bloqueadas e os administradores de grupo não podem modificá-las no nível do grupo, a menos que você as desbloqueie para todos os grupos no sistema. Para obter mais informações, consulte [Bloquear ou desbloquear as preferências do projeto para todos os grupos no sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plano</p></td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Novo: [!UICONTROL Padrão]</p>
   Ou
   <p>Atual: [!UICONTROL Plano]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>[!UICONTROL Administrador do Sistema]</p> <p><b>NOTA</b>:</p><p>Se você ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurar as preferências do projeto para toda a organização

{{step-1-to-setup}}

1. No painel esquerdo, clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Projetos]**.

1. No **Preferências do projeto** continue com uma das 4 seções listadas abaixo para configurar preferências para [!UICONTROL Status do projeto], [!UICONTROL Linhas de Tempo], [!UICONTROL Casos de negócios], e [!UICONTROL Vida após a morte].
1. Se quiser que todos os grupos da organização usem as mesmas preferências de projeto, verifique se cada preferência está bloqueada ![](assets/lock-toggle-button.png) (esse é o padrão).

   >[!IMPORTANT]
   >
   >Quando uma preferência de projeto está bloqueada, as alterações feitas nessa preferência são herdadas por todos os grupos no sistema. É importante se comunicar com os usuários e grupos em toda a organização para garantir que todas as necessidades sejam levadas em conta na maneira como você configura as preferências do projeto.

   Para obter informações sobre como desbloquear uma preferência para que todos os grupos possam configurá-la e gerenciá-la por conta própria, consulte [Bloquear ou desbloquear as preferências do projeto para todos os grupos no sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Clique em **[!UICONTROL Salvar]**.

* [[!UICONTROL Status do projeto]](#project-status)
* [[!UICONTROL Linhas de Tempo]](#timelines)
* [[!UICONTROL Casos de negócios]](#business-cases)
* [[!UICONTROL Vida após a morte]](#life-after-death)

### Status do projeto {#project-status}

Configure qualquer uma das seguintes preferências para projetos recém-criados em todo o sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permitir que usuários criem projetos sem usar um modelo]</td> 
   <td>  <p>Esta preferência permite que os usuários criem projetos sem usar um modelo ao criar um projeto das seguintes áreas: </p>
      <ul>
        <li>
        <p>Usar a opção [!UICONTROL Novo Projeto] em uma lista de projetos</p>
        </li>
          <li>
          <p>Converter um problema em um projeto a partir da página do problema</p>
          </li>
         </ul>
        <p>Essa preferência é ativada por padrão. </p> 
        <p><b>Nota</b></p>
        <p> Um administrador de grupo pode alterar essa preferência por um grupo. Quando um usuário pertence a vários grupos com preferências diferentes, ele pode criar um projeto sem um modelo se o Grupo padrão tiver essa preferência ativada.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Definir status do novo projeto como]</td> 
   <td> <p>Determine o status dos novos projetos.</p>  <p><b>NOTA</b>  
     <ul> 
      <li>Se você ou outro [!DNL Workfront] administrator oculta o status selecionado aqui, o status padrão muda para o primeiro status na lista de status.</li> 
     </ul> 
     <ul> 
      <li> <p>Se o status de um sistema ou grupo bloqueado for definido como o status padrão e depois alguém o desbloquear, o sistema tentará substituí-lo por um status bloqueado do mesmo tipo de status.</p> <p>Se não conseguir encontrar um, ele procurará um status obrigatório:</p> 
       <ul> 
        <li>Se houver um status obrigatório igual ao status padrão desbloqueado, o status obrigatório se tornará o status padrão, mesmo se ele estiver desbloqueado.</li> 
        <li>Se nenhum dos status obrigatórios for igual ao status padrão desbloqueado, o primeiro status obrigatório na lista de status se tornará o status padrão.</li> 
       </ul> <p>Para obter informações sobre os status obrigatórios, consulte os artigos <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de projeto do sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de tarefas do sistema</a>, e <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de problemas do sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calcular percentual concluído com base em]</td> 
   <td> <p>O Workfront calcula o percentual concluído de um projeto ou tarefa pai usando o percentual concluído de cada tarefa no projeto e a Duração ou as Horas planejadas de cada tarefa.</p><p>O percentual concluído de cada tarefa é definido manualmente pelos atribuídos da tarefa.</p><p>Você pode selecionar aqui se o Workfront usará a duração ou o planejamento de horas de tarefas para calcular o percentual concluído dos projetos.</p> <p>Se você selecionar [!UICONTROL Duração], a Duração de cada tarefa em um projeto determinará o percentual de conclusão geral do projeto, e a Duração de cada subtarefa determinará o percentual de conclusão geral de sua tarefa pai.</p> <p>Se você selecionar [!UICONTROL Duração], especifique as [!UICONTROL Horas típicas por dia de trabalho] e [!UICONTROL Dias de trabalho típicos por semana] na seção [!UICONTROL Linhas do tempo]. [!DNL Workfront] O usa essas informações ao calcular o percentual concluído de uma tarefa com base na Duração. </p> <p>Se você selecionar [!UICONTROL Horas Planejadas], certifique-se de que todas as tarefas em cada projeto tenham a quantidade de [!UICONTROL Horas Planejadas] definida, e que a quantidade não seja zero.</p><p>Para obter mais informações, consulte <a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md">Visão geral do Percentual de Término do Projeto</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Definir automaticamente a Condição do projeto com base no Status de Progresso]</td> 
   <td> <p>Esta preferência permite que os usuários definam a [!UICONTROL Condição] de um projeto manualmente como ([!UICONTROL No Destino], [!UICONTROL Em Risco], [!UICONTROL Em Problema]) ou [!DNL Workfront] Defina a [!UICONTROL Condição] (Status do Progresso) automaticamente com base na progressão do projeto na linha do tempo. Para obter mais informações sobre a condição dos projetos, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Visão geral da condição do projeto e do tipo de condição</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criar linhas de base automaticamente]</p> </td> 
   <td> <p>Esta preferência cria automaticamente uma linha de base (instantâneo) dos detalhes da tarefa e do projeto quando o status do projeto muda para [!UICONTROL Atual]. Para obter informações sobre como criar linhas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Criar linhas de base do projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método de Índice de Desempenho] </p> </td> 
   <td> <p>O Método Índice de desempenho (PIM) do projeto controla o método [!DNL Workfront] O usa o para calcular métricas de Valor Agregado, como o [!UICONTROL Índice de Desempenho de Custo] (CPI) e o [!UICONTROL Estimar Na Conclusão] (EAC). Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcular [!UICONTROL Índice de Desempenho de Custo] (CPI)</a> e <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calcular Estimativa na Conclusão] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Baseado em Hora]</strong>: [!DNL Workfront] usa [!UICONTROL Horas planejadas] para calcular métricas de desempenho como EAC e CPI. Quando o PIM é calculado com base nas horas, o EAC é exibido como um número de horas. Verifique se você tem um valor diferente de zero para [!UICONTROL Planned Hours].</li> 
     <li> <p><strong>[!UICONTROL Baseado em Custo]</strong>: [!DNL Workfront] usa o [!UICONTROL Custo de Trabalho Planejado] para calcular métricas de desempenho como EAC e CPI. Verifique se suas funções de trabalho ou usuários estão associados às taxas de Custo por hora. Quando o PIM é calculado com base nos Custos, o EAC é exibido como um valor de moeda.</p> <p>O gerente de projeto pode modificar essa configuração no nível do projeto, usando a área [!UICONTROL Finanças] no [!UICONTROL Detalhes do Projeto]. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gerenciar informações na área do projeto [!UICONTROL Finanças]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimativa no Término ]</p> </td> 
   <td> <p>Determinar quais dados [!DNL Workfront] O usa o para calcular a EAC [!UICONTROL Estimativa no Término], que representa o custo total projetado de um projeto.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calcular no nível do projeto]</strong>: EAC da tarefa pai e do projeto são determinados inserindo [!UICONTROL Horas Reais] ou [!UICONTROL Custo Real do Trabalho] nas Fórmulas EAC. Este cálculo inclui [!UICONTROL Horas efetivas] ou [!UICONTROL Custos e despesas] adicionados diretamente à tarefa ou projeto pai.</li> 
     <li> <p><strong>[!UICONTROL Extrair de tarefas/subtarefas]</strong>: a EAC da tarefa pai e do projeto é determinada pela soma da EAC de cada tarefa filho. Este cálculo exclui [!UICONTROL Horas Reais] ou [!UICONTROL Custos e Despesas Reais] adicionadas diretamente à tarefa ou projeto pai.</p> <p>O gerente de projeto pode modificar essa configuração no nível do projeto, usando a área [!UICONTROL Finanças] em [!UICONTROL Detalhes do Projeto].Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gerenciar informações na área do projeto [!UICONTROL Finanças]</a>.</p> </li> 
    </ul> <p>Para obter mais informações sobre como o EAC é calculado, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular [!UICONTROL Estimativa no Término] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Linhas de Tempo {#timelines}

Configure qualquer uma das seguintes preferências para projetos recém-criados em todo o sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agendar De]</td> 
   <td> <p>Determine se os novos projetos estão programados a partir da Data inicial ou da Data de conclusão quando são criados.</p> 
    <ul> 
     <li><strong>[!UICONTROL Data de Início]</strong>: novas tarefas padrão para a [!UICONTROL Assim que Possível] Restrição de Tarefa e os gerentes de projeto são solicitados a fornecer uma [!UICONTROL Data de Início Planejada] para o projeto.</li> 
     <li><strong>[!UICONTROL Data de conclusão]</strong>: Novas tarefas padrão para a [!UICONTROL O Mais Tarde Possível] Restrição de Tarefa e os gerentes de projeto são solicitados a fornecer uma [!UICONTROL Data de Conclusão Planejada] para o projeto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tempo de folga do usuário]</td> 
   <td> <p>Determine se o tempo de folga do Principal responsável por uma tarefa ajusta as datas planejadas para essa tarefa em um projeto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Considerar o tempo de folga do usuário nas durações de tarefas]</strong>: qualquer folga programada para o Principal responsável de uma tarefa ajusta as datas planejadas da tarefa se a folga ocorrer durante a duração da tarefa. Esta é a configuração padrão. </p> <p>Por exemplo, se uma tarefa com uma Restrição de [!UICONTROL Assim que Possível] estiver programada para iniciar em 1º de junho e terminar em 3 de junho, e o Destinatário principal tiver o dia 2 de junho marcado para Folga, as datas planejadas da tarefa serão ajustadas de 1º de junho a 4 de junho.</p> <p><b>IMPORTANTE</b>:</p> <p>A duração da tarefa não é alterada ao selecionar essa configuração. Somente as datas planejadas mudam, dependendo da Restrição da Tarefa.</p> </li> 
     <li><strong>[!UICONTROL Ignorar tempo de folga do usuário nas durações de tarefas]</strong>: as datas planejadas de cada tarefa em um projeto permanecem como planejadas originalmente, mesmo que o Destinatário principal de uma tarefa tenha uma folga durante sua duração.</li> 
    </ul> <p>Considere o seguinte ao selecionar opções para essa configuração:</p> 
    <ul> 
     <li>Quando você altera essa configuração, somente os projetos e modelos criados após a alteração herdam a configuração atualizada. </li> 
     <li> <p>O valor Restrição da Tarefa determina quais datas da tarefa planejada devem ser ajustadas: </p> 
      <ul> 
       <li>A data de início planejada</li> 
       <li>A data de conclusão planejada</li> 
       <li>Ambas as datas</li> 
       <li>Nenhuma data. </li> 
      </ul> <p>Por exemplo, se uma tarefa tiver uma Restrição de [!UICONTROL Datas Fixas], as datas não serão ajustadas quando o Destinatário Principal tiver folga, mesmo se a opção [!UICONTROL Considerar folga do usuário na duração da tarefa] estiver selecionada. Para obter informações sobre restrições de tarefa, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Visão geral de Restrição de Tarefa</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL As linhas do tempo do projeto são recalculadas automaticamente]</p> </td> 
   <td> <p>Determine quando a linha do tempo de um projeto é recalculada. Para obter informações sobre como recalcular a linha do tempo do projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular linhas do tempo do projeto</a>.</p> <p>As opções a seguir são ativadas por padrão. Você pode selecionar uma ou mais das seguintes configurações:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Todas as noites]</strong>: selecione esta opção para recalcular as linhas do tempo do projeto todas as noites. Quaisquer alterações feitas no projeto que possam afetar a linha do tempo não ficam visíveis imediatamente. [!DNL Workfront​​​] recalcula as linhas do tempo à noite somente para projetos em que ambas as condições a seguir sejam atendidas:</p> <p> 
       <ul> 
        <li>Tem um status de [!UICONTROL Atual]</li> 
        <li>Teve uma atualização nos últimos 3 meses</li> 
        <li>Tiverem um Tipo de atualização de um dos seguintes:</li>
        <ul>
        <li>Automático e Mediante alteração</li>
        <li>Somente mediante alteração</li>
        <li>Somente automática</li> 
      </ul>       
    <b>DICA:</b>
    <p>Projetos que possuem um tipo de atualização Somente manual não são afetados por essa configuração.</p>
    <li> <p><strong>Quando o escopo de um projeto é alterado</strong>: selecione esta opção para recalcular as linhas do tempo do projeto imediatamente quando ocorrer uma alteração no escopo do projeto. Para obter informações sobre o que constitui uma alteração de escopo de projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular linhas do tempo do projeto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Quando vários usuários são atribuídos a uma tarefa, use o agendamento de]</p> </td> 
   <td> <p>Se um projeto não tiver um agendamento atribuído ou se os usuários atribuídos às suas tarefas não tiverem um Agendamento atribuído a eles, [!DNL Workfront] usa o agendamento padrão do sistema para calcular a linha do tempo das tarefas.</p> <p>Se você atribuir vários usuários à mesma tarefa em um projeto e o projeto tiver um agendamento atribuído e os usuários atribuídos às tarefas também tiverem um agendamento atribuído a eles, a [!UICONTROL Workfront] usará os seguintes agendamentos:</p> 
    <ul> 
     <li><strong>[!UICONTROL Atribuição Principal]</strong>: [!DNL Workfront] usa a programação da Atribuição principal na tarefa para calcular linhas do tempo.</li> 
     <li><strong>[!UICONTROL Projeto]</strong>: [!DNL Workfront] O usa o cronograma do projeto para calcular a linha do tempo de cada tarefa.</li> 
    </ul> <p>Para obter mais informações sobre cronogramas, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Criar um agendamento</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Cálculos de Linha do Tempo] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Horas típicas por dia de trabalho]</strong>: Defina o número de horas em um dia de trabalho típico para os usuários que trabalharão nos projetos. O padrão é 8 horas.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Dias de trabalho típico por semana]</strong>: Defina a semana de trabalho padrão para os usuários que estão trabalhando em projetos. O padrão é 5 dias.</li> 
    </ul> <p>Essas 2 opções convertem dias em horas ou semanas em dias.</p> <p>Por exemplo, se você tiver uma tarefa com 8 Horas planejadas e a duração for calculada com base nas Horas planejadas, [!DNL Workfront] O converte essas horas em dias para mostrar a Duração como dias.</p> <p>No campo Typical [!UICONTROL work days per week] (Dias de trabalho típicos por semana do UICONTROL), [!DNL Workfront] O calcula o valor de FTE (equivalente a tempo integral) do seu sistema. Isso é o que [!DNL Workfront] O usa o ao calcular alocações para usuários.</p> <p>Esses valores são usados quando você está planejando cronogramas de projetos, orçamento de recursos ou registro de tempo em projetos. </p> <p>Eles não são usados quando você está estabelecendo folhas de horas para usuários no sistema, conforme descrito em <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Preferências de horas e folha de horas da [!UICONTROL Configurar]</a>.</p> <p><b>NOTA</b>:</p> <p>[!DNL Workfront] os administradores não podem desbloquear as preferências de [!UICONTROL Cálculos de linha do tempo].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Trimestres Personalizados]</p> </td> 
   <td> <p>Configure trimestres anuais personalizados para os usuários que trabalharão nos projetos. Os trimestres personalizados geralmente são trimestres que não correspondem ao detalhamento tradicional de trimestres durante um ano civil. Você pode adicionar vários trimestres personalizados. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Habilitar trimestres personalizados para projetos</a>.</p>  <p><b>NOTA</b>: </p><p>[!DNL Workfront] Os administradores não podem desbloquear as preferências de [!UICONTROL Custom Quarters].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Casos de negócios] {#business-cases}

Você pode criar um Business Case para projetos recém-criados em todo o sistema para enviar solicitações de projeto. É possível definir preferências para determinar quais áreas ficam visíveis na **[!UICONTROL Business Case]** formulário. Recomendamos ativar essas opções para que outras ferramentas, como o [!UICONTROL Otimizador de Portfolio], atualize corretamente. Para obter mais informações sobre o que cada campo exibe, consulte [Definir um Business Case: índice do artigo](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Depois que a variável [!DNL Workfront] o administrador habilita as seções no [!UICONTROL Business Case], um Proprietário do projeto pode criar um Business Case no nível do projeto. Para obter informações sobre como criar um Business Case, consulte [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Vida após a morte] {#life-after-death}

Configure qualquer uma das seguintes preferências para projetos recém-criados em todo o sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Depois que um projeto for marcado como Concluído, as pessoas ainda poderão] </p> </td> 
   <td> <p>Determine as regras da organização (ou grupo, se estiver configurando preferências de projeto para um grupo) em relação à possibilidade de exclusão de uma tarefa ou problema após a marcação do status do projeto como [!UICONTROL Concluído].</p> 
    <ul> 
     <li><strong>[!UICONTROL Excluir Tarefas]</strong>: permite que usuários excluam tarefas de um projeto depois que o projeto for marcado como [!UICONTROL Concluído].<br></li> 
     <li><strong>[!UICONTROL Excluir Problemas]</strong>: permite que usuários excluam problemas de um projeto depois que o projeto for marcado como [!UICONTROL Concluído].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Depois que um projeto é marcado como Concluído, Desativado ou com Aprovação pendente, as pessoas ainda podem]</p> </td> 
   <td> <p>Determine as regras para sua organização (ou grupo, se estiver configurando preferências de projeto para um grupo) em relação ao que acontece com tarefas, problemas, documentos e outros objetos em um projeto depois que o status do projeto é marcado <strong>[!UICONTROL Concluído]</strong>, <strong>[!UICONTROL Desativado]</strong>, ou é <strong>[!UICONTROL Pendente de Aprovação]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Adicionar e editar tarefas]</strong> Permite que os usuários:
      <ul>
       <li>Editar tarefas em um projeto depois que o projeto estiver marcado como [!UICONTROL Concluído], [!UICONTROL Desativado] ou estiver [!UICONTROL com Aprovação Pendente]. Isso inclui adicionar horas e alterar entradas de despesas em uma tarefa.</li>
       <li>Adicionar tarefas a um projeto.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Adicionar e editar problemas]</strong>: permite aos usuários:
      <ul>
       <li>Editar problemas em um projeto depois que ele for marcado como [!UICONTROL Concluído], [!UICONTROL Desativado] ou [!UICONTROL Com Aprovação Pendente].</li>
       <li>Adicionar problemas a um projeto depois que o projeto for marcado como [!UICONTROL Concluído] ou [!UICONTROL Desativado]. (Você não pode adicionar problemas a um projeto que esteja [!UICONTROL Pendente de Aprovação].)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Adicionar documentos ao projeto e às suas tarefas e problemas]</strong>: permite que os usuários adicionem documentos a um projeto (ou adicionem documentos a tarefas e problemas dentro do projeto) depois que o projeto for marcado como [!UICONTROL Concluído] ou [!UICONTROL Desativado].</p> <p>Essa opção não se aplica a projetos com aprovação pendente.</p> </li> 
     <li> <p><strong>[!UICONTROL Anexar modelos]</strong>: permite que os usuários anexem modelos a um projeto depois que o projeto for marcado como [!UICONTROL Concluído] ou [!UICONTROL Desativado].</p> <p>Essa opção não se aplica a projetos com aprovação pendente.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
