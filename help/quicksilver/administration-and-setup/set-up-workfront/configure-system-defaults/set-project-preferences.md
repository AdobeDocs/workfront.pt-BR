---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurar Preferências de Projeto do Sistema
description: Como administrador  [!DNL Adobe Workfront] , você pode configurar as preferências padrão para todos os projetos criados no sistema. Essas preferências afetam o comportamento do projeto, tarefa e problema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 90405d79f605d788331cb7a04ebf354dc4379bf5
workflow-type: tm+mt
source-wordcount: '2693'
ht-degree: 1%

---

# Configurar preferências de projeto em todo o sistema

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Como administrador do [!DNL Adobe Workfront], você pode configurar as preferências padrão para todos os projetos criados no sistema. Essas preferências afetam o comportamento do projeto, tarefa e problema.

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
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar as preferências do projeto para toda a organização

{{step-1-to-setup}}

1. No painel esquerdo, clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Projetos]**.

1. Na página **Preferências do Projeto**, continue com uma das 4 seções listadas abaixo para configurar as preferências de [!UICONTROL Status do Projeto], [!UICONTROL Linhas do Tempo], [!UICONTROL Casos de Negócios] e [!UICONTROL Vida após a Morte].
1. Se desejar que todos os grupos da organização usem as mesmas preferências de projeto, verifique se cada preferência está bloqueada ![](assets/lock-toggle-button.png) (esse é o padrão).

   >[!IMPORTANT]
   >
   >Quando uma preferência de projeto está bloqueada, as alterações feitas nessa preferência são herdadas por todos os grupos no sistema. É importante se comunicar com os usuários e grupos em toda a organização para garantir que todas as necessidades sejam levadas em conta na maneira como você configura as preferências do projeto.

   Para obter informações sobre como desbloquear uma preferência para que todos os grupos possam configurá-la e gerenciá-la sozinhos, consulte [Bloquear ou desbloquear preferências de projeto para todos os grupos no sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Clique em **[!UICONTROL Salvar]**.

* [[!UICONTROL Status do projeto]](#project-status)
* [[!UICONTROL Linhas de Tempo]](#timelines)
* [[!UICONTROL Casos de negócio]](#business-cases)
* [[!UICONTROL Vida após a Morte]](#life-after-death)

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
   <td> <p>Determine o status dos novos projetos.</p>  <p><b>OBSERVAÇÃO</b>  
     <ul> 
      <li>Se você ou outro administrador do [!DNL Workfront] ocultar o status selecionado aqui, o status padrão será alterado para o primeiro status na lista de status.</li> 
     </ul> 
     <ul> 
      <li> <p>Se o status de um sistema ou grupo bloqueado for definido como o status padrão e depois alguém o desbloquear, o sistema tentará substituí-lo por um status bloqueado do mesmo tipo de status.</p> <p>Se não conseguir encontrar um, ele procurará um status obrigatório:</p> 
       <ul> 
        <li>Se houver um status obrigatório igual ao status padrão desbloqueado, o status obrigatório se tornará o status padrão, mesmo se ele estiver desbloqueado.</li> 
        <li>Se nenhum dos status obrigatórios for igual ao status padrão desbloqueado, o primeiro status obrigatório na lista de status se tornará o status padrão.</li> 
       </ul> <p>Para obter informações sobre os status necessários, consulte os artigos <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de projetos do sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de tarefas do sistema</a> e <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de problemas do sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calcular percentual concluído com base em]</td> 
   <td> <p>O Workfront calcula o percentual concluído de um projeto ou tarefa pai usando o percentual concluído de cada tarefa no projeto e a Duração ou as Horas planejadas de cada tarefa.</p><p>O percentual concluído de cada tarefa é definido manualmente pelos atribuídos da tarefa.</p><p>Você pode selecionar aqui se o Workfront usará a duração ou o planejamento de horas de tarefas para calcular o percentual concluído dos projetos.</p> <p>Se você selecionar [!UICONTROL Duração], a Duração de cada tarefa em um projeto determinará o percentual de conclusão geral do projeto, e a Duração de cada subtarefa determinará o percentual de conclusão geral de sua tarefa pai.</p> <p>Se você selecionar [!UICONTROL Duração], especifique as [!UICONTROL Horas típicas por dia de trabalho] e [!UICONTROL Dias de trabalho típicos por semana] na seção [!UICONTROL Linhas do tempo]. [!DNL Workfront] usa essas informações ao calcular o percentual concluído de uma tarefa com base na Duração. </p> <p>Se você selecionar [!UICONTROL Horas Planejadas], certifique-se de que todas as tarefas em cada projeto tenham a quantidade de [!UICONTROL Horas Planejadas] definida, e que a quantidade não seja zero.</p><p>Para obter mais informações, consulte <a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md">Visão geral da Porcentagem Concluída do Projeto</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Definir automaticamente a Condição do projeto com base no Status de Progresso]</td> 
   <td> <p>Essa preferência permite que os usuários definam manualmente a [!UICONTROL Condição] de um projeto como ([!UICONTROL No Destino], [!UICONTROL Em Risco], [!UICONTROL Em Problema]) ou que [!DNL Workfront] defina a [!UICONTROL Condição] (Status de Progresso) automaticamente com base na progressão do projeto na linha do tempo. Para obter mais informações sobre a Condição de projetos, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Visão Geral da Condição de Projeto e Tipo de Condição</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criar linhas de base automaticamente]</p> </td> 
   <td> <p>Esta preferência cria automaticamente uma linha de base (instantâneo) dos detalhes da tarefa e do projeto quando o status do projeto muda para [!UICONTROL Atual]. Para obter informações sobre como criar linhas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Criar linhas de base do projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método de Índice de Desempenho] </p> </td> 
   <td> <p>O Método de Índice de Desempenho (PIM) do projeto controla o método [!DNL Workfront] usado para calcular métricas de Valor Agregado, como o [!UICONTROL Índice de Desempenho de Custo] (CPI) e o [!UICONTROL Estimar Na Conclusão] (EAC). Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcular [!UICONTROL Índice de Desempenho de Custo] (CPI)</a> e <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calcular Estimativa na Conclusão] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL baseado em Hora]</strong>: [!DNL Workfront] usa [!UICONTROL Horas Planejadas] para calcular métricas de desempenho como EAC e CPI. Quando o PIM é calculado com base nas horas, o EAC é exibido como um número de horas. Verifique se você tem um valor diferente de zero para [!UICONTROL Planned Hours].</li> 
     <li> <p><strong>[!UICONTROL Custo-baseado]</strong>: [!DNL Workfront] usa [!UICONTROL Custo de Trabalho Planejado] para calcular métricas de desempenho como EAC e CPI. Verifique se suas funções de trabalho ou usuários estão associados às taxas de Custo por hora. Quando o PIM é calculado com base nos Custos, o EAC é exibido como um valor de moeda.</p> <p>O gerente de projeto pode modificar essa configuração no nível do projeto, usando a área [!UICONTROL Finanças] no [!UICONTROL Detalhes do Projeto]. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gerenciar informações na área do projeto [!UICONTROL Finance]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimativa no Término ]</p> </td> 
   <td> <p>Determine quais dados [!DNL Workfront] usa para calcular a [!UICONTROL Estimativa no Término] (EAC) que representa o custo total projetado de um projeto.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calcular no nível do projeto]</strong>: EAC da tarefa pai e do projeto são determinados pela inserção de [!UICONTROL Horas Reais] ou [!UICONTROL Custo Real do Trabalho] nas Fórmulas EAC. Este cálculo inclui [!UICONTROL Horas efetivas] ou [!UICONTROL Custos e despesas] adicionados diretamente à tarefa ou projeto pai.</li> 
     <li> <p><strong>[!UICONTROL Roll-up from tasks/subtasks]</strong>: EAC da tarefa pai e do projeto são determinados pela soma de EAC de cada tarefa filho. Este cálculo exclui [!UICONTROL Horas Reais] ou [!UICONTROL Custos e Despesas Reais] adicionadas diretamente à tarefa ou projeto pai.</p> <p>O gerente de projeto pode modificar essa configuração no nível do projeto, usando a área [!UICONTROL Finanças] em [!UICONTROL Detalhes do Projeto].Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gerenciar informações na área do projeto [!UICONTROL Finanças]</a>.</p> </li> 
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
     <li><strong>[!UICONTROL Data de Início]</strong>: Novas tarefas padrão para [!UICONTROL Assim que Possível] Restrição de Tarefa e gerentes de projeto são solicitados a fornecer uma [!UICONTROL Data de Início Planejada] para o projeto.</li> 
     <li><strong>[!UICONTROL Data de Conclusão]</strong>: Novas tarefas padrão para a [!UICONTROL O Mais Tarde Possível] Restrição de Tarefa e gerentes de projeto são solicitados a fornecer uma [!UICONTROL Data de Conclusão Planejada] para o projeto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tempo de folga do usuário]</td> 
   <td> <p>Determine se o tempo de folga do Principal responsável por uma tarefa ajusta as datas planejadas para essa tarefa em um projeto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Considerar o tempo de folga do usuário nas durações da tarefa]</strong>: qualquer tempo de folga agendado para o Principal Atribuidor de uma tarefa ajusta as datas planejadas da tarefa se o tempo de folga ocorrer durante a duração da tarefa. Esta é a configuração padrão. </p> <p>Por exemplo, se uma tarefa com uma Restrição de [!UICONTROL Assim que Possível] estiver programada para iniciar em 1º de junho e terminar em 3 de junho, e o Destinatário principal tiver o dia 2 de junho marcado para Folga, as datas planejadas da tarefa serão ajustadas de 1º de junho a 4 de junho.</p> <p><b>IMPORTANTE</b>:</p> <p>A duração da tarefa não é alterada ao selecionar essa configuração. Somente as datas planejadas mudam, dependendo da Restrição da Tarefa.</p> </li> 
     <li><strong>[!UICONTROL Ignorar o tempo de folga do usuário nas durações de tarefas]</strong>: as datas planejadas de cada tarefa em um projeto permanecem como originalmente planejado, mesmo que o Destinatário Principal de uma tarefa tenha folga durante sua duração.</li> 
    </ul> <p>Considere o seguinte ao selecionar opções para essa configuração:</p> 
    <ul> 
     <li>Quando você altera essa configuração, somente os projetos e modelos criados após a alteração herdam a configuração atualizada. </li> 
     <li> <p>O valor Restrição da Tarefa determina quais datas da tarefa planejada devem ser ajustadas: </p> 
      <ul> 
       <li>A data de início planejada</li> 
       <li>A data de conclusão planejada</li> 
       <li>Ambas as datas</li> 
       <li>Nenhuma data. </li> 
      </ul> <p>Por exemplo, se uma tarefa tiver uma Restrição de [!UICONTROL Datas Fixas], as datas não serão ajustadas quando o Destinatário Principal tiver folga, mesmo se a opção [!UICONTROL Considerar folga do usuário na duração da tarefa] estiver selecionada. Para obter informações sobre restrições de tarefa, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Visão geral da Restrição de Tarefa</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL As linhas do tempo do projeto são recalculadas automaticamente]</p> </td> 
   <td> <p>Determine quando a linha do tempo de um projeto é recalculada. Para obter informações sobre como recalcular a linha de tempo do projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular linhas de tempo do projeto</a>.</p> <p>As opções a seguir são ativadas por padrão. Você pode selecionar uma ou mais das seguintes configurações:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Toda noite]</strong>: selecione esta opção para recalcular as linhas do tempo do projeto todas as noites. Quaisquer alterações feitas no projeto que possam afetar a linha do tempo não ficam visíveis imediatamente. [!DNL Workfront​​​] recalcula as linhas de tempo à noite somente para projetos em que ambas as condições a seguir sejam atendidas:</p> <p> 
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
    <li> <p><strong>Quando o escopo de um projeto for alterado</strong>: selecione esta opção para recalcular as linhas de tempo do projeto imediatamente, à medida que ocorrer uma alteração no escopo do projeto. Para obter informações sobre o que constitui uma alteração de escopo de projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular linhas do tempo do projeto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Quando vários usuários são atribuídos a uma tarefa, use o agendamento de]</p> </td> 
   <td> <p>Se um projeto não tiver um agendamento atribuído ou se os usuários atribuídos às suas tarefas não tiverem um Agendamento atribuído a eles, [!DNL Workfront] usará o agendamento padrão do sistema para calcular a linha do tempo das tarefas.</p> <p>Se você atribuir vários usuários à mesma tarefa em um projeto e o projeto tiver um agendamento atribuído e os usuários atribuídos às tarefas também tiverem um agendamento atribuído a eles, a [!UICONTROL Workfront] usará os seguintes agendamentos:</p> 
    <ul> 
     <li><strong>[!UICONTROL Atribuição Primária]</strong>: [!DNL Workfront] usa o agendamento da Atribuição Primária na tarefa para calcular linhas do tempo.</li> 
     <li><strong>[!UICONTROL Projeto]</strong>: [!DNL Workfront] usa a agenda do projeto para calcular a linha do tempo de cada tarefa.</li> 
    </ul> <p>Para obter mais informações sobre agendamentos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Criar um agendamento</a>.</p> </td> 
  </tr>

</tr> 
  <tr> 
   <td role="rowheader"> <p>Quando um usuário for atribuído à tarefa, use o cronograma de...</p> </td> 
   <td> 
<p>Se um projeto não tiver um agendamento atribuído ou se os usuários atribuídos às suas tarefas não tiverem um Agendamento atribuído a eles, [!DNL Workfront] usará o agendamento padrão do sistema para calcular a linha do tempo das tarefas.</p>

<p>Se você atribuir um usuário a uma tarefa em um projeto e o projeto e o usuário atribuído às tarefas tiverem agendamentos associados a elas, a [!UICONTROL Workfront] usará os seguintes agendamentos:</p> 
    <ul> 
     <li><strong>[!UICONTROL Usuário]</strong>: [!DNL Workfront] usa o agendamento do usuário atribuído na tarefa para calcular linhas do tempo.</li> 
     <li><strong>[!UICONTROL Projeto]</strong>: [!DNL Workfront] usa a agenda do projeto para calcular a linha de tempo da tarefa.</li> 
    </ul> <p>Para obter mais informações sobre agendamentos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Criar um agendamento</a>.</p>
</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Cálculos de Linha do Tempo] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Horas típicas por dia de trabalho]</strong>: Defina o número de horas em um dia de trabalho típico para os usuários que trabalharão nos projetos. O padrão é 8 horas.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Dias de trabalho típicos por semana]</strong>: define a semana de trabalho padrão para os usuários que estão trabalhando em projetos. O padrão é 5 dias.</li> 
    </ul> <p>Essas 2 opções convertem dias em horas ou semanas em dias.</p> <p>Por exemplo, se você tem uma tarefa com 8 Horas Planejadas e a duração é calculada com base nas Horas Planejadas, [!DNL Workfront] converte essas horas em dias para mostrar a Duração como dias.</p> <p>No campo Típico [!UICONTROL dias de trabalho por semana], o [!DNL Workfront] calcula o valor de FTE (Equivalente a Tempo Integral) do sistema. É o que [!DNL Workfront] usa ao calcular alocações para usuários.</p> <p>Esses valores são usados quando você está planejando cronogramas de projetos, orçamento de recursos ou registro de tempo em projetos. </p> <p>Elas não são usadas quando você está estabelecendo folhas de horas para usuários no sistema, conforme descrito em <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Configurar] preferências de hora e folha de horas</a>.</p> <p><b>NOTA</b>:</p> <p>[!DNL Workfront] os administradores não podem desbloquear as preferências de [!UICONTROL Cálculos de linha do tempo].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Trimestres Personalizados]</p> </td> 
   <td> <p>Configure trimestres anuais personalizados para os usuários que trabalharão nos projetos. Os trimestres personalizados geralmente são trimestres que não correspondem ao detalhamento tradicional de trimestres durante um ano civil. Você pode adicionar vários trimestres personalizados. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Habilitar trimestres personalizados para projetos</a>.</p>  <p><b>NOTA</b>: </p><p>[!DNL Workfront] Os administradores não podem desbloquear as preferências de [!UICONTROL Custom Quarters].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Casos de negócio] {#business-cases}

Você pode criar um Business Case para projetos recém-criados em todo o sistema para enviar solicitações de projeto. Você pode definir preferências para determinar quais áreas estão visíveis no formulário **[!UICONTROL Business Case]**. Recomendamos que você ative essas opções para que outras ferramentas, como o [!UICONTROL Portfolio Otimizer], sejam atualizadas corretamente. Para obter mais informações sobre o que cada campo exibe, consulte [Definir um Business Case: índice de artigo](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Depois que o administrador [!DNL Workfront] habilitar as seções no [!UICONTROL Business Case], um Proprietário do Projeto poderá criar um Business Case no nível do projeto. Para obter informações sobre como criar um Business Case, consulte [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Vida após a Morte] {#life-after-death}

Configure qualquer uma das seguintes preferências para projetos recém-criados em todo o sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Depois que um projeto for marcado como Concluído, as pessoas ainda poderão] </p> </td> 
   <td> <p>Determine as regras da organização (ou grupo, se estiver configurando preferências de projeto para um grupo) em relação à possibilidade de exclusão de uma tarefa ou problema após a marcação do status do projeto como [!UICONTROL Concluído].</p> 
    <ul> 
     <li><strong>[!UICONTROL Excluir Tarefas]</strong>: permite que usuários excluam tarefas de um projeto depois que o projeto é marcado como [!UICONTROL Concluído].<br></li> 
     <li><strong>[!UICONTROL Excluir Problemas]</strong>: permite que usuários excluam problemas de um projeto depois que o projeto é marcado como [!UICONTROL Concluído].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Depois que um projeto é marcado como Concluído, Desativado ou com Aprovação pendente, as pessoas ainda podem]</p> </td> 
   <td> <p>Determine as regras da sua organização (ou grupo, se estiver configurando preferências de projeto para um grupo) em relação ao que acontece com tarefas, problemas, documentos e outros objetos em um projeto depois que o status do projeto é marcado como <strong>[!UICONTROL Concluído]</strong>, <strong>[!UICONTROL Desativado]</strong> ou está <strong>[!UICONTROL com Aprovação Pendente]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Adicionar e editar tarefas:]</strong> Permite aos usuários:
      <ul>
       <li><p>Editar tarefas em um projeto depois que o projeto estiver marcado como [!UICONTROL Concluído], [!UICONTROL Desativado] ou estiver [!UICONTROL com Aprovação Pendente].</p>
           <p>Nota: Mesmo quando essa opção não está selecionada, os usuários podem adicionar e editar entradas de despesas. O registro de horas tem uma configuração separada. Para permitir ou impedir que os usuários registrem horas em projetos com status Concluído ou Inativo, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurar preferências de horas e folha de horas</a>.</p></li>
       <li>Adicionar tarefas a um projeto.</li>
      </ul></li>
     <li><strong>[!UICONTROL Adicionar e editar problemas]</strong>: Permite aos usuários:
      <ul>
       <li>Editar problemas em um projeto depois que ele for marcado como [!UICONTROL Concluído], [!UICONTROL Desativado] ou [!UICONTROL Com Aprovação Pendente].</li>
       <li>Adicionar problemas a um projeto depois que o projeto for marcado como [!UICONTROL Concluído] ou [!UICONTROL Desativado]. (Você não pode adicionar problemas a um projeto que esteja [!UICONTROL Pendente de Aprovação].)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Adicionar documentos ao projeto e a suas tarefas e problemas]</strong>: permite que os usuários adicionem documentos a um projeto (ou a documentos a tarefas e problemas dentro do projeto) depois que o projeto for marcado como [!UICONTROL Concluído] ou [!UICONTROL Desativado].</p> <p>Essa opção não se aplica a projetos com aprovação pendente.</p> </li> 
     <li> <p><strong>[!UICONTROL Anexar modelos]</strong>: permite aos usuários anexar modelos a um projeto depois que o projeto for marcado como [!UICONTROL Concluído] ou [!UICONTROL Desativado].</p> <p>Essa opção não se aplica a projetos com aprovação pendente.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
