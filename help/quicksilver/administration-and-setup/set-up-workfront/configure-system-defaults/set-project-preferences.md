---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurar preferências de projeto em todo o sistema
description: Como um [!DNL Adobe Workfront] administrador, você pode configurar as preferências padrão para todos os projetos criados em todo o sistema. Essas preferências afetam o comportamento do projeto, da tarefa e da ocorrência.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '2509'
ht-degree: 1%

---

# Configurar preferências de projeto em todo o sistema

Como um [!DNL Adobe Workfront] administrador, você pode configurar as preferências padrão para todos os projetos criados em todo o sistema. Essas preferências afetam o comportamento do projeto, da tarefa e da ocorrência.

>[!NOTE]
>
>Por padrão, essas preferências são bloqueadas e os administradores de grupo não podem modificá-las no nível de grupo, a menos que você as desbloqueie para todos os grupos em todo o sistema. Para obter mais informações, consulte [Bloquear ou desbloquear preferências de projeto para todos os grupos no sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar preferências de projeto para toda a organização

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Projetos]**.

1. Na página exibida, continue com uma das 4 seções listadas abaixo para configurar as preferências do [!UICONTROL Status do projeto], [!UICONTROL Linhas do tempo], [!UICONTROL Casos de negócios]e [!UICONTROL Vida após morte].
1. Se quiser que todos os grupos da organização usem as mesmas preferências de projeto, verifique se cada preferência está bloqueada ![](assets/lock-toggle-button.png) (esse é o padrão).

   >[!IMPORTANT]
   >
   >Quando uma preferência de projeto é bloqueada, todas as alterações feitas nessa preferência são herdadas por todos os grupos no sistema. É importante se comunicar com os usuários e grupos em toda a organização para garantir que todas as necessidades sejam contabilizadas na forma como você configura as preferências do projeto.

   Para obter informações sobre como desbloquear uma preferência para que todos os grupos possam configurá-la e gerenciá-la por conta própria, consulte [Bloquear ou desbloquear preferências de projeto para todos os grupos no sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Clique em **[!UICONTROL Salvar]**.

* [[!UICONTROL Status do projeto]](#project-status)
* [[!UICONTROL Linhas de Tempo]](#timelines)
* [[!UICONTROL Casos de negócio]](#business-cases)
* [[!UICONTROL Vida após a morte]](#life-after-death)

### Status do projeto {#project-status}

Configure qualquer uma das preferências a seguir para projetos recém-criados em todo o sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permitir que usuários criem projetos sem usar um modelo]</td> 
   <td>  <p>Essa preferência permite que os usuários criem projetos sem usar um modelo ao criar um projeto a partir das seguintes áreas: </p>
      <ul>
        <li>
        <p>Usar a opção [!UICONTROL Novo projeto] em uma lista de projetos</p>
        </li>
          <li>
          <p>Converter um problema em um projeto a partir da página do problema</p>
          </li>
         </ul>
        <p>Essa preferência é ativada por padrão. </p> 
        <p><b>Nota</b></p>
        <p> Um administrador de grupo pode alterar essa preferência para um grupo. Quando um usuário pertence a vários grupos com preferências diferentes, ele poderá criar um projeto sem um modelo se o Grupo doméstico tiver essa preferência ativada.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Definir o status do novo projeto como]</td> 
   <td> <p>Determine o status de novos projetos.</p>  <p><b>Nota</b>  
     <ul> 
      <li>Se você ou outro [!DNL Workfront] O administrador oculta o status selecionado aqui, o status padrão muda para o primeiro status na lista de status.</li> 
     </ul> 
     <ul> 
      <li> <p>Se um sistema bloqueado ou um status de grupo for definido como o status padrão e depois alguém o desbloquear, o sistema tentará substituí-lo por um status bloqueado do mesmo tipo de status.</p> <p>Se não encontrar um, ele procura um status obrigatório:</p> 
       <ul> 
        <li>Se houver um status obrigatório que seja igual ao status padrão desbloqueado, o status necessário se tornará o status padrão, mesmo se estiver desbloqueado.</li> 
        <li>Se nenhum dos status necessários for igual ao status padrão desbloqueado, o primeiro status necessário na lista de status se tornará o status padrão.</li> 
       </ul> <p>Para obter informações sobre os status necessários, consulte os artigos <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de projeto do sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Acessar a lista de status de tarefas do sistema</a>e <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Acesse a lista de status de problemas do sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calcular porcentagem concluída com base em]</td> 
   <td> <p>A porcentagem de conclusão de um projeto ou tarefa pai é baseada no progresso geral das tarefas. Essas informações podem ser calculadas com base na Duração ou nas Horas Planejadas das tarefas em um projeto.</p> <p>Se você selecionar [!UICONTROL Duração], a Duração de cada tarefa em um projeto determinará a porcentagem total concluída do projeto e a Duração de cada subtarefa determinará a porcentagem total concluída da tarefa pai.</p> <p>Se você selecionar [!UICONTROL Duração], certifique-se de especificar as [!UICONTROL Horário típico por dia de trabalho] e [!UICONTROL Dias de trabalho típicos por semana] na seção [!UICONTROL Linhas do tempo] . [!DNL Workfront] O usa essas informações ao calcular o percentual de conclusão de uma tarefa com base na Duração. </p> <p>Se você selecionar [!UICONTROL Horas planejadas], verifique se todas as tarefas em cada projeto têm a quantidade de [!UICONTROL Horas Planejadas] definida e se a quantidade não é zero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Definir automaticamente a condição do projeto com base no status de progresso]</td> 
   <td> <p>Essa preferência permite que os usuários definam a [!UICONTROL Condição] de um projeto manualmente ([!UICONTROL No Target], [!UICONTROL Em Risco], [!UICONTROL Em Problema]) ou tenham [!DNL Workfront] defina a [!UICONTROL Condição] (Status de progresso) automaticamente com base na progressão do projeto na linha do tempo. Para obter mais informações sobre a Condição dos projetos, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Visão geral da condição do projeto e do tipo de condição</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criar linhas de base automaticamente]</p> </td> 
   <td> <p>Essa preferência cria automaticamente uma linha de base (instantâneo) dos detalhes da tarefa e do projeto quando o status do projeto é alterado para [!UICONTROL Atual]. Para obter informações sobre como criar linhas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Criar linhas de base do projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método de índice de desempenho] </p> </td> 
   <td> <p>O Método do Índice de Desempenho (PIM) do projeto controla o método [!DNL Workfront] O usa o para calcular métricas de Valor Ganho, como [!UICONTROL Cost Performance Index] (CPI) e [!UICONTROL Estimate At Completion] (EAC). Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcular o [!UICONTROL Cost Performance Index] (CPI)</a> e <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calcular Estimativa na Conclusão] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Baseado em hora]</strong>: [!DNL Workfront] O usa [!UICONTROL Horas planejadas] para calcular métricas de desempenho como EAC e CPI. Quando o PIM é calculado com base em horas, o EAC é exibido como um número de horas. Certifique-se de ter um valor para [!UICONTROL Horas planejadas], diferente de zero.</li> 
     <li> <p><strong>[!UICONTROL baseado em custo]</strong>: [!DNL Workfront] O usa o [!UICONTROL Custo planejado da mão de obra] para calcular métricas de desempenho como EAC e CPI. Certifique-se de que suas funções ou usuários estejam associados às taxas de Custo por Hora. Quando o PIM é calculado com base em Custos, o EAC é exibido como um valor de moeda.</p> <p>O gerente de projeto pode modificar essa configuração no nível do projeto, usando a área [!UICONTROL Finance] em [!UICONTROL Detalhes do projeto]. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gerenciar informações na área [!UICONTROL Finance] do projeto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimativa na conclusão ]</p> </td> 
   <td> <p>Determinar quais dados [!DNL Workfront] O usa para calcular a [!UICONTROL Estimativa na conclusão] (EAC) que representa o custo total projetado de um projeto.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calcular no nível do projeto]</strong>: EAC para a tarefa pai e projeto são determinados inserindo [!UICONTROL Horas reais] ou [!UICONTROL Custo real da mão de obra] nas Fórmulas EAC. Esse cálculo inclui [!UICONTROL Horas reais] ou [!UICONTROL Custos e despesas] adicionados diretamente à tarefa pai ou ao projeto.</li> 
     <li> <p><strong>[!UICONTROL Acumular de tarefas/subtarefas]</strong>: EAC para a tarefa pai e o projeto são determinados pela soma do EAC para cada tarefa filho. Esse cálculo exclui [!UICONTROL Horas reais] ou [!UICONTROL Custos e despesas reais] adicionados diretamente à tarefa pai ou ao projeto.</p> <p>O gerente de projeto pode modificar essa configuração no nível do projeto, usando a área [!UICONTROL Finance] em [!UICONTROL Detalhes do projeto]. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gerenciar informações na área [!UICONTROL Finance] do projeto</a>.</p> </li> 
    </ul> <p>Para obter mais informações sobre como o EAC calcula, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular [!UICONTROL Estimativa na conclusão] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Linhas de Tempo {#timelines}

Configure qualquer uma das preferências a seguir para projetos recém-criados em todo o sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agendar de]</td> 
   <td> <p>Determine se os novos projetos são agendados a partir da Data inicial ou da Data de conclusão quando são criados.</p> 
    <ul> 
     <li><strong>[!UICONTROL Data de início]</strong>: Novas tarefas são padronizadas para a Restrição de tarefas do [!UICONTROL assim que possível] e os gerentes de projeto são solicitados a fornecer uma [!UICONTROL Data de início planejada] para o projeto.</li> 
     <li><strong>[!UICONTROL Data de conclusão]</strong>: Novas tarefas são padronizadas para a Restrição de Tarefas [!UICONTROL Como Atraso Possível] e os gerentes de projeto são solicitados a fornecer uma [!UICONTROL Data de Conclusão Planejada] para o projeto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tempo do usuário desligado]</td> 
   <td> <p>Determine se a hora do Destinatário Principal de uma tarefa ajusta as datas planejadas para essa tarefa em um projeto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Considere o tempo limite do usuário nas durações da tarefa]</strong>: Qualquer hora de agendamento para o Destinatário Principal de uma tarefa ajusta as datas planejadas da tarefa se o tempo limite ocorrer durante a duração da tarefa. Esta é a configuração padrão. </p> <p>Por exemplo, se uma tarefa com uma Restrição do [!UICONTROL Assim que possível] estiver programada para iniciar em 1° de junho e ser concluída em 3 de junho, e o Destinatário principal tiver o dia 2 de junho marcado para Tempo de desativação, as datas planejadas da tarefa serão ajustadas para 1º de junho a 4 de junho.</p> <p><b>IMPORTANTE</b>: A Duração da tarefa não é alterada ao selecionar essa configuração. Somente as datas planejadas são alteradas, dependendo da Restrição de Tarefa.</p> </li> 
     <li><strong>[!UICONTROL Ignorar tempo do usuário nas durações da tarefa]</strong>: As datas planejadas de cada tarefa em um projeto permanecem como originalmente planejadas, mesmo se o Destinatário Principal de uma tarefa tiver tempo livre durante sua duração.</li> 
    </ul> <p>Considere o seguinte ao selecionar as opções para esta configuração:</p> 
    <ul> 
     <li>Ao alterar essa configuração, somente os projetos e modelos criados após a alteração herdam a configuração atualizada. </li> 
     <li> <p>O valor de Restrição de Tarefa da tarefa determina quais datas de tarefa planejada ajustar: </p> 
      <ul> 
       <li>A data de início planejada</li> 
       <li>A data de conclusão planejada</li> 
       <li>Ambas as datas</li> 
       <li>Nenhuma data. </li> 
      </ul> <p>Por exemplo, se uma tarefa tiver uma Restrição de [!UICONTROL Datas fixas], as datas não se ajustarão quando o Destinatário principal tiver tempo limite, mesmo que a opção [!UICONTROL Considere o tempo limite do usuário na duração da tarefa] esteja selecionada. Para obter informações sobre restrições de tarefa, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Visão geral da restrição de tarefa</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL As linhas do tempo do projeto serão automaticamente recalculadas]</p> </td> 
   <td> <p>Determine quando a linha do tempo de um projeto é recalculada. Para obter informações sobre como recalcular a linha do tempo do projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular linhas do tempo do projeto</a>.</p> <p>As opções a seguir são ativadas por padrão. É possível selecionar uma ou mais das seguintes configurações:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL todas as noites]</strong>: Selecione essa opção para recalcular as linhas do tempo do projeto todas as noites. Quaisquer alterações feitas no projeto que possam afetar a linha do tempo não estarão imediatamente visíveis. [!DNL Workfront​​​] O recalcula as linhas do tempo à noite apenas para projetos em que ambas as condições a seguir sejam cumpridas:</p> <p> 
       <ul> 
        <li>Ter um status de [!UICONTROL Atual]</li> 
        <li>Tiveram uma atualização nos últimos 3 meses</li> 
        <li>Tiveram um Tipo de atualização de um dos seguintes:</li>
        <ul>
        <li>Automático e Mediante alteração</li>
        <li>Somente mediante alteração</li>
        <li>Somente automática</li> 
      </ul>       
    <b>DICA</b>
    <p>Os projetos que têm um Tipo de Atualização Manual Somente não são afetados por essa configuração.</p>
    <li> <p><strong>Quando o escopo de um projeto é alterado</strong>: Selecione essa opção para recalcular as linhas do tempo do projeto imediatamente, conforme ocorre uma alteração no escopo do projeto. Para obter informações sobre o que constitui uma alteração no escopo do projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular linhas do tempo do projeto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Quando vários usuários são atribuídos a uma tarefa, use o agendamento da]</p> </td> 
   <td> <p>Se um projeto não tiver um agendamento atribuído ou se os usuários atribuídos às suas tarefas não tiverem um Agendamento atribuído a eles, [!DNL Workfront] O usa o agendamento padrão do sistema para calcular a linha do tempo das tarefas.</p> <p>Se você atribuir vários usuários à mesma tarefa em um projeto tiver uma programação atribuída, e os usuários atribuídos às tarefas também tiverem uma programação atribuída a eles, a [!UICONTROL Workfront] usará as seguintes programações:</p> 
    <ul> 
     <li><strong>[!UICONTROL Atribuição primária]</strong>: [!DNL Workfront] O usa o agendamento da Atribuição primária na tarefa para calcular linhas do tempo.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] O usa o agendamento do projeto para calcular a linha do tempo de cada tarefa.</li> 
    </ul> <p>Para obter mais informações sobre programações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Criar um agendamento</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Cálculos da Linha do Tempo] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Horas típicas por dia de trabalho]</strong>: Defina o número de horas em um dia de trabalho típico para os usuários que trabalharão em projetos. O padrão é 8 horas.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Dias normais de trabalho por semana]</strong>: Defina a semana de trabalho padrão para os usuários que trabalharão em projetos. O padrão é 5 dias.</li> 
    </ul> <p>Essas 2 opções convertem dias em horas ou semanas em dias.</p> <p>Por exemplo, se você tiver uma tarefa com 8 Horas Planejadas e a duração for calculada com base nas Horas Planejadas, [!DNL Workfront] converte essas horas em dias para mostrar a Duração como dias.</p> <p>No campo Típico [!UICONTROL dias úteis por semana] , [!DNL Workfront] O calcula o valor de Equivalente de Tempo Total (FTE) para seu sistema. Isto é o que [!DNL Workfront] O usa o ao calcular alocações para usuários.</p> <p>Esses valores são usados quando você está planejando linhas do tempo dos projetos, orçando recursos ou registrando tempo em projetos. </p> <p>Eles não são usados ao estabelecer folhas de horas para usuários no sistema, conforme descrito em <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Configurar] preferências de hora e hora</a>.</p> <p><b>OBSERVAÇÃO</b>: [!DNL Workfront] os administradores não podem desbloquear as preferências de [!UICONTROL Cálculos da linha do tempo].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Trimestres Personalizados]</p> </td> 
   <td> <p>Configure trimestres anuais personalizados para os usuários que trabalharão em projetos. Os trimestres personalizados são normalmente trimestres que não correspondem à discriminação tradicional de trimestres durante um ano civil. Você pode adicionar vários trimestres personalizados. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Habilitar trimestres personalizados para projetos</a>.</p>  <p><b>OBSERVAÇÃO</b>: [!DNL Workfront] os administradores não podem desbloquear as preferências de [!UICONTROL Trimestres personalizados].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Casos de negócio] {#business-cases}

Você pode criar um Caso de negócios para projetos recém-criados em todo o sistema para enviar solicitações de projeto. É possível definir preferências para determinar quais áreas estão visíveis na variável **[!UICONTROL Caso de negócios]** formulário. Recomendamos que você ative essas opções para que outras ferramentas, como a [!UICONTROL Portfolio Otimizer], atualizar corretamente. Para obter mais informações sobre o que cada campo exibe, consulte [Definir um caso de negócios](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Depois que a variável [!DNL Workfront] O administrador habilita as seções na [!UICONTROL Caso de negócios], um Proprietário do projeto pode criar um Caso de negócios no nível do projeto. Para obter informações sobre como criar um Caso de Negócios, consulte [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Vida após a morte] {#life-after-death}

Configure qualquer uma das preferências a seguir para projetos recém-criados em todo o sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Após um projeto ser marcado como concluído, as pessoas ainda podem] </p> </td> 
   <td> <p>Determine as regras para sua organização (ou grupo, se estiver configurando preferências de projeto para um grupo) em relação a uma tarefa ou problema poder ser excluído depois que o status do projeto for marcado como [!UICONTROL concluído].</p> 
    <ul> 
     <li><strong>[!UICONTROL Excluir tarefas]</strong>: Permite que os usuários excluam tarefas de um projeto depois que o projeto é marcado como [!UICONTROL Concluído].<br></li> 
     <li><strong>[!UICONTROL Excluir problemas]</strong>: Permite que os usuários excluam problemas de um projeto depois que ele é marcado como [!UICONTROL Concluído].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Após um projeto ser marcado como Concluído, Adiado ou Pendente na aprovação, as pessoas ainda podem]</p> </td> 
   <td> <p>Determine as regras de sua organização (ou grupo, se estiver configurando as preferências do projeto para um grupo) em relação ao que acontece com tarefas, problemas, documentos e outros objetos em um projeto após o status do projeto ter sido marcado <strong>[!UICONTROL concluído]</strong>, <strong>[!UICONTROL inativo]</strong>ou é <strong>[!UICONTROL Aprovação pendente]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Adicionar e editar tarefas]</strong> Permite aos usuários:
      <ul>
       <li>Edite as tarefas em um projeto depois que ele for marcado como [!UICONTROL Concluído], [!UICONTROL Inativo] ou como [!UICONTROL Pendente Aprovação]. Isso inclui adicionar horas e alterar entradas de despesas em uma tarefa.</li>
       <li>Adicionar tarefas a um projeto.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Adicionar e editar problemas]</strong>: Permite aos usuários:
      <ul>
       <li>Edite os problemas em um projeto depois que ele for marcado como [!UICONTROL Concluído], [!UICONTROL inativo] ou [!UICONTROL pendente de aprovação].</li>
       <li>Adicione problemas a um projeto depois que ele for marcado como [!UICONTROL concluído] ou [!UICONTROL inativo]. (Não é possível adicionar problemas a um projeto que seja [!UICONTROL Aprovação pendente].)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Adicionar documentos ao projeto e às suas tarefas e problemas]</strong>: Permite que os usuários adicionem documentos a um projeto (ou adicionem documentos a tarefas e problemas no projeto) após o projeto ter sido marcado como [!UICONTROL Completo] ou [!UICONTROL Inativo].</p> <p>Essa opção não se aplica a projetos que estão pendentes de aprovação.</p> </li> 
     <li> <p><strong>[!UICONTROL Anexar modelos]</strong>: Permite que os usuários anexem modelos a um projeto depois que o projeto é marcado como [!UICONTROL concluído] ou [!UICONTROL inativo].</p> <p>Essa opção não se aplica a projetos que estão pendentes de aprovação.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
