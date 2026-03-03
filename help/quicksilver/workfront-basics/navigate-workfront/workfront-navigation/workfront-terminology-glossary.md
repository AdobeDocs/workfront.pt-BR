---
content-type: reference
navigation-topic: workfront-navigation
title: 'Glossário da terminologia do  [!DNL Adobe Workfront] '
description: O glossário do  [!DNL Adobe Workfront]  lista termos comumente usados na interface do  [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] , em relatórios ou quando você tenta entender o significado de conceitos do  [!DNL Workfront]  definidos na documentação do  [!DNL Workfront] .
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 087589f3d7a3fbb1611045b921e804aec3db9a74
workflow-type: tm+mt
source-wordcount: '21621'
ht-degree: 99%

---


# Glossário da terminologia do [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Este artigo deve ser usado como referência para entender os termos que você pode encontrar no aplicativo [!DNL Adobe Workfront], na documentação do [!DNL Workfront] ou ao falar sobre planejamento e gerenciamento do trabalho. Estamos atualizando essas informações no momento e, como resultado, esta tabela pode não estar completa. Removeremos este aviso quando considerarmos que as informações estão completas.

A tabela a seguir é uma lista de termos usados com frequência no Adobe Workfront:

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome do objeto</strong></th> 
   <th><strong>Descrição</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Nível de acesso]</td> 
   <td>Um perfil de usuário que determina como um usuário pode interagir com diferentes objetos e ferramentas no Workfront.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa ativa]</td> 
   <td>Uma tarefa incompleta em um projeto atual na qual a tarefa predecessora não impede o trabalho e que não possui uma restrição de tarefa com uma data inicial planejada para o futuro. Em outras palavras, é possível trabalhar nela hoje.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Atividade]</td> 
   <td>No [!DNL Workfront Goals], uma atividade é um indicador de progresso para uma meta. Pode ser uma barra de progresso que você atualiza manualmente ou um projeto associado à meta. Não é possível exibir atividades em um relatório e não é possível acessá-las por meio da API do [!DNL Workfront]. Para obter informações sobre atividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introdução a resultados e atividades no Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo efetivo]</td> 
   <td> <p>Para tarefas e problemas, este é o custo associado às horas efetivas registradas em relação à taxa de custo por hora do recurso atribuído à tarefa ou ao problema. Para projetos, este é o total de todos os [!UICONTROL custos efetivos] de tarefas e problemas no projeto. Para obter informações, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Monitorar custos</a>.</p>

<p>Os cálculos de [!UICONTROL custo efetivo] levam em consideração as [!UICONTROL horas efetivas legadas]. Para obter informações, consulte “[!UICONTROL Horas efetivas]” ou “[!UICONTROL Horas efetivas legadas]” nesta tabela. </p>   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo efetivo da despesa]</td> 
   <td> <p>A soma dos [!UICONTROL valores reais] de todas as despesas registradas para um projeto ou uma tarefa.</p> <b>EXEMPLO </b>
   <p>Se você criar uma despesa para a Tarefa 1 e inserir US$ 600,00 no campo [!UICONTROL Valor real], o [!UICONTROL Custo efetivo da despesa] dessa tarefa será de US$ 600,00. </p> 
   <p>Para um projeto, o [!DNL Workfront] usa a seguinte fórmula para calcular o [!UICONTROL Custo efetivo da despesa]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas efetivas]</td> 
   <td> <p>Em um relatório de projeto, tarefa ou problema, as [!UICONTROL horas efetivas] são a soma de todas as horas registradas no projeto, tarefa ou problema após maio de 2021.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span> se, a partir da guia [!UICONTROL Atualizações] da Tarefa 1, você clicar em “Tempo de registro” e inserir 25 horas, as horas efetivas da Tarefa 1 totalizarão 25 horas. </p> <p>[!DNL Workfront] calcula [!UICONTROL horas efetivas] para tarefas pai ou projetos usando as seguintes fórmulas:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project + [!UICONTROL Actual Hours] logged on issues in the project</code>  </p> </li> 
    </ul> 
   <p>Consulte também <strong>[!UICONTROL Horas efetivas legadas]</strong>.
    <p>Para obter mais informações, consulte <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Exibir horas efetivas</a>.</p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo efetivo do trabalho]</td> 
   <td> <p>O [!UICONTROL custo efetivo] associado à mão de obra investida em uma tarefa ou um projeto. </p> <p>Para uma tarefa, [!DNL Workfront] calcula o [!UICONTROL custo efetivo do trabalho] usando a seguinte fórmula:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Se a tarefa tiver um [!UICONTROL Tipo de custo] de [!UICONTROL Usuário por hora], o [!DNL Workfront] usará a taxa de usuários. Se a tarefa tiver um [!UICONTROL Tipo de custo] de [!UICONTROL Função por hora], o [!DNL Workfront] usará a taxa de funções no trabalho para calcular o [!UICONTROL custo efetivo do trabalho]. </p> <p>Para um projeto, o [!DNL Workfront] usa a seguinte fórmula para calcular o [!UICONTROL custo efetivo do trabalho]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Monitorar custos</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>por exemplo, se um usuário registrar 5 horas para uma tarefa com um [!UICONTROL Tipo de Custo] de [!UICONTROL Usuário por hora] e sua taxa horária for de US$ 100,00, o [!UICONTROL custo efetivo do trabalho] será de US$ 500,00.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Receita efetiva] </td> 
   <td> <p>A [!UICONTROL receita efetiva] de um projeto ou tarefa é a quantidade de dinheiro associada às [!UICONTROL horas efetivas] do projeto ou tarefa. </p> <p>Para obter informações sobre o monitoramento da receita no [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão geral de faturamento e receita</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Início efetivo]</td> 
   <td>O carimbo de data e hora de quando um usuário altera um objeto em andamento no trabalho atribuído a ele.</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Metodologia ágil]</td> 
   <td>Um tipo de metodologia baseada na evolução colaborativa de necessidades e soluções com equipes multifuncionais. Ela estimula a flexibilidade e a mudança com base em uma linha do tempo fixa.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Equipe Ágil]</td> 
   <td>Diferencia-se de uma equipe tradicional porque realiza seu trabalho prospectivo a partir de uma lista de pendências e trabalha nela dentro de um período de tempo definido, chamado de [!UICONTROL Iteração].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Todas as Minhas Equipes]</td> 
   <td> <p>Quando isso é referenciado em [!UICONTROL filtros], este campo exibe usuários que pertencem a qualquer uma das equipes às quais o usuário conectado pertence, ou itens de trabalho atribuídos a qualquer uma das equipes às quais o usuário conectado pertence. </p> <p>Recomendamos usar este campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório, que exibirá informações diferentes dependendo de quem fizer login para visualizá-lo, pois as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data da alocação]</td> 
   <td> <p>Esse campo pode ser encontrado nos seguintes tipos de relatórios:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Projeto] (Dados financeiros)</li> 
     <li>[!UICONTROL Hora orçada]</li> 
    </ul> <p>Para um<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->relatório de [!UICONTROL Projeto (Dados financeiros)]: </p> 
    <ul> 
     <li>Crie este relatório ao tentar entender <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> a quantidade de [!UICONTROL Horas planejadas] atribuídas aos seus recursos.</li> 
     <li> <p>A [!UICONTROL Data da alocação] é o primeiro dia (domingo) de uma semana em que a alocação de uma [!UICONTROL Função no trabalho] a uma tarefa começa. Um recurso ([!UICONTROL Função no trabalho]) pode ter tantas [!UICONTROL Datas de alocação] quantas semanas houver durante a [!UICONTROL Duração] das tarefas às quais está atribuído. Se as tarefas se estenderem por vários meses, o primeiro dia de um mês também pode se tornar uma [!UICONTROL Data da alocação], se cair dentro da [!UICONTROL Duração] da tarefa.</p> <p>Por exemplo, você pode ter uma [!UICONTROL Função no trabalho] atribuída a uma tarefa que se estende por 3 semanas e tem 90 [!UICONTROL Horas planejadas]. Essas horas são distribuídas uniformemente durante a duração da tarefa, o que faz com que todos os dias, 6 [!UICONTROL Horas planejadas] sejam atribuídas à sua função no trabalho:</p> <p><em> [!UICONTROL Horas planejadas diárias] = [!UICONTROL Total de Horas planejadas]/ Número de [!UICONTROL Dias de trabalho] durante a [!UICONTROL Duração] da tarefa </em> </p> <p>Como resultado, há três [!UICONTROL Datas de Alocação], uma para cada domingo de cada semana durante a [!UICONTROL Duração] da tarefa, cada uma com um determinado número de [!UICONTROL Horas Planejadas] associadas a elas.<br>Se a tarefa começar no meio da última semana de um mês e terminar duas semanas após o início de um novo mês, ela terá quatro [!UICONTROL Datas de Alocação]: uma para cada domingo de cada semana durante a [!UICONTROL Duração] da tarefa e uma para o primeiro dia do novo mês.</p> <p>Para aproveitar essas informações ao máximo, recomendamos que você crie um relatório de Projeto <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> (Dados Financeiros) e adicione um agrupamento de matriz para a [!UICONTROL Data da alocação] e, em seguida, agrupe os resultados semanalmente, mensalmente, trimestralmente ou anualmente para obter os dados mais precisos.<br>Para obter informações sobre como criar um agrupamento de matriz, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Criar um relatório de matriz</a>.</p> </li> 
    </ul> <p>As informações financeiras são preenchidas nos relatórios de [!UICONTROL Projeto (Dados financeiros)] somente quando os dados associados a elas têm menos de 5 anos. Por exemplo, se uma função no trabalho foi alocada a uma tarefa em janeiro de 2015 e hoje é setembro de 2021, um campo financeiro como a [!UICONTROL Data da alocação] da função no trabalho não é preenchido no relatório de [!UICONTROL Projeto (Dados financeiros)]. </p> 
    <div> 
     <p>Para um relatório de [!UICONTROL Hora orçada]:</p> 
     <ul> 
      <li>Crie este relatório ao tentar entender a quantidade de [!UICONTROL Horas orçadas] alocadas aos seus recursos ou aos seus projetos no Planejador de recursos.</li> 
      <li> <p>A [!UICONTROL Data da alocação] é o primeiro dia (um domingo) da semana para a qual você orçou as horas no [!UICONTROL Planejador de recursos]. </p> <p><b>DICA</b></p> <p>Se uma semana se dividir entre dois meses, ela gerará duas linhas no relatório: uma correspondente ao primeiro dia da semana (o último domingo do primeiro mês) e a segunda linha exibirá o primeiro dia do segundo mês. </p> <p>Por exemplo, se você orçou 8 horas para um usuário para a semana de 30 de junho (domingo) a 6 de julho (sábado), as duas linhas mostram uma [!UICONTROL Data da alocação] de 30 de junho e 1º de julho. </p> </p> <p>Para obter informações sobre como orçar recursos no [!DNL Resource Planner], consulte o artigo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Orçar recursos no [!DNL Resource Planner] usando as visualizações de [!UICONTROL Projeto] e [!UICONTROL Função]</a>.</p> <p>Para obter informações sobre como criar um relatório de [!UICONTROL Hora orçada], consulte <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Relatório: Hora orçada</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Avisos]</td> 
   <td> <p>Uma forma de comunicar aos usuários informações dentro do sistema. Esta informação frequentemente vem do [!DNL Workfront] para o administrador ou do administrador para o usuário. </p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Enviar avisos</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Integração de aplicativos]</td> 
   <td>Um aplicativo geralmente representa um conector para um aplicativo de software, mas também pode representar funções especiais que manipulam dados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisão do aprovador]</td> 
   <td> <p>No relatório de [!UICONTROL Aprovação de provas], este campo exibe decisões de aprovação de provas para provas que não estão mais ativas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estágio do aprovador]</td> 
   <td>No [!UICONTROL Relatório de aprovação de prova], esse campo exibe informações sobre um estágio atual de provas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aprovação]</td> 
   <td> <p>Um determinado item de trabalho, como uma tarefa, documento ou folha de horas, pode exigir que um supervisor ou outro usuário aprove o item de trabalho. Esse processo é chamado de aprovação. </p> <p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Visão geral do processo de aprovação</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data da aprovação]</td> 
   <td>No relatório [!UICONTROL Aprovação de prova], esse campo exibe a data de aprovação da prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aprovador]</td> 
   <td>Um usuário ou função de trabalho que precisa aprovar um determinado item de trabalho, ou o usuário que aprova entradas de horas em folhas de horas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuído a]</td> 
   <td> <p>Em um relatório de [!UICONTROL Tarefa ou problema], esse campo exibe o Proprietário da tarefa ou o problema, ou o [!UICONTROL Responsável principal]. Também é possível filtrar ou agrupar por esse campo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuição]</td> 
   <td>Um usuário, função de trabalho ou equipe atribuída a um problema ou tarefa. Projetos, portfólios ou programas não podem ter atribuições.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuições]</td> 
   <td> <p>Em um relatório de [!UICONTROL Tarefa] ou [!UICONTROL Problema], esse campo exibe uma lista de todas as entidades (usuários, funções de trabalho, equipes) atribuídas à tarefa ou problema. Você pode filtrar por esse campo usando os campos [!UICONTROL Usuários das atribuições] e [!UICONTROL Funções das atribuições]. Você pode filtrar pela equipe atribuída à tarefa ou problema usando o campo Equipe. Não é possível agrupar um relatório por este campo.</p> <p>Os itens de trabalho colocados na [!UICONTROL Lixeira] continuarão a ser exibidos em alguns relatórios que se referem ao objeto [!UICONTROL Atribuição] onde um modificador de filtro [!DNL OR] é usado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Funções das atribuições]</td> 
   <td>
   <p>Em um relatório de [!UICONTROL Tarefa] ou [!UICONTROL Problema], esse campo exibe informações sobre as funções de trabalho atribuídas às tarefas ou problemas. Este campo exibe [!UICONTROL Proprietários principais], bem como outras funções de trabalho atribuídas a tarefas ou problemas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status das atribuições]</td> 
   <td> <p>Em um relatório de atribuição, tarefa ou problema, o [!UICONTROL Status das atribuições] exibe se os usuários atribuídos a um item de trabalho clicaram no botão [!UICONTROL Trabalhar nisso] ou [!UICONTROL Concluído] para aceitar ou concluir o trabalho, respectivamente. Existem os seguintes [!UICONTROL Status das atribuições]:</p> 
    <ul> 
     <li><b>[!UICONTROL Solicitado]</b>: o usuário foi atribuído à tarefa ou ao problema, mas ainda não clicou no botão [!UICONTROL Trabalhar nisso] para começar a trabalhar nele.</li> 
     <li><b>[!UICONTROL Trabalhando]</b>: o usuário clicou no botão [!UICONTROL Trabalhando nisso] e está trabalhando no item no momento. </li> 
     <li><b>[!UICONTROL Concluído]</b>: o usuário clicou no botão [!UICONTROL Concluído] e concluiu seu trabalho no item. </li> 
    </ul> <p>Para obter mais informações, consulte a visão geral do botão <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Trabalhar nisso] e [!UICONTROL Concluído]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Equipes de atribuição]</td> 
   <td>
   <p>Em um relatório de [!UICONTROL Tarefa] ou [!UICONTROL Problema], esse campo exibe informações sobre as equipes atribuídas às tarefas ou problemas. O campo exibe [!UICONTROL Proprietários principais], bem como outras equipes atribuídas a tarefas ou problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuários das atribuições]</td> 
   <td>
   <p>Em um relatório de [!UICONTROL Tarefa] ou [!UICONTROL Problema], esse campo exibe informações sobre os usuários atribuídos às tarefas ou problemas. Este campo exibe [!UICONTROL Proprietários principais], bem como outros usuários atribuídos a tarefas ou problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atributo]</td> 
   <td>Um atributo é um traço de um objeto [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Área de auditoria]</td> 
   <td> <p>Auditorias são mensagens do sistema que registram uma ação que aconteceu no Workfront. Os seguintes tipos de auditoria são registrados:</p> 
    <ul> 
     <li>[!UICONTROL Alteração no escopo]</li> 
     <li>[!UICONTROL Ação de anexo]</li> 
     <li>[!UICONTROL Edição geral]</li> 
     <li>[!UICONTROL Alteração de status]</li> 
     <li>[!UICONTROL Observação]</li> 
     <li>[!UICONTROL Entrada combinada]</li> 
     <li>[!UICONTROL Entrada de erro]</li> 
     <li>[!UICONTROL Alteração de status]</li> 
     <li>[!UICONTROL Alteração de assinatura]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trilha de auditoria]</td> 
   <td>A coleção de notas gerada automaticamente por eventos que são rastreados por meio das Alterações registradas ([!UICONTROL Áreas de auditoria]). Cada nota registra quem fez a ação, o que fizeram e quando fizeram.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automática e mediante alteração]</td> 
   <td> <p>Um dos tipos de [!UICONTROL Atualizações de projeto]. Isso recalculará as linhas do tempo Projetadas e Planejadas do Projeto quando o processo de recálculo noturno for executado e quando qualquer atualização for feita no projeto ou nas tarefas dentro do Projeto. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecionar o tipo de atualização do projeto </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Disponibilidade</p></td> 
   <td> <p>Esse termo é usado em relação à "disponibilidade de usuários" ou "disponibilidade de recursos" e ilustra o tempo que o recurso (usuário ou função no trabalho) está disponível para trabalhar. </p> 
   <p>O Workfront calcula a disponibilidade de usuários usando vários campos e dependendo de quais configurações das preferências de gerenciamento de recursos estão no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências de gerenciamento de recursos</a>. </p>
   <p>Para obter mais informações sobre a disponibilidade de recursos, consulte <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introdução ao gerenciamento de recursos</a>.</p>
   Se preferir, a “capacidade” também é usada para se referir à disponibilidade de recursos. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Somente automático]</td> 
   <td> <p>Um dos tipos de [!UICONTROL Atualizações de projeto]. Isso recalculará as linhas do tempo projetadas e planejadas quando o processo de recálculo noturno for executado.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecionar o tipo de atualização do projeto</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Trabalho “Tudo normal”, que contribui para a execução das principais metas diárias de negócios.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Lista de pendências]</td> 
   <td>A área em um ambiente Ágil em que novos problemas são mantidos até que estejam prontos para serem trabalhados.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Linha de base]</td> 
   <td>Uma fonte de dados para avaliar as iterações em um ambiente Ágil.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Despesa faturável]</td> 
   <td> <p>Uma despesa marcada como faturável para o cliente. Pode ser uma despesa planejada ou real.</p> <p>Os campos Custo da despesa planejada e faturável e Custo efetivo da despesa faturável estão disponíveis para serem adicionados a exibições e relatórios. Eles não aparecem nas páginas de detalhes do projeto ou da tarefa.</p>
   <p>Você pode encontrar esses campos nos seguintes tipos de relatórios:</p>
   <ul>
   <li>Linha de base</li>
   <li>Modelo</li>
   <li>Projeto (Dados financeiros)</li>
   </ul>
   <p>Para obter mais informações sobre como marcar uma despesa como faturável, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Gerenciar despesas do projeto</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Registro de cobrança]</td> 
   <td> <p>Registra a receita, as horas ou as despesas que podem ser faturadas. Essas informações podem ser usadas para criar faturas em um sistema contábil externo.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Criar registros de cobrança</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Status do registro de cobrança</td> 
   <td> <p>Em um relatório de Hora ou Registro de cobrança, o status de um registro de cobrança indica se ele foi faturado ou não. Não é possível excluir um projeto ou editar um horário associado a um registro de cobrança faturado. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Criar registros de cobrança</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Identidade visual]</td> 
   <td><p>O processo de personalizar o [!DNL Workfront] para dar à interface uma aparência que espelhe sua empresa, usando suas cores e logotipos.</p><p><strong>OBSERVAÇÃO</strong><br>Se sua organização foi integrada à [!DNL Adobe Experience Cloud], a identidade visual não estará disponível.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navegação estrutural]</td> 
   <td> <p>A área na parte superior da página que mostra a localização hierárquica de onde o usuário está no aplicativo.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Para obter mais informações, consulte <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Visão geral de navegações estruturais</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status do orçamento]</td> 
   <td> <p>Este campo é obsoleto. Qualquer informação que esse campo possa exibir está relacionada a um recurso que o [!DNL Workfront] removeu e o campo não pode ser atualizado. </p> <p>Esse campo mostra se o projeto foi adicionado ao [!UICONTROL Planejador de Capacidade] e se o cálculo de orçamento foi concluído para ele. O campo [!UICONTROL Planejador de Capacidade] foi removido do [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is  not added to the capacity planner, its value is <i>Not Included</i>.  </li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is  added to the Capacity Planner but is excluded from the budget calculation,  the value is <i>Included but not Calculated</i>.  </li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is  added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Detalhamento]</td> 
   <td> <p>No Workfront Planning, é possível exibir registros conectados na visualização da linha do tempo de um registro usando o recurso Detalhamento. </p>
   <p>Detalhar os registros por suas conexões permite visualizar as linhas do tempo de outros registros conectados e entender como elas podem afetar o desempenho e os prazos de seus registros. </p>
   <p>Os registros conectados são exibidos aninhados em seus respectivos registros. </p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/planning/views/manage-the-timeline-view.md">Gerenciar a exibição da linha do tempo</a>. </p>
   </td> 
    </tr>

<tr> 
   <td>[!UICONTROL Data de conclusão orçada]</td> 
   <td> <p>Este campo é obsoleto. Qualquer informação que esse campo possa exibir está relacionada a um recurso que o [!DNL Workfront] removeu. Não é possível atualizar esse campo. </p>
   <p> Esse campo ainda está visível em relatórios e listas do [!UICONTROL projeto].</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custos orçados]</td>

<td> <p>Esse é o custo associado aos recursos de orçamento de um projeto. </p>
   <p>O campo é exibido nestas áreas do [!DNL Workfront] com os seguintes nomes:</p>
   <ul>
   <li><strong>[!UICONTROL Custos orçados]</strong>: no painel [!UICONTROL Resumo do business case]</li>
   <li><strong>[!UICONTROL Custo]</strong>: nas áreas de [!UICONTROL Utilização] ao exibir informações por [!UICONTROL Custo]</li>
   <li><strong>[!UICONTROL Custos orçados do projeto]</strong>: em listas e relatórios</li>
   </ul>   
    <p>O valor de [!UICONTROL Custos orçados] do projeto é calculado usando a seguinte fórmula:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Para obter mais informações sobre como calcular o [!UICONTROL Custos orçados] e compreender vários nomes para este conceito no [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcular custo orçado do projeto</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas orçadas]</td> 
   <td> <p>As horas orçadas para os recursos do trabalho que precisam concluir nos projetos. Esse campo se refere às horas orçadas na área [!UICONTROL Orçamento de recursos] do [!UICONTROL Business Case] (ou no [!UICONTROL Planejador de recursos]) para o projeto ou para os recursos do projeto.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Noções básicas dos [!UICONTROL Custos trabalhistas orçados] e as [!UICONTROL Horas orçadas] para os projetos</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Para obter informações sobre como orçar usuários no [!DNL Resource Planner], consulte o artigo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Recursos de orçamento no [!DNL Resource Planner] usando as exibições [!UICONTROL Projeto] e [!UICONTROL Função]</a>. </p> 
    <p>As horas orçadas na área [!UICONTROL Orçamento de recursos] do [!UICONTROL Business Case] ou do [!UICONTROL Planejador de recursos] são exibidas nas seguintes áreas do [!DNL Workfront] e com os seguintes nomes:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>Nome de exibição de [!UICONTROL Horas orçadas]</strong></td> 
        <td><strong>Áreas de [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Horas]</td> 
        <td>Área de [!UICONTROL Orçamento de recursos] do [!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Planejador de recursos] exibido por [!UICONTROL Horas]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Horas orçadas]</td> 
        <td> <p>Exibição de [!UICONTROL Horas] do relatório Utilização</p> <p>Para obter mais informações sobre o relatório [!UICONTROL Utilização], consulte o artigo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Visão geral do relatório [!UICONTROL Utilização de recursos]</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Horas orçadas]</td> 
        <td> <p>Relatório [!UICONTROL Horas orçadas]</p><p>O objeto [!UICONTROL Horas orçadas] no relatório Horas orçadas se refere às informações relacionadas a uma ferramenta de gerenciamento de recursos obsoleta. Somente o campo "[!UICONTROL Horas orçadas]" nesse relatório refere-se às horas orçadas na área [!UICONTROL Planejador de recursos] ou [!UICONTROL Orçamento de recursos] do [!UICONTROL Business Case] do projeto. </p> <p>Para obter mais informações sobre como criar um relatório, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Horas orçadas do Planejador de recursos] </td> 
        <td> <p>Encontrado nos seguintes relatórios:</p>
        <ul>
        <li>Relatório [!UICONTROL Projeto]
        <li>Relatório [!UICONTROL Projeto (dados financeiros)]
        <li>Relatório da [!UICONTROL Tarefa]
        <li>Relatório [!UICONTROL Problema]
        <li>Relatório [!UICONTROL Horas orçadas]</li>
        </ul>
         <p>Para obter mais informações sobre como criar um relatório, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Qualquer outra menção de [!UICONTROL Horas orçadas] no [!DNL Adobe Workfront] se refere às horas orçadas que usam recursos obsoletos que foram removidos do Workfront. Esses são campos somente para visualização e não são atualizados com as informações atuais quando você usa as ferramentas atuais de orçamento de recursos. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the  Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy  Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy  Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial  Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custos trabalhistas orçados]</td> 
   <td> <p>Este é o custo associado às horas que você, como gerente de recursos, destina ao orçamento das funções no trabalho, considerando o trabalho necessário para concluir os projetos. </p> <p>O [!UICONTROL Custos trabalhistas orçados] em um relatório de projeto é calculado usando a seguinte fórmula:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Este campo pode se referir ao seguinte:</p> 
    <ul> 
     <li> <p>Custos de mão de obra exibidos na área [!UICONTROL Orçamento de recursos] do [!UICONTROL Business Case] ou no [!UICONTROL Planejador de recursos] associados ao custo de funções no trabalho em um projeto. Para obter informações sobre como calcular o [!UICONTROL Custos trabalhistas orçados], consulte o artigo <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Noções básicas dos Custos trabalhistas orçados] e [!UICONTROL Horas orçadas] para projetos</a>.</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Custos de mão de obra exibidos na área [!UICONTROL Orçamento de recursos] do [!UICONTROL Business Case] que refletem os [!UICONTROL Custos de pessoas] estimados em uma iniciativa vinculada ao projeto do [!DNL Scenario Planner] quando você usa o planejador de cenários para orçar seus recursos de projeto. Para obter informações sobre iniciativas, consulte <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Visão geral das iniciativas no planejador de cenários</a>. </p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Visão geral do [!DNL Scenario Planner]</a>. </p> </li> 
     <p>Ela é exibida nestas áreas com os seguintes nomes:</p>
   <ul>
   <li><strong>[!UICONTROL Custos trabalhistas orçados]</strong>: na área [!UICONTROL Orçamento de recursos] do [!UICONTROL Business Case].
   <li><strong>[!UICONTROL Custos orçados]</strong>: na exibição [!UICONTROL Custos] do relatório [!UICONTROL Utilização]
   <p>Para obter mais informações, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Exibir informações sobre a utilização de recursos</a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: no projeto do [!DNL Resource Planner] ou nas exibições de [!DNL Role], ao visualizar por Custo
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: nos seguintes relatórios: 
   <ul>
    <li>Relatório [!UICONTROL Projeto]</li>
    <li>Relatório [!UICONTROL Projeto (dados financeiros)]</li>
    <li>Relatório da [!UICONTROL Tarefa]</li>
    <li>Relatório [!UICONTROL Problema]</li>
    <li>Relatório [!UICONTROL Horas orçadas]</li> 
    </ul>
    <p>Para obter mais informações sobre como criar um relatório, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in  Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>  .  </p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Data inicial orçada]</td> 
  <td> <p>Este campo é obsoleto. Qualquer informação que esse campo possa exibir está relacionada a um recurso que o [!DNL Workfront] removeu. Não é possível atualizar esse campo.</p>
  <p>Estas áreas foram removidas do [!DNL Workfront]. </p> 
  <p>O campo ainda está visível nos relatórios e listas do [!UICONTROL projeto].</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gráfico burndown]</td> 
   <td>Um gráfico de linhas que fornece uma representação visual do trabalho concluído e restante.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>Ferramenta usada para avaliar se um projeto deve ser movido do status [!UICONTROL Ideia] para o status [!UICONTROL Planejamento]. Em outras palavras, um [!UICONTROL business case] ajuda a organização a decidir se vale a pena iniciar e concluir o projeto ou não, principalmente ao compará-lo com outros projetos de um portfólio.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Criar um [!UICONTROL Business Case] para um projeto</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas orçadas de Business Case]</td> 
   <td> <p>Este campo é obsoleto. Qualquer informação que esse campo possa exibir está relacionada a um recurso que o [!DNL Workfront] removeu. Não é possível atualizar esse campo.</p> <p>Esse campo ainda está visível em listas e relatórios de projeto e de [!UICONTROL tarefa]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuição calculada]</td> 
   <td> <p>Um dos [!UICONTROL Tipos de duração] da tarefa. Isso calculará a porcentagem de um dia de trabalho de 8 horas que o usuário atribuído à tarefa será alocado para a tarefa, com base na [!UICONTROL Duration] da tarefa e no [!UICONTROL Work Required].</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Tarefa [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabalho calculado]</td> 
   <td> <p>Um dos [!UICONTROL Duration Types] da tarefa. Isso calculará o [!UICONTROL Work Required] em uma tarefa, considerando a [!UICONTROL Duration] e as porcentagens de [!UICONTROL Assignment] do usuário (que se baseiam em um dia de trabalho de 8 horas).</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão geral da [!UICONTROL Duration] e [!UICONTROL Duration Type] da tarefa</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>No Workfront, um relatório de calendário é um relatório dinâmico no qual os usuários podem visualizar a data e outros detalhes importantes de um evento, incluindo a data de vencimento, o status do trabalho e o usuário a quem o evento é atribuído.</p> <p> Para obter mais informações sobre relatórios de calendário, consulte <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Visão geral dos relatórios de calendário</a>.</p>
   <p> No Workfront Planning, uma exibição de Calendário é um tipo de exibição para um tipo de registro que exibe registros em um calendário. Você deve ter uma licença adicional para acessar o Workfront Planning. </p>
    </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Can Start]</td> 
   <td> <p>Este campo indica se uma tarefa está pronta para ser iniciada. Se o início estiver pronto, o campo [!UICONTROL Can Start] na tarefa será definido como [!UICONTROL True]. </p> <p>Para obter mais informações, consulte a <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">visão geral “[!UICONTROL Can Start]” para tarefas</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.  </li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.  </li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>Capacidade</p> </td> 
   <td> <p>Um tempo disponível do recurso quando ele pode ser alocado para trabalho. Consulte “Disponibilidade”. </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Category]</p> </td> 
   <td> <p>Uma categoria é um formulário personalizado. Você pode criar relatórios para esse objeto e pode mostrá-lo em outros relatórios de objeto. Nem todos os objetos podem ter um formulário ou categoria personalizada. Os seguintes objetos podem ter um formulário personalizado: <br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Expense]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL User]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Category Name]</td> 
   <td> <p>Quando adicionada como uma coluna à visualização de qualquer um dos seguintes objetos, exibe uma lista de todos os formulários personalizados associados a esses objetos:</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]<br></li> 
     <li>[!UICONTROL Issue]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Expense]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL User]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Management]</td> 
   <td>Uma área de prática com foco na definição, compreensão e adaptação do trabalho planejado a alterações nos fatores de escopo, programação, custo e recursos.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Order]</td> 
   <td>Um tipo de problema relacionado a um projeto que descreve uma alteração solicitada no escopo acordado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Only]</td> 
   <td>Um dos [!UICONTROL Update Types] do projeto. Atualiza somente as linhas do tempo do [!UICONTROL Project Projected] e do [!UICONTROL Planned] quando são feitas atualizações nas tarefas ou quando são realizadas edições no projeto ou nas tarefas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Order]</td> 
   <td> <p>Um dos tipos de [!UICONTROL Issue], geralmente indicando que uma quantidade não planejada de trabalho deve ser feita antes que o projeto possa ser concluído.</p> <p>Para obter mais informações sobre os tipos de [!UICONTROL Issue], consulte a seção “Tipos de problema padrão” no artigo <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Personalizar tipos de problema padrão</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Child Task]</td> 
   <td>Uma tarefa que seja uma [!UICONTROL Subtask] de uma [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>A coleção de [!UICONTROL Subtasks] para uma [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] e [!UICONTROL Training]</td> 
   <td>Módulos de aprendizado, certificações, padrões ou uma comunidade de prática.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>Uma ferramenta de comunicação para que os usuários definam expectativas em relação aos itens de entrega da tarefa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit Date]</td> 
   <td>Uma ferramenta de comunicação para o usuário definir expectativas em relação aos itens de entrega da tarefa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] e [!UICONTROL Reporting]</td> 
   <td>Padrões para revisar as exceções e condições de um projeto, programa ou portfólio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>Uma [!UICONTROL Company] é uma unidade organizacional no [!DNL Workfront]. </p> 
   <p> Você pode associar um usuário ou um projeto a uma empresa. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Criar e editar empresas</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion date]</td> 
   <td> <p>A data em que um projeto, tarefa ou problema está definido para ser concluído. Há vários tipos de [!UICONTROL Completion dates] no [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Actual Completion Date]. Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Visão geral da [!UICONTROL Actual Completion Date] do projeto</a>.</li> 
     <li>[!UICONTROL Planned Completion Date]. Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Definir a [!UICONTROL Planned Completion Date] do projeto</a> e <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Visão geral da [!UICONTROL Planned Completion Date] da tarefa</a>.</li> 
     <li>[!UICONTROL Projected Completion Date]. Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Visão geral da [!UICONTROL Projected Completion Date] de projetos, tarefas e problemas</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Day]</td> 
   <td>O dia, relativo ao início do [!UICONTROL Template], em que uma [!UICONTROL Template Task] ou um [!UICONTROL Template] deve estar concluído.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Mode]</td> 
   <td> <p>Indica como um projeto será marcado como [!UICONTROL Complete]. Pode ter dois valores:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: um usuário deve alterar o status do projeto para [!UICONTROL Complete].</li> 
     <li>[!UICONTROL Automatic]: o status do projeto será alterado automaticamente para [!UICONTROL Complete] quando todas as tarefas do projeto estiverem 100% concluídas e todos os problemas estiverem fechados.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>É uma representação visual do progresso de uma tarefa, problema ou projeto.</p> <p>Para projetos, a condição pode ser definida manualmente pelo proprietário do projeto ou pode ser definida automaticamente pelo [!DNL Workfront], com base no status do progresso do projeto. </p> <p>Os valores possíveis para a condição do projeto são:</p> 
    <ul> 
     <li>[!UICONTROL On Target]</li> 
     <li>[!UICONTROL At Risk]</li> 
     <li>[!UICONTROL In Trouble]</li> 
    </ul> <p>Para obter mais informações sobre as condições do projeto, consulte o artigo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Visão geral da [!UICONTROL Project Condition] e [!UICONTROL Condition Type]</a>.</p>
     <p>Você pode associar condições de tarefas e problemas a um número que pode ser exibido em relatórios. As listas abaixo exibem os nomes e números padrão para condições de tarefas e problemas. O administrador do sistema pode atualizar os nomes das condições e adicionar novas condições com números diferentes. Depois que um número é associado a uma condição, ele não pode ser editado.  </p> 
     <p>Para tarefas, a condição é definida manualmente pelo proprietário da tarefa. Os valores possíveis para a condição da tarefa são:</p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li> [!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> <p>Para obter mais informações sobre as condições da tarefa, consulte o artigo <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Atualizar [!UICONTROL Condition] de tarefas e problemas</a>.</p> <p>Para ocorrências, a condição é definida manualmente pelo proprietário do problema. Os valores possíveis para a condição de problema são:<br></p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li>[!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> 
   <p><b>NOTA</b></p>
    <p>Quando o campo [!UICONTROL Condition] é acompanhado nos relatórios de [!UICONTROL Journal Entry], [!UICONTROL New] e [!UICONTROL Old Number Values] exibem o número associado à condição em vez de seu nome. Se uma condição não tiver sido originalmente definida para uma tarefa ou um problema e você atualizá-la posteriormente, o lançamento documentado que captura a atualização exibirá o [!UICONTROL Old Number Value] do campo [!UICONTROL Condition] como -2.147.483.648. Consulte também “[!UICONTROL New Number Value]”, “[!UICONTROL Old Number Value]” e “[!UICONTROL Journal Entry]” neste artigo. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition Update]</td> 
   <td> <p>Este campo mostra a condição atual de tarefas, projetos ou problemas. Esta opção mostra as atualizações mais recentes que os proprietários de tarefas, projetos ou problemas indicaram no campo [!UICONTROL Update Status], juntamente com a nova condição.</p> <p>Comentários feitos em atualizações de condição não são exibidos na coluna [!UICONTROL Condition Update]. Somente a atualização principal é exibida.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connected record types]</td> 
   <td> <p>No Workfront Planning, é possível criar uma conexão entre uma das seguintes opções: </p>
   <ul>
   <li>Dois tipos de registro</li>
   <li>Um tipo de registro e um tipo de objeto do Workfront</li>
   <li>Um tipo de registro e um ativo do Adobe Experience Manager</li></ul>
   <p>A conexão de tipos de registro permite exibir informações de um registro ou tipo de objeto em outro tipo de registro.</p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/planning/architecture/connect-record-types-overview.md">Visão geral dos tipos de registros conectados</a>  </p>
  <p>O Workfront Planning exige uma licença adicional. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connected records]</td> 
   <td> <p>No Workfront Planning, depois de conectar dois tipos de registro, você pode conectar dois registros individuais desses tipos uns aos outros.  </p>
   <p>A conexão de registros permite exibir informações de um registro ou objeto de outro aplicativo em outro registro.</p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/planning/records/connected-records-overview.md">Visão geral de registros conectados</a>. </p>

<p>O Workfront Planning exige uma licença adicional. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connections]</td> 
   <td> <p>No Workfront Planning, as conexões podem se referir a tipos de registros conectados ou a registros conectados. O Workfront Planning exige uma licença adicional.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Constraint Date]</td> 
   <td> <p>Se você estiver usando uma [!UICONTROL Task Constraint] vinculada a uma data específica, como [!UICONTROL Must Start On], essa data específica se tornará a [!UICONTROL Constraint Date] da tarefa.</p> <p>As restrições de tarefa a seguir atualizam o campo [!UICONTROL Constraint Date]:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>DICA</b></p>   
     <ul> 
      <li> <p>Uma tarefa com uma [!UICONTROL Constraint] de [!UICONTROL Fixed Dates] não tem [!UICONTROL Constraint Date]. </p> </li> 
      <li> <p> A [!UICONTROL Constraint Date] só é visível em um relatório ou visualização personalizada.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>Se você estiver usando uma restrição de tarefa em uma tarefa de modelo vinculada a um dia específico, como “Deve iniciar em”, esse dia específico se tornará o dia da restrição da tarefa de modelo.</p> <p>As restrições de tarefa a seguir atualizam o campo [!UICONTROL Constraint Day]:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>DICA</b></p> <p>  O [!UICONTROL Constraint Day] só é visível em um relatório ou visualização personalizada. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Type]</td> 
   <td> <p>A tendência de agendamento de uma tarefa. Por exemplo, [!UICONTROL As Soon as Possible] agendará uma tarefa para iniciar assim que possível, e [!UICONTROL Finish No Later Than] agendará uma tarefa para ser concluída até a [!UICONTROL Constraint Date] e não depois.</p> <p>Para obter mais informações, consulte a <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">visão geral [!UICONTROL Task Constraint]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contextual Menu]</td> 
   <td>Um menu, localizado no lado esquerdo da tela, no qual os itens são alterados para se correlacionarem com o conteúdo ativo. Por exemplo, quando um usuário está visualizando um projeto, o [!UICONTROL Contextual Menu] exibirá links para informações e ferramentas relacionadas ao projeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>Um campo em um relatório de projeto ou tarefa que mostra informações sobre o usuário que é o [!UICONTROL Primary Contact] de um problema quando ele é convertido em um projeto ou tarefa. O campo também é exibido na seção [!UICONTROL Project Details], onde é exibido o nome do [!UICONTROL Primary Contact] do problema convertido. Consulte também “[!UICONTROL Primary Contact]” neste artigo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>O valor monetário que você deve gastar ao concluir um projeto, tarefa ou problema. </p> <p>Você pode rastrear vários tipos de custos de mão de obra, despesas e riscos relacionados ao projeto. Para obter informações sobre o rastreamento de custos no [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/track-costs.md">Rastrear custos</a>.</p> 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Cost Performance Index (CPI)]</td> 
   <td> <p>O [!UICONTROL Cost Performance Index (CPI)] descreve a relação a nível de projeto ou tarefa entre o custo planejado e o custo efetivo. Os gerentes de projeto analisam essa métrica para identificar tarefas ou projetos que estejam atualmente com custos abaixo ou acima do previsto em um determinado momento. O custo pode ser medido em horas ou moeda, dependendo do [!UICONTROL Performance Index Method (PIM)].</p> 
    <p> Para obter informações, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-cpi.md">Calcular Índice de desempenho de custo(CPI)</a>.</p>

</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Cost Schedule Performance Index (CSI)]</td> 
   <td> <p>O [!UICONTROL Cost Schedule Performance Index (CSI)] é um cálculo automático que combina o [!UICONTROL Cost Performance Index (CPI)] e o [!UICONTROL Schedule Performance Index (SPI)] em uma métrica geral que equilibra custo e programação. Ao multiplicar esses valores, uma única métrica pode justificar um cronograma prolongado com um orçamento menor, ou vice-versa. Os gerentes de projeto podem usar isso para determinar a integridade geral do projeto ou da tarefa quando o custo é sacrificado para cumprir o cronograma no meio do projeto.</p> 
    <p> Para obter informações, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-csi.md">Calcular Índice de desempenho do cronograma de custos</a>.</p>
    </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Cost Type]</td> 
   <td>Para uma tarefa, o [!UICONTROL Cost Type] determina como a tarefa acumulará custos. Alguns exemplos incluem [!UICONTROL Fixed Hourly], [!UICONTROL User Hourly] e [!UICONTROL User Hourly plus Fixed]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cross-Project Dependencies]</td> 
   <td> <p>Uma tarefa de um projeto depende de uma tarefa de um projeto diferente.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Criar predecessores entre projetos</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom Data]</td> 
   <td> <p>Dados exclusivos de uma organização. As organizações podem personalizar o aplicativo [!DNL Workfront] criando formulários e campos personalizados. Essas informações personalizadas podem gerar relatórios para KPIs, auditoria e mix de demandas. </p> <p>[!UICONTROL Custom Data] podem ser vinculados a:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Despesas]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Iterations]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Data Type]</td> 
   <td>A opção para especificar se um campo [!UICONTROL Custom Data] será armazenado no banco de dados como Texto, Data, Número ou Moeda.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Display Type]</td> 
   <td>O tipo de exibição de campo de um campo personalizado. Os exemplos incluem [!UICONTROL Drop-Down], [!UICONTROL Text Field], [!UICONTROL Text Area], [!UICONTROL Radio Buttons] etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Field]</td> 
   <td>Para dados personalizados que permitem ao usuário selecionar entre várias opções, esses são os valores que o usuário pode selecionar. As opções personalizadas são válidas apenas em [!UICONTROL Drop-Down], [!UICONTROL Multi-Select Drop-Down], [!UICONTROL Radio Buttons] e [!UICONTROL Checkboxes].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Form Label]</td> 
   <td>Ao usar um tipo de exibição personalizada com opções personalizadas, esse é o texto da interface do usuário que será exibido no menu suspenso, nas caixas de seleção ou nos botões de opção dessa opção personalizada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Value]</td> 
   <td>Ao usar um campo personalizado com opções personalizadas, este é o valor que será armazenado no banco de dados para uma opção específica.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom View]</td> 
   <td>Uma definição dos campos de dados ou colunas que são exibidos para cada objeto em uma lista.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>Uma organização que usa uma instância do Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome do objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Dashboards]</td> 
   <td> <p> É possível adicionar esse campo em um relatório ou em uma visualização do objeto Relatório para exibir os painéis nos quais o relatório está listado. </p> <p> Também é possível usar esse campo para filtrar relatórios listados em um painel específico. </p> <p> Para obter mais informações sobre como incluir informações do painel em relatórios de objetos de relatório, consulte a seção "Noções básicas sobre quais relatórios estão listados em painéis" no artigo <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Acessar e organizar relatórios</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Type]</td> 
   <td>Consulte "[!UICONTROL Custom Data Type]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Days Late]</td> 
   <td> <p>Esse campo mostra a diferença de data entre [!UICONTROL Planned Start] e [!UICONTROL Today] se [!UICONTROL Actual Completion Date] estiver ausente.</p> <p>Também mostra a diferença de data entre [!UICONTROL Actual Completion] e [!UICONTROL Planned Completion], quando [!UICONTROL Actual Completion Date] está presente.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Default Schedule]</td> 
   <td> <p>Horas de trabalho padrão personalizáveis a serem atribuídas a usuários e projetos dentro de uma organização. </p> <p>Os cronogramas são usados para calcular as datas planejadas, de início e de conclusão das tarefas atribuídas aos usuários.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Deliverable]</td> 
   <td>Bens ou serviços quantificáveis que devem ser fornecidos após a conclusão de um projeto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>Pontuação e priorização dos processos de admissão.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Department Goals]</td> 
   <td>Metas exclusivas de um departamento específico, focadas em melhorar as métricas operacionais no departamento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency]</td> 
   <td>O vínculo entre duas tarefas que exige que uma tarefa mude de status antes que a outra também possa mudar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency Type]</td> 
   <td> <p>O tipo de relação de cronograma entre uma tarefa e o(s) predecessor(es). Um exemplo é [!UICONTROL Finish-Start], que requer que a primeira tarefa esteja Finalizada antes que a segunda possa Iniciar.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Visão geral dos tipos de dependência de tarefa</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>Qualquer arquivo anexado a um objeto dentro do [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>Sempre que o mesmo documento for enviado para o mesmo objeto, um número de versão será atribuído a ele. Os usuários podem exibir e alterar várias opções de uma versão anterior de um documento.</p> <p>Para obter mais informações, consulte <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Gerenciar versões do documento</a>.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p>A data em que uma tarefa ou um problema deve ser concluído. A data de vencimento de uma tarefa ou problema é a mesma que a data de conclusão planejada.</p>
    <p>A data de vencimento da tarefa e do problema está visível nas listas de tarefas e problemas e nos relatórios.</p> 
    <p>Consulte também a data de conclusão planejada nesta tabela. 
    </td> 
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>A janela de tempo alocada para a conclusão de um problema de tarefa ou um projeto (conforme determinado pelo número de dias entre o [!UICONTROL Planned Start] e a Conclusão planejada).</p> 
    <ul> 
     <li>Para tarefas, a Duração será um campo editável se o tipo de duração da tarefa não for Simples. Se o Tipo de duração da tarefa for Simples ou se a Restrição da tarefa for Datas fixas, o cálculo da Duração será realizado pelo Workfront.</li> 
     <li>Para problemas, a Duração é sempre um campo editável e deve representar uma estimativa de um número de dias que exigiriam que o problema fosse resolvido.</li> 
     <li>Para projetos, a Duração é um cálculo realizado pelo [!DNL Workfront] e representa a diferença em dias entre o Início planejado da tarefa mais antiga e a [!UICONTROL Planned Completion] da tarefa mais recente no projeto.</li> 
    </ul> <p>Para obter mais informações sobre a diferença entre [!UICONTROL Duration] e [!UICONTROL Planned Duration] para tarefas, consulte o artigo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Diferença entre [!UICONTROL Planned Duration] e [!UICONTROL Duration] para tarefas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration in Minutes]</td> 
   <td>Este campo exibe as mesmas informações que o campo [!UICONTROL Duration] em minutos em vez de dias. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duration per Occurrence]</td> 
   <td> <p>Isso é exibido nas caixas [!UICONTROL Detalhes da tarefa] e [!UICONTROL Editar tarefa] de um pai de tarefas recorrentes. Ela exibe a duração de cada tarefa recorrente. Para obter informações sobre como criar tarefas recorrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Criar tarefas recorrentes</a>. </p> <p> <span>As durações modificadas em tarefas recorrentes individuais não exibem o valor indicado neste campo.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Tipo de duração]</td> 
   <td> <p>Um campo de tarefa que indica como o trabalho necessário para concluir a tarefa é alocado aos responsáveis ao longo da duração da tarefa. Ela representa a relação entre a [!UICONTROL Duração] da tarefa, o [!UICONTROL Trabalho necessário] e o tempo, ou [!UICONTROL Alocação], que os recursos atribuídos devem gastar na tarefa para concluí-la. </p> <p>Este campo aparece na guia [!UICONTROL Detalhes] de uma tarefa. </p> <p>As opções para o tipo de duração de uma tarefa são:</p> 
    <ul> 
     <li>[!UICONTROL Atribuição calculada]</li> 
     <li>[!UICONTROL Trabalho calculado]</li> 
     <li>[!UICONTROL Controlado pelo esforço]</li> 
     <li>[!UICONTROL Simples]</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Tarefa [!UICONTROL Duração] e [!UICONTROL Tipo de duração]</a>.</p> 
    --&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Unidade de duração]</td> 
   <td>A unidade utilizada para medir o tempo em uma pesquisa avançada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Controlado pelo esforço]</td> 
   <td>A relação entre o número de usuários e o tempo que a tarefa levará para ser concluída. À medida que você adiciona mais usuários, o tempo total programado para a conclusão da tarefa diminui, mas a duração da tarefa permanece a mesma. Por exemplo, se uma tarefa consiste em descascar um barril de amendoins, adicionar mais pessoas diminuirá o tempo programado, mas a duração em dias-pessoa permanecerá a mesma.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo decorrido]</td> 
   <td> <p>[!UICONTROL Tempo decorrido] é uma unidade de tempo para a [!UICONTROL Duração] de uma tarefa. É o tempo entre a [!UICONTROL Data inicial planejada] e a [!UICONTROL Data de conclusão planejada] de uma tarefa que inclui feriados, finais de semana e folga. Em outras palavras, o tempo decorrido é a passagem de dias do calendário. </p> <p>[!DNL Workfront] oferece suporte às seguintes unidades de tempo decorrido para a duração da tarefa:</p> 
    <ul> 
     <li> <p>[!UICONTROL Minutos decorridos]</p> </li> 
     <li> <p>[!UICONTROL Horas decorridas]</p> </li> 
     <li> <p>[!UICONTROL Dias decorridos]</p> </li> 
     <li> <p>[!UICONTROL Semanas decorridas]</p> </li> 
     <li> <p>[!UICONTROL Meses decorridos]</p> </li> 
    </ul> <p>Para obter mais informações sobre a duração da tarefa, incluindo o tempo decorrido, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Tarefa [!UICONTROL Duração] e [!UICONTROL Tipo de duração]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End Date]</td> 
   <td> <p> Em um relatório [!UICONTROL Taxa], esta é a data em que uma nova taxa de faturamento para uma função de trabalho no nível do projeto termina.  As horas associadas ao projeto anteriores a essa data são multiplicadas por essa taxa de faturamento para calcular a receita do projeto. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engajamento]</td> 
   <td>O [!UICONTROL Indicador do desempenho do trabalho] (WPI) que indica quando o compromisso e a crença na tarefa, projeto, equipe ou organização estão diminuindo. Isso indica que você precisa agir para reviver essa crença e o compromisso. O WPI seria medido fazendo-se perguntas simples, "Você entendeu o que se esperava de você? O trabalho atribuído a você fez alguma diferença para a organização? Você fez um ótimo trabalho?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Metas da empresa]</td> 
   <td>Metas multifuncionais que contribuem para as métricas das metas da empresa.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Estimativa na conclusão]</td> 
   <td><p>Como métrica de desempenho do projeto, a Estimativa na Conclusão (EAC) representa o custo total projetado do seu projeto ou tarefa quando estiver concluído.</p>
   <p>Como configuração de projeto, permite definir como o valor de EAC deve ser calculado.</p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-eac.md">Calcular EAC (Estimativa na conclusão)</a>. </p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Data estimada de entrega]</td> 
   <td>Nos relatórios de projetos, tarefas e problemas, a data estimada de entrega é a data em que o Workfront estima que o item deve ser concluído.</td> 
  </tr>


<tr> 
   <td>[!UICONTROL Evento]</td> 
   <td>Qualquer alteração em um projeto ou tarefa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Manipulador de eventos]</td> 
   <td>Tarefas automatizadas que ocorrem quando eventos ocorrem. Um exemplo comum é uma notificação automática por e-mail.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notificação de evento]</td> 
   <td>E-mail gerado a partir de um manipulador de eventos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Despesas]</td> 
   <td>Um custo não trabalhista em tarefas ou projetos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Externo]</td> 
   <td> <p>Normalmente, esse é um tipo de licença ou um usuário com essa licença. Um usuário com esse tipo de licença só tem a capacidade de revisar informações no sistema. Não podem participar ativamente do trabalho.</p> <p>Para obter mais informações, consulte a Visão geral das licenças do <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sistema externo]</td> 
   <td>Quaisquer serviços ou softwares armazenados e controlados fora do sistema de registro designado.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>Qualquer objeto do Workfront ou as informações associadas a ele, conforme exibido no banco de dados. </p>
   <p>Por exemplo, “projeto”, “usuário” e “hora” são objetos do Workfront e também campos. "Nome", "status", "proprietário" e "data inicial" são campos do Workfront associados aos objetos acima. </p>

<p>Quando se referem a objetos, os termos "objetos" e "campos" podem ser usados como sinônimos.</p>
   <p>No escopo dos relatórios, os “campos” referem-se aos objetos ou às informações sobre o objeto que você deseja capturar no relatório.</p>

<p><b>NOTA</b></p>

<p>Nos relatórios de texto mais detalhados, os campos referem-se aos objetos ou às suas informações tal como aparecem na base de dados.</p>
   <p>Às vezes, o nome que você vê na interface do usuário é diferente do nome do campo no banco de dados. Por exemplo, “problema” é o nome do objeto na interface do Workfront, mas “opTask” é o nome do objeto (ou do campo) no banco de dados do Workfront. </p> 
   <p> É importante usar o campo tal como aparece no banco de dados ao escrever um relatório, visualização, filtro ou agrupamento no modo texto, ou ao criar um campo calculado.</p>

<p>Para obter mais informações, consulte <a href="../../../wf-api/general/api-explorer.md">Explorador de API</a> e <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Visão geral do modo texto</a>.</p>

<p>Por padrão, o Workfront vem com um conjunto de campos que definem os objetos e suas informações. Você também pode criar campos personalizados para definir objetos, mas não pode criar objetos personalizados.</p>

<p>No Workfront Planning, você pode criar campos personalizados para todos os tipos de registro. Os tipos de registros do Workfront vêm com um número muito limitado de campos. Você deve criar todos os campos do zero e associá-los aos tipos de registro. Para obter informações, consulte <a href="/help/quicksilver/planning/fields/fields-overview.md">Visão geral do campo</a>. </p> <p>O Workfront Planning exige uma licença adicional. </p>   
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Um dos principais blocos de construção de um relatório ou elemento de lista que define quais informações são exibidas na tela. Para obter mais informações sobre elementos de relatórios, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de relatório: filtros, visualizações e agrupamentos</a>.</p> <p>O filtro determina os resultados exibidos em um relatório ou em uma lista do painel [!DNL Workfront], como projetos, tarefas ou problemas.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Gerenciamento do trabalho financeiro]</td> 
   <td>Processo para gerenciar custos de mão de obra, despesas e dados de receita no [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo estabelecido]</td> 
   <td>Você pode definir um valor fixo de custo para um projeto. Isso faz parte do [!UICONTROL Custo planejado] do projeto que representa a quantidade de dinheiro necessária para concluir o projeto. Para obter informações sobre custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Receita fixa]</td> 
   <td>Você pode definir uma quantia fixa de receita para um projeto. Isso faz parte da [!UICONTROL Receita planejada] do projeto que representa a quantidade de dinheiro que você pode obter se concluir o projeto. Para obter informações sobre receitas, consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão geral do faturamento e das receitas</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sinalizadores]</td> 
   <td> <p> Este campo é igual ao dos [!UICONTROL Ícones de status], mas só está disponível para os seguintes modos de exibição: </p> 
    <ul> 
     <li> [!UICONTROL Modelos] </li> 
     <li> [!UICONTROL Despesas] </li> 
    </ul> <p> Para obter mais informações, consulte o artigo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ícones de status integrados nas visualizações</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Pastas são usadas para organizar documentos ou relatórios associados a um objeto.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (Equivalente a Tempo Integral)</td> 
   <td>O Equivalente de Tempo Integral indica a quantidade de tempo em que um recurso está disponível para trabalho. 
   O campo [!UICONTROL FTE] é exibido nas seguintes áreas: 
  <ul>
   <li> Perfil do usuário, ao editar ou criar o usuário </li>
   <li> [!UICONTROL Planejador de recursos] </li>
   <li> [!UICONTROL Planejador de cenários] (requer licença adicional para o Planejador de cenários do Workfront) </li>
   <li> Listas de usuários e relatórios </li> </ul>

<p>O [!UICONTROL FTE] deve ser um número decimal até 1 e não pode ser 0. </p>
   <p> Um [!UICONTROL FTE] de 1 (que é o padrão para o campo [!UICONTROL FTE] de um usuário, conforme definido em seu perfil) significa que um recurso (usuário ou função) trabalha o número inteiro de horas, com base no cronograma que calcula sua disponibilidade. </p>
   <p>O administrador do Workfront decide qual cronograma usar para determinar a disponibilidade do usuário.  </p>
   <ul>
   <li> Quando o [!UICONTROL Cronograma padrão] é usado, o Workfront usa o [!UICONTROL FTE] do usuário encontrado no perfil para calcular a disponibilidade. </li>
   <li> Quando o cronograma do usuário é usado, o Workfront usa a folga do usuário, o valor do [!UICONTROL Tempo de trabalho] e as horas do [!UICONTROL Cronograma padrão] para calcular o [!UICONTROL FTE] do usuário. </li> </ul>

<p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências de gerenciamento de recursos</a>.  </p>
   <p>Para obter mais informações sobre como criar cronogramas no [!DNL Workfront], consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar um cronograma</a>. </p>

<p><b>NOTA</b></p>
   <p>Para todos os cálculos no [!UICONTROL Planejador de cenários], o Workfront usa o seguinte valor: 1 [!UICONTROL FTE] = 8 Horas.</p>
   <p>Para obter mais informações, consulte <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Introdução ao [!UICONTROL Planejador de cenários]</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G - I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome do objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Gráfico de Gantt]</td> 
   <td> <p>Uma linha do tempo visual das datas do projeto em uma visualização de calendário com base nas datas planejadas ou projetadas, conforme as tarefas do projeto estão programadas atualmente.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Meta]</td> 
   <td><p>Há dois conceitos de metas no [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Metas do projeto</b>: um conjunto de objetivos de negócios acordados pelos participantes relevantes de um projeto. As metas do projeto fazem parte do Business Case de um projeto. </p> <p>Não é possível exibir as metas do projeto em listas ou relatórios, mas você pode acessá-las por meio da API. </p> <p>Para obter informações sobre as metas do projeto de Business Case, consulte <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Criar metas do Business Case </a>. </p> </li> 
     <li> <p><b>Metas estratégicas</b>: uma meta estratégica é um objetivo que você cria para planejar sua estratégia de trabalho para um período específico. Você pode criar esses tipos de metas usando o [!DNL Workfront Goals]. Sua organização deve comprar uma licença adicional e você deve ter acesso a esse recurso para poder criar metas estratégicas. [!DNL Workfront Goals] estão disponíveis somente com uma licença adicional.</p> 
     <p>Para obter mais informações, consulte Visão geral do <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals]</a>. </p> 
     <p>Você pode exibir metas estratégicas em um relatório de metas ou projetos e acessá-las por meio da API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Hierarquia de meta]</td> 
   <td> <p>Nos relatórios de [!UICONTROL Meta] e [!UICONTROL Projeto], este é um campo de coleção que mostra as metas na hierarquia às quais uma meta estratégica pertence quando se alinha a outras metas. Os objetivos são separados por um delimitador ▸. </p> <p>Apenas os pais da meta e a meta são exibidos neste campo. As metas de tarefas-filho não são exibidas. </p> <p>Para obter informações sobre como alinhar metas no [!DNL Workfront Goals], consulte a <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Visão geral do alinhamento de metas no [!DNL Workfront Goals]</a>. </p> 
   <p>Este campo só estará visível se sua organização tiver comprado o [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte Visão geral do <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals]</a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Pontuação de sucesso da meta]</td> 
   <td> Em um [!UICONTROL Relatório do projeto], esse campo era usado para fazer referência às metas de nível de projeto associadas ao [!UICONTROL Business] Case. No momento, esse campo está obsoleto e não está associado a nenhuma funcionalidade.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Goals] </td> 
   <td> <p>Em um relatório de [!UICONTROL Project], é um campo de coleta que exibe todas as metas estratégicas associadas a um projeto. As metas são separadas por vírgulas.</p> <p>Este campo só estará visível se sua organização tiver comprado o [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte a Visão geral do <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals]l</a>. Para obter mais informações sobre metas estratégicas e metas do projeto no [!DNL Workfront], consulte “[!UICONTROL Goal]” neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>Configurações de interface que afetam todos os usuários. As [!UICONTROL Global Interface Preferences] podem ser substituídas pelas [!UICONTROL User Interface Preferences].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>Um conjunto de usuários (possivelmente do mesmo departamento ou unidade de negócios) que têm acesso aos mesmos objetos. Além dos usuários, os grupos podem ser associados a portfólios, programas, projetos, <span> modelos de projeto, </span> empresas, equipes, agendamentos, modelos de layout e perfis de folha de horas.</p> <p>Você também pode conceder permissões a objetos por grupo. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Visão geral e grupos</a>.</p> <p>Em uma lista ou relatório de objetos de um dos tipos a seguir, você pode usar o campo [!UICONTROL Group] para listar quais objetos desse tipo estão associados a um grupo específico: usuário, portfólio, programa, projeto, <span>modelo de projeto</span>, empresa, equipe, agendamento, modelo de layout ou perfil da folha de horas.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Group Administrator]</td> 
   <td> <p>Usuários que gerenciam os objetos, o acesso e os usuários dos grupos de usuários designados.</p> <p> Em um relatório de [!UICONTROL Group], esse campo exibe os nomes dos usuários designados como [!UICONTROL Group Administrators] no Grupo. Para obter mais informações sobre Administradores de grupo, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group with Administration Access]</td> 
   <td> <p> Em um [!UICONTROL Layout Template], [!UICONTROL Timesheet Profile] ou [!UICONTROL Schedule report], esse campo exibe os grupos cujos administradores de grupo têm acesso para modificar o modelo. Você também pode filtrar esse relatório por esse campo. </p> <p> Para obter mais informações, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Grouping]</td> 
   <td> <p>Um elemento de relatório usado para categorizar informações em uma lista por um critério comum.</p> <p>Para obter mais informações, consulte a seção "[!UICONTROL Groupings]" no artigo <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de relatório: filtros, visualizações e agrupamentos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Handoff Date]</td> 
   <td> <p>A data em que uma tarefa fica disponível para ser realizada. A [!UICONTROL Handoff Date] é um cálculo e não pode ser definida manualmente. <br>Para obter mais informações sobre [!UICONTROL Handoff Date], consulte o artigo <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">Visão geral de [!UICONTROL Task Handoff Date]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>Um nome alternativo para descrever a área [!UICONTROL Requests] do [!DNL Workfront]. Você pode usar a área [!UICONTROL Requests] para processar tíquetes de suporte ao cliente, solicitações de projeto, tíquetes de suporte técnico etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Owner]</td> 
   <td>Em um relatório [!UICONTROL Hour], o [!UICONTROL Owner] é o usuário ao qual as horas são atribuídas. É diferente do usuário que está realmente registrando o horário. Às vezes, essas duas entidades podem ser dois usuários diferentes. <br>Para obter mais informações sobre o registro de tempo para outro usuário, consulte o artigo <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Tempo de registro</a>.</td> 
  </tr>

<tr> 
   <td>Status da hora</td> 
   <td> <p>Um atributo definido pelo Workfront para as horas efetivas que os usuários registram para tarefas, problemas ou projetos. </p>

As entradas de horas podem ter um dos seguintes status no Workfront:
<ul>
   <li><b>Enviado</b>: as horas foram registradas em um projeto, tarefa ou problema. Elas fazem parte de um registro de cobrança ou ainda não foram adicionadas a um registro de cobrança.</li>
   <li><b>Aprovado</b>: as horas foram registradas e aprovadas pelo proprietário do projeto. Elas fazem parte de um registro de cobrança ou ainda não foram adicionadas a um registro de cobrança.</li> 
   <li><b>Não aprovado</b>: as horas foram registradas e rejeitadas pelo proprietário do projeto. Elas fazem parte de um registro de cobrança ou ainda não foram adicionadas a um registro de cobrança.</li>
   <li><b>Faturado</b>: as horas foram registradas, adicionadas a um registro de cobrança e o status do registro de cobrança foi marcado como Faturado. Elas não precisavam ser aprovadas pelo proprietário do projeto.</li>
   <li><b>Faturado e Aprovado</b>: as horas foram registradas, aprovadas pelo proprietário do projeto e o status do registro de cobrança foi marcado como Faturado.</li>
   </ul>

<p>Quando as horas fazem parte de um registro de cobrança, o Status da hora indica se as horas foram aprovadas ou se o Registro de cobrança ao qual pertencem foi faturado. O Status da hora de uma entrada de hora é visível apenas em uma lista de horas ou um relatório. </p>

<p>Para obter mais informações sobre como adicionar horas a registros de faturamento, consulte a seção "Adicionar horas a registros de faturamento" no artigo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Criar registros de faturamento</a>.</p>

<p>Para obter mais informações sobre o tempo de aprovação de projetos, consulte <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Exigir tempo para ser aprovado para um projeto</a>.</p>

<p><b>DICA</b></p>

<p>As horas gerais que não estão conectadas diretamente a itens de trabalho não exibem um status de hora. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>Um atributo que pode ser definido para Horas efetivas que os usuários registram para tarefas, problemas ou projetos. Também é um atributo para as horas registradas que não estão diretamente vinculadas ao trabalho, como [!UICONTROL Vacation] e [!UICONTROL Time Off].</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Gerenciar tipos de hora</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>A ID é um indicador alfanumérico associado a cada objeto no [!DNL Workfront]. Identifica exclusivamente cada objeto no banco de dados do [!DNL Workfront]. Você pode visualizar a ID de qualquer objeto em um relatório ou uma lista para cada objeto. </p> <p><b>DICA</b></p>   <p>Você também pode exibir a ID no URL da página do objeto. Por exemplo, a ID de um projeto pode ser semelhante ao número destacado no seguinte URL, ao acessar a página [!UICONTROL Project Details]:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL IMS]</td> 
   <td>Sistema de gerenciamento de identidades. O Adobe IMS exige que você faça logon no Workfront por meio da Adobe, em vez de usar seu nome de usuário e senha do Workfront.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Individual Goals]</td> 
   <td>Metas individuais que contribuem para as métricas das metas da equipe, mas que não estão relacionadas ao desenvolvimento pessoal ou de carreira.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Inherited Access]</td> 
   <td>Função de compartilhamento que permite que o acesso se propague de um objeto para outro. Por exemplo, o acesso herdado do usuário do projeto definido nos registros do programa e do portfólio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>No [!DNL Workfront Scenario Planner], você pode dividir um plano em várias iniciativas para facilitar o gerenciamento do plano. <span>Você pode criar um relatório [!UICONTROL Initiative] e acessar as informações de [!UICONTROL Initiative] em um relatório de [!UICONTROL Project].</span></p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Visão geral do [!DNL Scenario Planner]</a>. </p> <p>O relatório [!DNL Initiative] não está visível na instância [!DNL Workfront], a menos que a empresa tenha comprado uma licença do [!DNL Workfront Scenario Planner]. Não é possível acessar [!UICONTROL Initiatives] por meio da API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>O tipo de relatório [!UICONTROL Initiative Job Role] exibe informações sobre as funções de trabalho associadas a uma iniciativa de plano no [!DNL Workfront Scenario Planner].</span> </p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">Visão geral do [!DNL Scenario Planner]</a>. </p> <p><span>Esse tipo de relatório não é visível na sua instância do [!DNL Workfront], a menos que sua empresa tenha comprado uma licença do [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role Hours]</span> </td> 
   <td> <p><span> Em um relatório [!UICONTROL Initiative Job Role], esse campo exibe o número de horas associadas a uma função de trabalho em uma iniciativa.</span> </p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">Visão geral do [!DNL Scenario Planner]</a>. </p> <p>Esse campo e o tipo de relatório [!UICONTROL Initiative Job Role] não estão visíveis na sua instância do [!DNL Workfront], a menos que sua empresa tenha adquirido uma licença do [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role Count]</td> 
   <td> <p>Em um relatório [!UICONTROL Initiative Job Role], é exibido o número de funções de trabalho específicas associadas a uma iniciativa.</p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">Visão geral do [!DNL Scenario Planner]</a>. </p> <p>Esse campo e o tipo de relatório [!UICONTROL Initiative Job Role] não estão visíveis na sua instância do [!DNL Workfront], a menos que sua empresa tenha adquirido uma licença do [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Last Published Date]</td> 
   <td> <p>Um campo em um relatório [!UICONTROL Initiative], [!UICONTROL Initiative Job Role] e [!UICONTROL Project] que exibe a data em que uma iniciativa de plano foi publicada pela última vez em um projeto. É possível publicar iniciativas para criar projetos ou atualizar projetos vinculados às iniciativas.</p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">Visão geral do [!DNL Scenario Planner]</a>. </p> <p><span>Para obter informações sobre como publicar iniciativas, consulte</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publicar cenários para criar e atualizar projetos no [!DNL Workfront Scenario Planner]</a>. Esse tipo de relatório não é visível na sua instância do [!DNL Workfront], a menos que sua empresa tenha adquirido uma licença do [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inline Search]</td> 
   <td>Uma pesquisa realizada, no processo de preencher um formulário, para localizar possíveis entradas para um campo específico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface Setup]</td> 
   <td>A área do aplicativo que permite definir Exibições personalizadas, Filtros, Agrupamentos, Controles de lista etc.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Is Company Goal]</p></td> 
   <td> <p>No [!DNL goal reports], exibe um valor "[!UICONTROL True]/ [!UICONTROL False]" para cada meta estratégica para indicar se a organização está atribuída à meta como seu proprietário. </p> 
   <p>Esse campo estará visível apenas se a organização tiver adquirido o [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte a Visão geral do <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals]</a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue]</td> 
   <td> <p>Um item de trabalho não planejado que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Ele é triado e avaliado para consideração adicional do esforço do trabalho</p> <p>Um [!UICONTROL Issue] também pode ser uma solicitação do [!UICONTROL Help Desk]. [!UICONTROL Change Orders], [!UICONTROL Requests] e [!UICONTROL Bugs] também são [!UICONTROL Issues].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Management]</td> 
   <td> <p>O processo e as regras que regem a definição de tipos de problemas e o processo de roteamento, triagem ou tráfego associado a cada tipo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Owner]</td> 
   <td>A equipe ou os usuários responsáveis por testar e concluir um problema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>Um período no qual uma equipe produz um conjunto predefinido de entregáveis.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome do objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Job Role]</td> 
   <td> <p>Usada para identificar as funções e responsabilidades diárias de um usuário. Funções no trabalho podem ser atribuídas a itens de trabalho para identificar a habilidade necessária para concluir um processo de trabalho sem atribuí-lo a um usuário específico. </p> <p>Um usuário pode ter mais de uma função. Os exemplos incluem Designer gráfico ou Consultor.</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções no trabalho</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journal Entry]</p> </td> 
   <td> <p>Um objeto reportável que fornece informações sobre atualizações do sistema para campos rastreados que aparecem na área [!UICONTROL Updates] de projetos, tarefas, problemas e outros objetos.</p> <p>Para saber mais, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Relatório na área Atualizações com um relatório de lançamento documentado</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban Flag]</td> 
   <td> <p>Em um Relatório de [!UICONTROL Task] ou Relatório de [!UICONTROL Issue], o campo [!UICONTROL Kanban Flag] exibe o status do sinalizador definido na matéria no [!UICONTROL Kanban board].  Os valores possíveis são [!UICONTROL On Track], [!UICONTROL Ready to Pull] e [!UICONTROL Is Blocked].</p> <p>Para obter mais informações sobre como definir o status do sinalizador em stories no [!UICONTROL Kanban story board], consulte o artigo <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Usar sinalizadores em stories no [!UICONTROL Kanban board]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPIs</td> 
   <td>Um valor mensurável que mostra a eficácia com que uma empresa está atingindo os principais objetivos de negócios.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>Tempo decorrido após a [!UICONTROL Planned Completion Date] da tarefa predecessora ter sido aprovada, até que a tarefa dependente possa começar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Types]</td> 
   <td> <p>O método de cálculo de [!UICONTROL Lag]. Pode ser:</p> 
    <ul> 
     <li>[!UICONTROL Days] (dias úteis)</li> 
     <li>[!UICONTROL Calendar Days] (ignorar feriados)</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL Day of Week]</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Visão geral dos tipos de defasagem</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Large Thumbnail]</td> 
   <td> <p> Em uma lista ou relatório de [!UICONTROL Document], é exibida uma visualização do documento em miniatura. </p> <p>Selecione <strong>[!UICONTROL Large Thumbnail]</strong> para exibir uma miniatura de 400 pixels de largura no relatório.</p> <p>O tamanho da miniatura é ajustado quando você modifica a largura da coluna em uma lista ou relatório.</p> <p>Consulte também "[!UICONTROL Thumbnail]" neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last 10 Viewers]</td> 
   <td> <p>Em uma lista de relatórios, esse campo exibe os nomes de até dez usuários que visualizaram o relatório mais recentemente.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>Esse campo exibe a última atualização inserida em um objeto pelo proprietário do objeto. Essa é a atividade ou interação mais recente do proprietário em um objeto.</p> <p>A coluna [!DNL Last Condition Note] estará vazia se o texto da última nota de um objeto tiver sido excluído. Quando uma nova nota é inserida no objeto, ela se torna a última nota e é exibida novamente na coluna. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Finance Update Date]</td> 
   <td>Em um relatório [!UICONTROL project], esse campo captura a data e a hora em que as finanças do projeto foram calculadas e atualizadas pela última vez. Para obter informações sobre as finanças do projeto, consulte <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Visão geral das finanças do projeto</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Note]</td> 
   <td> <p>Esse campo exibe a última atualização inserida em um objeto por qualquer usuário. Essa é a atividade ou interação mais recente em um objeto.</p> <p>A coluna [!UICONTROL Last Note] estará vazia se o texto da última nota de um objeto tiver sido excluído. Quando uma nova nota é inserida no objeto, ela se torna a última nota e é exibida novamente na coluna.</p>
   <p>Quando este campo é adicionado a um relatório da [!UICONTROL Task], as atualizações deixadas em objetos filho — como problemas, subtarefas ou documentos — da tarefa não são exibidas nessa coluna.</p> 
   <p><b>Nota</p>
   <p>A última observação adicionada a um objeto usando a API não é exibida em um relatório no Workfront. O campo [!DNL Last Note] estará vazio se a atualização mais recente em um objeto tiver sido adicionada usando a API. </p>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed By]</td> 
   <td> <p>Em uma lista de relatórios, esse campo exibe informações sobre o último usuário que visualizou o relatório.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed Date]</td> 
   <td> <p>Em uma lista de relatórios, esse campo exibe a data da última exibição do relatório.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout Template]</td> 
   <td>Definido pelo administrador do sistema ou administrador de grupo para identificar as guias e os relatórios exibidos no espaço de trabalho de um determinado usuário.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layout Type]</td> 
   <td>Em conjunto com [!UICONTROL Custom Views], o [!UICONTROL Layout Type] especifica o tipo de [!UICONTROL Custom View]. Atualmente, somente Lista está disponível. Futuramente, [!UICONTROL Detail] (a visualização de [!UICONTROL Detail] de um objeto) poderá se tornar disponível.</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there  are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.   
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.  </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>    </p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection  of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Legacy Actual Hours]</td> 
   <td> <p>Em um relatório de projeto, tarefa ou problema, [!UICONTROL Legacy Actual Hours] é a soma de todas as horas registradas no projeto, tarefa ou problema a qualquer momento, inclusive antes de maio de 2021.</p>  
   <p>As Horas efetivas legadas são exibidas como Horas efetivas na área de Detalhes de um projeto, tarefa ou problema. </p>
   <p>Consulte também <strong>Horas efetivas</strong>.
    <p>Para obter mais informações, consulte <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Visualizar horas efetivas</a>.</p>
    </td> 
  </tr>  <tr> 
   <td>[!UICONTROL License Type]</td> 
   <td>O tipo de licença alocada para um [!UICONTROL Access Level]. Será [!UICONTROL Full User], [!UICONTROL Limited User] ou [!UICONTROL Requester].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Plan]</td> 
   <td> <p>Em uma exibição ou relatório de [!UICONTROL Group], esse campo mostra o número máximo de licenças [!UICONTROL Plan] que podem ser atribuídas a usuários que têm o respectivo grupo designado como [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Work]</td> 
   <td> <p>Em uma exibição ou relatório de [!UICONTROL Group], esse campo mostra o número máximo de licenças de [!UICONTROL Work] que podem ser atribuídas a usuários que têm o respectivo grupo designado como [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>Um Tipo de licença que permite a criação de um [!DNL Access Level] que contenha privilégios somente de visualização, com a capacidade de enviar problemas, inserir observações e fazer upload de documentos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controls]</td> 
   <td> <p>Parte da [!UICONTROL Interface Setup] que permite vincular Filtros, Visualizações e Agrupamentos personalizados a usuários individuais ou globalmente a todos os usuários.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Lookup fields]</td> 
   <td> <p>No Workfront Planning, depois de estabelecer a conexão entre dois tipos de registro e vincular registros individuais, é possível fazer referência aos campos dos registros vinculados no registro do qual você está se conectando.</p>
   <p>Por exemplo, se você conectar um tipo de registro Campanha a um tipo de objeto Projeto do Workfront, é possível exibir o campo Orçamento dos projetos conectados nos registros da campanha. O campo de projeto Orçamento é um campo de pesquisa de projetos em uma campanha.</p> <p>Os valores dos campos de pesquisa são preenchidos automaticamente nos registros aos quais estão conectados.</p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/planning/records/connected-records-overview.md">Visão geral de registros conectados</a>.</p>
   <p>O Workfront Planning exige uma licença adicional.</p>
    </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome do objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Manual Only]</td> 
   <td> <p>Um dos [!UICONTROL Update Types] de um [!UICONTROL Project]. Esta configuração permite que as linhas do tempo [!UICONTROL Project Projected] e [!UICONTROL Planned] sejam atualizadas apenas quando você clicar em “[!UICONTROL Recalculated Timelines]”. Projetos configurados dessa maneira serão ignorados durante o processo noturno de recálculo e quando o projeto ou as tarefas no projeto forem atualizadas.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecionar o [!UICONTROL Update Type] do projeto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Refere-se ao usuário conectado no momento. </p> <p>Recomendamos usar este campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório, que exibirá informações diferentes dependendo de quem fizer login para visualizá-lo, pois as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max Users]</td> 
   <td> <p>Este campo é obsoleto. Qualquer informação que este campo possa exibir está relacionada a um recurso que o [!DNL Workfront] removeu e o campo não pode ser atualizado. </p> <p>Em versões anteriores do [!DNL Workfront], você poderia atualizar este campo ao criar ou editar uma função de trabalho. Ele exibia o número total de usuários que podiam ser associados a uma função em cada projeto. Um valor zero é permitido para um número ilimitado de usuários que podem ser atribuídos a um projeto. </p>O campo ainda está visível em alguns relatórios e listas, mas as informações exibidas não podem ser atualizadas. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Um marcador que pode ser associado a uma tarefa para indicar que um ponto-chave no projeto foi atingido quando a tarefa for concluída. Geralmente, você pode usar marcos para mostrar um evento significativo, como a conclusão de uma fase do projeto ou um conjunto de atividades críticas. Os [!UICONTROL Milestones] são normalmente associados a tarefas principais. Você deve criar marcos antes de anexá-los a tarefas. Para obter informações sobre marcos, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Criar um caminho de marcos</a> e <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Associar marcos a tarefas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Milestone Path]</td> 
   <td>Uma coleção de [!UICONTROL milestones]. [!UICONTROL Milestone Paths] são usados para distinguir projetos com certos tipos de [!UICONTROL Milestones] de projetos com um conjunto diferente de [!UICONTROL Milestones].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone Task]</td> 
   <td>Uma tarefa sinalizada para indicar um evento relatável a ser medido.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>Uma única etapa dentro de um cenário no [!DNL Workfront Fusion] que executa alguma função com base no aplicativo associado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Primary Role]</td> 
   <td> <p>Quando referenciado em filtros, exibe os usuários que têm a mesma [!UICONTROL Primary Role] do usuário conectado ou itens de trabalho atribuídos à [!UICONTROL Primary Role] do usuário conectado.</p> <p>Recomendamos usar este campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório, que exibirá informações diferentes dependendo de quem fizer login para visualizá-lo, pois as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Home Team]</td> 
   <td> <p>Quando referenciado em filtros, este campo exibe os usuários que pertencem à [!UICONTROL Home Team] do usuário conectado ou os itens de trabalho atribuídos à [!UICONTROL Home Team] do usuário conectado. </p> <p>Recomendamos usar este campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório, que exibirá informações diferentes dependendo de quem fizer login para visualizá-lo, pois as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Naming convention]</td> 
   <td>Um conjunto de regras em toda a organização que usa dados para criar nomes de projetos, tarefas e itens de entrega.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>Uma integração que não requer codificação manual ou configuração de API. Também chamada de integração “pronta para uso”.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navigation Menu]</td> 
   <td>O painel superior central do aplicativo que tem links para as áreas principais do [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL New Number Value]</td> 
   <td>Em um relatório de [!UICONTROL Journal Entry], é exibido o valor atualizado de um campo que substitui o [!UICONTROL Old Number Value].
   Para obter mais informações, consulte “[!UICONTROL Old Number Value]” neste artigo.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Non-Billable Expense]</td> 
   <td> <p>Uma despesa que não está marcada como faturável para o cliente. Pode ser uma despesa planejada ou real.</p> <p>Os campos Custo de despesa não faturável planejado e Custo de despesa não faturável real estão disponíveis para serem adicionados a visualizações e relatórios. Eles não aparecem nas páginas de detalhes do projeto ou da tarefa.</p>
   <p>Você pode encontrar esses campos nos seguintes tipos de relatórios:</p>
   <ul>
   <li>Linha de base</li>
   <li>Modelo</li>
   <li>Projeto (Dados financeiros)</li>
   </ul>
   <p>Para obter mais informações sobre como marcar uma despesa como faturável, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Gerenciar despesas do projeto</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Non Work Day]</td> 
   <td>Um dia que não está alocado para a conclusão de atribuições. Normalmente, é um dia de férias, feriado ou fim de semana. A exibição do termo no explorador de API. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Observação]</td> 
   <td>Um comentário ou atualização feito em um objeto do [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note Text]</td> 
   <td> <p>Exibe o texto de uma atualização inserida por um usuário em qualquer objeto. </p> </td> 
  </tr>

<tr data-mc-conditions="">

<td>[!UICONTROL Number of Linked Goals]</td> 
   <td> <p>Em um relatório [!UICONTROL Project], é o número de metas estratégicas associadas ao projeto. Para obter informações sobre como associar projetos a metas estratégicas, consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Adicionar projetos a metas no [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Para obter informações sobre metas estratégicas, consulte também "[!UICONTROL Goal]" neste artigo.</p> 
   <p>Esse campo estará visível apenas se a organização tiver adquirido o [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Adicionar projetos a metas no [!UICONTROL Adobe Workfront Goals]</a>. </p> </td> 
  </tr>

<tr>

<td>[!UICONTROL Número de Filhos]</td> 
   <td> <p>Em um relatório de [!UICONTROL Project], esse é o número de tarefas filhas ou subtarefas que uma tarefa tem. 
   <p><b>DICA</b></p>
   Você pode adicionar o cálculo de <code>{numberOfChildren}</code> a um campo personalizado calculado no formulário personalizado de tarefa para mostrar em um campo personalizado o número de filhos da tarefa. Para obter mais informações, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md">Adicionar um campo calculado a um formulário</a>. 
    </td>


</tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>As informações exibidas no [!DNL Adobe Workfront] são representadas por objetos armazenados no banco de dados do [!DNL Workfront]. Os objetos direcionam as informações no Workfront. Alguns exemplos de objetos são:</p> 
    <ul> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Custom forms]</li>
     <li>[!UICONTROL Custom fields]</li>  
     <li>[!UICONTROL Horas]</li> 
     <li>[!UICONTROL Billing Rates]</li> 
     <li>[!UICONTROL Modelos]</li> 
     <li>[!UICONTROL Template tasks]</li>

<p><b>NOTA</b></p>
  <p>Esta não é uma lista completa. </p>

</ul> <p>Para obter mais informações, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Noções básicas de objetos no [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object Types]</td> 
   <td>Se você criar um relatório ou uma lista contendo todos os formulários personalizados, poderá usar esse campo como uma exibição ou um filtro para ver quais tipos de objeto estão associados a cada formulário. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Old Number Value]</td> 
   <td>Em um relatório de [!UICONTROL Journal Entry], é exibido o valor original de um campo antes de ele ser atualizado. Depois que o valor de um campo for atualizado, ele será exibido como o [!UICONTROL New Number Value] em um relatório de [!UICONTROL Journal Entry]. Para obter mais informações, consulte também "[!UICONTROL New Number Value]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL On Change Only]</td> 
   <td> <p>Um dos tipos de [!UICONTROL Atualizações de projeto]. Quando selecionado, as linhas do tempo [!UICONTROL Project Projected] e [!UICONTROL Planned] são atualizadas apenas quando uma atualização ou alteração é feita no projeto ou em uma tarefa dentro do projeto. Não atualiza o projeto todas as noites.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecionar o tipo de atualização do projeto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>O nome do [!UICONTROL Issue] no banco de dados do [!DNL Workfront], usado em relatórios do modo de texto ou dados personalizados calculados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>Um problema ou tarefa que não está concluído, mas sendo trabalhado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>Abreviação de Organograma. É um gráfico que mostra a hierarquia de uma organização. Também está na guia na tela de detalhes do [!UICONTROL User] que exibe e permite configurar as relações entre [!UICONTROL Company] e [!UICONTROL Reporting] do [!UICONTROL User].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organizational Setup]</td> 
   <td>Define [!UICONTROL Companies], [!UICONTROL Groups] e [!UICONTROL Security Profiles] para sua organização.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Other Groups]</td> 
   <td> <p>Em um relatório ou exibição que lista usuários, esse campo exibe todos os grupos dos quais cada usuário é membro. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency]</span> </td> 
   <td> 
    <div> 
     <p>Em um relatório de [!UICONTROL Job Role], essa é a moeda associada a uma função no trabalho. É uma substituição da [!UICONTROL Base Currency], conforme estabelecida na área [!UICONTROL Setup] pelo administrador do [!DNL Workfront]. </p> 
     <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções no trabalho</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Billing/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>Em um relatório de [!UICONTROL Job Role], essa é a taxa de cobrança por hora da função no trabalho usando a [!UICONTROL Override Currency] selecionada da função no trabalho.</p> 
     <p> Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções no trabalho</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Cost/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>Em um relatório de [!UICONTROL Job Role], essa é a taxa de custo por hora da função no trabalho usando a [!UICONTROL Override Currency] selecionada da função no trabalho. </p> 
     <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções no trabalho</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Owner]</td> 
   <td>O usuário responsável pela conclusão do objeto designado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Owner Type]</span> </td> 
   <td> 
    <div> 
     <p>Em um relatório de [!UICONTROL Goal], exibe o tipo de proprietário atribuído a uma meta estratégica. A seguir estão os tipos de proprietário de meta:</p> 
     <ul> 
      <li> <p>[!UICONTROL User]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>Nenhum valor é exibido nesse campo quando o proprietário da meta é sua organização. </p> 
     <p>Isso requer uma licença adicional. Para obter informações sobre o [!DNL Workfront Goals], consulte a visão geral do <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals]</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome do objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Parameter]</td> 
   <td> <p>Um [!UICONTROL parameter] é um campo personalizado. Você pode criar um relatório para todos os parâmetros ou campos personalizados em seu sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent]</td> 
   <td>Em um relatório, este campo mostra informações sobre o item-pai do objeto. Por exemplo, em um relatório de [!UICONTROL issue], pode mostrar informações sobre a tarefa ou o projeto em que o problema está registrado; em um relatório de tarefa, pode mostrar informações sobre a tarefa-pai direta ou sobre o projeto. Para obter mais informações sobre quais objetos podem ter itens-pai no [!DNL Workfront], consulte a seção “Interdependência e hierarquia de objetos” no artigo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Noções básicas de objetos no [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Lag]</td> 
   <td>O tempo que deve decorrer entre o início da [!UICONTROL Parent Task] e o início da [!UICONTROL Subtask].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Task]</td> 
   <td>Também conhecida como [!UICONTROL Summary Task]. Esta é uma tarefa que tem Subtarefas (também chamada de [!UICONTROL Children Tasks]). A [!UICONTROL Duration], o [!UICONTROL Work Required] e o [!UICONTROL Percent Complete] da tarefa-pai são calculados a partir das Subtarefas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Part-Time Resources]</td> 
   <td>Um usuário licenciado que tem menos capacidade do que o cronograma padrão definido no sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percent Complete]</td> 
   <td> <p>Um campo de projeto, tarefa ou problema que mostra qual porcentagem do trabalho associado à tarefa, projeto ou problema foi concluída.</p> <p>Você pode atualizar esse campo manualmente para problemas e tarefas de trabalho. </p> <p>Para projetos e tarefas-pai, esse campo é um acúmulo de todas as tarefas de trabalho e você não pode atualizá-lo manualmente. </p> <p>Para obter mais informações, consulte a <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Visão geral [!UICONTROL Percent Complete] do projeto</a>.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Performance Index Method (PIM)]</td> 
   <td> <p>O [!UICONTROL Performance Index Method (PIM)] do projeto controla o método que o Adobe Workfront usa para calcular as métricas de desempenho do projeto, como Índice de Desempenho de Custo (CPI), Índice de Desempenho do Cronograma de Custo (CSI), Índice de Desempenho do Cronograma (SPI) e Estimativa na Conclusão (EAC).</p> 
   <p>O Workfront calcula esses valores usando horas ou custo.</p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/set-pim.md">Definir o PIM (Método de Índice de Desempenho)</a>.</p>
   </td> 
  </tr>
 <tr> 
   <td>[!UICONTROL Permission]</td> 
   <td> <p>Direitos concedidos a um usuário em um objeto, normalmente fornecidos para que ele possa concluir o trabalho no item ou visualizá-lo. Você pode conceder permissões para:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Views]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL Groupings]</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral das permissões de compartilhamento em objetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Este é um tipo de licença completa no sistema do [!DNL Workfront]. Os usuários devem ter este recurso para acessar todos os recursos no [!DNL Workfront].</p> <p>Para obter mais informações, consulte a visão geral das licenças do <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (no [!DNL Scenario Planner])</td> 
   <td> <p>Um plano é o objeto principal ao trabalhar com o Planejador de cenários do [!DNL Workfront]. Você pode destacar a estratégia para o futuro próximo e de longo prazo da sua empresa, identificar cada resultado de alto nível e adicioná-lo como um plano ao planejador de cenários do [!DNL Workfront]. </p> <p>Você não pode exibir planos do [!DNL Scenario Planner] em um relatório e não pode acessá-los por meio da API do [!DNL Workfront]. </p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte a <a href="../../../scenario-planner/scenario-planner-overview.md">Visão geral do [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned]</td> 
   <td> <p>O intervalo de tempo dentro do qual algo está programado para ocorrer. Ao criar projetos, tarefas ou problemas no [!DNL Workfront], você estabelece as datas planejadas de início e término, bem como o período planejado durante o qual elas ocorrem. Esses valores representam a intenção original ou estimativa de quanto tempo um item deve levar para ser concluído. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Benefit]</td> 
   <td>Essa é uma entrada manual para o gerente de projetos estimar se a conclusão de um projeto traria algum benefício monetário para a organização. A especificação desse valor pode fazer parte da montagem de um [!UICONTROL Business Case] para o projeto. Você deve ter permissões [!UICONTROL Manage] para o projeto para atualizar esse valor.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Planned Budgeted Hours]</td> 
   <td> <p>Em um relatório de [!UICONTROL Budgeted Hour], é exibido o número de horas orçadas para projetos ou [!UICONTROL Job Roles] no [!UICONTROL Resource Planner]. </p> <p>Para obter informações sobre projetos ou funções de orçamento no [!UICONTROL Resource Planner], consulte o artigo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Recursos de orçamento no [!UICONTROL Resource Planner] usando os modos de exibição [!UICONTROL Project] e [!UICONTROL Role]</a>. Para obter informações sobre o relatório [!UICONTROL Budgeted Hours], consulte o artigo <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Relatório: hora orçada</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>Você pode definir manualmente a [!UICONTROL Planned Completion Date] de uma tarefa, projeto ou problema para uma data de sua escolha. Se você não definir a [!UICONTROL Planned Completion Date], o [!DNL Workfront] a definirá automaticamente. Quando definida automaticamente, a [!UICONTROL Planned Completion Date] será: [!UICONTROL Planned Start Date] + [!UICONTROL Duration]</p> <p>Para obter mais informações, consulte os seguintes artigos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Visão geral da tarefa [!UICONTROL Planned Completion Date]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Definir a [!UICONTROL Planned Completion Date] do projeto</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Cost]</td> 
   <td> <p>Um total do [!UICONTROL Planned Labor Cost] e do [!UICONTROL Planned Expense Cost] do projeto. Isso não inclui o [!UICONTROL Planned Risk Cost] no projeto.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Date Alignment]</td> 
   <td> <p>Esse é um indicador automático que o Workfront atribui a projetos, tarefas e problemas para mostrar quando um item será concluído em relação à data de conclusão planejada. </p>
   <p>A seguir, estão os valores possíveis para o indicador Alinhamento à data planejada: </p>
<ul>
<li>Será terminado na data de conclusão planejada</li>
<li>Será terminado antes da data de conclusão planejada</li>
<li>Será terminado depois da data de conclusão planejada</li></ul>
<p>O Alinhamento à data planejada está visível em listas e relatórios de projetos, tarefas e problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration]</td> 
   <td> <p>A [!UICONTROL Planned Duration] de uma tarefa geralmente é a mesma que a [!UICONTROL Duration] da tarefa. Representa a diferença em dias entre a [!UICONTROL Planned Start] e a [!UICONTROL Planned Completion Dates] da tarefa. </p> <p>Quando a tarefa tem um tipo de [!UICONTROL Duration] de [!UICONTROL Effort Driven], a [!UICONTROL Planned Duration] pode diferir da [!UICONTROL Duration] da tarefa com base nos recursos atribuídos a ela. </p> <p>Por exemplo, se uma tarefa com um Tipo de [!UICONTROL Duration] de [!UICONTROL Effort Driven] tiver uma [!UICONTROL Duration] de 3 dias e você atribuir um recurso com horário integral à tarefa, a [!UICONTROL Planned Duration] também será de 3 dias. Se você atribuir três recursos com um cronograma de tempo integral à mesma tarefa, a [!UICONTROL Duration] permanecerá 3 dias, mas a [!UICONTROL Planned Duration] será de 1 dia. A [!UICONTROL Planned Duration] também altera as datas de [!UICONTROL Planned Start] e [!UICONTROL Planned Completion] da tarefa para refletir a nova [!UICONTROL Planned Duration]. Como resultado, a linha do tempo do projeto também é afetada. </p> <p>Para obter mais informações sobre a diferença entre [!UICONTROL Duration] e [!UICONTROL Planned Duration] para tarefas, consulte o artigo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Diferença entre [!UICONTROL Planned Duration] e [!UICONTROL Duration] para tarefas</a>.</p> <p>Projetos e problemas não têm uma [!UICONTROL Planned Duration]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration Minutes]</td> 
   <td> <p>Os [!UICONTROL Planned Duration Minutes] de um projeto ou problema são a [!UICONTROL Duration] do projeto ou problema em minutos. </p> <p>As tarefas não têm um campo [!UICONTROL Planned Duration Minutes]. </p> <p>[!UICONTROL Template Tasks] têm um campo [!UICONTROL Planned Duration Minutes] que exibe a [!UICONTROL Planned Duration] da tarefa em minutos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Expense Cost]</td> 
   <td> <p>A soma dos [!UICONTROL Planned Amounts] de todas as despesas registradas para um projeto ou uma tarefa.</p> <p><b>EXEMPLO</b></p>
   <p>Se você criar uma despesa para a Tarefa 1 e inserir US$ 600,00 no campo [!UICONTROL Planned Amount], o [!UICONTROL Planned Expense Cost] para essa tarefa será de US$ 600,00. </p> 
   <p>Para um projeto, o [!DNL Workfront] usa a seguinte fórmula para calcular o [!UICONTROL Planned Expense Cost]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Hours]</td> 
   <td> <p>Esse campo aparece nas áreas de [!UICONTROL projects], [!UICONTROL tasks] e problemas, relatórios de projetos, tarefas ou problemas, além de ferramentas de gerenciamento de recursos como o [!UICONTROL Resource Planner], o [!UICONTROL Workload Balancer] e o relatório de [!UICONTROL Utilization]. </p> <p>Ele mostra o número de horas que o proprietário do projeto estima que cada tarefa ou problema deve levar para ser concluído. Para projetos, geralmente é um pacote das [!UICONTROL Planned Hours] das tarefas no projeto. </p> <p>O campo [!UICONTROL Planned Hours] pode exibir informações diferentes, dependendo de onde você as exibe. Para obter informações sobre horas planejadas, consulte <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Visão geral das horas planejadas</a>.</p> <p>As horas planejadas são armazenadas em minutos no banco de dados do [!DNL Workfront]. Ao escrever cálculos usando esse campo, considere o fato de que as horas sejam exibidas como minutos.<br></p> <p>Por padrão, as horas planejadas são distribuídas igualmente a todos os dias dentro da duração de um item de trabalho e também igualmente para todos os recursos atribuídos à tarefa. Os usuários podem atualizar o número diário de horas planejadas para um item de trabalho ou as horas planejadas individuais para cada destinatário.</p> <p>A atualização desse campo é diferente para projetos, tarefas e problemas: </p> 
    <ul> 
     <li> <p>Para problemas, você pode atualizar manualmente esse campo.As horas planejadas de problemas não são adicionadas às horas planejadas do projeto. </p> <p><b>DICA</b></p> <p>Em um relatório de problemas, um dos campos [!UICONTROL Planned Hours] é substituído pelo campo [!UICONTROL Work].O campo exibe o número de horas planejadas do problema. Para obter mais informações, consulte os campos "trabalho" ou "[!UICONTROL Work]" nesta tabela. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Para tarefas, você pode atualizar manualmente esse campo quando o [!UICONTROL Duration Type] da tarefa é [!UICONTROL Calculated Assignment] ou [!UICONTROL Simple]. Este campo é calculado pelo [!DNL Workfront] quando o [!UICONTROL Duration Type] da tarefa é [!UICONTROL Calculated Work] ou [!UICONTROL Effort Driven].<br>Para obter informações sobre [!UICONTROL Task Duration], consulte o artigo <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão geral da [!UICONTROL Duration] e [!UICONTROL Duration Type] da tarefa</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Para projetos, o [!DNL Workfront] calcula as horas planejadas adicionando todas as horas planejadas de todas as tarefas do projeto. </p> </li> 
    </ul> <p><b>DICA</b></p> <p>Você também pode exibir [!UICONTROL Planned Hours] nos relatórios de [!UICONTROL project], [!UICONTROL task] ou [!UICONTROL issues] usando o modo de texto e os campos adicionais de referência. Para obter mais informações, consulte os campos "<code>work</code>", "[!UICONTROL Work]" e "<code>workRequiredExpression</code>" nesta tabela. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Labor Cost]</td> 
   <td> 
    <p>Para uma tarefa, a taxa por hora do usuário ou da função multiplicada pelo número de horas atribuídas ao usuário ou à função.</p> <p>Para um projeto, é um total de todos os [!UICONTROL Planned Labor Costs] de todas as tarefas.</p> <p>O uso da taxa do usuário ou da função depende do tipo de custo selecionado para determinada tarefa. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md">Rastrear custos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Revenue]</td> 
   <td> <p>Tarefas e projetos podem exibir um valor para [!UICONTROL Planned Revenue] no [!DNL Workfront]. A [!UICONTROL Planned Revenue] representa a quantia associada às [!UICONTROL Planned Hours] das tarefas no projeto. Para projetos, também pode incluir a [!UICONTROL Fixed Revenue] do projeto. </p> <p>Para tarefas, é a receita associada às [!UICONTROL Planned Hours] de tarefas. As horas planejadas de todas as tarefas são acumuladas até as horas planejadas do projeto para contribuir com o cálculo das [!UICONTROL Planned Hours] do projeto. </p> 
   <p>[!DNL Workfront] calcula a [!UICONTROL Planned Revenue] de tarefas e projetos usando as seguintes fórmulas:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>A [!UICONTROL Planned Revenue] do projeto exibida na área [!UICONTROL Project Details] e nos relatórios do projeto é diferente da Receita planejada exibida no relatório [!UICONTROL Utilization]. </p> <p>A [!UICONTROL Planned Revenue] na área [!UICONTROL Project Details] reflete a receita da tarefa, bem como a receita fixa do projeto. A [!UICONTROL Planned Revenue] no [!UICONTROL Utilization Report] exibe a [!UICONTROL Planned Revenue] associada apenas às tarefas do projeto. </p> 
     <p><b>EXEMPLO</b></p>  
      <p>Se o projeto tiver uma tarefa com 10 horas, atribuída a um consultor com uma taxa por hora de US$ 20, e o projeto tiver US$ 100 de [!UICONTROL Fixed Revenue], o relatório de [!UICONTROL Utilization] exibirá US$ 200 para [!UICONTROL Planned Revenue] (a [!UICONTROL Planned Revenue] associada às horas da tarefa). A seção [!UICONTROL Project Details] exibe US$ 300 (a [!UICONTROL Planned Revenue] da tarefa e a receita fixa do projeto). </p> 
    <p>Para obter informações sobre o rastreamento da receita em [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Visão geral de faturamento e receita</a>. </p> 
    <p>Para obter informações sobre os cálculos de [!UICONTROL Planned Revenue] no [!UICONTROL Utilization report], consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Visualizar informações de utilização de recursos</a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Risk Cost]</td> 
   <td> <p>O total do [!UICONTROL Potential Cost] de todos os riscos no projeto, considerando sua probabilidade de ocorrência. Esse valor não está incluído no [!UICONTROL Planned Cost] do projeto.</p> <p>O [!UICONTROL Planned Risk Cost] de um projeto é calculado pela seguinte fórmula:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>Uma coleção de guias e seções definida pelo administrador, exibida no [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>Um componente de uma guia em uma página de portal ou painel. Geralmente, um único relatório, gráfico, calendário ou lista de informações principais.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>Uma guia em um portal ou painel que contém até três seções do portal.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Uma coleção de projetos com características unificadoras. Esses projetos geralmente competem pelos mesmos recursos, orçamento ou período. Você pode dividir portfólios em programas e associar os projetos aos programas antes que eles sejam adicionados a um portfólio.</p> <p>Para obter mais informações sobre portfólios, consulte <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Noções básicas sobre a metodologia de portfólio</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>Uma área de prática focada no gerenciamento de uma coleção ou de programas e esforços de projeto relacionados.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>Uma ferramenta do [!DNL Workfront] que ajuda na avaliação e priorização de projetos em um portfólio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Owner]</td> 
   <td>A parte interessada responsável pela definição de prioridades e pelo orçamento de um portfólio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Potential Risk Cost]</td> 
   <td>Esse é um campo do projeto que você pode localizar em listas e relatórios. Mostra o custo potencial dos riscos associados ao projeto, caso ocorram. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular o custo do risco em potencial </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessor]</td> 
   <td> <p>Uma tarefa que deve ser concluída antes da conclusão de uma tarefa dependente. Também é uma tarefa marcada como uma [!UICONTROL Dependency] para outra tarefa. Os predecessores permitem que o planejador defina a lógica de dependência sequencial, de modo que uma tarefa seja iniciada após a conclusão de outra.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Visão geral de predecessores de tarefa</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Company]</td> 
   <td>A empresa à qual o usuário pertence, conforme designado nas configurações do usuário. As empresas também podem ser associadas a projetos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Contact]</td> 
   <td><p>O [!UICONTROL Primary Contact] é o criador de um problema e é automaticamente designado pelo [!DNL Workfront] quando alguém cria o problema. Você pode atualizar manualmente esse campo se tiver permissões de [!DNL Manage] para o problema. Um problema pode ter apenas um Contato principal.</p> 
   <p>Se você alterar o Contato principal, o usuário originalmente designado como contato principal ainda terá acesso de [!UICONTROL Manage] ao problema.</p>
   <p>Ao converter um problema em uma tarefa ou projeto, o usuário designado como [!UICONTROL Primary Contact] do problema torna-se o [!UICONTROL Converted Issue Originator] do projeto ou tarefa. Se o [!UICONTROL Primary Contact] do problema for atualizado após a conversão do problema, o [!UICONTROL Converted Issue Originator] será preservado como [!UICONTROL Primary Contact] do problema no momento em que a conversão ocorrer. Consulte também "[!UICONTROL Converted Issue Originator]" neste artigo.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>Um valor que pode ser atribuído a uma tarefa, problema ou projeto para designar a respectiva importância. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>Em uma [!UICONTROL Note] ou [!UICONTROL Document], essa opção torna esse objeto oculto para a maioria dos visualizadores. Para uma Fila de solicitação de ajuda privada, somente os usuários na equipe do projeto podem enviar problemas para essa fila (ou projeto) por meio da área [!UICONTROL Requests].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>Todas as informações sobre uma conta de usuário.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>Um subconjunto em um portfólio em que projetos semelhantes podem ser agrupados para alcançar um benefício bem definido.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Management]</td> 
   <td>Gerenciamento de dependências interprojetos, riscos, problemas, requisitos e soluções para manter a integridade do programa e obter os benefícios definidos do programa.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Owner]</td> 
   <td>A parte interessada responsável por supervisionar e organizar atividades para garantir que as metas do projeto se alinhem aos objetivos da empresa.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>Em um relatório de [!UICONTROL Goal], exibe a porcentagem de progresso de uma meta estratégica em relação à sua conclusão. A porcentagem do progresso é exibida como um número. Para obter informações sobre metas estratégicas, consulte também "[!UICONTROL Goal]" nesta tabela.</p> <p>Esse campo só estará visível se a organização tiver adquirido o [!DNL Workfront] Goals. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Adicionar projetos a metas no [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progress Status]</td> 
   <td> <p>Em um relatório de Projeto, Tarefa e Meta, esse campo exibe seu status do progresso. Para obter mais informações, consulte os seguintes artigos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Visão geral do status do progresso do projeto</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Visão geral do status do progresso da tarefa</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Visão geral do progresso e da condição da meta no [!DNL Adobe Workfront Goals]</a> </p>
     <p>O relatório de [!UICONTROL Goal] e o [!UICONTROL Progress Status] para o campo [!DNL goals] estarão visíveis apenas se a organização tiver adquirido o [!DNL Workfront Goals]. Para obter informações sobre metas estratégicas no [!DNL Workfront Goals], consulte a Visão geral do <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals]</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>Uma grande quantidade de trabalho que deve ser concluída dentro de um período específico e deve usar um orçamento e um número de recursos específicos. Para torná-lo gerenciável, divida o projeto em uma série de tarefas. Concluir todas as tarefas resulta na conclusão do projeto. Para obter informações sobre o planejamento de um projeto, consulte a <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Visão geral de como planejar um projeto</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Assignment Planned Hours]</td> 
   <td> <p>Em um relatório de [!UICONTROL Initiative Job Role], exibe o número de [!UICONTROL Planned Hours] associadas a uma função no trabalho atribuída a tarefas ou problemas no projeto. Esse campo e o tipo de relatório [!UICONTROL Initiative Job Role] não são exibidos na sua instância do [!DNL Workfront], a menos que sua empresa tenha adquirido uma licença do [!DNL Workfront Scenario Planner]. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">Visão geral do [!DNL Workfront Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Details]</td> 
   <td>Os detalhes do status atual de um projeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Budgeted Cost]</td> 
   <td> <p> Esse é o [!UICONTROL Budgeted Cost] de um projeto, conforme exibido em listas e relatórios.</p><p>Consulte também "[!UICONTROL Budgeted Cost]" neste artigo.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>Um conjunto de políticas que regem os limites para criação de projetos, categorização e nomenclatura dos projetos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>Em um relatório [!UICONTROL Hour], esse campo é reservado para informações financeiras vinculadas às horas registradas com o tipo de hora de [!UICONTROL Project Time]. Os projetos podem ter as próprias taxas de faturamento e, se uma hora for registrada diretamente em um projeto, essas taxas serão usadas nos cálculos. Com base nas configurações, os projetos também podem ter moedas diferentes e pode haver uma conversão de moeda para essas horas. O objeto [!UICONTROL Project Overhead] permite que o [!DNL Workfront] obtenha essas informações.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Owner]</td> 
   <td>O usuário responsável pelo gerenciamento do escopo, linha do tempo e atribuições de um projeto. O aprovador padrão para ordens de alteração, alterações financeiras e itens de entrega.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>Processos para desenvolver e manter o cronograma do projeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Sponsor]</td> 
   <td>Um perfil de parte interessada designado ao qual cada um dos seus usuários deve se relacionar. No [!DNL Workfront], eles são designados como [!UICONTROL Access Levels]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Teams]</td> 
   <td> <p>A coleção de usuários ou funções atribuída a um projeto</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Visão geral da equipe de projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project tracking]</td> 
   <td>Os dados usados para medir a integridade e o escopo de um projeto</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projected]</td> 
   <td> <p>Uma estimativa do carimbo de data e hora de quando o trabalho será concluído com base nas horas planejadas e na porcentagem concluída de uma tarefa, problema ou projeto.</p> <p>Refere-se a datas ou à [!UICONTROL Duration] de tarefas, problemas ou projetos. Geralmente, designa datas e durações mais reais em relação ao ciclo dos itens de trabalho, depois que algum trabalho já foi concluído ou que algum tempo passou. </p> <p>Por exemplo, a [!UICONTROL Projected Completion Date] de uma tarefa é a data em que o [!DNL Workfront] estima que a tarefa será concluída, com base em quanto trabalho foi feito até o momento, quantas pessoas estão atribuídas a ela e quanto tempo passou desde a data inicial.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Deadline]</td> 
   <td> <p>Em relatórios que contêm o objeto [!UICONTROL Document Version] (como um relatório [!UICONTROL Document Version] e [!UICONTROL Proof Approval]), esse campo exibe o dia da semana, a data, a hora do dia e o ano do prazo de prova.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Decision]</td> 
   <td> <p>Em relatórios que contêm o objeto [!UICONTROL Document Version] (como um relatório [!UICONTROL Document Version] e [!UICONTROL Proof Approval]), esse campo exibe o status de decisão da prova (pendente, alterações necessárias ou aprovado)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td> <p>Em relatórios que contêm o objeto [!UICONTROL Document Version] (como um relatório [!UICONTROL Document Version] e [!UICONTROL Proof Approval]), esse campo exibe o nome da prova.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Pages]</td> 
   <td> <p>Em relatórios que contêm o objeto [!UICONTROL Document Version] (como um relatório [!UICONTROL Document Version] e [!UICONTROL Proof Approval]), esse campo exibe o número de páginas incluídas na prova.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Progress]</td> 
   <td> <p>Em relatórios que contêm o objeto [!UICONTROL Document Version] (como um relatório [!UICONTROL Document Version] e [!UICONTROL Proof Approval]), esse campo exibe o status do progresso da prova ([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commented] ou [!UICONTROL Decision Made]).</p> <p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Visão geral do progresso da prova</a> em <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Visão geral do progresso e do status da prova</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>Um processo de revisão no qual um ou mais usuários marcam e comentam o conteúdo que deve ser alterado em uma imagem, um documento de texto, um vídeo ou um conteúdo interativo da Web.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>Em uma [!UICONTROL Note] ou um [!UICONTROL Document], essa opção torna esse objeto acessível a outros usuários ou até mesmo a pessoas de fora do [!DNL Workfront]. Para uma [!UICONTROL Help Request Queue], [!UICONTROL Public] significa que todos os usuários que podem enviar problemas a um projeto podem enviá-los por meio da área [!UICONTROL Requests].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>A percepção da qualidade do trabalho na organização.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>Também chamada de Fila de suporte técnico ou [!UICONTROL Help Request Queue]. Este é um projeto que foi publicado na área [!UICONTROL Requests] para permitir que os usuários enviem problemas para ele. Geralmente, as filas são criadas para tópicos específicos, como [!UICONTROL Bugs], [!UICONTROL Project Requests], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Properties]</td> 
   <td>Essas configurações definem regras de envio de problemas para um projeto que está sendo publicado na área [!UICONTROL Requests].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Topic]</td> 
   <td> <p>Uma propriedade em uma [!UICONTROL Help Request Queue] que permite que os usuários enviem um problema para selecionar um tópico. Os tópicos podem:</p> 
    <ul> 
     <li>Estar associados a um formulário de dados personalizado.</li> 
     <li>Atribuir o problema automaticamente a um usuário, função ou equipe por meio da regra de roteamento definida para o tópico selecionado.</li> 
     <li>Mover o problema para um projeto ou uma fila diferente por meio da regra de roteamento definida no tópico selecionado.</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Criar tópicos da fila</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>Em um relatório [!UICONTROL Access Level], você pode indicar manualmente uma [!UICONTROL Rank] do [!UICONTROL Access Level]. Isso ajuda você, como administrador do [!DNL Workfront], a identificar visualmente o nível de complexidade associado a cada nível de acesso. Por exemplo, você pode fornecer números mais baixos para níveis de acesso mais complexos (nível de [!UICONTROL Plan]) e números mais altos para níveis de acesso menos complexos (nível de [!UICONTROL Requester]). Não é possível classificar os níveis de acesso padrão. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>Este campo em um relatório de tarefa indica se uma tarefa [!UICONTROL Agile] foi marcada como [!UICONTROL Ready] na lista de pendências. Esse sinalizador se aplica somente a tarefas [!UICONTROL Agile], que são tarefas atribuídas a uma equipe [!UICONTROL Agile]. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p>No Workfront Planning, um registro é uma instância exclusiva de um tipo de registro.</p>
<p>Depois de adicionar um tipo de registro a um espaço de trabalho, você pode começar a adicionar registros desse tipo na página do tipo de registro.</p>
<p>Por exemplo, “Campanha” pode ser um tipo de registro e “Campanha de verão para EMEA” é um registro do tipo de registro Campanha.</p>
<p>Para obter informações sobre como criar registros, consulte <a href="/help/quicksilver/planning/records/create-records.md">Criar registros</a>. </p> <p>O Workfront Planning exige uma licença adicional. </p></td> 
  </tr>


<tr> 
   <td>[!UICONTROL Record type]</td> 
   <td> <p>O tipo de objeto do Workfront Planning.</p>
<p>Diferentemente do Workfront, onde os tipos de objeto são predefinidos, no Workfront Planning você pode criar seus próprios tipos de objeto. Os tipos de objeto do Workfront Planning são chamados de tipos de registro.</p>
<p>Por exemplo, no Workfront, os tipos de objeto Programa, Portfólio, Projeto, Tarefa ou Problema já estão criados.</p>
<p>No Workfront Planning, você pode criar qualquer tipo de registro que atenda aos fluxos de trabalho da sua organização. Posteriormente, você poderá definir como os tipos de registros se relacionam entre si ou formam dependências.</p> Para obter informações sobre como criar tipos de registro, consulte <a href="/help/quicksilver/planning/architecture/create-record-types.md">Criar tipos de registro</a>. </p> <p>O Workfront Planning exige uma licença adicional. </p></td> 
  </tr>

<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Recurrence Frequency]</td> 
   <td> <p>Um campo exibido na caixa [!UICONTROL Task Details] ou [!UICONTROL Edit Task] de uma tarefa principal de tarefas recorrentes. É a frequência com que as tarefas se repetem. Para obter informações sobre como criar tarefas recorrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Criar tarefas recorrentes</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference Number]</td> 
   <td> <p>Projetos, tarefas e problemas são associados automaticamente a um número de referência exclusivo à medida que são criados. Você pode visualizar o [!UICONTROL Reference Number] na página [!UICONTROL Details] de projetos, tarefas ou problemas, ou em uma lista ou relatório. </p> <p><b>DICA</b><p><br>É possível usar números de referência quando dois itens tiverem o mesmo nome, pois os números de referência são sempre únicos. </p> <p>[!DNL Workfront] gera automaticamente números de referência sequenciais no nível do sistema. Cada projeto, tarefa ou problema recebe o próximo número disponível na sequência. <br></p> <p>Por exemplo, se o Usuário A criar uma tarefa, o [!DNL Workfront] poderá atribuir automaticamente à tarefa o Número de referência 100. Se o Usuário B criar um problema logo após, o [!DNL Workfront] atribuirá o problema ao Número de referência 101. Não é possível editar manualmente os Números de referência. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rejection Issue]</td> 
   <td>Em um relatório de projeto ou de tarefa, esse é o problema criado quando a aprovação do projeto ou da tarefa é rejeitada. Para obter informações sobre problemas de rejeição, consulte o artigo <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Criar um processo de aprovação para itens de trabalho</a>. </td> 
  </tr>

<tr>
  <td>Tipos de relação</td>
  <td><p>Os objetos do Workfront são sempre conectados uns aos outros usando um dos seguintes tipos de relação:</p>

<ul><li> <b>Um para muitos</b>: nesta relação, um objeto pode ser conectado a vários outros objetos de tipos diferentes. Por exemplo, um projeto pode ter várias tarefas. A relação projeto-tarefas é uma relação um para muitos. Não é possível exibir essa relação em um relatório usando a interface padrão. Você deve usar os relatórios do modo de texto para visualizar relações um para muitos.</li>
  <li><b>Um para um</b>: nesta relação, um objeto só pode ser conectado a outro objeto de um tipo diferente. Por exemplo, um projeto só pode ter um grupo. A relação Projeto-Grupo é uma relação um para um. Você pode visualizar relações de um para um entre objetos em um relatório padrão.</li>
  <li><b>Muitos para um</b>: nesta relação, vários objetos podem ser conectados somente a um outro objeto de um tipo diferente. Por exemplo, várias tarefas podem ser conectadas ao mesmo projeto. A relação tarefas-projeto é uma relação muitos para um. Você pode visualizar relações muitos para um entre objetos em um relatório padrão. </li>
  <li><b>Muitos para muitos</b>: nesta relação, vários objetos do mesmo tipo podem ser conectados a vários objetos de um tipo diferente. Por exemplo, vários usuários podem pertencer a várias outras equipes, e as equipes podem pertencer a vários usuários. Não é possível exibir essa relação em um relatório usando a interface padrão. Você deve usar os relatórios do modo de texto para visualizar relações muitos para muitos. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Remaining Risk Cost]</td> 
   <td> <p>Um campo de projeto que mostra a diferença entre o [!UICONTROL Planned Risk Cost] de um projeto e o total de todos os [!UICONTROL Actual Costs] de todos os riscos do projeto. </p> <p>O [!UICONTROL Remaining Risk Cost] de um projeto é calculado usando a seguinte fórmula:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Replanning]</td> 
   <td>Alterar as datas de um projeto para reparar ou superar problemas. Por exemplo, um projeto que esteve suspenso por vários meses precisaria ser replanejado para refletir datas precisas. Essa é uma operação manual para ajustar as datas do projeto ou as datas das tarefas. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>Um gráfico ou tabela que contém informações sobre um determinado objeto do [!DNL Workfront] e os atributos relacionados.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>Um tipo de problema colocado em uma única fila centralizada e não está relacionado a um esforço do trabalho em andamento.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request Queue]</td> 
   <td>A lista de pendências de problemas gerenciados por um processo de tráfego e triagem.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Request velocity]</td> 
   <td>Tempo total do ciclo de trabalho para admissão e conclusão de uma solicitação.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>Normalmente, é um tipo de licença. Um usuário com uma licença de Solicitante pode enviar solicitações para que um novo trabalho ocorra no sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reserved Time]</td> 
   <td>Dias especificados no Tempo pessoal do usuário, indicando que ele não estará disponível para trabalho. Consulte "[!UICONTROL Non Work Days]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Issue]</td> 
   <td> <p>Em um relatório de problemas, use esse campo nas exibições ou filtros para se referir ao problema que resolve o problema. </p> <p>Para obter informações sobre como exibir objetos resolvedores em relatórios, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Exibir informações de objetos resolvíveis e resolvedores em um relatório</a> em <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão geral de objetos resolvedores e resolvíveis </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Project]</td> 
   <td> <p>Em um relatório de problemas, use esse campo nas exibições ou filtros para se referir ao projeto que resolve o problema. </p> <p>Para obter informações sobre como exibir objetos resolvedores em relatórios, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Exibir informações de objetos resolvíveis e resolvedores em um relatório</a> em <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão geral de objetos resolvedores e resolvíveis </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Task]</td> 
   <td> <p>Em um relatório de problemas, use esse campo nas exibições ou filtros para se referir à tarefa que resolve o problema. </p> <p>Para obter informações sobre como exibir objetos resolvedores em relatórios, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Exibir informações de objetos resolvíveis e resolvedores em um relatório</a> em <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão geral de objetos resolvedores e resolvíveis </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>Usuários ou funções que existem no [!DNL Workfront] e são atribuídos a equipes do projeto, tarefas e problemas. Eles são responsáveis por concluir o trabalho associado a projetos, tarefas ou problemas. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in  Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management] é um conjunto de ferramentas corporativas que permite prever precisamente o uso dos recursos com base na disponibilidade, de forma que o trabalho exigido seja concluído no prazo e dentro do orçamento. </p> <p>Com as ferramentas de gerenciamento de recursos, você pode planejar a capacidade a longo prazo e as necessidades de programação a curto prazo para os recursos. </p> <p>Para obter informações sobre o gerenciamento de recursos no [!DNL Workfront], consulte <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introdução ao gerenciamento de recursos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager IDs]</td> 
   <td><p>Em um relatório de projeto, você pode usar essa opção ao criar um filtro para localizar um gerente de recursos específico. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Managers]</td> 
   <td> <p>Em um relatório de projeto ou exibição de lista, esse é um campo informativo que mostra os usuários designados para executar atividades de gerenciamento de recursos no projeto.  Ao usar "[!UICONTROL Resource Managers]" em um relatório, uma lista de gerentes de recursos é exibida, com cada gerente de recursos do projeto separado por uma vírgula. Você pode designar até 30 gerentes de recursos em um determinado projeto.</p> <p>Para obter mais informações, consulte o artigo <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Designar Gerentes de recursos para um projeto ou modelo </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Horas orçadas do Planejador de recursos] </td> 
   <td>As horas orçadas para o projeto e os recursos associados a ele no [!UICONTROL Resource Planner]. Consulte também “[!UICONTROL Budgeted Hours]” neste artigo. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Planejador de recursos] </td> 
   <td>Uma ferramenta avançada do [!DNL Workfront] que permite visualizar e gerenciar recursos entre projetos, funções de trabalho ou usuários. Para obter informações, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Visão geral do planejador de recursos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Labor Cost]</td> 
   <td> <p>Este é o custo associado às horas orçadas para as funções de trabalho do projeto usando o planejador de recursos. </p> <p>Consulte também “Custo do trabalho orçado” neste artigo. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Resource Pools]</td> 
   <td> <p>Conjuntos de recursos são coleções de usuários que podem ser associados a um projeto. Os usuários no mesmo conjunto de recursos geralmente pertencem ao mesmo departamento, têm habilidades semelhantes ou complementares ou são financiados pelo mesmo orçamento. Você pode associar vários conjuntos de recursos a um projeto ou a um usuário. Um conjunto de recursos pode ser atribuído exclusivamente a um projeto ou compartilhado por vários projetos.</p> 
   <p>Para obter mais informações sobre conjuntos de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Visão geral dos conjuntos de recursos </a>.</p> 
   <p>Nos relatórios de projetos, os conjuntos de recursos mostram todos os conjuntos associados a um projeto. Este objeto não pode ser usado em um agrupamento.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>Um relatório que exibe o número de horas disponíveis durante um determinado período e o número de horas agendadas para cada usuário no relatório. Isso também é calculado em [!UICONTROL Average Hours Per Day] e uma porcentagem de alocação.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>No [!DNL Workfront Goals], um resultado é um indicador de progresso de uma meta. Pode ser um número, um valor percentual ou um valor de moeda que você atualiza manualmente. Não é possível exibir resultados em um relatório e você não pode acessá-los por meio da API do [!DNL Workfront]. Para obter informações sobre atividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introdução a resultados e atividades no Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>Um valor faturável da tarefa ou do projeto. O valor pode ser por hora, fixo ou uma combinação de ambos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>O tipo de receita determina como a tarefa acumulará receita. Alguns exemplos incluem [!UICONTROL Fixed Hourly], [!UICONTROL Role Hourly] e [!UICONTROL Role Hourly w/Cap]. Para obter informações sobre o acompanhamento de receita no [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão geral de faturamento e receita</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>Normalmente, é um tipo de licença. Um usuário com uma licença de [!UICONTROL Reviewer] que pode revisar e aprovar itens de trabalho no sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk]</td> 
   <td> <p>Isso pode se referir aos seguintes conceitos no [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>Um campo em um projeto que indica o risco que um projeto pode ter. Você pode priorizar a execução dos projetos com base no nível de risco. Os projetos podem ter os seguintes níveis de risco:</p> <p>- [!UICONTROL Very Low]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL High]</p> <p>- [!UICONTROL Very High]</p> <p>Os níveis de riscos que você indica para um projeto não podem ser personalizados. </p> <p> Para obter informações sobre como atualizar o risco de um projeto, consulte a seção “Configurações do projeto” do artigo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar projetos</a>. É possível exibir o campo de risco de um projeto em relatórios. </p> </li> 
     <li> <p>Um evento que pode ocorrer durante o ciclo de vida de um projeto que identifica um impacto potencial no custo, escopo ou programação do projeto. Você define riscos potenciais a um projeto e associa uma probabilidade de ocorrência ou um custo à medida que cria o business case do projeto. Para obter informações sobre como adicionar riscos ao business case do projeto, consulte “Criar e editar riscos em projetos”. </p> <p>Não é possível exibir riscos definidos no [!UICONTROL Business Case] em relatórios. Você só pode exibir vários tipos de custos de risco em relatórios e listas. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Cost]</td> 
   <td> <p>O custo associado aos riscos em um projeto. A seguir estão os custos de risco associados aos projetos que você pode exibir nos relatórios:</p> 
    <ul> 
     <li> <p>[!UICONTROL Actual Cost]: um campo em um risco que mostra o custo real do risco que ocorreu. Além de relatórios e listas, é possível localizá-los na caixa [!UICONTROL Edit Risk] ao editar ou criar um risco. </p> <p>Para custos de projetos, tarefas ou problemas, consulte “[!UICONTROL Actual Cost]” neste artigo. </p> </li> 
     <li> <p>[!UICONTROL Planned Risk Cost]: um campo no projeto que mostra um total de todos os [!UICONTROL Potential Risk Costs] do projeto. Consulte também “[!UICONTROL Planned Risk Cost]” neste artigo. </p> <p>Para obter informações sobre custo do risco em potencial, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular custo do risco em potencial </a>. </p> </li> 
     <li> <p>[!UICONTROL Remaining Risk Cost]: um campo no projeto que exibe a diferença entre o total dos [!UICONTROL Actual Costs] de todos os riscos e o [!UICONTROL Planned Risk Cost]. Consulte também “Custo do risco restante” neste artigo. </p> </li>
    </ul> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Management]</td> 
   <td>Processos para identificar, reduzir e monitorar riscos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>Consulte “[!UICONTROL Job Role]” neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>Atribuição ou movimentação automática de um problema, geralmente devido a um Tópico da fila ou por ser a Rota padrão (Regra de roteamento) para a fila.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing Rule]</td> 
   <td>Uma configuração em projetos e tópicos de fila que atribui automaticamente um problema a um usuário, função ou equipe, ou move o problema para outro projeto ou tópico da fila. As Regras de roteamento geralmente são usadas com as Filas de solicitações de ajuda para atribuir automaticamente os problemas recebidos.</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome do objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Saved Search]</td> 
   <td>Uma pesquisa para a qual os critérios foram salvos. As pesquisas salvas facilitam sua repetição sem a necessidade de inserir os critérios de pesquisa novamente.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scenario] (no [!DNL Workfront Fusion]) </td> 
   <td> <p>Um cenário é composto por uma série de etapas (módulos) que indicam como os dados devem ser transferidos e transformados entre aplicativos/serviços.</p> <p>Para obter informações sobre cenários no [!DNL Workfront Fusion], consulte a visão geral de cenários do <a href="https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview">[!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (no [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>No [!DNL Scenario Planner], um cenário é uma cópia de um plano. </p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte a <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">visão geral do [!DNL Scenario Planner]</a>. </p> <p>Para obter informações sobre como criar cenários, consulte <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Criar e comparar cenários de planos no [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule]</td> 
   <td>A programação de trabalho semanal, incluindo horários de trabalho, combinada com dias de folga (como feriados) e dias de exceção (como um dia de trabalho de sábado). Você pode associar cronogramas a projetos e usuários.</td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Schedule Performance Index (SPI)]</td> 
   <td><p>O [!UICONTROL Schedule Performance Index (SPI)] descreve a relação entre o agendamento planejado e o agendamento real. O Adobe Workfront calcula o SPI nos níveis de projeto e tarefa. Os gerentes de projeto analisam essa métrica para identificar se as tarefas ou projetos estão atualmente adiantados ou atrasados em relação ao cronograma.</p>
  <p>Para obter informações, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-spi.md">Calcular SPI (Índice de desempenho de programação)</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule Exemption]</td> 
   <td>Também conhecido como [!UICONTROL Modified Shift]. Dias programados em contraste com os horários regulares de trabalho semanais definidos pela programação. Por exemplo, um sábado agendado para trabalhar, quando o cronograma está configurado para trabalhar apenas de segunda a sexta-feira, seria uma [!UICONTROL Schedule Exemption].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheduled Report]</td> 
   <td> <p>Ao criar um relatório de relatórios, você pode exibir informações sobre os agendamentos do relatório, se ele estiver agendado para entrega usando o campo [!UICONTROL Scheduled Report]. Este campo mostra vários valores, um para cada cronograma de cada relatório, em uma lista com marcadores. Para obter mais informações sobre a programação de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Visão geral da entrega de relatórios</a>.</p> <p>Uma vez que esse campo mostra vários valores, ele não pode ser usado em um agrupamento. Você pode acessá-lo somente em um filtro ou em uma visualização. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alteração no escopo]</td> 
   <td>Uma [!UICONTROL Audit Trail] que, se ativa, gera uma nota sempre que uma alteração for feita no Escopo de um projeto ou tarefa, por exemplo, se uma [!UICONTROL Task Duration] ou os [!UICONTROL Predecessors] forem alterados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>Uma área na tela, com o próprio cabeçalho, criada para organizar os dados personalizados para fins de exibição.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section Break]</td> 
   <td>Uma lacuna ou borda entre seções.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>As configurações que permitem que um usuário interaja com determinados objetos no sistema e não com outros. Consulte também "[!UICONTROL Access Levels]" neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>A área em que os administradores podem definir as configurações e preferências do sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td> <p>[!UICONTROL Severity] é uma indicação da probabilidade de um item afetar a conclusão do trabalho. Por exemplo, um problema com alta [!UICONTROL Severity] pode bloquear completamente a conclusão de uma tarefa, mas um problema com baixa [!UICONTROL Severity] pode ser meramente superficial.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref">Atualizar severidade do problema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severities]</td> 
   <td>Consulte "[!UICONTROL Severity]" neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>A ação de permitir que outros usuários visualizem ou editem um item específico no [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack Date]</td> 
   <td>Em uma visualização ou relatório de tarefas, a [!UICONTROL Slack Date] exibe a data exata em que uma tarefa pode definitivamente impactar a [!UICONTROL Completion Date] do projeto. Para obter informações sobre a [!UICONTROL Slack Date] de uma tarefa, consulte <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Visão geral da data do Slack da tarefa</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assignments]</td> 
   <td> <p>Ao atribuir tarefas ou problemas a usuários, o [!DNL Workfront] faz recomendações ([!UICONTROL Smart Assignments]) sobre quem são os melhores usuários para concluir o trabalho, com base no tempo disponível para concluí-lo e sua relação com o projeto.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Visão geral de atribuições inteligentes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Indica o objeto-pai de outro objeto. Por exemplo, um documento anexado a uma tarefa tem o nome da tarefa no campo [!UICONTROL Source] de um relatório ou exibição [!UICONTROL Document]; um problema registrado em um projeto tem o nome do projeto no campo [!UICONTROL Source] de um relatório ou exibição de problema. </p> 
   <p>Os seguintes relatórios exibem uma coluna Origem, na qual você pode visualizar informações sobre o objeto-pai:</p>
  <ul><li>Relatórios de problema</li>
    <li>Relatórios de hora</li>
    <li>Relatórios de documento </li>
    </ul>
   <p>Se os usuários não tiverem permissões para o objeto-pai de um problema, hora ou documento, a coluna Origem do relatório será exibida em branco, mesmo quando o relatório estiver configurado para ser exibido ou entregue com os direitos de acesso de outro usuário. </p>
   <p> Para mostrar informações sobre o objeto-pai no relatório, recomendamos adicionar uma coluna para o objeto pai, onde você pode visualizar o nome do objeto pai. </p>
    <p>Por exemplo, você pode adicionar qualquer um dos itens a seguir a um relatório com uma coluna Origem: </p>
    <ul><li>As colunas Nome do projeto, Nome da tarefa ou Nome do problema em um relatório de horas ou de documento.</li>
    <li>As colunas Nome do projeto ou Nome da tarefa em um relatório de problema. </li> </ul>
    Para obter mais informações, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Executar e entregar um relatório com direitos de acesso de outro usuário</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start Date]</td> 
   <td> <p>A data em que o trabalho em um item está definido para iniciar. Há vários tipos de datas iniciais no [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Planned]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL Projected] </li> 
    </ul> <p>Em um [!UICONTROL Rate report], esta é a data em que uma nova taxa de cobrança para uma função no trabalho no nível do projeto inicia.  As horas associadas ao projeto que estão após essa data são multiplicadas por essa taxa de cobrança para calcular a receita no projeto. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Um indicador usado para sinalizar a posição do fluxo de trabalho de um item de trabalho ou de uma meta estratégica.</p> <p>Para projetos, o [!UICONTROL Status] é uma configuração no projeto que indica se o projeto está:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL On Hold] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>Para obter mais informações sobre o Status de um projeto, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Acessar a lista de status de projetos do sistema</a>.</p>
    <p>Para tarefas, o [!UICONTROL Status] é uma configuração na tarefa que indica se a tarefa é:</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>Para obter mais informações sobre o status da tarefa, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Acessar a lista de status de tarefas do sistema</a></p> <p>Para problemas, o [!UICONTROL Status] é uma configuração no problema que indica se esse problema está:</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Awaiting Feedback]</li> 
     <li>[!UICONTROL On Hold]</li> 
     <li>[!UICONTROL Resolved]</li> 
     <li>[!UICONTROL Won't Resolve]</li> 
     <li>[!UICONTROL Cannot Duplicate]</li> 
     <li>[!UICONTROL Verified Complete]</li> 
     <li>[!UICONTROL Reopened]</li> 
    </ul> <p>Para obter mais informações sobre os status de problemas, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acessar a lista de status de problemas do sistema</a>.</p> 
    <p>Para metas estratégicas, o [!UICONTROL Status] é uma configuração na meta que indica se a meta está:</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL Draft]</li> 
      <li>[!UICONTROL Inactive]</li> 
      <li>[!UICONTROL Closed]</li> 
     </ul> 
     <p>Para obter mais informações sobre metas estratégicas, consulte também "[!UICONTROL Goal]" ou "[!UICONTROL Goals]" neste artigo. </p> 
     <p>Para metas estratégicas, este campo estará visível somente se sua organização tiver adquirido o [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte Visão geral de <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals]</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alteração de status]</td> 
   <td>Uma [!UICONTROL Audit Trail]. Uma nota é gerada quando um usuário altera o status do projeto, da tarefa ou do problema.</td> 
  </tr> 
  <tr> 
   <td>Ícones de Status</td> 
   <td> <p>Você pode adicionar o campo [!UICONTROL Status Icons] integrado como uma coluna em suas visualizações para melhorar a visibilidade em pontos-chave sobre seus objetos, como:</p> 
    <ul> 
     <li>Um objeto tem documentos em anexo</li> 
     <li>Um objeto está associado a um processo de aprovação</li> 
     <li>Um objeto tem notas adicionais associadas a ele</li> 
     <li>Uma despesa é faturável ou reembolsável </li> 
     <li>Uma tarefa está em um caminho crítico</li> 
     <li>Um usuário pertence a uma empresa, equipe ou está localizado em um fuso horário diferente</li> 
    </ul> <p>Você pode adicionar o campo [!UICONTROL Status Icons] nas exibições dos seguintes objetos: </p> 
    <ul> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Template Tasks]</li> 
     <li>[!UICONTROL Modelos]</li> 
     <li>[!UICONTROL Despesas]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Users]</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ícones de status integrados em visualizações</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Update]</td> 
   <td> <p>Em um relatório de projeto, tarefa ou problema, este campo mostra a atualização de status mais recente que os proprietários do objeto forneceram na área “[!UICONTROL Updates]”.Para projetos, significa os comentários feitos pelo proprietário do projeto, e para tarefas e problemas, significa os comentários feitos pelos responsáveis.</p> 
   <p> Comentários feitos ao atualizar o status de um objeto não são exibidos na coluna [!UICONTROL Status Update].</p> <p>Para mostrar os status “[!UICONTROL New]”, “[!UICONTROL In Process]” e “[!UICONTROL Complete]”, use a coluna [!UICONTROL Status].</p> <p>Para obter mais informações sobre status, consulte o artigo <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Atualizar status da tarefa</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statuses]</td> 
   <td>Consulte "[!UICONTROL Status]" neste artigo.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Um gráfico que representa o status dos stories (tarefas na Metodologia Ágil) e como elas estão progredindo em direção à conclusão.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>Uma métrica usada para medir a dificuldade ou a complexidade de um story. As equipes Ágil podem escolher se desejam usar Horas ou Pontos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>Uma métrica usada para medir a dificuldade ou a complexidade de um story. As equipes Ágil podem escolher se desejam usar Horas ou Pontos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>Trabalho de longo prazo que altera a organização ou como ela funciona.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategic Alignment]</td> 
   <td>Medição e alinhamento de metas da empresa em portfólios e programas.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Isso é usado nas colunas do relatório ao usar a interface do modo de texto. </p>
   <p>O <code>[!UICONTROL stretch]</code> é usado para identificar quais colunas ocupam espaço extra não necessário para a visualização. A largura da interface do usuário do espaço de trabalho para um usuário típico é de cerca de 850 pixels. Isso significa que, se você tiver uma visualização com quatro
   colunas (150 pixels cada), a visualização ocupa 600 de 850 pixels. Há 250 pixels extras na interface que serão adicionados às colunas com uma porcentagem de ampliação fornecida. </p>
   <p>O alongamento de uma coluna é aplicado ao usar a linha de código adicional: <code>[!UICONTROL usewidths=true]</code> para pelo menos uma das colunas na visualização. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Subscribers]</td> 
   <td> <p>Usuários que assinam projetos, tarefas ou problemas.</p> <p>Ao usar esse campo em um relatório, uma lista de assinantes é exibida, com cada assinante separado por vírgula.</p> <p>Para obter mais informações, consulte o artigo <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Assinar itens no [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Summary Task]</td> 
   <td>Consulte “[!UICONTROL Parent Task]” neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtask]</td> 
   <td>Uma tarefa derivada, localizada sob uma tarefa principal.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>Um conjunto de políticas que controla as alterações e a manutenção de um sistema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>O processo de interligar diferentes sistemas computacionais e aplicações de software, física ou funcionalmente, para que atuem como um todo coordenado.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task]</td> 
   <td> <p>Uma atividade que deve ser executada como uma etapa para atingir uma meta final (concluir o projeto).</p>

<p>As tarefas são unidades de trabalho menores que concluem um projeto, o que representa uma unidade de trabalho maior.</p>
   <p>Tarefas nunca podem existir independentemente. Elas sempre fazem parte de um projeto. </p>
   <p>Para obter mais informações sobre tarefas, consulte <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Visão geral de tarefas</a>.</p> 
   <p>Para obter informações sobre como criar tarefas, consulte <a href="/help/quicksilver/manage-work/tasks/create-tasks/create-tasks-in-project.md">Criar tarefas em um projeto</a>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Attribute]</td> 
   <td>Outros campos ou objetos associados a uma tarefa. Eles indicam determinados detalhes sobre a tarefa. Alguns exemplos são [!UICONTROL Planned Completion Date] e [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Constraint]</td> 
   <td>Consulte "[!UICONTROL Constraint Type]" e "[!UICONTROL Constraint Date]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Management]</td> 
   <td>Um conjunto de políticas que governa os limites para a criação, atribuição, fechamento e visibilidade de tarefas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Owner]</td> 
   <td>A equipe ou usuário responsável pela estimativa de esforço e conclusão da tarefa</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Uma coleção de usuários que trabalham para metas ou objetivos de negócios semelhantes. Esses usuários podem ser atribuídos coletivamente a um item de trabalho, atribuindo a equipe a ele.</p> <p>Para obter mais informações sobre equipes, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Visão geral de equipes</a>.</p> <p>Os projetos podem ter uma [!UICONTROL Project Team] que contém todos os usuários ou funções associados ao trabalho no projeto.</p> <p>Para obter mais informações sobre equipes de projeto, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral das equipes de projeto</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>Os modelos de projeto são estruturas genéricas dos projetos mais repetíveis. Você pode definir tarefas, colocar tópicos em fila, personalizar formulários, anexar documentos ou aprovações ao criar um modelo de projeto para economizar tempo quando precisar criar um novo projeto. </p> <p>Você pode anexar modelos aos projetos já existentes ou usá-los para criar novos projetos. Todas as informações especificadas no modelo são transferidas para os projetos criados que o utilizam. </p> <p>Para obter mais informações sobre modelos, consulte <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Visão geral dos modelos de projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>Uma tarefa que faz parte de um modelo. As tarefas de modelo se tornam tarefas no projeto criado usando o modelo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>Uma [!UICONTROL Note] e a respectiva coleção de respostas relacionadas a um tópico específico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> Em uma lista ou relatório de [!UICONTROL Document], é exibida uma visualização do documento em miniatura. </p> <p> Selecione <strong>[!UICONTROL Thumbnail]</strong>  para exibir uma miniatura de 33 a 66 pixels de largura no relatório. </p> <p>O tamanho da miniatura é ajustado quando você modifica a largura da coluna em uma lista ou relatório.</p> <p>Consulte também "[!UICONTROL Large Thumbnail]" neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>É possível criar um relatório de [!UICONTROL Time Off] para visualizar quando os usuários indicaram uma folga em seu perfil. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet]</td> 
   <td> <p>Um cartão de ponto que permite aos usuários registrar as horas efetivas que dedicaram a projetos, tarefas ou problemas, ou as horas dedicadas a outras atividades não relacionadas ao trabalho, como reuniões ou treinamentos. Além de registrar a quantidade de tempo dedicado ao trabalho, você também pode indicar se o tempo está relacionado ao trabalho ou se representa tempo de sobrecarga, usando Tipos de hora para definir seus registros de tempo. Para obter informações sobre folhas de horas, consulte <a href="../../../timesheets/timesheets/timesheets-overview.md">Visão geral sobre folhas de horas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet Profile]</td> 
   <td> <p>Um [!UICONTROL Timesheet Profile] é um modelo que o [!DNL Workfront] usa para criar folhas de horas automaticamente para os usuários associados a elas. </p> <p>Você pode definir várias configurações, que serão aplicadas a cada folha de horas quando ela for criada. Algumas dessas configurações são: a frequência com que a folha de horas deve ser criada (semanalmente, a cada duas semanas, duas vezes por mês ou mensalmente), o dia de início da folha de horas, os aprovadores da folha de horas e os [!UICONTROL Hour Types] disponíveis que os usuários podem associar às horas registradas.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Top Parent ID] </td> 
   <td> <p>Esse campo permite identificar e filtrar dados sobre um grupo de nível superior e os respectivos subgrupos em uma lista ou relatório.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Top Parent Name] </td> 
   <td> <p>Esse campo permite identificar dados sobre um grupo de nível superior e os respectivos subgrupos em uma [!UICONTROL View] de uma lista ou relatório.</p> <p>Também é possível fazer isso usando o campo [!UICONTROL Top Parent ID].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Hours]</td> 
   <td> <p>Em um [!UICONTROL project report], esse campo exibe a soma arredondada de todas as horas do projeto, na última vez que as finanças do projeto foram calculadas. As [!UICONTROL Actual Hours] refletem as horas exatas registradas no projeto. Geralmente, as [!UICONTROL Actual Hours] devem corresponder às [!UICONTROL Total Hours]. Se as [!UICONTROL Total Hours] parecerem significativamente diferentes do campo [!UICONTROL Actual Hours], você deverá recalcular as finanças no projeto.</p> <p>Para obter mais informações sobre como recalcular as finanças do projeto, consulte o artigo <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Recalcular finanças do projeto</a>.</p> <p>Em uma exibição [!UICONTROL Standard] da folha de horas, esse campo se refere ao total de horas registradas para itens com relação às datas exibidas em uma folha de horas. O campo [!UICONTROL Total Hours] das folhas de horas nessa exibição integrada faz referência ao campo "[!UICONTROL hoursDuration]" que calcula dinamicamente a diferença em horas entre as datas inicial e final da folha de horas. Isso será usado para exibir a coluna [!UICONTROL Total Hours] em vermelho se o usuário registrar mais tempo do que as horas disponíveis no intervalo de tempo da folha de horas. Para obter mais informações, consulte <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Exibir total de horas na folha de horas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking Mode]</td> 
   <td> <p>Um atributo de tarefa. Isso determina como e quando as linhas do tempo projetadas serão atualizadas para uma tarefa. Por exemplo:</p> 
    <ul> 
     <li>[!UICONTROL User Must Update] requer que uma tarefa seja atualizada manualmente. Caso contrário, a atualização se tornará [!UICONTROL Behind Schedule] e, em seguida, [!UICONTROL Late].</li> 
     <li>A [!UICONTROL Auto Complete] concluirá automaticamente uma tarefa quando a Data de vencimento ou a [!UICONTROL Planned Completion Date] tiver passado.</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Visão geral do modo de rastreamento da tarefa</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Um evento que inicia um cenário.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trouble Task]</td> 
   <td>Uma tarefa incompleta com uma condição [!UICONTROL Late], [!UICONTROL Behind Schedule] ou [!UICONTROL At Risk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unassigned Task]</td> 
   <td>Uma tarefa que não está atribuída a nenhum Usuário, Função ou Equipe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Update Type]</td> 
   <td> <p>Uma configuração em um projeto que determina quando a linha do tempo projetada do projeto será recalculada. O [!UICONTROL Update Type] pode ter os seguintes valores:</p> 
    <ul> 
     <li>[!UICONTROL Automatic and On Change]</li> 
     <li>[!UICONTROL Somente automático]</li> 
     <li>[!UICONTROL Manual Only] </li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecionar o tipo de atualização do projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User]</td> 
   <td>Uma conta criada no [!DNL Workfront] para permitir que uma pessoa faça logon e interaja com o sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL User Delegation]</p> </td> 
   <td> <p>Um objeto relatável que informa:</p> 
    <ul> 
     <li>Quais usuários delegaram as aprovações de tarefas, problemas e projetos</li> 
     <li>Quais usuários tiveram as aprovações de tarefas, problemas e projetos delegadas a eles</li> 
     <li>Quando estas delegações começam e terminam</li> 
    </ul> <p>Para saber mais, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Criar um relatório de delegação de usuário</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface]</td> 
   <td>Todos os aspectos visuais e interativos do aplicativo [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface Preferences]</td> 
   <td>[!UICONTROL User Interface Setup]. Os administradores do [!DNL Workfront] podem alterar essas configurações para personalizar aspectos da interface do usuário.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilization]</td> 
   <td>A disponibilidade de um usuário ou uma função com base na programação atribuída, PTO e carga de trabalho atual.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Utilization]</td> 
   <td> <p>Uma pesquisa combinada com um relatório que mostra como os Usuários (Recursos) são alocados ou superalocados. Consulte "[!UICONTROL Resource Utilization]" neste artigo.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V – Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome do objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Velocity]</td> 
   <td>Uma medição do tempo total do ciclo de trabalho (quanto tempo leva para concluir uma tarefa) e com que frequência o trabalho é realizado no tempo originalmente comprometido (taxa de trabalho para compromisso).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>As exibições referem-se a um elemento de relatório que permite modificar as colunas em um relatório ou em uma lista de objetos.</p> 
   <p> Exibição também se refere ao direito de um usuário de visualizar apenas informações em um objeto, de acordo com seu nível de acesso ou em um nível de compartilhamento de permissões nesse objeto.</p> 
   <p>No Workfront Planning, os registros são exibidos na página do tipo de registro, em um dos seguintes tipos de exibição:</p>
   <ul><li>Tabela</li>
   <li>Linha do tempo</li>
   <li>Calendário</li></ul>
   <p>No Workfront Planning, as exibições incluem os filtros, agrupamentos, classificações e outras configurações aplicadas aos registros na tela.</p> <p>Para obter informações, consulte <a href="/help/quicksilver/planning/views/manage-record-views.md">Gerenciar exibições de registros</a>.</p>   
   <p>O Workfront Planning exige uma licença adicional.</p>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL View Icons]</td> 
   <td> <p> Esse campo é igual aos ícones de status, mas está disponível apenas para as seguintes exibições: </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> Para obter mais informações, consulte o artigo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ícones de status integrados nas exibições</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Month]</td> 
   <td> <p>Em uma lista de relatórios, exibe o número de vezes que o relatório foi visualizado durante o último mês.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Quarter]</td> 
   <td>Em uma lista de relatórios, exibe o número de vezes que o relatório foi visualizado durante o último trimestre.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Visualizar uso de relatório</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizações no ano passado]</td> 
   <td>Em uma lista de relatórios, exibe o número de vezes que o relatório foi visualizado durante o último ano.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizações neste mês]</td> 
   <td> <p>Em uma lista de relatórios, exibe o número de vezes que o relatório foi visualizado durante este mês.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizações neste trimestre]</td> 
   <td>Em uma lista de relatórios, exibe o número de vezes que o relatório foi visualizado durante este trimestre.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizações neste ano]</td> 
   <td>Em uma lista de relatórios, exibe o número de vezes que o relatório foi visualizado durante este ano.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Visualizar uso de relatório</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> Em um relatório, ao usar a interface do [!UICONTROL Modo de texto], a linha de código em que é possível especificar a largura de cada coluna em pixels. O Workfront fornece uma largura sugerida para cada campo;
porém, dependendo do tipo de campo e do formato, talvez você queira fazer ajustes.
Você deve usar a linha de código <code>[!UICONTROL usewidths=true]</code> adicional para aplicar a largura especificada para a coluna. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>Em um relatório de projeto, tarefa ou problema, usar a seguinte instrução no modo de texto exibe as horas planejadas do projeto, tarefa ou problema:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Para obter informações sobre como usar o modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Visão geral da sintaxe do modo de texto</a>. </p> 
   <p><b>DICA</b> 
   <p>Em um relatório de problema, a adição de um dos campos de [!UICONTROL horas planejadas] adiciona o campo <code>work </code> ao relatório. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabalho]</td> 
   <td> <p>Um dos dois tipos de licença principais. Concede menos acesso do que o [!UICONTROL Plano], mas permite criar e fazer atualizações no sistema. Um usuário com uma licença de Trabalho tem mais permissões do que um usuário com uma licença [!UICONTROL Externa], [!UICONTROL Revisor] ou [!UICONTROL Solicitante].</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]Visão geral de licenças</a>.</p> <p>O trabalho pode se referir ao número de [!UICONTROL horas planejadas] de um projeto, tarefa ou problema.Para obter mais informações, consulte o campo “[!UICONTROL Trabalho]” nesta tabela. </p> <p><b>DICA</b></p> <p> Em um relatório de problema, a adição de um dos campos de [!UICONTROL horas planejadas] adiciona o campo <code>work </code> ao relatório. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estrutura do detalhamento do trabalho]</td> 
   <td>Uma estrutura hierárquica das tarefas a serem executadas pela equipe do projeto, com base no relacionamento pai/filho.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Esforço do trabalho] </td> 
   <td> 
    <p>Um gerente de projeto pode decidir usar esse campo em vez do campo [!UICONTROL Horas planejadas] para estimar o esforço necessário para concluir uma tarefa. Esse campo torna-se visível somente quando as seguintes condições são atendidas:</p> 
     <ul> 
      <li> <p>A tarefa tem o [!UICONTROL tipo de duração Simples]. </p> <p><b>DICA</b></p> <p> Se você atualizar o [!UICONTROL tipo de duração] da tarefa para qualquer outro tipo, esse campo ficará oculto. </p> </li> 
      <li>O gerente de projeto habilitou o [!UICONTROL Uso do esforço do trabalho] para calcular automaticamente o campo [!UICONTROL Horas planejadas] da tarefa no projeto. </li> 
     </ul> 
     <p>Para obter informações sobre como usar o [!UICONTROL Esforço do trabalho] em vez de [!UICONTROL Horas planejadas] para estimar o esforço da tarefa, consulte <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Visão geral do esforço do trabalho</a>. </p> 
     <p>Você pode exibir esse campo em relatórios e listas de tarefas.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Item de trabalho]</td> 
   <td> <p>Esse campo se refere a tarefas ou problemas no [!DNL Workfront]. </p> <p>O relatório [!UICONTROL Item de trabalho] exibe informações de tarefas e problemas. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Combinação do gerenciamento do trabalho]</td> 
   <td>Um [!UICONTROL indicador do desempenho do trabalho] (WPI) da proporção de trabalho alocado para administrar a empresa e para alterar a empresa. O WPI de combinação ajuda você a entender, em um nível organizacional, se sua estratégia tem alguma alocação de trabalho real aplicada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurso de gerenciamento do trabalho]</td> 
   <td>Uma designação de uma persona no sistema que se qualifica para receber trabalho ou registrar tempo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Funções e responsabilidades do gerenciamento do trabalho]</td> 
   <td>Definir os proprietários e as partes interessadas para gerenciar o escopo, a execução e as aprovações do problema, tarefa, projeto, programa ou portfólio designado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL SLA do gerenciamento do trabalho]</td> 
   <td>Uma métrica quantificável acordada por todas as partes interessadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parte interessada do gerenciamento do trabalho]</td> 
   <td>Uma coleção de usuários com interesse adquirido nos resultados de uma solicitação de trabalho.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pontos de contato do gerenciamento do trabalho]</td> 
   <td>Registros digitalizados da comunicação entre as partes interessadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicadores do desempenho do trabalho] </td> 
   <td> <p>Proporção de combinação, capacidade, velocidade, qualidade e engajamento.</p> <p>WPI é um acrônimo comum (em inglês) para [!UICONTROL Indicador de desempenho do trabalho].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Processo de trabalho]</td> 
   <td> <p>O método no qual o trabalho é recebido, priorizado e executado. A maneira como você executa o trabalho normalmente é chamada de “fluxo de trabalho” ou “plano de projeto” (uma lista de tarefas com datas, relações de predecessores e assim por diante). </p> <p>Alguns exemplos de um processo de trabalho incluem a produção de um único ativo ou a entrega de uma campanha com vários ativos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modelo de fluxo de trabalho]</td> 
   <td>No relatório [!UICONTROL Aprovação de prova], esse campo exibe todos os modelos de fluxo de trabalho anexados a uma prova. Se não houver modelos anexados, a coluna ficará em branco.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Tempo de trabalho]</td> 
   <td>

<p>Representa a porcentagem do tempo [!UICONTROL Equivalente de tempo integral (FTE)] em que o usuário está disponível para trabalho efetivo, sem incluir a sobrecarga. O [!UICONTROL tempo de trabalho] deve ser um número decimal até 1 e não pode ser 0. Por exemplo, uma disponibilidade de 20% para o trabalho efetivo seria de 0,2.</p>
   </p>O padrão do campo é 1, indicando que um usuário gasta todo o [!UICONTROL FTE] no trabalho efetivo relacionado ao projeto.  </p>
   <p>O sistema usa esse número para calcular a disponibilidade do usuário para o trabalho efetivo relacionado ao projeto. </p>
   <p> Exceções de cronograma e folgas também podem afetar a capacidade do usuário. </p>
   <p>Para obter mais informações sobre como criar cronogramas no Workfront, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar um cronograma</a>. </p>
    <p>O Workfront calcula a disponibilidade de um usuário dependendo das preferências de gerenciamento de recursos na área [!UICONTROL Configuração]. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configurar preferências de gerenciamento de recursos</a>. </p> 
   <p>Você pode atualizar o [!UICONTROL Tempo de trabalho] de um usuário ao editar ou criar o usuário. Para obter informações, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Editar perfil de um usuário</a></p> 
   <b>DICA</b> 
   <p>Defina o valor de [!UICONTROL Tempo de trabalho] como 1 para indicar que o usuário está disponível para o trabalho relacionado ao projeto durante todo o período integral.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo no trabalho]</td> 
   <td>Na documentação do Workfront, esse termo é usado para descrever o tempo alocado ao trabalho, de acordo com um cronograma.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>Em um relatório de projeto, tarefa ou problema, usar a seguinte instrução no modo de texto exibe o número de horas planejadas do projeto, tarefa ou problema seguido da palavra “Horas”:</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Para obter informações sobre como usar o modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Visão geral da sintaxe do modo de texto</a>. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Espaço de trabalho] </td> 
   <td> <p>No Planejamento do Workfront, um espaço de trabalho é uma coleção de tipos de registro que define o ciclo de vida operacional de uma determinada organização. Um espaço de trabalho é a estrutura de trabalho de uma unidade organizacional.</p>
   <p>O Workfront Planning exige uma licença adicional. </p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/planning/architecture/create-workspaces.md">Criar espaços de trabalho</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


