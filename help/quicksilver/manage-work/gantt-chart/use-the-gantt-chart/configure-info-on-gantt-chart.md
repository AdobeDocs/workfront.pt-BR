---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: Configure como as informações são exibidas no gráfico [!UICONTROL Gantt]
description: Você pode configurar quais informações serão exibidas no Gráfico de Gantt da Lista de Tarefas e no Gráfico de Gantt da Lista de Projetos.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Configure como as informações são exibidas no [!UICONTROL Gráfico de Gantt]

<!-- Audited: 5/2025 -->

Você pode configurar quais informações serão exibidas no Gráfico de Gantt da Lista de Tarefas e no Gráfico de Gantt da Lista de Projetos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacote</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> 
   <p>[!UICONTROL Light] ou superior<p>
   <p>[!UICONTROL Review] ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>[!UICONTROL Exibir] ou superior acesso a Projetos e Tarefas</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>[!UICONTROL Exibir] ou superior acesso ao projeto e às tarefas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Light<p>
   <p>Or</p>
   <p>Current: Review</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] or higher access to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Entender as opções de exibição

A tabela a seguir detalha as opções de exibição do [!UICONTROL Gráfico de Gantt]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Datas Efetivas</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="atual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>A [!UICONTROL Data de Início Efetivo] e a [!UICONTROL Data de Término Efetivo] são exibidas com um ícone de triângulo. Se a [!UICONTROL Data de Término Efetivo] for nula, somente a [!UICONTROL Data de Início Efetivo] será exibida.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Visão geral da [!UICONTROL Data de Término Efetivo] </a> e <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Visão geral do projeto [!UICONTROL Data de Início Efetivo] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atribuições]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="atribuições_em_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>Mostra os atribuídos da tarefa. Passe o mouse sobre o link Detalhes ao lado do nome do destinatário para ver informações mais detalhadas sobre ele, incluindo a porcentagem de sua alocação para a tarefa.</p> <p>Os atribuídos não são exibidos no [!UICONTROL Gráfico de Gantt] quando o [!UICONTROL Gráfico de Gantt] é exportado para o PDF. Quando o [!UICONTROL Gráfico de Gantt] é exportado para o PDF, os atribuídos somente são exibidos na lista de tarefas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linha de Base]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gantt.png"> </td> 
   <td> <p>Um instantâneo de projeto que representa dados importantes sobre o projeto incluído no plano de projeto inicial. As linhas de base podem ser usadas em toda a linha do tempo do projeto. Quando você habilita a exibição de linhas de base no [!UICONTROL Gráfico de Gantt], selecione qual linha de base deseja exibir. Você pode exibir somente uma linha de base no [!UICONTROL Gráfico de Gantt] por vez e ela será exibida na forma de uma barra cinza.</p> <p>Para obter mais informações sobre linhas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">Criar linhas de base do projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de Confirmação]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>A data fornecida por um destinatário como compromisso de quando a tarefa será concluída é exibida com um marcador no [!UICONTROL Gráfico de Gantt]. </p> <p>Para obter mais informações sobre datas de confirmação, consulte a visão geral <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL Data de Confirmação]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % Concluído]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  A porcentagem da tarefa que está concluída é exibida na linha da tarefa.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Caminho Crítico]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>As tarefas que podem afetar a linha do tempo do projeto são consideradas parte do Caminho crítico e estão claramente marcadas em vermelho. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marco] Diamantes</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamonds.png"> </td> 
   <td> <p>Um ícone de diamante é exibido depois da tarefa associada a uma etapa. Passe o mouse sobre uma etapa para ver o nome e a data da etapa. O administrador [!DNL Workfront] determina a cor de cada diamante de etapas.</p> <p>Para obter mais informações sobre etapas, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Criar um caminho de etapas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Linhas de [!UICONTROL Milestone]</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>Uma linha é exibida após a tarefa associada a uma etapa. Passe o mouse sobre uma etapa para ver o nome e a data da etapa. O administrador [!DNL Workfront] determina a cor de cada linha de marco.</p> <p> Para obter mais informações sobre marcos, consulte  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Criar um caminho de etapas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predecessoras]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="predecessor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>Uma linha de uma tarefa para outra que mostra a relação da predecessora entre as duas tarefas. Para realçar uma linha predecessora individual, passe o mouse sobre ela. Clique para mantê-lo destacado. É possível destacar apenas uma linha predecessora por vez.</p> <p>Um ícone [!UICONTROL Predecessor] é exibido ao lado de qualquer tarefa que tenha um relacionamento de predecessor que abranja várias páginas no gráfico de Gantt ou em qualquer tarefa que tenha um predecessor de vários projetos.</p> <p>Clique no ícone [!UICONTROL Predecessor] para exibir todas as tarefas predecessoras e sucessoras e seus detalhes, como nome da tarefa, tipo de relacionamento predecessor e datas chave.</p> <p>Observação: o [!UICONTROL Gráfico de Gantt] em uma lista de projetos exibe informações sobre predecessores entre projetos. Para obter mais informações sobre como criar relações de predecessoras entre projetos diferentes, consulte <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Criar predecessoras entre projetos</a></p> <p>Para obter mais informações sobre predecessores, consulte <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">Impor predecessores</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status de Progresso]</td> 
   <td> <p>[!UICONTROL No Prazo] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time_out_2017.png"></p> <p>[!UICONTROL Atrás]    <img src="assets/task-behind--oct.-2017.png" alt="task_behind_out_out_2017.png"></p> <p>[!UICONTROL Em Risco]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>Atrasado        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>O status do progresso atual em uma determinada tarefa. </p> <p>Para obter mais informações, consulte a visão geral <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Tarefa [!UICONTROL Progress Status]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Datas Projetadas</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_projects_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>A linha do tempo projetada esperada que marca as datas de Início e Término Projetadas com base no trabalho atual concluído, mais o trabalho restante. </p> <p>Para obter mais informações sobre as datas de conclusão projetadas, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Visão geral da data de conclusão projetada para projetos, tarefas e problemas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar opções de exibição

1. Vá para o **Gráfico de Gantt da Lista de Tarefas** ou o **Gráfico de Gantt da Lista de Projetos**.\
   Para obter mais informações sobre a localização dos gráficos de Gantt, consulte [Introdução ao [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

1. (Opcional) Selecione a configuração **Alternar para datas projetadas** para exibir as tarefas por suas datas projetadas. Por padrão, as tarefas são exibidas por suas Datas planejadas.
1. Clique no ícone **Opções**. A caixa de diálogo **Opções** é aberta.\
   ![Opções.png](assets/options-350x129.png)

1. Selecione as opções de configuração que você deseja exibir no [!UICONTROL Gráfico de Gantt].

   >[!NOTE]
   >
   > Nem todas as opções de configuração estão disponíveis na Lista de Projetos [!UICONTROL Gráfico de Gantt].

1. Clique em qualquer lugar no Gráfico de Gantt para fechar a caixa de diálogo **Opções**.
