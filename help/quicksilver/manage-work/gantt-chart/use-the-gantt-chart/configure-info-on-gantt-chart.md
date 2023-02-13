---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: Configure como as informações são exibidas no [!UICONTROL Gantt] Gráfico
description: Você pode configurar quais informações são exibidas no Gráfico de Gantt da Lista de Tarefas e no Gráfico de Gantt da Lista de Projetos.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# Configure como as informações são exibidas no [!UICONTROL Gráfico de Gantt]

Você pode configurar quais informações serão exibidas em ambas as listas de tarefas [!UICONTROL Gráfico de Gantt] e a lista de projetos [!UICONTROL Gráfico de Gantt].

## Requisitos de acesso

Você deve ter o seguinte para seguir as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>[!UICONTROL View] ou acesso superior a Projetos e tarefas</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>[!UICONTROL View] ou acesso superior ao projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Entender as opções de exibição

A tabela a seguir detalha as opções de exibição da variável [!UICONTROL Gráfico de Gantt]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datas reais]</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="atual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL Data de início real] e [!UICONTROL Data de conclusão real] são exibidas com um ícone de triângulo. Se a [!UICONTROL Data de conclusão real] for nula, somente a [!UICONTROL Data de início real] será exibida.</p> <p>Para obter mais informações sobre datas de início e conclusão, consulte <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Visão geral do projeto [!UICONTROL Data de conclusão real] </a> e <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Visão geral do projeto [!UICONTROL Data de início real] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atribuições]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="atribuições_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>Mostra os destinatários da tarefa. Passe o mouse sobre o <strong>[!UICONTROL Detalhes]</strong> link ao lado do nome de um destinatário para ver informações mais detalhadas sobre ele, incluindo a porcentagem de sua alocação para a tarefa.</p> <p>Os destinatários não são exibidos no [!UICONTROL Gantt chart] quando o [!UICONTROL Gantt chart] é exportado para o PDF. Quando o [!UICONTROL Gantt chart] é exportado para o PDF, os destinatários são exibidos somente na lista de tarefas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linha de base]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gantt.png"> </td> 
   <td> <p>Um instantâneo de projeto que representa os principais dados sobre o projeto incluídos no plano de projeto inicial. As linhas de base podem ser utilizadas durante toda a vida do projeto. Ao ativar a exibição de linhas de base no [!UICONTROL Gantt chart], selecione qual linha de base deseja exibir. É possível exibir apenas uma linha de base no [!UICONTROL Gantt chart] de cada vez, ela será mostrada na forma de uma barra cinza.</p> <p>Para obter mais informações sobre linhas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">Criar linhas de base do projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data da confirmação]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>A data que um destinatário assume como compromisso de quando a tarefa será concluída é exibida com um marcador no [!UICONTROL Gantt chart]. </p> <p>Para obter mais informações sobre datas de confirmação, consulte <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Visão geral da [!UICONTROL Data da confirmação]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % concluído]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  A porcentagem da tarefa concluída é exibida na linha de tarefa.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Caminho crítico]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>As tarefas que podem afetar a linha do tempo do projeto são consideradas parte do Caminho Crítico e claramente marcadas em vermelho. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marco] Ouros</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamantes.png"> </td> 
   <td> <p>Um ícone de diamante é exibido depois da tarefa associada a um marco. Passe o mouse sobre um marco para visualizar o nome e a data do marco. O [!DNL Workfront] O administrador determina a cor de cada diamante de marco.</p> <p>Para obter mais informações sobre marcos, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Criar um caminho de marco</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Linhas de [!UICONTROL Milestone]</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>Uma linha é exibida após a tarefa associada a um marco. Passe o mouse sobre um marco para visualizar o nome e a data do marco. O [!DNL Workfront] o administrador determina a cor de cada linha de marco.</p> <p> Para obter mais informações sobre marcos, consulte  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Criar um caminho de marco</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predecessores]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="predecessor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>Uma linha de uma tarefa a outra que mostra a relação do antecessor entre as duas tarefas. Para destacar uma linha predecessora individual, passe o mouse sobre ela. Clique para mantê-lo destacado. Você só pode realçar uma linha antecessora por vez.</p> <p>A <strong>[!UICONTROL Predecessor]</strong> é exibido ao lado de qualquer tarefa que tenha uma relação antecessora que abrange várias páginas no gráfico de Gantt ou em qualquer tarefa que tenha um antecessor entre projetos.</p> <p>Clique no botão <strong>[!UICONTROL Predecessor]</strong> ícone para exibir todos os antecessores e tarefas sucessoras, bem como detalhes sobre cada tarefa, como nome da tarefa, tipo de relacionamento antecessor e datas-chave.</p> <p>Observação: O [!UICONTROL Gantt Chart] em uma lista de projetos exibe informações sobre predecessores entre projetos. Para obter mais informações sobre como criar relacionamentos predecessores entre diferentes projetos, consulte <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Criar antecessores entre projetos</a></p> <p>Para obter mais informações sobre predecessores, consulte <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">Impor predecessores</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status de progresso]</td> 
   <td> <p>[!UICONTROL No Horário] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time_Oct._2017.png"></p> <p>[!UICONTROL atrás]    <img src="assets/task-behind--oct.-2017.png" alt="task_behind_Oct._2017.png"></p> <p>[!UICONTROL Em Risco]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>Atrasado        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>O status do progresso atual em uma determinada tarefa. </p> <p>Para obter informações mais detalhadas sobre cada tipo de [!UICONTROL Progress Status], consulte <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Visão geral do status de progresso da tarefa [!UICONTROL]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datas projetadas]</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_project_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>A linha do tempo projetada esperada que marca o [!UICONTROL Início projetado] e as [!UICONTROL datas de conclusão] com base no trabalho atual concluído, além do trabalho restante. </p> <p>Para obter mais informações sobre datas de conclusão projetadas, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Visão geral da [!UICONTROL Data de conclusão projetada] para projetos, tarefas e problemas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar opções de exibição

1. Ir para a Lista de Tarefas [!UICONTROL Gráfico de Gantt] ou na lista de projetos [!UICONTROL Gráfico de Gantt].\
   Para obter mais informações sobre onde a variável [!UICONTROL Gráfico de Gantt] estiver localizado, consulte [Introdução ao [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

1. (Opcional) Selecione o **[!UICONTROL Alterar para datas projetadas]** configuração para exibir as tarefas por seus [!UICONTROL Datas Projetadas]. Por padrão, as tarefas são exibidas por seus [!UICONTROL Datas Planejadas] no [!UICONTROL Gráfico de Gantt].
1. Clique no ícone de opções para exibir o **[!UICONTROL Opções]** caixa de diálogo.\
   ![Options.png](assets/options-350x129.png)

1. Selecione as opções de configuração que deseja exibir no [!UICONTROL Gráfico de Gantt].

   >[!NOTE]
   > Nem todas as opções de configuração estão disponíveis na Lista de projetos [!UICONTROL Gráfico de Gantt].

1. Clique em qualquer lugar na [!UICONTROL Gráfico de Gantt] para fechar o **[!UICONTROL Opções]** caixa de diálogo.
