---
content-type: reference
navigation-topic: workfront-navigation
title: Glossário de [!DNL Adobe Workfront] terminologia
description: O [!DNL Adobe Workfront] O glossário lista termos comumente usados no Adobe Workfront.
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 7b5b0fd95e39f37153e36abb4e3b8e738ac26d21
workflow-type: tm+mt
source-wordcount: '19399'
ht-degree: 0%

---

# Glossário de [!DNL Adobe Workfront] terminologia

>[!IMPORTANT]
>
>Este artigo deve ser usado como referência para entender os termos que você pode encontrar na variável [!DNL Adobe Workfront] no [!DNL Workfront] documentação ou quando, em geral, fala sobre planejamento e gerenciamento de trabalho. No momento, estamos atualizando essas informações e, como resultado, essa tabela pode não estar concluída. Eliminaremos essa isenção de responsabilidade quando considerarmos essas informações exaustivas.

A tabela a seguir é uma lista de termos comumente usados no Adobe Workfront:

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome Objeto</strong></th> 
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
   <td>Uma tarefa incompleta em um projeto atual que não é impedida de ser trabalhada por uma tarefa predecessora e não tem uma restrição de tarefa com uma data de início planejada futura. Por outras palavras, pode ser trabalhado hoje.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Atividade]</td> 
   <td>Em [!DNL Workfront Goals], uma atividade é um indicador de progresso para uma meta. Pode ser uma barra de progresso que você atualiza manualmente ou um projeto que está associado à meta. Não é possível exibir atividades em um relatório e não é possível acessá-las por meio da variável [!DNL Workfront] API. Para obter informações sobre atividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introdução aos resultados e atividades nas Metas da Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo Real]</td> 
   <td> <p>Para tarefas e problemas, esse é o custo associado às horas reais registradas em relação à taxa de Custo por hora do recurso atribuído à tarefa ou problema. Para projetos, este é um total de todos os [!UICONTROL Custos reais] das tarefas e problemas do projeto. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo Real de Despesa]</td> 
   <td> <p>A soma dos [!UICONTROL Valores Reais] para todas as despesas registradas em um projeto ou tarefa.</p> <b>EXEMPLO </b>
   <p>Se você criar uma despesa para a Tarefa 1 e inserir $600.00 no campo [!UICONTROL Quantia Real], o [!UICONTROL Custo de Despesa Real] para essa tarefa será de $600.00. </p> 
   <p>Para um projeto, [!DNL Workfront] O usa a seguinte fórmula para calcular o [!UICONTROL Custo de Despesa Real]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas reais]</td> 
   <td> <p>Em um projeto, tarefa ou relatório de emissão, [!UICONTROL Horas reais] são a soma de todas as horas registradas no projeto, tarefa ou problema.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span> Se, na guia [!UICONTROL Atualizações] da Tarefa 1, você clicar em "Tempo de Log" e inserir 25 horas, as Horas Reais da Tarefa 1 = 25 horas. </p> <p>[!DNL Workfront] O calcula [!UICONTROL Horas reais] para tarefas pai ou projetos usando as seguintes fórmulas:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo Real Da Mão De Obra]</td> 
   <td> <p>O [!UICONTROL Custo Real] associado à mão de obra investida em uma tarefa ou projeto. </p> <p>Para uma tarefa, [!DNL Workfront] O calcula o [!UICONTROL Custo Real da Mão de obra] usando a seguinte fórmula:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Se a tarefa tiver um [!UICONTROL Cost Type] de [!UICONTROL User Hhour], [!DNL Workfront] O usa a taxa do usuário. Se a tarefa tiver um [!UICONTROL Cost Type] de [!UICONTROL Função por hora], [!DNL Workfront] O usa a taxa de função da tarefa para calcular o [!UICONTROL Custo Real da Mão de obra]. </p> <p>Para um projeto, [!DNL Workfront] O usa a seguinte fórmula para calcular o [!UICONTROL Custo Real da Mão de obra]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Por exemplo, se um usuário registra 5 horas em uma tarefa com um [!UICONTROL Usuário por hora] [!UICONTROL Tipo de custo] e sua taxa por hora é de US$ 100, o [!UICONTROL Custo real da mão de obra] é de US$ 500.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Receita Real] </td> 
   <td> <p>A [!UICONTROL Receita real] de um projeto ou tarefa é a quantidade de dinheiro associada à [!UICONTROL Horas reais] do projeto ou da tarefa. </p> <p>Para obter informações sobre como rastrear receita em [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão Geral da Faturamento e Receita</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Início real]</td> 
   <td>O carimbo de data e hora quando um usuário altera um objeto em andamento no trabalho atribuído a ele.</td> 
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
   <td>Metodologia da [!UICONTROL Ágil]</td> 
   <td>Um tipo de metodologia baseada na evolução colaborativa de necessidades e soluções com equipes multifuncionais. Ele estimula a flexibilidade e a mudança com base em um cronograma fixo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>Diferem da equipe tradicional porque tiram seu trabalho em potencial de um registro retroativo e trabalham nele dentro de um período de tempo definido como uma [!UICONTROL Iteration].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Todas as minhas equipes]</td> 
   <td> <p>Quando referenciado em [!UICONTROL filters], esse campo exibe os usuários que pertencem a qualquer uma das equipes às quais o usuário conectado pertence ou itens de trabalho atribuídos a qualquer uma das equipes às quais o usuário conectado pertence. </p> <p>Recomendamos usar esse campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório que exibirá informações diferentes dependendo de quem faz logon para exibi-lo, já que as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de alocação]</td> 
   <td> <p>Você pode encontrar esse campo nos seguintes tipos de relatórios:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project] (Dados financeiros)</li> 
     <li>[!UICONTROL Horário orçado]</li> 
    </ul> <p>Para um<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->Relatório do [!UICONTROL Project (Dados financeiros)]: </p> 
    <ul> 
     <li>Criar este relatório ao tentar entender <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> a quantidade de [!UICONTROL Horas Planejadas] atribuída aos seus recursos.</li> 
     <li> <p>A [!UICONTROL Data de alocação] é o primeiro dia (domingo) de uma semana em que a alocação de uma [!UICONTROL função do trabalho] para uma tarefa é iniciada. Um recurso ([!UICONTROL Função do trabalho]) pode ter tantas [!UICONTROL Datas da alocação] quanto tem semanas durante a [!UICONTROL Duração] das tarefas às quais está atribuído. Se as tarefas se estenderem por vários meses, o primeiro dia de um mês também poderá se tornar uma [!UICONTROL Alocação Data], se estiver dentro da [!UICONTROL Duração] da tarefa.</p> <p>Por exemplo, você pode ter uma [!UICONTROL Função do trabalho] atribuída a uma tarefa que abrange mais de 3 semanas e tem 90 [!UICONTROL Horas planejadas]. Essas horas são espalhadas uniformemente durante a duração da tarefa, o que faz com que todos os dias atribuam 6 [!UICONTROL Horas Planejadas] à sua função de trabalho:</p> <p><em> [!UICONTROL Horas Diárias Planejadas] = [!UICONTROL Total Planned Hours]/ Número de [!UICONTROL Dias de Trabalho] durante a [!UICONTROL Duração] da tarefa </em> </p> <p>Como resultado, há três [!UICONTROL Datas de alocação], uma para cada domingo de cada semana durante a [!UICONTROL Duração] da tarefa, cada uma com um determinado número de [!UICONTROL Horas planejadas] associadas a elas.<br>Se a tarefa começar no meio da última semana de um mês e terminar duas semanas após o início de um novo mês, a tarefa terá quatro [!UICONTROL Datas de alocação]: um para cada domingo de cada semana durante a [!UICONTROL Duração] da tarefa e um para o primeiro dia do novo mês.</p> <p>Para aproveitar ao máximo essas informações, recomendamos criar um <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Relatório do Projeto (Dados Financeiros) e adicione um agrupamento de matriz para [!UICONTROL Data de Alocação], em seguida, agrupe os resultados semanalmente, mensalmente, trimestralmente ou anualmente para obter os dados mais precisos.<br>Para obter informações sobre como criar um agrupamento de matriz, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Criar um relatório de matriz</a>.</p> </li> 
    </ul> <p>As informações financeiras são preenchidas nos relatórios do [!UICONTROL Project (Financial Data)] somente quando os dados associados a elas tiverem menos de 5 anos. Por exemplo, se uma função de trabalho foi alocada para uma tarefa em janeiro de 2015 e hoje é setembro de 2021, um campo financeiro como a [!UICONTROL Alocação Data] para a função de trabalho não é preenchido no relatório [!UICONTROL Project (Financial Data)]. </p> 
    <div> 
     <p>Para um relatório da [!UICONTROL Hora do orçamento]:</p> 
     <ul> 
      <li>Crie este relatório ao tentar entender a quantidade de [!UICONTROL Horário orçado] alocada aos seus recursos ou aos seus projetos no Planejador de Recursos.</li> 
      <li> <p>A [!UICONTROL Alocação Data] é o primeiro dia (um domingo) da semana para a qual você fez o orçamento das horas no [!UICONTROL Resource Planner]. </p> <p>Dica:   <p>Se uma semana se estender por dois meses, ela gerará duas linhas no relatório: um correspondente ao primeiro dia da semana (domingo da primeira semana, que é durante o primeiro mês), e a segunda linha exibe o primeiro dia do segundo mês. </p> <p>Por exemplo, se você orçar 8 horas para um usuário para a semana de 30 de junho (domingo) a 6 de julho (sábado), as duas linhas exibem uma [!UICONTROL Data de alocação] de 30 de junho e 1 de julho. </p> </p> <p>Para obter informações sobre como orçar recursos no [!DNL Resource Planner], consulte o artigo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Recursos orçamentais na [!DNL Resource Planner] usando as exibições [!UICONTROL Project] e [!UICONTROL Role]</a>.</p> <p>Para obter informações sobre como criar um relatório [!UICONTROL Hora do orçamento], consulte <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Relatório: Hora do Orçamento</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anúncios]</td> 
   <td> <p>Uma maneira de comunicar aos usuários informações dentro do sistema. Geralmente, essas informações vêm de [!DNL Workfront] ao Administrador ou do Administrador ao usuário. </p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Enviar anúncios</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Integração de aplicativos]</td> 
   <td>Um aplicativo geralmente representa um conector para um aplicativo de software, mas também pode representar funções especiais que manipulam dados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisão do aprovador]</td> 
   <td> <p>No relatório [!UICONTROL Proof Approval], este campo exibe as decisões de aprovação de prova para provas que não estão mais ativas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fase Aprovador]</td> 
   <td>No [!UICONTROL Proof Approval report], este campo exibe informações sobre um estágio atual de provas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aprovação]</td> 
   <td> <p>Um determinado item de trabalho, como uma tarefa, documento ou folha de ponto, pode exigir que um supervisor ou outro usuário faça logoff no item de trabalho. Esse processo de aprovação é chamado de aprovação. </p> <p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Visão geral do processo de aprovação</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de aprovação]</td> 
   <td>No relatório [!UICONTROL Proof Approval], este campo exibe a data em que uma prova foi aprovada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aprovador]</td> 
   <td>Um usuário ou função de trabalho que deve fazer logoff em um determinado item de trabalho, ou o usuário que aprova entradas de hora nas folhas de horas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuído a]</td> 
   <td> <p>Em um relatório da [!UICONTROL Tarefa ou ocorrência], esse campo exibe o Proprietário da tarefa ou o problema ou o [!UICONTROL Destinatário principal]. Também é possível filtrar ou agrupar por esse campo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuição]</td> 
   <td>Um usuário, função de trabalho ou equipe atribuída a um problema ou tarefa. Projetos, portfólios ou programas não podem ter atribuições.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuições]</td> 
   <td> <p>Em um relatório [!UICONTROL Tarefa] ou [!UICONTROL Problema], esse campo exibe uma lista de todas as entidades (usuários, funções de trabalho, equipes) atribuídas à tarefa ou problema. Você pode filtrar por esse campo usando os campos [!UICONTROL Atribuir usuários] e [!UICONTROL Atribuir funções]. Você pode filtrar pela equipe atribuída à tarefa ou problema usando o campo Equipe . Não é possível agrupar um relatório por esse campo.</p> <p>Os itens de trabalho que foram colocados na [!UICONTROL Reciclagem] continuarão a ser exibidos em alguns relatórios que se referem ao objeto [!UICONTROL Atribuição], onde uma [!DNL OR] o modificador de filtro é usado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuir funções]</td> 
   <td>
   <p>Em um relatório [!UICONTROL Tarefa] ou [!UICONTROL Problema], esse campo exibe informações sobre as funções do trabalho atribuídas às tarefas ou problemas. Este campo exibe [!UICONTROL Proprietários primários], bem como outras funções de trabalho atribuídas a tarefas ou problemas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status da Atribuição]</td> 
   <td> <p>Em um relatório de atribuição, tarefa ou emissão, o [!UICONTROL Status da Atribuição] exibe se os usuários atribuídos a um item de trabalho clicaram no botão [!UICONTROL Trabalhar nele] ou [!UICONTROL Concluído] para aceitar ou concluir o trabalho. Os seguintes [!UICONTROL Status da atribuição] existem:</p> 
    <ul> 
     <li><b>[!UICONTROL Solicitado]</b>: o usuário foi atribuído à tarefa ou problema, mas ainda não clicou no botão [!UICONTROL Trabalhar nela] para começar a trabalhar nela.</li> 
     <li><b>[!UICONTROL Trabalho]</b>: o usuário clicou no botão [!UICONTROL Trabalhar nele] e está trabalhando no item no momento. </li> 
     <li><b>[!UICONTROL Concluído]</b>: o usuário clicou no botão [!UICONTROL Concluído] e concluiu seu trabalho no item. </li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">Visão geral dos botões [!UICONTROL Trabalhar nisso] e [!UICONTROL concluído]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuir equipes]</td> 
   <td>
   <p>Em um relatório [!UICONTROL task] ou [!UICONTROL problema], esse campo exibe informações sobre as equipes atribuídas às tarefas ou problemas. O campo exibe [!UICONTROL Proprietários primários], bem como outras equipes atribuídas a tarefas ou problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuir usuários]</td> 
   <td>
   <p>Em um relatório da [!UICONTROL Tarefa] ou da [!UICONTROL Problema], esse campo exibe informações sobre os usuários atribuídos às tarefas ou problemas. Este campo exibe [!UICONTROL Proprietários primários], bem como outros usuários atribuídos a tarefas ou problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atributo]</td> 
   <td>Um atributo é uma característica de um [!DNL Workfront] objeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Área de auditoria]</td> 
   <td> <p>As auditorias são mensagens do sistema que registram uma ação que aconteceu no Workfront. Os seguintes tipos de auditoria são registrados:</p> 
    <ul> 
     <li>[!UICONTROL Alteração de escopo]</li> 
     <li>[!UICONTROL Ação do anexo]</li> 
     <li>[!UICONTROL Edição geral]</li> 
     <li>[!UICONTROL Alteração de status]</li> 
     <li>[!UICONTROL Nota]</li> 
     <li>[!UICONTROL Entrada combinada]</li> 
     <li>[!UICONTROL Entrada de erro]</li> 
     <li>[!UICONTROL Alteração de status]</li> 
     <li>[!UICONTROL Alteração de assinatura]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trilha de auditoria]</td> 
   <td>A coleção de notas geradas automaticamente por eventos que são rastreados por meio das Alterações registradas ([!UICONTROL Áreas de auditoria]). Cada nota registra quem fez a ação, o que fez e quando o fez.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automático E Ao Alterar]</td> 
   <td> <p>Um dos tipos de [!UICONTROL Project Update]. Isso recalcula as linhas do tempo Projetadas e Planejadas do Projeto quando o processo de recálculo noturno é executado e quando qualquer atualização é feita no Projeto ou Tarefas no Projeto. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecione o Tipo de Atualização do projeto </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Disponibilidade</p></td> 
   <td> <p>Este termo é usado em relação à "disponibilidade do usuário" ou à "disponibilidade de recursos" e ilustra o tempo que o recurso (usuário ou função de trabalho) está disponível para funcionar. </p> 
   <p>O Workfront calcula a disponibilidade do usuário usando vários campos e dependendo das configurações das preferências do Gerenciamento de Recursos no seu sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências do Gerenciamento de recursos</a>. </p>
   <p>Para obter mais informações sobre disponibilidade de recursos, consulte <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introdução ao Gerenciamento de recursos</a></p>
   Como alternativa, "capacidade" também é usada para se referir à disponibilidade de recursos. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automático somente]</td> 
   <td> <p>Um dos tipos de [!UICONTROL Project Update]. Isso recalcula as linhas do tempo Projetadas e Planejadas quando o processo de recálculo noturno é executado.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecione o Tipo de Atualização do projeto</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>O trabalho "como de costume" que contribui para atingir os objetivos principais de negócios do dia a dia.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>A área em um ambiente ágil onde são mantidos novos problemas até que estejam prontos para serem trabalhadas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Linha de base]</td> 
   <td>Uma fonte de dados para medir iterações em um ambiente ágil.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Registro de Faturamento]</td> 
   <td> <p>Registra a receita, horas ou despesas que podem ser faturadas. Essas informações podem ser usadas para criar faturas em um sistema de contabilidade externo.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Criar registros de faturamento</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Status do Registro de Faturamento</td> 
   <td> <p>Em um Registro de Faturamento ou Relatório de Hora, o Status de um registro de faturamento indica se o registro de faturamento foi Faturado ou Não Faturado. Não é possível excluir um projeto ou editar o tempo associado a um registro de faturamento faturado. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Criar registros de faturamento</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>O processo de personalização [!DNL Workfront] para dar à interface uma aparência que espelhe sua empresa usando suas cores e logotipos.</p><p><strong>OBSERVAÇÃO</strong><br>Se sua organização tiver sido integrada ao [!DNL Adobe Experience Cloud], a marca não está disponível.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navegação estrutural]</td> 
   <td> <p>A área na parte superior da página que mostra a localização hierárquica de onde o usuário está no aplicativo.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Para obter mais informações, consulte <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Visão geral das navegações estruturais</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status do Orçamento]</td> 
   <td> <p>Este é um campo obsoleto. Qualquer informação que esse campo possa exibir está relacionada a um recurso que [!DNL Workfront] O foi removido e o campo não pode ser atualizado. </p> <p>Este campo mostra se o projeto foi adicionado ao [!UICONTROL Capacity Planner] e se o cálculo do orçamento foi concluído para ele. O [!UICONTROL Capacity Planner] foi removido do [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de Conclusão Orçada]</td> 
   <td> <p>Este é um campo obsoleto. Qualquer informação que esse campo possa exibir está relacionada a um recurso que [!DNL Workfront] foi removido. Este campo não pode ser atualizado. </p>
   <p> Este campo ainda está visível nos relatórios e nas listas do [!UICONTROL project] e do [!UICONTROL tasks].</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo orçado]</td>

<td> <p>Esse é o custo associado aos recursos orçamentários de um projeto. </p>
   <p>O campo é exibido nas seguintes áreas de [!DNL Workfront] Sob os seguintes nomes:</p>
   <ul>
   <li><strong>[!UICONTROL Custo orçado]</strong>: no painel [!UICONTROL Business Case Summary]</li>
   <li><strong>[!UICONTROL Custo]</strong>: nas áreas [!UICONTROL Utilização] ao exibir informações pelo [!UICONTROL Custo]</li>
   <li><strong>[!UICONTROL Custo Previsto do Projeto]</strong>: em listas e relatórios</li>
   </ul>   
    <p>O [!UICONTROL Custo orçado] do projeto é calculado usando a seguinte fórmula:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Para obter mais informações sobre o cálculo do [!UICONTROL Custo orçado] e para entender vários nomes desse conceito em [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcular Custo do Projeto Orçado</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horário orçado]</td> 
   <td> <p>As horas orçadas para recursos para o trabalho que precisam realizar nos projetos. Este campo refere-se às horas orçadas na área [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case] (ou no [!UICONTROL Resource Planner]) do projeto ou dos recursos do projeto.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Entenda o [!UICONTROL Custo de mão de obra orçada] e o [!UICONTROL Horário orçado] para projetos</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Para obter informações sobre como orçar usuários no [!DNL Resource Planner], consulte o artigo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Recursos orçamentais na [!DNL Resource Planner] usando as exibições [!UICONTROL Project] e [!UICONTROL Role]</a>. </p> 
    <p>As horas orçadas na área [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case] ou no [!UICONTROL Resource Planner] são exibidas nas seguintes áreas do [!DNL Workfront] e sob os seguintes nomes:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL Horário do orçamento] nome de exibição</strong></td> 
        <td><strong>Áreas de [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>Área [!UICONTROL Resource Budgeting] da [!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planner] exibido pela [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Horário orçado]</td> 
        <td> <p>Exibição do relatório de utilização [!UICONTROL Horas]</p> <p>Para obter mais informações sobre o relatório de [!UICONTROL Utilização], consulte o artigo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Visão geral do relatório [!UICONTROL Utilização de recursos]</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Horas]</td> 
        <td> <p>Relatório [!UICONTROL Hora do orçamento]</p><p>O objeto [!UICONTROL Hora do orçamento] no relatório Hora do orçamento refere-se às informações relacionadas a uma ferramenta de gerenciamento de recursos obsoleta. Somente o "[!UICONTROL Bud. O campo Horas]" neste relatório refere-se às horas orçadas no [!UICONTROL Resource Planner] ou na área [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case] do projeto. </p> <p>Para obter mais informações sobre como criar um relatório, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
        <td> <p>Encontrado nos seguintes relatórios:</p>
        <ul>
        <li>Relatório do [!UICONTROL Project]
        <li>Relatório do [!UICONTROL Project (Dados financeiros)]
        <li>Relatório da [!UICONTROL Tarefa]
        <li>Relatório [!UICONTROL Problema]
        <li>Relatório [!UICONTROL Hora do orçamento]</li>
        </ul>
         <p>Para obter mais informações sobre como criar um relatório, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Qualquer outra menção ao [!UICONTROL Horário orçado] em [!DNL Adobe Workfront] refere-se às horas orçadas usando recursos obsoletos que foram removidos do Workfront . Esses são campos somente visualização e não são atualizados com as informações atuais quando você usa as ferramentas de orçamento de recursos atuais. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo de mão de obra orçada]</td> 
   <td> <p>Esse é o custo associado às horas que você, como o Gerenciador de Recursos, orçou para suas funções de cargo pelo trabalho que elas precisam concluir nos projetos. </p> <p>O [!UICONTROL Custo de mão de obra orçada] em um relatório do projeto é calculado usando a seguinte fórmula:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Este campo pode se referir ao seguinte:</p> 
    <ul> 
     <li> <p>Custos de mão de obra exibidos na área [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case] ou no [!UICONTROL Resource Planner] que estão associados ao custo das funções de trabalho em um projeto. Para obter informações sobre o cálculo do [!UICONTROL Custo de mão de obra orçada], consulte o artigo <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Entenda o custo orçado da mão de obra] e [!UICONTROL Horas orçadas] para projetos</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Custos de mão de obra exibidos na área [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case] que refletem os [!UICONTROL People Custos] estimados em uma iniciativa vinculada ao projeto a partir do [!DNL Scenario Planner] ao usar o Planejador de cenário para orçar os recursos do projeto. Para obter informações sobre iniciativas, consulte <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Visão geral das iniciativas no Planejador de cenário</a>. </p> <p>O [!DNL Scenario Planner] exige uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">O [!DNL Scenario Planner] visão geral</a>. </p> </li> 
     <p>Ele é exibido nas seguintes áreas de sob os seguintes nomes:</p>
   <ul>
   <li><strong>[!UICONTROL Custo de mão de obra orçada]</strong>: na área [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case].
   <li><strong>[!UICONTROL Custo orçado]</strong>: na visualização [!UICONTROL Utilização] do relatório [!UICONTROL Custo]
   <p>Para obter mais informações, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Exibir informações de utilização de recursos </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: no [!DNL Resource Planner] Projeto ou [!DNL Role] exibições, ao exibir por Custo
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: nos seguintes relatórios: 
   <ul>
    <li>Relatório do [!UICONTROL Project]</li>
    <li>Relatório do [!UICONTROL Project (Dados financeiros)]</li>
    <li>Relatório da [!UICONTROL Tarefa]</li>
    <li>Relatório [!UICONTROL Problema]</li>
    <li>Relatório [!UICONTROL Hora do orçamento]</li> 
    </ul>
    <p>Para obter mais informações sobre como criar um relatório, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Data de início do orçamento]</td> 
  <td> <p>Este é um campo obsoleto. Qualquer informação que esse campo possa exibir está relacionada a um recurso que [!DNL Workfront] foi removido. Este campo não pode ser atualizado.</p>
  <p>Essas áreas foram removidas de [!DNL Workfront]. </p> 
  <p>O campo ainda está visível nos relatórios e listas do [!UICONTROL project] e da [!UICONTROL task].</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gráfico de detalhamento]</td> 
   <td>Um gráfico de linhas que fornece uma representação visual do trabalho concluído e restante.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>Uma ferramenta usada para avaliar se um projeto deve ser transferido do status [!UICONTROL Idea] para o status [!UICONTROL Planning]. Em outras palavras, um [!UICONTROL business case] ajuda a organização a decidir se vale a pena iniciar e concluir o projeto, especialmente ao comparar projetos com outros em um portfólio.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Criar um [!UICONTROL Business Case] para um projeto </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horário Previsto para Caso Comercial]</td> 
   <td> <p>Este é um campo obsoleto. Qualquer informação que esse campo possa exibir está relacionada a um recurso que [!DNL Workfront] foi removido. Este campo não pode ser atualizado.</p> <p>Este campo ainda está visível nas listas e relatórios do projeto e da [!UICONTROL tarefa]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuição calculada]</td> 
   <td> <p>Um dos Tipos de tarefa [!UICONTROL Duration]. Isso calculará a porcentagem de um dia de trabalho de 8 horas que o usuário atribuído à tarefa será alocada para a tarefa, com base na [!UICONTROL Duration] da tarefa e no [!UICONTROL Work Required].</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão geral da tarefa [!UICONTROL Duração] e [!UICONTROL Tipo de duração]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabalho Calculado]</td> 
   <td> <p>Uma das tarefas [!UICONTROL Duration Types]. Isso calculará o [!UICONTROL Trabalho necessário] em uma tarefa, dados a [!UICONTROL Duração] e as porcentagens do usuário [!UICONTROL Atribuição] (que são baseadas em um dia de trabalho de 8 horas).</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão geral da tarefa [!UICONTROL Duração] e [!UICONTROL Tipo de duração]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendário]</td> 
   <td> <p>Há dois tipos de calendários no [!DNL Workfront]: o [!UICONTROL Home Calendar] e os relatórios de calendário.</p> <p>O [!UICONTROL Home Calendar] é um calendário pessoal que permite ao usuário gerenciar sua carga de trabalho em relação às horas disponíveis em [!DNL Workfront]. O usuário também pode integrar o [!UICONTROL Home Calendar] com o [!DNL Outlook] ([!DNL Google] e [!DNL Microsoft] integração futura). </p> <p>Para obter mais informações sobre o [!UICONTROL Home Calendar], consulte <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">Exibição do [!UICONTROL Home Calendário]</a>.</p> <p>Um relatório de calendário é um relatório dinâmico no qual os usuários podem visualizar a data e outros detalhes importantes de um evento, incluindo a data de vencimento, o status do trabalho e o usuário ao qual o evento é atribuído.</p> <p> Para obter mais informações sobre relatórios de calendário, consulte <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Visão geral dos relatórios de calendário</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Pode Iniciar]</td> 
   <td> <p>Este campo indica se uma tarefa está pronta para começar a ser trabalhada. Se o início estiver pronto para ser trabalhado no campo [!UICONTROL Pode iniciar] na tarefa estiver definido como [!UICONTROL Verdadeiro]. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">Visão geral da "[!UICONTROL pode iniciar]" para tarefas</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
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
   <td> <p>Um tempo disponível do recurso quando ele pode ser alocado para o trabalho. Consulte "Disponibilidade". </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Categoria]</p> </td> 
   <td> <p>Uma categoria é um formulário personalizado. Você pode criar relatórios para esse objeto e também pode exibi-lo em outros relatórios de objeto. Nem todos os objetos podem ter um formulário ou categoria personalizada. Os seguintes objetos podem ter um formulário personalizado: <br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Tarefa]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Documento]</li> 
     <li>[!UICONTROL Despesa]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL Usuário]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da categoria]</td> 
   <td> <p>Quando adicionado como uma coluna à exibição de qualquer um dos seguintes objetos, exibe uma lista de todos os formulários personalizados associados a esses objetos:</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Tarefa]<br></li> 
     <li>[!UICONTROL Problema]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Documento]<br></li> 
     <li>[!UICONTROL Despesa]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL Usuário]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gerenciamento de alterações]</td> 
   <td>Uma área de prática focada na definição, compreensão e adaptação do trabalho planejado às alterações no escopo, programação, custo e fatores de recursos.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Alterar ordem]</td> 
   <td>Um tipo de problema levantado em relação a um projeto que descreve uma alteração solicitada ao âmbito acordado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alterar somente]</td> 
   <td>Um dos [!UICONTROL Update Types] do projeto. Ela só atualiza as linhas do tempo do [!UICONTROL Project Projected] e do [!UICONTROL Planned] quando são feitas atualizações para Tarefas ou edições no Projeto ou Tarefas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alterar ordem]</td> 
   <td> <p>Um dos tipos de [!UICONTROL Problema], geralmente indicando que uma quantidade não planejada de trabalho deve ser feita antes que o projeto possa ser concluído.</p> <p>Para obter mais informações sobre tipos de [!UICONTROL Problema], consulte a seção "Tipos de problema padrão" no artigo <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Personalizar tipos de problemas padrão</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa Filho]</td> 
   <td>Uma tarefa que é uma [!UICONTROL Subtarefa] de uma [!UICONTROL Tarefa pai] ([!UICONTROL Tarefa resumo]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filhos]</td> 
   <td>A coleção de [!UICONTROL Subtarefas] em uma [!UICONTROL Tarefa pai] ([!UICONTROL Tarefa resumo]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] e [!UICONTROL Training]</td> 
   <td>Módulos de aprendizagem, certificações, padrões ou uma comunidade de práticas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Confirmação]</td> 
   <td>Uma ferramenta de comunicação para que os usuários definam expectativas em relação aos resultados da tarefa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data da confirmação]</td> 
   <td>Uma ferramenta de comunicação para o usuário definir expectativas em relação aos resultados da tarefa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comunicações] e [!UICONTROL Relatórios]</td> 
   <td>Padrões para revisar as exceções e a integridade de um projeto, programa ou portfólio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>Uma [!UICONTROL Company] é uma unidade organizacional no [!DNL Workfront]. </p> 
   <p> Você pode associar um usuário ou um projeto a uma empresa. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Criar e editar empresas</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de conclusão]</td> 
   <td> <p>A data em que um projeto, tarefa ou problema é definido para ser concluído. Há vários tipos de [!UICONTROL datas de conclusão] em [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Data de conclusão real]. Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Visão geral do projeto [!UICONTROL Data de conclusão real] </a>.</li> 
     <li>[!UICONTROL Data de conclusão planejada]. Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Definir o projeto [!UICONTROL Data de conclusão planejada]</a> e <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Visão geral da tarefa [!UICONTROL Data de conclusão planejada]</a>.</li> 
     <li>[!UICONTROL Data de conclusão prevista]. Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Visão geral da [!UICONTROL Data de conclusão projetada] para projetos, tarefas e problemas</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dia de conclusão]</td> 
   <td>O dia, relativo ao início do [!UICONTROL Modelo], em que uma [!UICONTROL Tarefa de modelo] ou um [!UICONTROL Modelo] deve ser concluído.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de conclusão]</td> 
   <td> <p>Isso indica como um projeto será marcado como [!UICONTROL concluído]. Ela pode ter dois valores:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: Um usuário deve alterar o status do projeto para [!UICONTROL concluído].</li> 
     <li>[!UICONTROL Automático]: O status do projeto será alterado automaticamente para [!UICONTROL Concluído] quando todas as tarefas do projeto estiverem 100% concluídas e todos os problemas forem fechados.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condição]</td> 
   <td> <p>Essa é uma representação visual do progresso de uma tarefa, problema ou projeto.</p> <p>Para projetos, a condição pode ser definida manualmente pelo proprietário do projeto ou pode ser definida automaticamente por [!DNL Workfront], com base no status do progresso do projeto. </p> <p>Os valores possíveis para a condição do projeto são:</p> 
    <ul> 
     <li>[!UICONTROL No Target]</li> 
     <li>[!UICONTROL Em Risco]</li> 
     <li>[!UICONTROL Em Problemas]</li> 
    </ul> <p>Para obter mais informações sobre a condição do projeto, consulte o artigo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Visão geral da [!UICONTROL Condição do projeto] e do [!UICONTROL Tipo de condição]</a>.</p>
     <p>Você pode associar condições de tarefa e emissão a um número que pode ser exibido em relatórios. As listas abaixo exibem os nomes e números padrão para as condições de tarefa e emissão. O administrador do sistema pode atualizar os nomes das condições e pode adicionar novas condições com números diferentes. Depois que um número é associado a uma condição, ele não pode ser editado.  </p> 
     <p>Para tarefas, a condição é definida manualmente pelo proprietário da tarefa. Os valores possíveis para a condição da tarefa são:</p> 
    <ul> 
     <li>[!UICONTROL Indo sem problemas] (0)<br></li> 
     <li> [!UICONTROL Algumas Preocupações] (1)<br></li> 
     <li>[!UICONTROL Blocos de acesso principais] (2)</li> 
    </ul> <p>Para obter mais informações sobre a condição da tarefa, consulte o artigo <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Atualizar a [!UICONTROL Condição] para tarefas e problemas</a>.</p> <p>Para problemas, a condição é definida manualmente pelo proprietário do problema. Os valores possíveis para a condição de problema são:<br></p> 
    <ul> 
     <li>[!UICONTROL Indo sem problemas] (0)<br></li> 
     <li>[!UICONTROL Algumas Preocupações] (1)<br></li> 
     <li>[!UICONTROL Blocos de acesso principais] (2)</li> 
    </ul> 
   <p><b>Nota</b></p>
    <p>Quando o campo [!UICONTROL Condição] é rastreado nos relatórios [!UICONTROL Entrada do diário], as [!UICONTROL Novas] e [!UICONTROL Valores antigos de número] exibem o número associado à condição em vez de seu nome. Se uma condição originalmente não estiver definida para uma tarefa ou problema e você a atualizar posteriormente, o lançamento que captura a atualização exibirá o [!UICONTROL Valor do Número Antigo] do campo [!UICONTROL Condição] como -2,147,483,648. Consulte também "[!UICONTROL Novo valor numérico]", "[!UICONTROL Valor antigo do número]" e "[!UICONTROL Lançamento de entrada]" neste artigo. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atualização de condição]</td> 
   <td> <p>Este campo mostra a condição atual de tarefas, projetos ou problemas. Esta opção mostra as atualizações mais recentes que os proprietários de tarefas, projetos ou problemas forneceram no campo [!UICONTROL Atualizar Status], juntamente com a nova condição.</p> <p>Os comentários feitos nas atualizações de condição não são exibidos na coluna [!UICONTROL Atualização de condição]; somente a atualização principal é exibida.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data da restrição]</td> 
   <td> <p>Se você estiver usando uma [!UICONTROL Restrição de tarefa] vinculada a uma data específica, como [!UICONTROL Deve iniciar em], essa data específica se tornará a [!UICONTROL Constraint Date] da tarefa.</p> <p>As restrições de tarefa a seguir atualizam o campo [!UICONTROL Data da restrição]:</p> 
    <ul> 
     <li>[!UICONTROL Deve Iniciar Em]</li> 
     <li>[!UICONTROL Deve Terminar Em]</li> 
     <li>[!UICONTROL Iniciar Até]</li> 
     <li>[!UICONTROL Iniciar sem antes]</li> 
    </ul> <p>Dica:   
     <ul> 
      <li> <p>Uma tarefa com uma [!UICONTROL Restrição] de [!UICONTROL Datas fixas] não tem [!UICONTROL Constraint Date]. </p> </li> 
      <li> <p> [!UICONTROL Data da restrição] só pode ser visualizada em um relatório ou em uma visualização personalizada.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>Se você estiver usando uma Restrição de Tarefa em uma tarefa de modelo vinculada a um dia específico, como Deve começar em, esse dia específico se tornará o Dia de Restrição da tarefa de modelo.</p> <p>As restrições de tarefa a seguir atualizam o campo [!UICONTROL Constraint Day] :</p> 
    <ul> 
     <li>[!UICONTROL Deve Iniciar Em]</li> 
     <li>[!UICONTROL Deve Terminar Em]</li> 
     <li>[!UICONTROL Iniciar Até]</li> 
     <li>[!UICONTROL Iniciar sem antes]</li> 
    </ul> <p>Dica: O [!UICONTROL Constraint Day] só pode ser visualizado em um relatório ou em uma visualização personalizada. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de restrição]</td> 
   <td> <p>A tendência de agendamento de uma Tarefa. Por exemplo, o [!UICONTROL Assim que possível] agendará uma tarefa para ser iniciada assim que possível e o [!UICONTROL Concluir até o fim] agendará uma tarefa para ser concluída pela [!UICONTROL Constraint Date] e não mais tarde.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Visão geral da [!UICONTROL Restrição de tarefa]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menu contextual]</td> 
   <td>Um menu, localizado no lado esquerdo da tela, no qual os itens são alterados para correlacionar-se com o conteúdo ativo. Por exemplo, quando um usuário está visualizando um Projeto, o [!UICONTROL Contextual Menu] exibirá links para informações e ferramentas relacionadas ao Projeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Originador de Problemas Convertidos]</td> 
   <td>Um campo em um relatório de projeto ou tarefa que exibe informações sobre o usuário que é o [!UICONTROL Primary Contact] de um problema quando o problema é convertido em um projeto ou tarefa. O campo também é exibido na seção [!UICONTROL Detalhes do projeto], onde exibe o nome do [!UICONTROL Primary Contact] da edição convertida. Consulte também "[!UICONTROL Primary Contact]" neste artigo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custo]</td> 
   <td> <p>A quantia monetária que você deve gastar ao concluir um projeto, tarefa ou emissão. </p> <p>Você pode rastrear vários tipos de custos para mão de obra, despesas, riscos relacionados ao projeto.Para obter informações sobre como rastrear custos em [!DNL Workfront] see <a href="../../../manage-work/projects/project-finances/track-costs.md">Rastrear custos</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de custo]</td> 
   <td>Para uma tarefa, o [!UICONTROL Cost Type] determina como a tarefa provisionará custos. Alguns exemplos incluem [!UICONTROL Fixo por hora], [!UICONTROL Usuário por hora] e [!UICONTROL Usuário por hora mais fixo]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependências entre projetos]</td> 
   <td> <p>Uma tarefa de um projeto depende de uma tarefa de um projeto diferente.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Criar antecessores entre projetos</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Dados personalizados]</td> 
   <td> <p>Dados exclusivos de uma organização. As organizações podem personalizar o [!DNL Workfront] criando formulários personalizados e campos personalizados. Essas informações personalizadas podem gerar relatórios para KPIs, auditoria e mix de demanda. </p> <p>[!UICONTROL Dados personalizados] pode ser vinculado a:</p> 
    <ul> 
     <li>[!UICONTROL Projetos]</li> 
     <li>[!UICONTROL Tarefas]</li> 
     <li>[!UICONTROL Usuários]</li> 
     <li>[!UICONTROL Empresas]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Documentos]</li> 
     <li>[!UICONTROL Despesas]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programas]</li> 
     <li>[!UICONTROL Iterações]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de dados personalizados]</td> 
   <td>A opção para especificar se um campo [!UICONTROL Dados personalizados] é armazenado no banco de dados como Texto, uma Data, um Número ou Moeda.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de exibição personalizada]</td> 
   <td>O tipo de exibição de campo de um campo personalizado. Os exemplos incluem [!UICONTROL Suspenso], [!UICONTROL Campo de texto], [!UICONTROL Área de texto], [!UICONTROL Botões de opção] etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campo personalizado]</td> 
   <td>Para dados personalizados que permitem ao usuário selecionar entre várias opções, esses são os valores que podem ser selecionados por um Usuário. As opções personalizadas são válidas apenas no [!UICONTROL Suspenso], [!UICONTROL Multisseleção Suspensa], [!UICONTROL Botões de opção] e [!UICONTROL Caixas de seleção].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rótulo do formulário personalizado]</td> 
   <td>Ao usar um Tipo de exibição personalizado com opções personalizadas, esse é o texto da Interface do usuário que será exibido no menu suspenso, nas caixas de seleção ou nos botões de opção para essa opção personalizada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor personalizado]</td> 
   <td>Ao usar um campo Personalizado com Opções Personalizadas, esse é o valor que será armazenado no banco de dados para uma Opção específica.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibição personalizada]</td> 
   <td>Uma definição dos campos de dados, ou colunas, exibidos para cada objeto em uma lista.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cliente]</td> 
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
   <th>Nome Objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Painéis]</td> 
   <td> <p> É possível adicionar esse campo a um relatório ou a uma lista do objeto de relatório para exibir os painéis nos quais o relatório está listado em uma lista. </p> <p> Também é possível usar esse campo para filtrar relatórios listados em um painel específico. </p> <p> Para obter mais informações sobre como incluir informações de painel em relatórios de objetos de relatório, consulte a seção "Entendendo os relatórios que estão listados em painéis" no artigo <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Acessar e organizar relatórios</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de dados]</td> 
   <td>Consulte "[!UICONTROL Tipo de dados personalizados]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dias de atraso]</td> 
   <td> <p>Este campo mostra uma diferença de data entre [!UICONTROL Início planejado] e [!UICONTROL Hoje] se a [!UICONTROL Data de conclusão real] estiver ausente.</p> <p>Também mostra uma diferença de data entre [!UICONTROL Conclusão real] e [!UICONTROL Preenchimento planejado], quando uma [!UICONTROL Data de conclusão real] estiver presente.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Programação padrão]</td> 
   <td> <p>Horário de trabalho padrão personalizável a ser atribuído a usuários e projetos em uma organização. </p> <p>As programações são usadas para calcular as datas planejadas, de início e de conclusão das tarefas atribuídas aos usuários.</p> </td> 
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
   <td>[!UICONTROL Metas do departamento]</td> 
   <td>Metas exclusivas para um departamento específico que se concentra em melhorar as métricas operacionais no departamento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependência]</td> 
   <td>O link entre duas tarefas que exigem uma tarefa para alterar o status antes que a outra tarefa também possa alterar o status.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de dependência]</td> 
   <td> <p>O tipo de relacionamento de agendamento entre uma tarefa e seu(s) antecessor(es). Um exemplo é [!UICONTROL Finish-Start], que requer que a primeira tarefa tenha que terminar antes que a segunda tarefa possa iniciar.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Visão geral dos tipos de dependência de tarefa</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Documento]</td> 
   <td>Qualquer arquivo anexado a um objeto em [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Versão do documento]</td> 
   <td> <p>Cada vez que o mesmo documento é carregado no mesmo objeto, ele recebe um número de versão. Os usuários podem exibir e alterar várias opções de uma versão anterior de um documento.</p> <p>Para obter mais informações, consulte <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Gerenciar versões do documento</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duração]</td> 
   <td> <p>A janela de tempo alocada para a conclusão de um problema de tarefa, ou projeto (conforme determinado pelo número de dias entre o [!UICONTROL Planejado Start] e a Conclusão Planejada).</p> 
    <ul> 
     <li>Para tarefas, a Duração é um campo editável se o Tipo de duração da tarefa não for Simples. Se o Tipo de duração da tarefa for Simples, ou se a Restrição de tarefa for Datas fixas, a Duração é um cálculo executado pelo Workfront.</li> 
     <li>Para problemas, o campo Duration é sempre um campo editável e deve representar uma estimativa de um número de dias que exigiria que o problema fosse resolvido.</li> 
     <li>Para projetos, Duração é um cálculo executado por [!DNL Workfront] e representa a diferença em dias entre o Início planejado da tarefa mais antiga e o [!UICONTROL Planejado Completion] da tarefa mais recente no projeto.</li> 
    </ul> <p>Para obter mais informações sobre a diferença entre [!UICONTROL Duração] e [!UICONTROL Duração planejada] para tarefas, consulte o artigo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Diferença entre [!UICONTROL Duração planejada] e [!UICONTROL Duração] para tarefas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duração em minutos]</td> 
   <td>Este campo exibe as mesmas informações do campo [!UICONTROL Duração] em minutos em vez de dias. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duração por ocorrência]</td> 
   <td> <p>Isso é exibido nas caixas [!UICONTROL Detalhes da tarefa] e [!UICONTROL Editar tarefa] de um pai de tarefas recorrentes. Ele exibe a duração de cada tarefa recorrente. Para obter informações sobre como criar tarefas recorrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Criar tarefas recorrentes</a>. </p> <p> <span>As durações modificadas em tarefas recorrentes individuais não exibem o valor indicado neste campo.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Tipo de duração]</td> 
   <td> <p>Um campo de tarefa que indica como o trabalho necessário para concluir a tarefa é alocado para os destinatários na duração da tarefa. Ela representa a relação entre a [!UICONTROL Duração] da tarefa, o [!UICONTROL Trabalho necessário] e a quantidade de tempo, ou [!UICONTROL Alocação], os recursos atribuídos devem ser gastos na tarefa para concluí-la. </p> <p>Este campo aparece na guia [!UICONTROL Detalhes] de uma tarefa. </p> <p>As opções são:</p> 
    <ul> 
     <li>[!UICONTROL Atribuição calculada]</li> 
     <li>[!UICONTROL Trabalho Calculado]</li> 
     <li>[!UICONTROL Esforço orientado]</li> 
     <li>[!UICONTROL Simples]</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão geral da tarefa [!UICONTROL Duração] e [!UICONTROL Tipo de duração]</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Duração Unit]</td> 
   <td>A unidade usada para medir o tempo em uma pesquisa de energia.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Esforço orientado]</td> 
   <td>A relação entre o número de usuários e a quantidade de tempo que a tarefa levará para ser concluída. À medida que você adiciona mais usuários, o tempo total agendado para a tarefa ser concluída diminui, mas a duração da tarefa permanece a mesma. Por exemplo, se uma tarefa estiver bombardeando um barril de amendoins, adicionar mais pessoas diminuirá o tempo agendado, mas a duração em dias-pessoa permanecerá a mesma.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo decorrido]</td> 
   <td> <p>[!UICONTROL Tempo decorrido] é uma unidade de tempo para a [!UICONTROL Duração] de uma tarefa. É o tempo entre a [!UICONTROL Data de início planejada] e a [!UICONTROL Data de conclusão planejada] de uma tarefa que inclui feriados, finais de semana e tempo limite. Por outras palavras, o tempo decorrido é a passagem dos dias de calendário. </p> <p>[!DNL Workfront] O suporta as seguintes unidades de tempo decorrido para a duração da tarefa:</p> 
    <ul> 
     <li> <p>[!UICONTROL Minutos Atrasados]</p> </li> 
     <li> <p>[!UICONTROL Horas Decorrido]</p> </li> 
     <li> <p>[!UICONTROL Dias decorrido]</p> </li> 
     <li> <p>[!UICONTROL Semanas Decortadas]</p> </li> 
     <li> <p>[!UICONTROL Meses Atrasados]</p> </li> 
    </ul> <p>Para obter mais informações sobre a duração da tarefa, incluindo o tempo decorrido, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão geral da tarefa [!UICONTROL Duração] e [!UICONTROL Tipo de duração]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data final]</td> 
   <td> <p> Em um relatório da [!UICONTROL Rate], essa é a data em que uma nova taxa de faturamento de uma função de cargo no nível do projeto termina. As horas associadas ao projeto que são anteriores a essa data são multiplicadas por essa taxa de faturamento para calcular a receita no projeto. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>O [!UICONTROL Work Performance Indicator] (WPI) que indica quando o compromisso e a crença na tarefa, projeto, equipe ou organização estão em declínio. Isso indica que você precisa agir para reviver essa crença e esse compromisso. O WPI seria medido fazendo perguntas simples, "Você entendeu o que era esperado de você? O trabalho que você recebeu fez diferença para a organização? Você fez um ótimo trabalho?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Metas corporativas]</td> 
   <td>Metas multifuncionais que contribuem para as métricas das metas da empresa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Evento]</td> 
   <td>Qualquer alteração em um projeto ou tarefa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event Handler]</td> 
   <td>Tarefas automatizadas que ocorrem quando os eventos ocorrem. Um exemplo comum é uma notificação por email automatizada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event notification]</td> 
   <td>Email gerado a partir de um manipulador de eventos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Despesas]</td> 
   <td>Um custo não mão de obra em tarefas ou projetos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Externo]</td> 
   <td> <p>Geralmente, um tipo de licença ou um usuário com tal licença, que só tem a capacidade de revisar informações no sistema.</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] visão geral das licenças</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sistema externo]</td> 
   <td>Qualquer serviço ou software que seja armazenado e controlado fora do sistema de registro designado.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Campo]</td> 
   <td><p>Qualquer objeto do Workfront ou as informações associadas a ele, como aparece no banco de dados. </p>
   <p>Por exemplo, "projeto", "usuário", "hora" são objetos Workfront e campos. "Nome", "status", "proprietário", "data inicial" são campos Workfront associados aos objetos acima. </p>

<p>Ao se referir a objetos, os termos "objetos" e "campos" podem ser usados alternadamente.</p>
   <p>No escopo do relatório, os "campos" se referem aos objetos ou às informações sobre o objeto que você deseja capturar no relatório.</p>

<p><b>Nota</b></p>

<p>Nos relatórios com mais texto, os campos referem-se aos objetos ou suas informações, conforme aparecem no banco de dados.</p>
   <p>Às vezes, o nome que você vê na interface do usuário é diferente do nome do campo no banco de dados. Por exemplo, "problema" é o nome do objeto na interface do Workfront, mas "opTask" é o nome do objeto (ou o campo) no banco de dados do Workfront. </p> 
   <p> É importante usar o campo como ele aparece no banco de dados ao gravar um relatório em modo de texto, exibir, filtrar ou agrupar, ou ao criar um campo calculado.</p>

<p>Para obter mais informações, consulte <a href="../../../wf-api/general/api-explorer.md">API Explorer</a> e <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Visão geral do modo de texto</a>.</p>

<p>Por padrão, o Workfront vem com um conjunto de campos que definem ambos os objetos e suas informações. Também é possível criar campos personalizados para definir objetos, mas não é possível criar objetos personalizados.</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filtro]</td> 
   <td> <p>Um dos blocos fundamentais de um relatório ou um elemento de lista que define quais informações são exibidas na tela. Para obter mais informações sobre elementos de relatório, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de relatório: filtros, visualizações e agrupamentos</a>.</p> <p>O filtro determina os resultados que são exibidos em um relatório ou em um [!DNL Workfront] listagem de painéis, como projetos, tarefas ou problemas.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Processo para gerenciar dados de custos, despesas e receita da mão de obra em [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo Fixo]</td> 
   <td>Você pode definir uma quantia fixa de custo para um projeto. Isso faz parte do [!UICONTROL Custo planejado] do projeto, que representa a quantidade de dinheiro que você precisa para concluir o projeto. Para obter informações sobre custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Receita fixa]</td> 
   <td>Você pode definir uma quantia fixa de receita para um projeto. Isso faz parte da [!UICONTROL Receita planejada] do projeto, que representa a quantia de dinheiro que você pode obter se concluir o projeto. Para obter informações sobre a receita, consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão Geral da Faturamento e Receita</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sinalizadores]</td> 
   <td> <p> Este é o mesmo campo que [!UICONTROL Status Icons], mas está disponível somente para as seguintes exibições: </p> 
    <ul> 
     <li> [!UICONTROL Modelos] </li> 
     <li> [!UICONTROL Despesas] </li> 
    </ul> <p> Para obter mais informações, consulte o artigo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ícones de status incorporados nas exibições</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta]</td> 
   <td>As pastas são usadas para organizar documentos ou relatórios associados a um objeto.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (Equivalente de tempo completo)</td> 
   <td>É o Equivalente de Tempo Total que indica a quantidade de tempo em que um recurso está disponível para trabalho. 
   O campo [!UICONTROL FTE] é exibido nas seguintes áreas: 
  <ul>
   <li> Perfil do usuário, ao editar ou criar o usuário </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Planner de cenário] (requer licença adicional para o Workfront Scenario Planner) </li>
   <li> Listas e relatórios de usuários </li> </ul>

<p>O [!UICONTROL FTE] deve ser um número decimal até 1 e não pode ser 0. </p>
   <p> Um [!UICONTROL FTE] de 1 (que é o padrão para o campo [!UICONTROL FTE] de um usuário, conforme definido em seu perfil) significa que um recurso (usuário ou função) funciona por todo o número de horas, com base na programação que calcula sua disponibilidade. </p>
   <p>O administrador do Workfront decide qual programação usar para determinar a disponibilidade do usuário.  </p>
   <ul>
   <li> Quando a [!UICONTROL Programação padrão] é usada, a Workfront usa o [!UICONTROL FTE] do usuário encontrado em seu perfil para calcular a disponibilidade. </li>
   <li> Quando a Programação do Usuário é usada, a Workfront usa o tempo limite do usuário, o valor de [!UICONTROL Tempo de Trabalho] e as horas da [!UICONTROL Programação Padrão] para calcular o [!UICONTROL FTE] do usuário. </li> </ul>

<p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências do Gerenciamento de recursos</a>.  </p>
   <p>Para obter mais informações sobre como criar programações em [!DNL Workfront], consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar um agendamento</a>. </p>

<p><b>Nota</b></p>
   <p>Para todos os cálculos no [!UICONTROL Scenario Planner], o Workfront usa o seguinte valor: 1 [!UICONTROL FTE] = 8 Horas.</p>
   <p>Para obter mais informações, consulte <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Introdução ao [!UICONTROL Scenario Planner]</a>. </p>
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
   <th>Nome Objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Gráfico de Gantt]</td> 
   <td> <p>Uma linha do tempo visual das datas do projeto em uma exibição de calendário com base nas datas planejadas ou projetadas conforme as tarefas do projeto estão programadas no momento.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Objetivo]</td> 
   <td><p>Há dois conceitos de metas em [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Objetivos do projeto</b>: Um conjunto de objetivos empresariais acordados pelas partes interessadas relevantes de um projeto. As metas do projeto são parte do Business Case de um projeto. </p> <p>Não é possível exibir as metas do projeto em listas ou relatórios, mas você pode acessá-las por meio da API. </p> <p>Para obter informações sobre as metas do projeto de Caso de Negócios, consulte <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Criar metas de caso de negócios </a>. </p> </li> 
     <li> <p><b>Objetivos estratégicos</b>: Uma meta estratégica é um objetivo que você cria para planejar sua estratégia de trabalho para um período específico. Você pode criar esses tipos de metas usando [!DNL Workfront Goals]. Sua organização deve comprar uma licença adicional e você deve ter acesso a esse recurso para criar metas estratégicas. [!DNL Workfront Goals] estão disponíveis somente com uma licença adicional.</p> 
     <p>Para obter mais informações, consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] visão geral </a>. </p> 
     <p>É possível exibir metas estratégicas em um relatório de meta ou projeto e acessá-las por meio da API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Hierarquia de metas]</td> 
   <td> <p>Nos relatórios [!UICONTROL Meta] e [!UICONTROL Projeto], esse é um campo de coleção que exibe as metas na hierarquia à qual uma meta estratégica pertence quando está alinhada com outras metas. As metas são separadas por um delimitador de ▸. </p> <p>Somente os pais da meta e da meta são exibidos neste campo. As metas secundárias não são exibidas. </p> <p>Para obter informações sobre como alinhar metas em [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Visão geral do alinhamento da meta em [!DNL Workfront Goals]</a>. </p> 
   <p>Este campo estará visível somente se sua organização tiver comprado [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] visão geral </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Pontuação de sucesso da meta]</td> 
   <td> Em um [!UICONTROL Project report] esse campo costumava se referir às metas no nível do projeto associadas ao caso [!UICONTROL Business]. No momento, esse é um campo obsoleto e não está associado a nenhuma funcionalidade.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Metas] </td> 
   <td> <p>Em um relatório do [!UICONTROL Project], este é um campo de coleção que exibe todas as metas estratégicas associadas a um projeto. As metas são separadas por vírgulas.</p> <p>Este campo estará visível somente se sua organização tiver comprado [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] visão geral</a>. Para obter mais informações sobre objetivos estratégicos e objetivos de projeto em [!DNL Workfront], consulte "[!UICONTROL Objetivo]" neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Preferências da interface global]</td> 
   <td>Configurações da interface que afetam todos os usuários. [!UICONTROL Preferências da interface global] podem ser substituídas pelas [!UICONTROL Preferências da interface do usuário].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Grupo]</td> 
   <td> <p>Uma coleção de usuários (possivelmente do mesmo departamento ou unidade comercial) que têm acesso aos mesmos objetos. Além dos usuários, os grupos podem ser associados a portfólios, programas, projetos,<span> modelos de projeto,</span> empresas, equipes, agendamentos, modelos de layout e perfis de folha de ponto.</p> <p>Também é possível conceder permissões a objetos por grupo. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Visão geral dos grupos</a>.</p> <p>Em uma lista ou relatório de objetos de um dos seguintes tipos, é possível usar o campo [!UICONTROL Group] para listar quais objetos desse tipo estão associados a um grupo específico: usuário, portfólio, programa, projeto, <span>modelo de projeto</span>, empresa, equipe, agendamento, modelo de layout ou perfil de folha de ponto.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Group Administrator]</td> 
   <td> <p>Usuários que gerenciam objetos, acesso e usuários de grupos de usuários designados.</p> <p> Em um relatório do [!UICONTROL Group], esse campo exibe os nomes dos usuários designados como [!UICONTROL Group Administrators] no Grupo. Para obter mais informações sobre Administradores de grupo, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Grupo com acesso de administração]</td> 
   <td> <p> Em um [!UICONTROL Modelo de layout], [!UICONTROL Perfil de folha de tempo] ou [!UICONTROL Agendar relatório], esse campo exibe os Grupos cujos administradores de grupo têm acesso para modificar o modelo. Também é possível filtrar esse relatório por esse campo. </p> <p> Para obter mais informações, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Agrupamento]</td> 
   <td> <p>Um elemento de relatório usado para categorizar as informações em uma lista por um critério comum.</p> <p>Para obter mais informações, consulte a seção "[!UICONTROL Groupings]" no artigo <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de relatório: filtros, visualizações e agrupamentos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de transferência]</td> 
   <td> <p>A data em que uma tarefa se torna disponível para trabalho. A [!UICONTROL Handoff Date] é um cálculo e não pode ser definido manualmente. <br>Para obter mais informações sobre a [!UICONTROL Data de Handoff], consulte o artigo <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">Visão geral da [!UICONTROL Data de hansff da tarefa]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>A parte de [!DNL Workfront] que mantém todas as filas de emissão. O [!UICONTROL Help Desk] pode ser usado para processar tíquetes de suporte ao cliente, solicitações de projeto, tíquetes de suporte técnico etc. É o mesmo que a área [!UICONTROL Solicitações].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proprietário]</td> 
   <td>Em um relatório [!UICONTROL Hora], o [!UICONTROL Proprietário] é o usuário ao qual as horas são atribuídas. Isso é diferente do usuário que está registrando o tempo. Às vezes, essas duas entidades podem ser dois usuários diferentes. <br>Para obter mais informações sobre o tempo de registro para outro usuário, consulte o artigo <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Tempo de registro</a>.</td> 
  </tr>

<tr> 
   <td>Status de Hora</td> 
   <td> <p>Um atributo definido pela Workfront para as Horas reais que os usuários registram para tarefas, problemas ou projetos. </p>

As entradas de hora podem ter um dos seguintes status no Workfront:
<ul>
   <li><b>Enviado</b>: as horas foram registradas em um projeto, tarefa ou problema. Eles fazem parte de um registro de faturamento ou ainda não foram adicionados a um registro de faturamento.</li>
   <li><b>Aprovado</b>: as horas foram registradas e aprovadas pelo Proprietário do projeto. Eles fazem parte de um registro de faturamento ou ainda não foram adicionados a um registro de faturamento.</li> 
   <li><b>Não Aprovado</b>: as horas foram registradas e rejeitadas pelo proprietário do projeto. Eles fazem parte de um registro de faturamento ou ainda não foram adicionados a um registro de faturamento.</li>
   <li><b>Faturado</b>: as horas foram registradas, adicionadas a um registro de faturamento e o status do registro de faturamento foi marcado como Faturado. Eles não precisaram ser aprovados pelo Proprietário do Projeto.</li>
   <li><b>Faturado e Aprovado</b>: as horas foram registradas, aprovadas pelo Proprietário do Projeto e o status do registro de faturamento foi marcado como Faturado.</li>
   </ul>


<p>Quando as horas são parte de um registro de faturamento, o Status da Hora indica se as horas foram aprovadas ou se o Registro de Faturamento ao qual elas pertencem foi cobrado. O Status da hora de uma entrada de hora é visível somente em uma lista de horas ou relatório. </p>

<p>Para obter mais informações sobre como adicionar horas a registros de faturamento, consulte a seção "Adicionar horas a registros de faturamento" no artigo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Criar registros de faturamento</a>.</p>

<p>Para obter mais informações sobre aprovação de tempo em projetos, consulte <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Exigir tempo para ser aprovado para um projeto</a>.</p>

<p><b>DICA</b></p>

<p>As Horas Gerais que não estão conectadas diretamente aos itens de trabalho não exibem um Status de Hora. </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Tipo de hora]</td> 
   <td> <p>Um atributo que pode ser definido para Horas reais que os usuários registram para tarefas, problemas ou projetos. Este também é um atributo para as horas registradas que não estão diretamente vinculadas ao trabalho, como [!UICONTROL Férias] e [!UICONTROL Tempo desligado].</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Gerenciar tipos de hora</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>A ID é um indicador alfanumérico associado a cada objeto em [!DNL Workfront]. Ela identifica exclusivamente cada objeto na variável [!DNL Workfront] banco de dados. Você pode exibir a ID de qualquer objeto em um relatório ou em uma lista para cada objeto. </p> <p>Dica:   <p>Você também pode exibir a ID no URL da página do objeto. Por exemplo, a ID de um projeto pode ser semelhante ao número descrito no seguinte URL, quando você acessa a página [!UICONTROL Detalhes do projeto]:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Metas individuais]</td> 
   <td>Objetivos individuais que contribuem para as métricas dos objetivos da equipe, mas não estão relacionados com o desenvolvimento pessoal ou de carreira.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Acesso herdado]</td> 
   <td>Função de compartilhamento que permite o acesso para propagar de objeto para outro. Por exemplo, o acesso herdado do usuário do projeto definido nos registros do programa e do portfólio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>No [!DNL Workfront Scenario Planner], você pode dividir um plano em várias iniciativas para facilitar o gerenciamento do plano. <span>Você pode criar um relatório da [!UICONTROL Initiative] e acessar as informações da [!UICONTROL Initiative] em um relatório do [!UICONTROL Project].</span></p> <p>O [!DNL Scenario Planner] exige uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">O [!DNL Scenario Planner] visão geral</a>. </p> <p>O [!DNL Initiative] não está visível em seu [!DNL Workfront] , a menos que sua empresa tenha comprado um [!DNL Workfront Scenario Planner] licença. Não é possível acessar as [!UICONTROL Iniciativas] por meio da API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>O tipo de relatório [!UICONTROL Initiative Job Role] exibe informações sobre as funções do trabalho associadas a uma iniciativa de plano na [!DNL Workfront Scenario Planner].</span> </p> <p>O [!DNL Scenario Planner] exige uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">O [!DNL Scenario Planner] visão geral</a>. </p> <p><span>Esse tipo de relatório não está visível em [!DNL Workfront] , a menos que sua empresa tenha comprado um [!DNL Workfront Scenario Planner] licença.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Iniciativa Trabalho - Horas de Função da Iniciativa]</span> </td> 
   <td> <p><span> Em um relatório da [!UICONTROL Initiative Job Role], é exibido o número de horas associadas a uma função de cargo em uma iniciativa.</span> </p> <p>O [!DNL Scenario Planner] exige uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">O [!DNL Scenario Planner] visão geral</a>. </p> <p>Este campo e o tipo de relatório [!UICONTROL Initiative Job Role] não estão visíveis em sua [!DNL Workfront] , a menos que sua empresa tenha comprado um [!DNL Workfront Scenario Planner] licença.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Iniciativa Contagem de Funções da Iniciativa]</td> 
   <td> <p>Em um relatório da [!UICONTROL Initiative Job Role], é exibido o número de uma função de trabalho específica associada a uma iniciativa.</p> <p>O [!DNL Scenario Planner] exige uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">O [!DNL Scenario Planner] visão geral</a>. </p> <p>Este campo e o tipo de relatório [!UICONTROL Initiative Job Role] não estão visíveis em sua [!DNL Workfront] , a menos que sua empresa tenha comprado um [!DNL Workfront Scenario Planner] licença.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última data de publicação da iniciativa]</td> 
   <td> <p>Um campo em um relatório da [!UICONTROL Initiative], da [!UICONTROL Initiative Job Role] e do [!UICONTROL Project] que exibe a data em que uma iniciativa de plano foi publicada em um projeto pela última vez. Você pode publicar iniciativas para criar projetos ou atualizar projetos vinculados às iniciativas.</p> <p>O [!DNL Scenario Planner] exige uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">O [!DNL Scenario Planner] visão geral</a>. </p> <p><span>Para obter informações sobre iniciativas de publicação, consulte</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publique cenários para criar e atualizar projetos na [!DNL Workfront Scenario Planner]</a>. Este campo não está visível em sua [!DNL Workfront] , a menos que sua empresa tenha comprado um [!DNL Workfront Scenario Planner] licença.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pesquisa em linha]</td> 
   <td>Uma pesquisa realizada, no processo de preenchimento de um formulário, para localizar possíveis entradas para um campo específico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuração da interface]</td> 
   <td>A área do aplicativo que permite definir Exibições personalizadas, Filtros, Agrupamentos, Controles de lista etc.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL É Objetivo Da Empresa]</p></td> 
   <td> <p>Em [!DNL goal reports], isso exibe um valor "[!UICONTROL Verdadeiro]/ [!UICONTROL Falso]" para cada meta estratégica para indicar se sua organização está atribuída à meta como seu proprietário. </p> 
   <p>Este campo estará visível somente se sua organização tiver comprado [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] visão geral </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problema]</td> 
   <td> <p>Um item de trabalho não planejado que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Ele é testado e avaliado para mais consideração do esforço de trabalho</p> <p>Um [!UICONTROL Problema] também pode ser uma solicitação do [!UICONTROL Help Desk]. [!UICONTROL Alterar pedidos], [!UICONTROL solicitações] e [!UICONTROL bugs] também são [!UICONTROL problemas].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gerenciamento de problemas]</td> 
   <td> <p>O processo e as regras que regem a definição de tipos de emissão e o processo de roteamento, triagem ou tráfego associado a cada tipo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Proprietário da ocorrência]</td> 
   <td>A equipe ou usuários responsáveis por testar e concluir um problema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>Um período em que uma equipe produz um conjunto predefinido de deliveries.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Função do trabalho]</td> 
   <td> <p>Usado para identificar as funções e responsabilidades diárias de um usuário. As funções de trabalho podem ser atribuídas a itens de trabalho para identificar a habilidade necessária para concluir um processo de trabalho sem atribuí-lo a um usuário específico. </p> <p>Um usuário pode ter mais de uma função. Os exemplos incluem Designer gráfico ou Consultor.</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Lançamento de entrada]</p> </td> 
   <td> <p>Um objeto reportável que informa informações sobre atualizações do sistema para campos rastreados que aparecem na área [!UICONTROL Atualizações] de projetos, tarefas, problemas e outros objetos.</p> <p>Para saber mais, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Relatório sobre a área [!UICONTROL Atualizações]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicador Kanban]</td> 
   <td> <p>Em um Relatório da [!UICONTROL Tarefa] ou Relatório da [!UICONTROL Problema], o campo [!UICONTROL Indicador Kanban] exibe o status do sinalizador definido na história do quadro da [!UICONTROL Kanban]. Os valores possíveis são [!UICONTROL On Track], [!UICONTROL Ready to Pull] e [!UICONTROL Is Blocked].</p> <p>Para obter mais informações sobre como definir o status do sinalizador em histórias no [!UICONTROL Kanban stories], consulte o artigo <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Use sinalizadores em histórias no quadro do [!UICONTROL Kanban]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPIs</td> 
   <td>Um valor mensurável que demonstra a eficácia com que uma empresa está a atingir objetivos comerciais fundamentais.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atraso]</td> 
   <td>O tempo que deve passar após a [!UICONTROL Data de conclusão planejada da tarefa antecessora] ter passado até que a tarefa dependente possa começar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipos de tag]</td> 
   <td> <p>O método de cálculo do [!UICONTROL Lag]. Pode ser:</p> 
    <ul> 
     <li>[!UICONTROL Dias] (dias úteis)</li> 
     <li>[!UICONTROL Dias do calendário] (ignorar feriados)</li> 
     <li>[!UICONTROL Porcentagem]</li> 
     <li>[!UICONTROL Dia da semana]</li> 
    </ul> <p>Para obter mais informações, consulte a seção "[!UICONTROL Lag Types overview]" em <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Visão geral dos tipos de atraso</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniatura grande]</td> 
   <td> <p> Em uma lista ou relatório do [!UICONTROL Document], ele exibe uma pré-visualização do documento em uma miniatura. </p> <p>Selecionar <strong>[!UICONTROL Miniatura grande]</strong> para visualizar uma miniatura de 400 pixels no relatório.</p> <p>O tamanho da miniatura se ajusta ao modificar a largura da coluna em uma lista ou relatório.</p> <p>Consulte também "[!UICONTROL Miniatura]" neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Últimos 10 visualizadores]</td> 
   <td> <p>Em uma lista de relatórios, esse campo exibe os nomes de até 10 usuários que visualizaram o relatório mais recentemente.<br>Para obter mais informações sobre uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última Nota de Condição]</td> 
   <td> <p>Este campo exibe a última atualização inserida em um objeto pelo proprietário, Esta é a atividade ou interação mais recente do proprietário em um objeto.</p> <p>O [!DNL Last Condition Note] estiver vazia se o texto da nota da última nota de um objeto tiver sido excluído. Quando uma nova nota é inserida no objeto, ela se torna a última nota e é exibida novamente na coluna . </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data da última atualização financeira]</td> 
   <td>Em um relatório do [!UICONTROL project], esse campo captura a data e a hora em que as finanças do projeto foram calculadas e atualizadas pela última vez. Para obter informações sobre as finanças do projeto, consulte <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Visão geral das finanças do projeto</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última observação]</td> 
   <td> <p>Este campo exibe a última atualização inserida em um objeto por qualquer usuário. Essa é a atividade ou interação mais recente em um objeto.</p> <p>A coluna [!UICONTROL Última observação] fica vazia se o texto da última nota de um objeto foi excluído. Quando uma nova nota é inserida no objeto, ela se torna a última nota e é exibida novamente na coluna .</p>
   <p>Quando esse campo é adicionado a um relatório da [!UICONTROL Tarefa], quaisquer atualizações deixadas em objetos filho — como problemas, subtarefas, documentos etc. — da tarefa não é exibido nesta coluna.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última visualização por]</td> 
   <td> <p>Em uma lista de relatórios, esse campo exibe informações sobre o usuário que visualizou o relatório por último.<br>Para obter mais informações sobre uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data da última visualização]</td> 
   <td> <p>Em uma lista de relatórios, esse campo exibe a data em que o relatório foi exibido por último.<br>Para obter mais informações sobre uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Modelo de layout]</td> 
   <td>Definido pelo Administrador do sistema ou Administrador do grupo para identificar as guias e os relatórios exibidos no espaço de trabalho de um determinado usuário.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de layout]</td> 
   <td>Em conjunto com [!UICONTROL Visualizações personalizadas], o [!UICONTROL Tipo de layout] especifica o tipo de [!UICONTROL Visualização personalizada]. Atualmente, somente a Lista está disponível. Futuramente, [!UICONTROL Detalhe] (a exibição [!UICONTROL Detalhe] de um objeto) poderá se tornar disponível.</td> 
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
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa da biblioteca]</td> 
   <td>Um modelo para uma única tarefa usada para fornecer um nome consistente das [!UICONTROL Tarefas] e [!UICONTROL Tarefas de modelo] no aplicativo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de licença]</td> 
   <td>O tipo de licença alocada para um [!UICONTROL Access Level]. Ele é [!UICONTROL Usuário completo], [!UICONTROL Usuário limitado] ou [!UICONTROL Solicitante].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plano de limite de licença]</td> 
   <td> <p>Em uma visualização ou relatório do [!UICONTROL Group], esse campo mostra o número máximo de licenças do [!UICONTROL Plan] que podem ser atribuídas a usuários que têm o respectivo grupo designado como seu [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabalho com limite de licença]</td> 
   <td> <p>Em uma visualização ou relatório do [!UICONTROL Group], esse campo mostra o número máximo de licenças do [!UICONTROL Work] que podem ser atribuídas a usuários que têm o respectivo grupo designado como seu [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuário limitado]</td> 
   <td>Um Tipo de Licença que permite a criação de um [!DNL Access Level] que contém privilégios somente visualização, com a capacidade de enviar problemas, inserir observações e fazer upload de documentos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controles]</td> 
   <td> <p>Uma parte da [!UICONTROL Interface Setup] que permite vincular filtros, exibições e agrupamentos personalizados a usuários individuais ou globalmente a todos os usuários.</p> </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Manual only]</td> 
   <td> <p>Um dos [!UICONTROL Project] tipos de atualização do [!UICONTROL Project]. Essa configuração permite que as linhas do tempo do [!UICONTROL Project Projected] e do [!UICONTROL Planned] sejam atualizadas somente quando o "[!UICONTROL Recalculated Timelines]" for clicado. Os projetos configurados dessa forma serão ignorados durante o processo de ligeiro recálculo e quando o Projeto ou Tarefa no Projeto for atualizado.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecione o projeto [!UICONTROL Atualizar tipo] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Refere-se ao usuário conectado no momento. </p> <p>Recomendamos usar esse campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório que exibirá informações diferentes dependendo de quem faz logon para exibi-lo, já que as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Máximo de usuários]</td> 
   <td> <p>Este é um campo obsoleto. Qualquer informação que esse campo possa exibir está relacionada a um recurso que [!DNL Workfront] O foi removido e o campo não pode ser atualizado. </p> <p>Em versões anteriores de [!DNL Workfront], é possível atualizar esse campo ao criar ou editar uma função de trabalho. Ele exibia o número total de usuários que podem ser associados a uma função em cada projeto. Um valor zero permitido para um número ilimitado de usuários que podem ser atribuídos a um projeto. </p>O campo ainda está visível em alguns relatórios e listas, mas as informações exibidas não podem ser atualizadas. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Marco]</td> 
   <td> <p>Um marcador que pode ser associado a uma tarefa para indicar que um ponto-chave no Projeto foi atingido quando a tarefa é concluída. Geralmente é possível usar marcos para mostrar um evento significativo, como a conclusão de uma fase do projeto ou um conjunto de atividades críticas. [!UICONTROL Marcos] normalmente estão associados a tarefas principais. Você deve criar os marcos antes de anexá-los a tarefas. Para obter informações sobre marcos, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Criar um caminho de marco</a> e <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Associar marcos a tarefas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Caminho do marco]</td> 
   <td>Uma coleção de [!UICONTROL marcos]. [!UICONTROL Caminhos de marcos] são usados em Projetos para distinguir projetos com determinados tipos de [!UICONTROL Marcos] de projetos com um conjunto diferente de [!UICONTROL Marcos].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Tarefa de marco]</td> 
   <td>Uma tarefa sinalizada para indicar um evento relatável a ser medido.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Módulo]</td> 
   <td>Uma única etapa em um cenário em [!DNL Workfront Fusion] que executa algumas funções com base no aplicativo associado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Minha função principal]</td> 
   <td> <p>Quando isso é referenciado em filtros, exibe usuários que têm a mesma [!UICONTROL Função primária] que o usuário conectado ou itens de trabalho atribuídos à [!UICONTROL Função primária] do usuário conectado.</p> <p>Recomendamos usar esse campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório que exibirá informações diferentes dependendo de quem faz logon para exibi-lo, já que as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Minha equipe inicial]</td> 
   <td> <p>Quando referenciado em filtros, esse campo exibe os usuários que pertencem à [!UICONTROL Home Team] do usuário conectado ou os itens de trabalho atribuídos à [!UICONTROL Home Team] do usuário conectado. </p> <p>Recomendamos usar esse campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório que exibirá informações diferentes dependendo de quem faz logon para exibi-lo, já que as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Convenção de nomenclatura]</td> 
   <td>Um conjunto de regras em toda a organização que usa dados para criar nomes de projetos, tarefas e resultados.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Integração nativa]</td> 
   <td>Uma integração que não requer codificação manual ou configuração de API. Também conhecida como integração "pronta para uso".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menu Navegação]</td> 
   <td>O painel superior central do aplicativo que tem links para as áreas principais do [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL Novo valor numérico]</td> 
   <td>Em um relatório do [!UICONTROL Journal Entry], esse relatório exibe o valor atualizado de um campo que substitui o [!UICONTROL Valor antigo do número].
   Para obter mais informações, consulte "[!UICONTROL Valor antigo do número]" neste artigo.</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Dia não útil]</td> 
   <td>Um dia não alocado para a conclusão de qualquer atribuição. Geralmente é dia de férias, feriado ou fim de semana.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nota]</td> 
   <td>Um comentário ou atualização feito em um [!DNL Workfront] objeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto da nota]</td> 
   <td> <p>Isso exibe o texto de uma atualização inserida por um usuário em qualquer objeto. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Número de metas vinculadas]</td> 
   <td> <p>Em um relatório do [!UICONTROL Project], esse é o número de metas estratégicas associadas ao projeto. Para obter informações sobre como associar projetos com metas estratégicas, consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Adicionar projetos às metas em  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Para obter informações sobre metas estratégicas, consulte "[!UICONTROL Objetivo]" neste artigo.</p> 
   <p>Este campo estará visível somente se sua organização tiver comprado [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Adicionar projetos às metas no [!UICONTROL Adobe Workfront Metas]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Objeto]</td> 
   <td> <p>As informações exibidas em [!DNL Adobe Workfront] é representado por objetos armazenados no [!DNL Workfront] banco de dados. Os objetos são o que direciona as informações no Workfront. Alguns exemplos de objetos são:</p> 
    <ul> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programas]</li> 
     <li>[!UICONTROL Projetos]</li> 
     <li>[!UICONTROL Tarefas]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Documentos]</li> 
     <li>[!UICONTROL Painéis]</li> 
     <li>[!UICONTROL Relatórios]</li> 
     <li>[!UICONTROL Grupos]</li> 
     <li>[!UICONTROL Equipes]</li> 
     <li>[!UICONTROL Usuários]</li> 
     <li>[!UICONTROL Empresas]</li> 
     <li>[!UICONTROL Formulários personalizados]</li>
     <li>[!UICONTROL Campos personalizados]</li>  
     <li>[!UICONTROL Hours]</li> 
     <li>[!UICONTROL Taxas de faturamento]</li> 
     <li>[!UICONTROL Modelos]</li> 
     <li>[!UICONTROL Tarefas do modelo]</li>

<p><b>Nota</b></p>
  <p>Esta não é uma lista extensa. </p>

</ul> <p>Para obter mais informações, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Entender objetos na [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipos de objeto]</td> 
   <td>Se você criar um relatório ou uma lista contendo todos os formulários personalizados, poderá usar esse campo como uma visualização ou filtro para ver quais tipos de objeto estão associados a cada formulário. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Valor antigo do número]</td> 
   <td>Em um relatório do [!UICONTROL Journal Entry], esse relatório exibe o valor original de um campo antes de ele ser atualizado. Uma vez que o valor de um campo é atualizado, ele será exibido como o [!UICONTROL Novo valor numérico] em um relatório [!UICONTROL Lançamento de entrada]. Para obter mais informações, consulte também "[!UICONTROL Novo valor numérico]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL somente sobre alterações]</td> 
   <td> <p>Um dos tipos de atualização do projeto [!UICONTROL]. Quando essa opção é selecionada, as linhas do tempo do [!UICONTROL Project Projected] e do [!UICONTROL Planned] são atualizadas apenas quando uma atualização ou alteração é feita no Projeto ou em uma tarefa no Projeto. Não atualiza o projeto todas as noites.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecione o Tipo de Atualização do projeto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa operacional]</td> 
   <td> <p>O nome do [!UICONTROL Problema] no [!DNL Workfront] banco de dados, usado em relatórios de modo de texto ou dados personalizados calculados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abrir]</td> 
   <td>Um problema ou tarefa que não está concluído, mas que está sendo trabalhado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>Abreviação de Organograma. Este é um gráfico que mostra a hierarquia de uma organização. Também está na guia na tela de detalhes do [!UICONTROL Usuário] que exibe e permite a configuração dos relacionamentos [!UICONTROL User] e [!UICONTROL Reporting] do [!UICONTROL Usuário].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuração organizacional]</td> 
   <td>Isso define [!UICONTROL Empresas], [!UICONTROL Grupos] e [!UICONTROL Perfis de segurança] para sua organização.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Outros grupos]</td> 
   <td> <p>Em um relatório ou visualização que lista usuários, esse campo exibe todos os grupos dos quais cada usuário é membro. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Substituir Moeda]</span> </td> 
   <td> 
    <div> 
     <p>Em um relatório da [!UICONTROL Função do trabalho], essa é a moeda associada a uma função de cargo. É uma substituição da [!UICONTROL Moeda de base], conforme estabelecido na área [!UICONTROL Configuração] pela variável [!DNL Workfront] administrador. </p> 
     <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Substituir Faturamento/Hora da Moeda]</span> </td> 
   <td> 
    <div> 
     <p>Em um relatório da [!UICONTROL Função do trabalho], essa é a taxa de faturamento por hora da função de trabalho usando a [!UICONTROL Substituir moeda] selecionada da função de trabalho.</p> 
     <p> Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Substituir Custo/Hora da Moeda]</span> </td> 
   <td> 
    <div> 
     <p>Em um relatório da [!UICONTROL Função do trabalho], essa é a taxa de custo por hora da função do trabalho usando a [!UICONTROL Substituir moeda] selecionada da função de trabalho. </p> 
     <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Proprietário]</td> 
   <td>O usuário responsável pela conclusão do objeto designado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Tipo de proprietário]</span> </td> 
   <td> 
    <div> 
     <p>Em um relatório da [!UICONTROL Meta], isso exibe o tipo de proprietário atribuído a uma meta estratégica. Estes são os tipos de proprietário de meta:</p> 
     <ul> 
      <li> <p>[!UICONTROL Usuário]</p> </li> 
      <li> <p>[!UICONTROL Equipe] </p> </li> 
      <li> <p>[!UICONTROL Grupo]</p> </li> 
     </ul> 
     <p>Nenhum valor é exibido neste campo quando o proprietário da meta é sua organização. </p> 
     <p>Isso requer uma licença adicional. Para obter informações sobre [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] visão geral</a>. </p> 
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
   <th>Nome Objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Parâmetro]</td> 
   <td> <p>Um [!UICONTROL parameter] é um campo personalizado. Você pode criar um relatório para todos os parâmetros ou campos personalizados em seu sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pai]</td> 
   <td>Em um relatório, esse campo mostra informações sobre o pai do objeto. Por exemplo, em um relatório do [!UICONTROL issue], ele pode mostrar informações sobre a tarefa ou projeto em que o problema está conectado; em um relatório de tarefa, ele pode mostrar informações sobre a tarefa pai direto ou sobre o projeto. Para obter mais informações sobre quais objetos podem ter pais em [!DNL Workfront], consulte a seção "Interdependência e hierarquia de objetos" no artigo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Entender objetos em [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atraso pai]</td> 
   <td>O tempo que deve passar entre o início da [!UICONTROL Tarefa pai] e o início da [!UICONTROL Subtarefa].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa pai]</td> 
   <td>Também conhecida como [!UICONTROL Summary Task]. Esta é uma tarefa que tem Subtarefas (também chamadas [!UICONTROL Tarefas filhas]). A [!UICONTROL Duração], [!UICONTROL Trabalho necessário] e [!UICONTROL Porcentagem concluída] da tarefa pai são calculadas a partir das subtarefas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Recursos em tempo parcial]</td> 
   <td>Um usuário licenciado que tem menos capacidade do que o agendamento padrão definido no sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Porcentagem concluída]</td> 
   <td> <p>Um projeto, tarefa ou campo de ocorrência que mostra qual porcentagem do trabalho associado à tarefa, projeto ou ocorrência foi concluída.</p> <p>Você pode atualizar esse campo manualmente para problemas e tarefas de trabalho. </p> <p>Para projetos e tarefas pai, esse campo é um rollup de todas as tarefas de trabalho e não é possível atualizá-lo manualmente. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Visão geral da [!UICONTROL Porcentagem concluída] do projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permissão]</td> 
   <td> <p>Direitos que são concedidos a um usuário em um objeto, normalmente dados para que ele possa concluir o trabalho no item ou visualizar o item. É possível conceder permissões para:</p> 
    <ul> 
     <li>[!UICONTROL Projetos]</li> 
     <li>[!UICONTROL Tarefas]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programas]</li> 
     <li>[!UICONTROL Relatórios]</li> 
     <li>[!UICONTROL Painéis]</li> 
     <li>[!UICONTROL Documentos]</li> 
     <li>[!UICONTROL Forms personalizado]</li> 
     <li>[!UICONTROL Exibições]</li> 
     <li>[!UICONTROL Filtros]</li> 
     <li>[!UICONTROL Groupings]</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral do compartilhamento de permissões em objetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Este é um tipo de licença completo no [!DNL Workfront] sistema. Os usuários devem ter isso para acessar todos os recursos em [!DNL Workfront].</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] visão geral das licenças</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (no [!DNL Scenario Planner])</td> 
   <td> <p>Um plano é o objeto principal ao trabalhar com a variável [!DNL Workfront] Planejador de cenário. Você pode destacar a estratégia para o futuro próximo e de longo prazo de sua empresa e identificar cada resultado de alto nível e adicioná-lo como plano à variável [!DNL Workfront] Planejador de cenário. </p> <p>Não é possível exibir [!DNL Scenario Planner] planos em um relatório e não é possível acessá-los por meio da variável [!DNL Workfront] API. </p> <p>O [!DNL Scenario Planner] exige uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">O [!DNL Scenario Planner] visão geral</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planejado]</td> 
   <td> <p>O período durante o qual algo está programado para ocorrer. Ao criar projetos, tarefas ou problemas no [!DNL Workfront], você estabelece as datas de início e término planejadas, bem como o período planejado durante o qual ocorrem. Esses valores representam sua intenção original ou estimativa de quanto tempo um item deve demorar para ser concluído. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefício planejado]</td> 
   <td>Esta é uma entrada manual para o Gerente de projeto estimar se a conclusão de um projeto traria algum benefício monetário para a organização. A especificação desse valor pode fazer parte da montagem de um [!UICONTROL Business Case] para o projeto. Você deve ter permissões do [!UICONTROL Manage] para atualizar esse valor.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Horas Planejadas Orçadas]</td> 
   <td> <p>Em um relatório [!UICONTROL Hora do orçamento], exibe a quantidade de horas orçadas para Projetos ou [!UICONTROL Funções de trabalho] no [!UICONTROL Planejador de recursos]. </p> <p>Para obter informações sobre como orçar projetos ou funções no [!UICONTROL Resource Planner], consulte o artigo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Recursos de orçamento no [!UICONTROL Resource Planner] usando as exibições [!UICONTROL Project] e [!UICONTROL Role]</a>. Para obter informações sobre o relatório [!UICONTROL Horário orçado], consulte o artigo <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Relatório: Hora do Orçamento</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de conclusão planejada]</td> 
   <td> <p>Você pode definir manualmente a [!UICONTROL Data de conclusão planejada] para uma data de sua escolha. Se você não definir a [!UICONTROL Data de conclusão planejada], [!DNL Workfront] O configura automaticamente. Quando definido automaticamente, a [!UICONTROL Data de conclusão planejada] é: [!UICONTROL Data de início planejada] + [!UICONTROL Duração]</p> <p>Para obter mais informações, consulte os seguintes artigos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Visão geral da tarefa [!UICONTROL Data de conclusão planejada]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Definir o projeto [!UICONTROL Data de conclusão planejada]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo planejado]</td> 
   <td> <p>Um total do [!UICONTROL Custo planejado da mão de obra] e o [!UICONTROL Custo de despesa planejada] do projeto. Isso não inclui o [!UICONTROL Custo de Risco Planejado] no projeto.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Duração planejada]</td> 
   <td> <p>A [!UICONTROL Duração planejada] de uma tarefa geralmente é a mesma que a [!UICONTROL Duração] da tarefa. Ela representa a diferença em dias entre a [!UICONTROL Início planejado] e as [!UICONTROL Datas de conclusão planejadas] da tarefa. </p> <p>Quando a tarefa tem um Tipo [!UICONTROL Duração] de [!UICONTROL Esforço orientado], a [!UICONTROL Duração planejada] pode ser diferente da [!UICONTROL Duração] da tarefa, com base na quantidade de recursos que você atribui à tarefa. </p> <p>Por exemplo, se uma tarefa com um Tipo de [!UICONTROL Duração] de [!UICONTROL Esforço Orientado] tiver uma [!UICONTROL Duração] de 3 dias e você atribuir um recurso com um cronograma de tempo completo à tarefa, a [!UICONTROL Duração Planejada] também será de 3 dias. Se você atribuir três recursos com um cronograma de tempo completo à mesma tarefa, a [!UICONTROL Duração] permanecerá em 3 dias, mas a [!UICONTROL Duração planejada] se tornará 1 dia. A [!UICONTROL Duração planejada] também altera as datas de [!UICONTROL Início planejado] e [!UICONTROL Conclusão planejada] da tarefa para refletir a nova [!UICONTROL Duração planejada]. Como resultado, a linha do tempo do projeto também é afetada. </p> <p>Para obter mais informações sobre a diferença entre [!UICONTROL Duração] e [!UICONTROL Duração planejada] para tarefas, consulte o artigo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Diferença entre [!UICONTROL Duração planejada] e [!UICONTROL Duração] para tarefas</a>.</p> <p>Projetos e problemas não têm uma [!UICONTROL Duração planejada]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Duração planejada Minutos]</td> 
   <td> <p>A [!UICONTROL Duração planejada] de um projeto ou um problema é a [!UICONTROL Duração] do projeto ou problema em minutos. </p> <p>As tarefas não têm um campo [!UICONTROL Minutos de duração planejada]. </p> <p>[!UICONTROL Tarefas do modelo] tem um campo [!UICONTROL Minutos da duração planejada] que exibe a [!UICONTROL Duração planejada] da tarefa em minutos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo de Despesa Planejada]</td> 
   <td> <p>A soma dos [!UICONTROL Quantias Planejadas] para todas as despesas registradas em um projeto ou tarefa.</p> <p><b>EXEMPLO</b></p>
   <p>Se você criar uma despesa para a Tarefa 1 e inserir $600,00 no campo [!UICONTROL Quantia Planejada], o [!UICONTROL Custo de Despesa Planejada] para essa tarefa será de $600,00. </p> 
   <p>Para um projeto, [!DNL Workfront] O usa a seguinte fórmula para calcular o [!UICONTROL Custo de Despesa Planejada]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Horas planejadas]</td> 
   <td> <p>Este campo aparece nos [!UICONTROL projetos], [!UICONTROL tarefas] e emite áreas, relatórios para projetos, tarefas ou problemas e ferramentas de gerenciamento de recursos como o [!UICONTROL Resource Planner], o [!UICONTROL Workload Balancer] e o relatório [!UICONTROL Usation]. </p> <p>Ele mostra a quantidade de horas que o Proprietário do Projeto estima que cada tarefa ou emissão deve levar para ser concluída. Para projetos, geralmente é um rollup das [!UICONTROL Horas Planejadas] das tarefas no projeto. </p> <p>O campo [!UICONTROL Horas planejadas] pode exibir informações diferentes dependendo de onde você as visualiza. Para obter informações sobre Horas Planejadas, consulte <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Visão geral das Horas Planejadas</a>.</p> <p>As Horas Planejadas são armazenadas em minutos na variável [!DNL Workfront] banco de dados. Ao gravar cálculos usando esse campo, verifique se as horas são exibidas como minutos.<br></p> <p>Por padrão, as Horas Planejadas são distribuídas igualmente para todos os dias dentro da duração de um item de trabalho e também igualmente para todos os recursos atribuídos à tarefa. Os usuários podem atualizar a quantidade diária de Horas Planejadas para um item de trabalho ou as Horas Planejadas individuais para cada destinatário.</p> <p>A atualização deste campo difere para projetos, tarefas e problemas: </p> 
    <ul> 
     <li> <p>Em caso de problemas, é possível atualizar manualmente esse campo. Horas Planejadas de Edição não são adicionadas às Horas Planejadas do Projeto. </p> <p>Dica: Em um relatório de edição, um dos campos [!UICONTROL Horas planejadas] é substituído pelo campo [!UICONTROL Trabalho]. O campo exibe o número de Horas Planejadas sobre o problema. Para obter mais informações, consulte os campos "trabalho" ou "[!UICONTROL Trabalho]" nesta tabela. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Para tarefas, você pode atualizar manualmente esse campo quando o [!UICONTROL Duration Type] da tarefa for [!UICONTROL Calculated Assignment] ou [!UICONTROL Simple]. Esse campo é calculado por [!DNL Workfront] quando o [!UICONTROL Duration Type] da tarefa for [!UICONTROL Calculated Work] ou [!UICONTROL Effort Driven].<br>Para obter informações sobre a [!UICONTROL Duração da tarefa], consulte o artigo <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão geral da tarefa [!UICONTROL Duração] e [!UICONTROL Tipo de duração]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Para projetos, [!DNL Workfront] O calcula as Horas Planejadas adicionando todas as Horas Planejadas de todas as tarefas no projeto. </p> </li> 
    </ul> <p><b>DICA</b></p> <p>Você pode exibir [!UICONTROL Horas planejadas] no [!UICONTROL project], na [!UICONTROL task] ou nos relatórios [!UICONTROL issues] também usando o modo de texto e os campos adicionais de referência. Para obter mais informações, consulte o<code>work</code>", "[!UICONTROL Trabalho]" e "<code>workRequiredExpression</code>" nesta tabela. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo planejado da mão de obra]</td> 
   <td> 
    <p>Para uma tarefa, a taxa horária do usuário ou função multiplicada pelo número de horas atribuídas ao usuário ou função.</p> <p>Para um projeto, é um total de todos os [!UICONTROL Custos planejados de mão de obra] de todas as tarefas.</p> <p>Se a taxa do usuário ou da função for usada depende do Tipo de Custo selecionado para a tarefa em questão. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md">Rastrear custos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Receita planejada]</td> 
   <td> <p>Tarefas e projetos podem exibir um valor para a [!UICONTROL Receita planejada] em [!DNL Workfront]. [!UICONTROL Receita planejada] representa a quantidade de dinheiro associada às [!UICONTROL Horas planejadas] das tarefas no projeto. Para projetos, também pode incluir a [!UICONTROL Receita fixa] do projeto. </p> <p>Para tarefas, essa é a receita associada às [!UICONTROL Horas planejadas] de tarefas. As Horas Planejadas de todas as tarefas são acumuladas até as Horas Planejadas do projeto para contribuir para o cálculo do projeto [!UICONTROL Horas Planejadas]. </p> 
   <p>[!DNL Workfront] O calcula a [!UICONTROL Receita planejada] para tarefas e projetos usando as seguintes fórmulas:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>O projeto [!UICONTROL Receita planejada] exibido na área [!UICONTROL Detalhes do projeto] e nos relatórios do projeto é diferente da Receita planejada exibida no relatório [!UICONTROL Utilização]. </p> <p>A [!UICONTROL Receita planejada] na área [!UICONTROL Detalhes do projeto] reflete a receita da tarefa, bem como a receita fixa do projeto. A [!UICONTROL Receita planejada] no [!UICONTROL Relatório de utilização] exibe [!UICONTROL Receita planejada] associada apenas às tarefas no projeto. </p> 
     <p><b>EXEMPLO</b></p>  
      <p>Se o projeto tiver uma tarefa com 10 horas, atribuída a um consultor com uma taxa de US$ 20 por hora e o projeto tiver US$ 100 [!UICONTROL Receita fixa], o relatório [!UICONTROL Utilização] exibirá US$ 200 para [!UICONTROL Receita Planejada] (a [!UICONTROL Receita Planejada] associada às horas na tarefa). A seção [!UICONTROL Detalhes do projeto] exibe $300 (a [!UICONTROL Receita planejada] da tarefa e a Receita fixa do projeto). </p> 
    <p>Para obter informações sobre como rastrear receita em [!DNL Workfront] see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Visão Geral da Faturamento e Receita</a>. </p> 
    <p>Para obter informações sobre os cálculos da [!UICONTROL Receita planejada] no [!UICONTROL Utilização report], consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Exibir informações de utilização de recursos </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo de Risco Planejado]</td> 
   <td> <p>O total do [!UICONTROL Custo Potencial] de todos os riscos no fator do projeto na probabilidade de ocorrerem. Esse valor não está incluído no [!UICONTROL Custo planejado] do projeto.</p> <p>O [!UICONTROL Custo de Risco Planejado] de um projeto é calculado pela seguinte fórmula:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>Uma coleção definida pelo administrador de Guias e Seções do Portal que aparece na [!DNL Workfront] Aplicativo [!UICONTROL Início] e outros Painéis.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>Um componente de uma guia em uma página de painel ou portal. Geralmente, um único Relatório, Gráfico, Calendário ou lista de informações-chave.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>Uma guia em um portal ou painel que contém até três seções do portal.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Uma coleção de projetos com características unificadoras. Esses projetos geralmente competem pelos mesmos recursos, orçamento ou período. É possível dividir o Portfolio em Programas e associar os projetos aos Programas antes que eles sejam adicionados a um Portfolio.</p> <p>Para obter mais informações sobre portfólios, consulte <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Visão geral do Portfolio em [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>Uma área de prática focada no gerenciamento de uma coleção ou programas relacionados e esforços do projeto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Otimizer]</td> 
   <td>A [!DNL Workfront] para ajudar a avaliar e priorizar projetos dentro de um portfólio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Owner]</td> 
   <td>A parte interessada responsável pela definição de prioridades e pelo orçamento de uma carteira.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custo do Risco Potencial]</td> 
   <td>Este é um campo de projeto que você pode localizar em listas e relatórios. Mostra o custo potencial dos riscos associados ao projeto, caso estes ocorram. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular Custo de Risco Potencial </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessor]</td> 
   <td> <p>Uma tarefa que deve ser concluída antes da conclusão de uma tarefa dependente. Também é uma tarefa marcada como uma [!UICONTROL Dependency] para outra tarefa. Os antecessores permitem que o planejador defina a lógica de dependência de sequência, como iniciar uma tarefa após a conclusão de outra tarefa.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Visão geral dos antecessores de tarefas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Empresa principal]</td> 
   <td>A Empresa à qual o usuário pertence, conforme designado nas configurações do usuário. As empresas também podem ser associadas a Projetos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contato principal]</td> 
   <td><p>O [!UICONTROL Primary Contact] é o criador de um problema e é automaticamente designado por [!DNL Workfront] quando a pessoa cria o problema. Você pode atualizar manualmente esse campo se tiver [!DNL Manage] permissões para o problema. Um problema pode ter apenas um Contato Principal.</p> 
   <p>Se você alterar o Contato principal, o usuário originalmente designado como o contato principal ainda terá acesso ao problema no [!UICONTROL Manager].</p>
   <p>Ao converter um problema em uma tarefa ou projeto, o usuário designado como [!UICONTROL Primary Contact] do torna-se o [!UICONTROL Converted Issue Originator] do projeto ou tarefa. Se o [!UICONTROL Primary Contact] do problema for atualizado após a conversão, o [!UICONTROL Converted Issue Originator] será preservado como o [!UICONTROL Primary Contact] do problema no momento em que a conversão aconteceu. Consulte também "[!UICONTROL Converted Issue Originator]" neste artigo.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Prioridade]</td> 
   <td>Um valor que pode ser atribuído a uma tarefa, ocorrência ou projeto para designar o quão importante ele é. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Privado]</td> 
   <td>Em uma [!UICONTROL Nota] ou [!UICONTROL Documento], essa opção torna esse objeto oculto para a maioria dos visualizadores. Para uma fila de suporte técnico privado, somente os usuários na equipe de fila podem enviar problemas para essa fila por meio da área de [!UICONTROL Help Desk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Perfil]</td> 
   <td>Todas as informações sobre uma conta de usuário.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>Um subconjunto dentro de um portfólio, em que projetos semelhantes podem ser agrupados para obter um benefício bem definido.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gerenciamento do programa]</td> 
   <td>Gerenciamento de dependências entre projetos, riscos, problemas, requisitos e soluções para manter o programa saudável e alcançar o benefício definido do programa.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Proprietário do programa]</td> 
   <td>A parte interessada responsável pela supervisão e organização das atividades, a fim de assegurar que os objetivos do projeto sejam coerentes com os objetivos da empresa.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>Em um relatório da [!UICONTROL Meta], isso exibe a porcentagem da proximidade de conclusão de um objetivo estratégico. A porcentagem do progresso é exibida como um número. Para obter informações sobre metas estratégicas, consulte "[!UICONTROL Objetivo]" nesta tabela.</p> <p>Este campo estará visível somente se sua organização tiver comprado [!DNL Workfront] Metas. Para obter informações sobre como gerenciar metas estratégicas usando [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Adicionar projetos às metas em [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status de progresso]</td> 
   <td> <p>Em um relatório de Projeto, Tarefa e Meta, esse campo exibe o Status do Progresso de projetos, tarefas ou metas estratégicas. Para obter mais informações, consulte os seguintes artigos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Visão geral do status de progresso do projeto</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Visão geral do status de progresso da tarefa</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Visão geral do progresso e da condição da meta em [!DNL Adobe Workfront Goals]</a> </p>
     <p>O relatório da [!UICONTROL Meta] e o [!UICONTROL Progress Status] para [!DNL goals] estiverem visíveis somente se a organização tiver comprado [!DNL Workfront Goals]. Para obter informações sobre objetivos estratégicos em [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] visão geral</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>Uma grande quantidade de trabalho que deve ser concluída dentro de um período de tempo específico e deve utilizar um orçamento específico e um número de recursos. Para gerenciá-lo, divida o projeto em uma série de tarefas. Concluir todas as tarefas resulta na conclusão do projeto. Para obter informações sobre o planejamento de um projeto, consulte <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Planejar uma visão geral do projeto</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuições do projeto Horas planejadas]</td> 
   <td> <p>Em um relatório da [!UICONTROL Initiative Job Role], esse relatório exibe o número de [!UICONTROL Planned Hours] associado a uma função de trabalho atribuída a tarefas ou problemas no projeto. Este campo e o tipo de relatório [!UICONTROL Initiative Job Role] não são exibidos em sua [!DNL Workfront] , a menos que sua empresa tenha comprado um [!DNL Workfront Scenario Planner] licença. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">O [!DNL Workfront Scenario Planner] visão geral</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Detalhes do projeto]</td> 
   <td>Os detalhes do status atual de um Projeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo Previsto do Projeto]</td> 
   <td> <p> Este é o [!UICONTROL Custo orçado] de um projeto como ele é exibido em listas e relatórios.</p><p>Consulte também "[!UICONTROL Custo orçado]" neste artigo.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gerenciamento de projetos]</td> 
   <td>Um conjunto de políticas que governa os limites para a criação, categorização e nomeação de projetos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Despesas gerais do projeto]</td> 
   <td>Em um relatório [!UICONTROL Hora], esse campo é reservado para informações financeiras vinculadas às horas registradas com o tipo de hora do [!UICONTROL Project Time]. Os projetos podem ter suas próprias Taxas de Faturamento e, se uma hora for registrada diretamente em um projeto, essas taxas serão usadas em cálculos. Com base nas configurações do projeto, os projetos também podem ter moedas diferentes e pode haver uma conversão de moeda para essas horas. O objeto [!UICONTROL Project Overhead] permite [!DNL Workfront] para obter essas informações.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proprietário do projeto]</td> 
   <td>O usuário responsável por gerenciar o escopo, a linha do tempo e as atribuições de um projeto. O aprovador padrão para ordens de alteração, alterações financeiras e resultados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planejamento de projeto]</td> 
   <td>Processos para desenvolver e manter o cronograma do projeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projetor]</td> 
   <td>Um perfil de parte interessada designado com o qual cada usuário deve se relacionar. Em [!DNL Workfront], eles são designados como [!UICONTROL Access Levels]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Teams]</td> 
   <td> <p>A coleção de Usuários ou Funções atribuídas a um Projeto</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Visão geral da equipe do projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rastreamento de projeto]</td> 
   <td>Os dados utilizados para medir a saúde e o âmbito de um projeto</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projetado]</td> 
   <td> <p>Uma estimativa do carimbo de data e hora de quando o trabalho será concluído com base nas horas planejadas e na porcentagem de conclusão de uma tarefa, emissão ou projeto.</p> <p>Refere-se às datas ou à [!UICONTROL Duração] de tarefas, problemas ou projetos. Geralmente, ele designa datas e durações que são mais verdadeiras para a vida útil dos itens de trabalho, depois que algum trabalho já foi concluído ou algum tempo passou. </p> <p>Por exemplo, a [!UICONTROL Data de conclusão projetada] de uma tarefa é a data em que [!DNL Workfront] estima que a tarefa será concluída, com base no trabalho feito até agora, no número de pessoas atribuídas a ela e no tempo decorrido desde a data de início.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Prazo da prova]</td> 
   <td> <p>Nos relatórios que contêm o objeto [!UICONTROL Document Version] (como um relatório [!UICONTROL Document Version] e o relatório [!UICONTROL Proof Approval]), esse campo exibe o dia da semana, a data, a hora do dia e o ano do prazo de prova.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisão de prova]</td> 
   <td> <p>Nos relatórios que contêm o objeto [!UICONTROL Versão do documento] (como um relatório [!UICONTROL Versão do documento] e o relatório [!UICONTROL Aprovação da prova]), esse campo exibe o status de decisão da prova (pendente, alterações necessárias ou aprovadas)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da prova]</td> 
   <td> <p>Nos relatórios que contêm o objeto [!UICONTROL Document Version] (como um relatório [!UICONTROL Document Version] e o relatório [!UICONTROL Proof Approval]), esse campo exibe o nome da prova.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Páginas de prova]</td> 
   <td> <p>Nos relatórios que contêm o objeto [!UICONTROL Document Version] (como um relatório [!UICONTROL Document Version] e o relatório [!UICONTROL Proof Approval]), esse campo exibe o número de páginas incluídas na prova.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Progress]</td> 
   <td> <p>Nos relatórios que contêm o objeto [!UICONTROL Document Version] (como um relatório [!UICONTROL Document Version] e o relatório [!UICONTROL Proof Approval]), é exibido o status do progresso da prova ([!UICONTROL Enviado], [!UICONTROL Aberto], [!UICONTROL Comentado], [!UICONTROL Decisão tomada]).</p> <p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Visão geral do progresso da prova</a> em <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Visão geral do progresso e status da prova</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>Um processo de revisão em que um ou mais usuários marcam e comentam o conteúdo que deve ser alterado em uma imagem, um documento de texto, um vídeo ou conteúdo interativo da Web.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Público]</td> 
   <td>Em uma [!UICONTROL Nota] ou [!UICONTROL Documento], essa opção torna esse objeto acessível a outros usuários ou mesmo a pessoas de fora [!DNL Workfront]. Para uma [!UICONTROL Help Desk Queue], [!UICONTROL Público] significa que todos os usuários que podem enviar problemas podem enviar problemas por meio da área da [!UICONTROL Help Desk].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Qualidade]</td> 
   <td>A percepção da qualidade do trabalho dentro da organização.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fila]</td> 
   <td>Também chamado de [!UICONTROL Help Desk Queue]. Este é um Projeto que foi publicado na área [!UICONTROL Help Desk] para permitir que os usuários enviem Problemas a ele. Geralmente, as filas são criadas para tópicos específicos, como Erros, Solicitações de projeto etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propriedades da fila]</td> 
   <td>Essas configurações definem Regras de envio de ocorrência para um Projeto que está sendo publicado no [!UICONTROL Help Desk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tópico da fila]</td> 
   <td> <p>Uma propriedade em uma [!UICONTROL Help Desk Queue] que permite que os usuários que enviam um problema selecionem um Tópico. Os tópicos podem:</p> 
    <ul> 
     <li>Esteja associado a um Formulário de dados personalizado.</li> 
     <li>Atribua o Problema automaticamente a um Usuário, Função ou Equipe por meio da Regra de Roteamento definida no Tópico selecionado.</li> 
     <li>Mova o problema para um Projeto ou Fila diferente pelo conjunto de regras de roteamento no tópico selecionado.</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Criar Tópicos da Fila</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Classificação]</td> 
   <td> <p>Em um relatório do [!UICONTROL Nível de acesso], é possível indicar manualmente uma [!UICONTROL Classificação] do [!UICONTROL Nível de acesso]. Isso ajuda você, como a [!DNL Workfront] para identificar visualmente o nível de complexidade associado a cada Nível de acesso. Por exemplo, você pode fornecer números mais baixos para Níveis de Acesso mais complexos no nível do ([!UICONTROL Plano]) e números mais altos para Níveis de Acesso menos complexos no nível do ([!UICONTROL Requester]). Não é possível classificar os Níveis de Acesso padrão. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pronto]</td> 
   <td> <p>Este campo em um relatório de tarefa indica se uma tarefa [!UICONTROL Agile] foi marcada como [!UICONTROL Ready] no backlog. Esse sinalizador se aplica somente às tarefas do [!UICONTROL Ágil], que são tarefas atribuídas a uma equipe do [!UICONTROL Ágil]. </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Frequência de recorrência]</td> 
   <td> <p>Um campo que é exibido na caixa [!UICONTROL Detalhes da tarefa] ou na caixa [!UICONTROL Editar tarefa] de um pai de tarefas recorrentes. É a frequência com que as tarefas na recorrência ocorrem. Para obter informações sobre como criar tarefas recorrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Criar tarefas recorrentes</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número de referência]</td> 
   <td> <p>Projetos, tarefas e problemas são associados automaticamente a um número de referência exclusivo à medida que são criados. Você pode visualizar o [!UICONTROL Número de referência] na página [!UICONTROL Detalhes] de projetos, tarefas ou problemas, ou em uma lista ou relatório. </p> <p><b>DICA</b><p><br>Você pode diferir para números de referência quando dois itens têm o mesmo nome, já que os números de referência são sempre exclusivos. </p> <p>[!DNL Workfront] gera automaticamente o número de referência sequencial no nível do sistema. Cada projeto, tarefa ou problema obtém o próximo número disponível na sequência. <br></p> <p>Por exemplo, se o Usuário A criar uma tarefa, [!DNL Workfront] pode atribuir automaticamente à tarefa o Número de referência de 100. Se o Usuário B criar um problema logo depois disso, [!DNL Workfront] atribui ao problema o Número de referência 101. Não é possível editar números de referência manualmente. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reject Issue]</td> 
   <td>Em um relatório de projeto ou tarefa, esse é o problema criado quando a aprovação do projeto ou da tarefa é rejeitada. Para obter informações sobre problemas de rejeição, consulte o artigo <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Criar um processo de aprovação para itens de trabalho</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo de Risco Restante]</td> 
   <td> <p>Um campo de projeto que mostra a diferença entre o [!UICONTROL Custo de Risco Planejado] de um projeto e o total de todos os [!UICONTROL Custos Reais] de todos os riscos do projeto. </p> <p>O [!UICONTROL Custo de Risco Restante] de um projeto é calculado usando a seguinte fórmula:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Replanejamento]</td> 
   <td>Alterar as datas de um projeto para reparar ou superar problemas. Por exemplo, um projeto que está em espera por vários meses precisaria ser replanejado para refletir datas precisas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Relatório]</td> 
   <td>Um gráfico ou tabela contendo informações sobre um dado [!DNL Workfront] e seus atributos relacionados.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Solicitação]</td> 
   <td> <p>Um tipo de problema que é acionado em uma única fila centralizada e não está relacionado a um esforço de trabalho contínuo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Fila de solicitações]</td> 
   <td>O backlog de problemas gerenciados por um processo de tráfego e triagem.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Velocidade da solicitação]</td> 
   <td>Tempo total do ciclo de trabalho para receber e concluir uma solicitação.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>Normalmente, é do tipo licença. Um usuário com uma licença do Requester pode enviar solicitações para que um novo trabalho ocorra no sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Horário reservado]</td> 
   <td>Dias especificados no Horário Pessoal de um Usuário, indicando que o Usuário não estará disponível para trabalho. Consulte "[!UICONTROL Dias não úteis]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver Problema]</td> 
   <td> <p>Em um relatório de problema, use esse campo em exibições ou filtros para se referir ao problema que resolve o problema. </p> <p>Para obter informações sobre como exibir a resolução de objetos em relatórios, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Exibir informações de objetos resolvíveis e resolvidos em um relatório</a> em <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral da Solução e Objetos Resolvíveis </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver Projeto]</td> 
   <td> <p>Em um relatório de problema, use esse campo em exibições ou filtros para se referir ao projeto que resolve o problema. </p> <p>Para obter informações sobre como exibir a resolução de objetos em relatórios, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Exibir informações de objetos resolvíveis e resolvidos em um relatório</a> em <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral da Solução e Objetos Resolvíveis </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver Tarefa]</td> 
   <td> <p>Em um relatório de problema, use esse campo em exibições ou filtros para se referir à tarefa que resolve o problema. </p> <p>Para obter informações sobre como exibir a resolução de objetos em relatórios, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Exibir informações de objetos resolvíveis e resolvidos em um relatório</a> em <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral da Solução e Objetos Resolvíveis </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurso]</td> 
   <td>Usuários e/ou funções existentes no sistema e atribuídos a equipes e tarefas do projeto.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>O [!UICONTROL Resource Management] é um conjunto de ferramentas corporativas que permite prever com precisão o uso de seus recursos com base em sua disponibilidade para que o trabalho que deve ser feito seja concluído a tempo e no orçamento. </p> <p>Com as ferramentas de Gerenciamento de Recursos, você pode planejar a capacidade de longo prazo e as necessidades de agendamento de curto prazo para seus recursos. </p> <p>Para obter informações sobre o Gerenciamento de recursos em [!DNL Workfront], consulte <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introdução ao Gerenciamento de recursos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL IDs do Gerenciador de recursos]</td> 
   <td><p>Em um relatório de projeto, você pode usar essa opção ao criar um filtro para localizar um gerenciador de recursos específico. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Managers]</td> 
   <td> <p>Em um relatório de projeto ou exibição de lista, esse é um campo informativo que exibe os usuários designados para realizar atividades de gerenciamento de recursos no projeto.  Quando você usa "[!UICONTROL Resource Managers]" em um relatório, uma lista de gerentes de recursos é exibida, com cada gerenciador de recursos no projeto separado por vírgula. Você pode designar até 30 gerentes de recursos em um determinado projeto.</p> <p>Para obter mais informações, consulte o artigo <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Designar Gerentes de Recursos para um projeto ou modelo </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
   <td>As horas orçadas para o projeto e os recursos associados a ele no [!UICONTROL Resource Planner]. Consulte também "[!UICONTROL Horas orçadas]" neste artigo. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>Uma [!DNL Workfront] ferramenta que permite visualizar e gerenciar recursos em projetos, funções ou usuários. Para obter mais informações, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Visão geral do Planejador de recursos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planner de Recursos Custo de Mão de obra Orçada]</td> 
   <td> <p>Esses são os custos associados às horas orçadas para funções de job do projeto usando o Planejador de Recursos. </p> <p>Consulte também "Custo de mão de obra orçada" neste artigo. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Resource Pools]</td> 
   <td> <p>Os Pools de Recursos são coleções de usuários que podem ser associados a um projeto. Os usuários no mesmo Pool de Recursos geralmente pertencem ao mesmo departamento, têm habilidades semelhantes ou complementares ou são financiados pelo mesmo orçamento. Você pode associar vários Pools de Recursos a um projeto ou a um usuário. Um pool de recursos pode ser atribuído exclusivamente a um projeto ou compartilhado por vários projetos.</p> 
   <p>Para obter mais informações sobre pools de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Visão geral dos pools de recursos </a>.</p> 
   <p>Nos relatórios do projeto, os Grupos de Recursos mostram todos os pools associados a um projeto. Este objeto não pode ser usado em um agrupamento.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilização de Recursos]</td> 
   <td>Um relatório que exibe o número de horas disponíveis durante um determinado período e o número de horas agendadas para cada usuário no relatório. Isso também é calculado em [!UICONTROL Média de horas por dia] e em uma porcentagem de alocação.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Resultado]</td> 
   <td>Em [!DNL Workfront Goals], um resultado é um indicador de progresso para uma meta. Pode ser um número, um valor percentual ou um valor monetário que você atualiza manualmente. Não é possível exibir resultados em um relatório e não é possível acessá-los por meio da variável [!DNL Workfront] API. Para obter informações sobre atividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introdução aos resultados e atividades nas Metas da Adobe Workfront</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Receita]</td> 
   <td>Um valor faturável para a tarefa ou projeto. O valor pode ser por hora, fixo ou uma combinação de ambos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de receita]</td> 
   <td>O tipo de receita determina como a tarefa irá acumular receita. Alguns exemplos incluem [!UICONTROL Fixo por hora], [!UICONTROL Função por hora] e [!UICONTROL Função por hora com tampa]. Para obter informações sobre como rastrear receita em [!DNL Workfront] see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão Geral da Faturamento e Receita</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>Normalmente, é do tipo licença. Um usuário com uma licença do [!UICONTROL Reviewer] tem a capacidade de revisar e aprovar itens de trabalho no sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risco]</td> 
   <td> <p>Isso pode se referir aos seguintes conceitos em [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>Um campo em um projeto que indica o risco de um projeto. É possível priorizar a execução dos projetos com base no nível de risco. Os projetos podem ter os seguintes níveis de risco:</p> <p>- [!UICONTROL Muito Baixo]</p> <p>- [!UICONTROL Baixo]</p> <p>- [!UICONTROL Médio]</p> <p>- [!UICONTROL High]</p> <p>- [!UICONTROL Muito Alto]</p> <p>Os níveis de riscos indicados para um projeto não podem ser personalizados. </p> <p> Para obter informações sobre como atualizar o Risco de um projeto, consulte a seção "Configurações do projeto" do artigo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar projetos</a>. É possível exibir o campo de risco de um projeto em relatórios. </p> </li> 
     <li> <p>Um evento que pode ocorrer durante a vida de um projeto que identifica um impacto potencial no custo, escopo ou agendamento do projeto. Você define riscos potenciais para um projeto e associa uma probabilidade de ocorrerem ou um custo à medida que cria o Caso de negócios do projeto. Para obter informações sobre como adicionar riscos ao Caso de negócios do projeto, consulte "Criar e editar riscos em projetos". </p> <p>Não é possível exibir riscos definidos no [!UICONTROL Business Case] nos relatórios. Você só pode exibir vários tipos de Custos de risco em relatórios e listas. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custo do risco]</td> 
   <td> <p>O custo associado aos riscos em um projeto. A seguir estão os custos de risco associados aos projetos que podem ser exibidos nos relatórios:</p> 
    <ul> 
     <li> <p>[!UICONTROL Custo Real]: um campo em um risco que mostra o custo real do risco que ocorreu. Além dos relatórios e listas, você pode localizá-los na caixa [!UICONTROL Editar risco] ao editar ou criar um risco. </p> <p>Para custos de projeto, tarefa ou emissão, consulte "[!UICONTROL Custo Real]" neste artigo. </p> </li> 
     <li> <p>[!UICONTROL Custo de Risco Planejado]: um campo no projeto que mostra um total de todos os [!UICONTROL Custos de Risco Potencial] para o projeto. Consulte também "[!UICONTROL Custo de Risco Planejado]" neste artigo. </p> <p>Para obter informações sobre o Custo do Risco Potencial, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular Custo de Risco Potencial </a>. </p> </li> 
     <li> <p>[!UICONTROL Custo de Risco Restante]: um campo no projeto que exibe a diferença entre o total dos [!UICONTROL Custos reais] de todos os riscos e o [!UICONTROL Custo de risco planejado]. Consulte também "Custo de Risco Restante" neste artigo. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gerenciamento de riscos]</td> 
   <td>Processos para identificar, mitigar e monitorar o risco.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Função]</td> 
   <td>Consulte "[!UICONTROL Função do trabalho]" neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Roteamento]</td> 
   <td>Atribuir ou mover um problema automaticamente, normalmente devido a um tópico da fila ou por ser a rota padrão (regra de roteamento) para a fila.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Regra de roteamento]</td> 
   <td>Uma configuração em Projetos e filas que atribui automaticamente um problema a um usuário, função ou equipe, ou moveu o problema para outro projeto ou fila. As Regras de Roteamento geralmente são usadas com Filas do Help Desk para atribuir automaticamente Problemas de entrada.</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pesquisa salva]</td> 
   <td>Uma pesquisa cujos critérios de pesquisa foram salvos. Pesquisas salvas facilitam a execução do mesmo novamente sem precisar inserir os critérios de pesquisa novamente.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Cenário] (em [!DNL Workfront Fusion]) </td> 
   <td> <p>Um cenário é composto por uma série de etapas (módulos) que indicam como os dados devem ser transferidos e transformados entre aplicativos/serviços.</p> <p>Para obter informações sobre cenários em [!DNL Workfront Fusion], consulte <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] visão geral do cenário</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cenário] (na variável [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>No [!DNL Scenario Planner], um cenário é uma cópia de um plano. </p> <p>O [!DNL Scenario Planner] exige uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">O [!DNL Scenario Planner] visão geral</a>. </p> <p>Para obter informações sobre como criar cenários, consulte <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Crie e compare cenários de plano na [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Programação]</td> 
   <td>O horário de trabalho semanal, incluindo os horários de trabalho, combinado com os dias de férias (como os feriados) e os dias de exceção (como o dia de trabalho de sábado). Os agendamentos podem ser aplicados a Projetos e Usuários.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Isenção da Programação]</td> 
   <td>Também conhecido como [!UICONTROL Modificado Shift]. Dias programados em contraste com os horários de trabalho semanais regulares definidos pelo horário. Por exemplo, um sábado agendado para funcionar, quando a Programação estiver configurada para Somente trabalhar de segunda a sexta-feira, seria uma [!UICONTROL Schedule Isenção].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Relatório agendado]</td> 
   <td> <p>Ao criar um relatório de relatórios, você pode exibir informações sobre os agendamentos do relatório, se o relatório estiver agendado para entrega usando o campo [!UICONTROL Relatório agendado]. Este campo mostra vários valores, um para cada agendamento de cada relatório, em uma lista com marcadores. Para obter mais informações sobre como agendar relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Visão geral da entrega de relatórios</a>.</p> <p>Como esse campo mostra vários valores, ele não pode ser usado em um agrupamento. Você pode acessá-lo somente em um filtro ou uma visualização. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alteração de escopo]</td> 
   <td>Uma [!UICONTROL Trilha de auditoria] que, se estiver ativa, gera uma nota sempre que uma alteração é feita no Escopo de um projeto ou tarefa, como se uma [!UICONTROL Task Duration] ou [!UICONTROL Predecessors] fossem alteradas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seção]</td> 
   <td>Uma área na tela, com seu próprio cabeçalho, criada para organizar os Dados personalizados para fins de exibição.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seção Break]</td> 
   <td>Uma lacuna ou borda entre seções.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Segurança]</td> 
   <td>As configurações que permitem que um usuário interaja com determinados objetos no sistema e não com outros. Consulte também "[!UICONTROL Níveis de acesso]" neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuração]</td> 
   <td>A área onde os administradores podem configurar as configurações e preferências do sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severidade]</td> 
   <td> <p>[!UICONTROL Gravidade] é uma indicação da probabilidade de um item afetar a conclusão do trabalho. Por exemplo, um problema com alta [!UICONTROL Severity] pode bloquear completamente a conclusão de uma tarefa, mas um problema com baixa [!UICONTROL Severity] pode ser meramente superficial.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Atualizar gravidade do problema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severidades]</td> 
   <td>Consulte "[!UICONTROL Severity]" neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Compartilhamento]</td> 
   <td>A ação de permitir que outros usuários visualizem ou editem um item específico em [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack Date]</td> 
   <td>Em uma visualização de tarefa ou relatório, a [!UICONTROL Slack Date] exibe a data exata em que uma tarefa pode definitivamente afetar a [!UICONTROL Data de conclusão] do projeto. Para obter informações sobre a [!UICONTROL Slack Date] de uma tarefa, consulte <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Visão geral da Data Slack da tarefa</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuições inteligentes]</td> 
   <td> <p>Ao atribuir tarefas ou problemas aos usuários, [!DNL Workfront] O faz recomendações ([!UICONTROL Atribuições inteligentes]) sobre quem os melhores usuários devem concluir o trabalho, com base no tempo que têm disponível para concluí-lo e em seu relacionamento com o projeto.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Visão geral de atribuições inteligentes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Origem]</td> 
   <td> <p>Indica o objeto pai de outro objeto. Por exemplo, um documento anexado a uma tarefa tem o nome da tarefa no campo [!UICONTROL Source] de um relatório ou visualização do [!UICONTROL Document]; um problema registrado em um projeto tem o nome do projeto no campo [!UICONTROL Source] de um relatório ou visualização da ocorrência. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de início]</td> 
   <td> <p>A Data em que o trabalho em um item está definido para iniciar. Há várias Datas de início em [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Planejado]</li> 
     <li>[!UICONTROL Real]</li> 
     <li>[!UICONTROL Projetado] </li> 
    </ul> <p>Em um [!UICONTROL Rate report], essa é a data em que uma nova taxa de faturamento de uma função de cargo é iniciada no nível do projeto. As horas associadas ao projeto que estão após essa data são multiplicadas por essa taxa de faturamento para calcular a receita no projeto. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Um indicador usado para sinalizar uma posição de workflow de um item de trabalho ou de uma meta estratégica.</p> <p>Para Projetos, o [!UICONTROL Status] é uma configuração no Projeto que indica se o Projeto é:</p> 
    <ul> 
     <li>[!UICONTROL Atual]</li> 
     <li>[!UICONTROL Em Retenção] </li> 
     <li>[!UICONTROL concluído] </li> 
     <li>[!UICONTROL inativo]</li> 
    </ul> <p>Para obter mais informações sobre o Status do projeto, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Acessar a lista de status de projeto do sistema</a>.</p>
    <p>Para Tarefas, o [!UICONTROL Status] é uma configuração na Tarefa que indica se a Tarefa é:</p> 
    <ul> 
     <li>[!UICONTROL Novo]</li> 
     <li>[!UICONTROL Em Andamento]</li> 
     <li>[!UICONTROL concluído]</li> 
    </ul> <p>Para obter mais informações sobre o Status da Tarefa, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Acessar a lista de status de tarefas do sistema</a></p> <p>Para problemas, o [!UICONTROL Status] é uma configuração do problema que indica se esse problema é:</p> 
    <ul> 
     <li>[!UICONTROL Novo]</li> 
     <li>[!UICONTROL Em Andamento]</li> 
     <li>[!UICONTROL Aguardando feedback]</li> 
     <li>[!UICONTROL Em Retenção]</li> 
     <li>[!UICONTROL Resolvido]</li> 
     <li>[!UICONTROL não resolverá]</li> 
     <li>[!UICONTROL Não Pode Duplicar]</li> 
     <li>[!UICONTROL Verificado Concluído]</li> 
     <li>[!UICONTROL Reaberto]</li> 
    </ul> <p>Para obter mais informações sobre Status do problema, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acesse a lista de status de problemas do sistema</a>.</p> 
    <p>Para metas estratégicas, o [!UICONTROL Status] é uma configuração na meta que indica se a meta é:</p> 
     <ul> 
      <li>[!UICONTROL Ativo]</li> 
      <li>[!UICONTROL Rascunho]</li> 
      <li>[!UICONTROL Inativo]</li> 
      <li>[!UICONTROL Fechado]</li> 
     </ul> 
     <p>Para obter mais informações sobre metas estratégicas, consulte "[!UICONTROL Meta]" ou "[!UICONTROL Metas]" neste artigo. </p> 
     <p>Para metas estratégicas, esse campo fica visível somente se a organização tiver comprado [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] visão geral</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alteração de status]</td> 
   <td>Uma [!UICONTROL Audit Trail]. Uma observação é gerada quando um usuário altera o Status do projeto, da tarefa ou do problema.</td> 
  </tr> 
  <tr> 
   <td>Ícones de Status</td> 
   <td> <p>É possível adicionar o campo integrado [!UICONTROL Status Icons] como uma coluna em suas visualizações para aumentar a visibilidade em pontos-chave sobre seus objetos, como:</p> 
    <ul> 
     <li>Um objeto tem documentos anexados</li> 
     <li>Um objeto está associado a um processo de aprovação</li> 
     <li>Um objeto tem observações adicionais associadas a ele</li> 
     <li>Uma despesa é faturável ou reembolsável </li> 
     <li>Uma tarefa está em um caminho crítico</li> 
     <li>Um usuário pertence a uma empresa, uma equipe ou está localizado em um fuso horário diferente </li> 
    </ul> <p>Você pode adicionar o campo [!UICONTROL Status Icons] nas exibições dos seguintes objetos: </p> 
    <ul> 
     <li>[!UICONTROL Tarefas]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Projetos]</li> 
     <li>[!UICONTROL Tarefas de modelo]</li> 
     <li>[!UICONTROL Modelos]</li> 
     <li>[!UICONTROL Despesas]</li> 
     <li>[!UICONTROL Documentos]</li> 
     <li>[!UICONTROL Usuários]</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ícones de status incorporados nas exibições</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atualização de status]</td> 
   <td> <p>Este campo mostra a atualização de status mais recente que os usuários forneceram no campo '[!UICONTROL Update Status]'. Os comentários feitos nas atualizações de status não são exibidos na coluna [!UICONTROL Atualização de status].</p> <p>Para mostrar os status '[!UICONTROL Novo],' '[!UICONTROL Em Processo]' e '[!UICONTROL Completo]', use a coluna [!UICONTROL Status].</p> <p>Os comentários feitos nas atualizações de status não são exibidos na coluna [!UICONTROL Atualização de status].</p> <p>Para obter mais informações sobre status, consulte o artigo <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Atualizar status da tarefa</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td>Consulte "[!UICONTROL Status]" neste artigo.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Um gráfico que representa o status das histórias (tarefas na metodologia ágil) e como elas estão progredindo para a conclusão.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Horas da história]</td> 
   <td>Uma métrica usada para medir a dificuldade ou a complexidade de uma História. As equipes ágeis podem escolher usar Horas ou Pontos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Pontos de história]</td> 
   <td>Uma métrica usada para medir a dificuldade ou a complexidade de uma História. As equipes ágeis podem escolher usar Horas ou Pontos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL estratégico]</td> 
   <td>Trabalho de longo prazo que muda a organização ou como ela funciona.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Alinhamento estratégico]</td> 
   <td>Avaliação e alinhamento das metas da empresa em portfólios e programas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assinantes]</td> 
   <td> <p>Usuários que assinam Projetos, Tarefas ou Problemas.</p> <p>Ao usar esse campo em um relatório, uma lista de assinantes é exibida, com cada assinante separado por vírgula.</p> <p>Para obter mais informações, consulte o artigo <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Inscrever-se em itens em [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa de resumo]</td> 
   <td>Consulte "[!UICONTROL Tarefa pai]" neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtarefa]</td> 
   <td>Uma tarefa filho, que está localizada em uma tarefa pai.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Governança do sistema]</td> 
   <td>Um conjunto de políticas que rege as mudanças e a manutenção de um sistema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Integração do sistema]</td> 
   <td>O processo de interligação física ou funcional de diferentes sistemas informáticos e aplicações informáticas, a fim de atuar como um todo coordenado.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Tarefa]</td> 
   <td> <p>Uma atividade que deve ser executada como uma etapa para atingir uma meta final (conclusão do projeto).</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Visão geral das tarefas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atributo da tarefa]</td> 
   <td>Outros campos ou objetos que estão associados a uma Tarefa e indicam determinados detalhes sobre ela. Alguns exemplos são [!UICONTROL Data de conclusão planejada] e [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Restrição de tarefa]</td> 
   <td>Consulte "[!UICONTROL Tipo de restrição]" e "[!UICONTROL Data da restrição]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gerenciamento de tarefas]</td> 
   <td>Um conjunto de políticas que governa os limites para criação, atribuição, fechamento e visibilidade de tarefas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Proprietário da tarefa]</td> 
   <td>A equipe ou usuário responsável pela estimativa de esforço e conclusão da tarefa</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Equipe]</td> 
   <td> <p>Uma coleção de usuários que trabalham para metas ou objetivos de negócios semelhantes. Esses usuários podem ser atribuídos coletivamente a um item de trabalho, atribuindo a equipe ao item de trabalho.</p> <p>Para obter mais informações sobre equipes, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Visão geral das equipes</a>.</p> <p>Os projetos podem ter uma [!UICONTROL Project Team], que contém todos os usuários ou funções associados ao trabalho no projeto.</p> <p>Para obter mais informações sobre equipes de projeto, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral da equipe do projeto</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Modelo]</td> 
   <td> <p>Os modelos de projeto são contornos genéricos de seus projetos mais repetíveis. Você pode definir tarefas, tópicos de fila, formulários personalizados, anexar documentos ou aprovações ao criar um modelo de projeto para economizar tempo quando precisar criar um novo projeto. </p> <p>Você pode anexar modelos a projetos existentes ou usá-los para criar novos projetos. Todas as informações especificadas no modelo são transferidas para os projetos que são criados usando. </p> <p>Para obter mais informações sobre modelos, consulte <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Visão geral do modelo de projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa de modelo]</td> 
   <td>Uma tarefa que faz parte de um modelo. Tarefas do modelo se tornam Tarefas no Projeto criado usando o Modelo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>Uma [!UICONTROL Nota] e sua coleção de respostas que se relacionam a um tópico específico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniatura]</td> 
   <td> <p> Em uma lista ou relatório do [!UICONTROL Document], ele exibe uma pré-visualização do documento em uma miniatura. </p> <p> Selecionar <strong>[!UICONTROL Miniatura]</strong>  para visualizar uma miniatura de 33-66 pixels no relatório. </p> <p>O tamanho da miniatura se ajusta ao modificar a largura da coluna em uma lista ou relatório.</p> <p>Consulte também "[!UICONTROL Miniatura grande]" neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo desligado]</td> 
   <td>Você pode criar um relatório [!UICONTROL Tempo desligado] para visualizar quando os usuários indicaram tempo de folga em seu perfil. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet]</td> 
   <td> <p>Um cartão de ponto que permite que os usuários insiram as horas reais em que passaram trabalhando em projetos, tarefas ou problemas, ou horas gastas em outras atividades não relacionadas ao trabalho, como reuniões ou treinamento. Além de inserir a quantidade de tempo gasto trabalhando, você também pode indicar se o tempo está relacionado ao trabalho ou se equivale ao tempo de sobrecarga usando Tipos de hora para definir suas entradas de tempo. Para obter informações sobre folhas de ponto, consulte <a href="../../../timesheets/timesheets/timesheets-overview.md">Visão geral das folhas de horas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Perfil de folha de horas]</td> 
   <td> <p>Um [!UICONTROL Timesheet Profile] é um modelo que [!DNL Workfront] O usa o para criar automaticamente folhas de horas para os usuários associados a elas. </p> <p>É possível definir várias configurações que serão aplicadas a cada folha de ponto durante a criação. Algumas dessas configurações são: com que frequência a folha de ponto deve ser criada (semanalmente, a cada duas semanas, duas vezes por mês ou mensalmente), o dia de início da folha de ponto, os aprovadores da folha de ponto, os [!UICONTROL Hour Types] disponíveis que os usuários podem associar com horas registradas.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL ID principal do pai] </td> 
   <td> <p>Este campo permite identificar e filtrar dados sobre um grupo de nível superior e seus subgrupos em uma lista ou relatório.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome principal] </td> 
   <td> <p>Este campo permite identificar dados sobre um grupo de nível superior e seus subgrupos em uma [!UICONTROL View] para uma lista ou relatório.</p> <p>Também é possível fazer isso usando o campo [!UICONTROL Top Parent ID] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Horas]</td> 
   <td> <p>Em um [!UICONTROL project report], esse campo exibe a soma arredondada de todas as horas no projeto, a última vez que as finanças do projeto foram calculadas. [!UICONTROL Horas reais] refletem as horas exatas registradas no projeto. Normalmente, as [!UICONTROL Horas reais] devem corresponder ao [!UICONTROL Total Hours]. Se o [!UICONTROL Total Hours] parecer significativamente diferente do campo [!UICONTROL Horas reais], você deverá Recalcular as finanças do projeto.</p> <p>Para obter mais informações sobre o recálculo das finanças do projeto, consulte o artigo <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Recalcular as finanças do projeto</a>.</p> <p>Em uma visualização da folha de ponto [!UICONTROL Padrão], esse campo se refere ao total de horas registradas para os itens das datas exibidas em uma folha de ponto. O campo [!UICONTROL Total Hours] das folhas de tempo nessa exibição integrada faz referência ao campo "[!UICONTROL hoursDuration]" que calcula dinamicamente a diferença em horas entre as datas inicial e final da folha de ponto. Isso é usado para exibir a coluna [!UICONTROL Total Hours] em vermelho se o usuário registrar mais tempo do que as horas disponíveis no intervalo de tempo da folha de ponto. Para obter mais informações, consulte <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Exibir o total de horas na folha de ponto</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de rastreamento]</td> 
   <td> <p>Um atributo de uma Tarefa. Isso determinou como e depois as linhas do tempo projetadas serão atualizadas para uma Tarefa. Por exemplo:</p> 
    <ul> 
     <li>[!UICONTROL Usuário deve atualizar] requer que uma tarefa seja atualizada manualmente. Caso contrário, ele se tornará [!UICONTROL Atrás da programação] e depois [!UICONTROL Tarde].</li> 
     <li>A [!UICONTROL Conclusão automática] concluirá automaticamente uma tarefa quando a Data de vencimento, ou [!UICONTROL Data de conclusão planejada], tiver passado.</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Visão geral do modo de rastreamento de tarefas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Um evento que inicia um cenário.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa com problemas]</td> 
   <td>Uma tarefa incompleta com uma condição de [!UICONTROL Atraso], [!UICONTROL Atrasado] ou [!UICONTROL Em Risco].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa Não Atribuída]</td> 
   <td>Uma Tarefa que não é atribuída a nenhum Usuário, Função ou Equipe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de atualização]</td> 
   <td> <p>Uma configuração no Projeto que determina quando a linha do tempo Projetada do Projeto será recalculada. As opções são:</p> 
    <ul> 
     <li>[!UICONTROL Automático e On Change]</li> 
     <li>[!UICONTROL Automático somente]</li> 
     <li>[!UICONTROL Manual only] </li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecione o Tipo de Atualização do projeto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuário]</td> 
   <td>Uma conta criada em [!DNL Workfront] para permitir que uma pessoa faça logon e interaja com o sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Delegação de usuário]</p> </td> 
   <td> <p>Um objeto reportável que informa:</p> 
    <ul> 
     <li>Quais usuários delegaram tarefas, emissões e aprovações de projetos</li> 
     <li>Quais usuários tiveram aprovações de tarefa, emissão e projeto delegadas a eles</li> 
     <li>Quando estas delegações começam e terminam</li> 
    </ul> <p>Para saber mais, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Criar um relatório de delegação de usuários</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface do usuário]</td> 
   <td>Todos os aspectos visuais e interativos da [!DNL Workfront] aplicativo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Preferências da interface do usuário]</td> 
   <td>[!UICONTROL Configuração da interface do usuário]. [!DNL Workfront] Os administradores podem alterar essas configurações para personalizar aspectos da interface do usuário.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilização]</td> 
   <td>A disponibilidade de um usuário ou função com base no agendamento atribuído, PTO e carga de trabalho atual.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilização pelo usuário]</td> 
   <td> <p>Uma pesquisa combinada com um relatório que mostra como os Usuários (Recursos) são alocados ou alocados em excesso. Consulte "[!UICONTROL Resource Usation]" neste artigo.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Velocity]</td> 
   <td>Uma medida do tempo total do ciclo de trabalho (quanto tempo leva para concluir um trabalho) e a frequência com que o trabalho é feito no tempo originalmente comprometido (rácio trabalho/comprometimento).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>As exibições podem ser usadas para modificar as colunas em um Relatório ou em uma lista de projetos, tarefas ou problemas, ou podem ser usadas para indicar o direito de um usuário de exibir apenas informações em um nível de acesso ou em um nível de compartilhamento de permissões.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibir ícones]</td> 
   <td> <p> Este é o mesmo campo que os Ícones de status, mas só está disponível para as seguintes exibições: </p> 
    <ul> 
     <li> [!UICONTROL Documentos] </li> 
    </ul> <p> Para obter mais informações, consulte o artigo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ícones de status incorporados nas exibições</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibições no mês passado]</td> 
   <td> <p>Em uma lista de relatórios, ela exibe o número de vezes que o relatório foi visualizado durante o último mês.<br>Para obter mais informações sobre uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibições no último trimestre]</td> 
   <td>Em uma lista de relatórios, exibe o número de vezes que o relatório foi visualizado durante o último trimestre.<br>Para obter mais informações sobre uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Visualizar uso de relatório</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibições no ano passado]</td> 
   <td>Em uma lista de relatórios, ela exibe o número de vezes que o relatório foi visualizado durante o último ano.<br>Para obter mais informações sobre uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibições neste mês]</td> 
   <td> <p>Em uma lista de relatórios, ela exibe o número de vezes que o relatório foi visualizado durante esse mês.<br>Para obter mais informações sobre uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibições Neste Trimestre]</td> 
   <td>Em uma lista de relatórios, exibe o número de vezes que o relatório foi visualizado durante esse trimestre.<br>Para obter mais informações sobre uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizar uso de relatório</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibições Este Ano]</td> 
   <td>Em uma lista de relatórios, ela exibe o número de vezes que o relatório foi visualizado durante esse ano.<br>Para obter mais informações sobre uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Visualizar uso de relatório</a>.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>Em um projeto, tarefa ou relatório de emissão, usando a seguinte instrução no modo de texto, exibe as Horas Planejadas do projeto, tarefa ou problema:</p>
   <p></p><p></p> 
   <p>Para obter informações sobre como usar o modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Visão geral da sintaxe do modo de texto</a>. </p> 
   <p><b>DICA</b> 
   <p>Em um relatório de problema, adicionar um dos campos [!UICONTROL Horas planejadas] adiciona a variável <code>work </code>para o relatório. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabalho]</td> 
   <td> <p>Um dos dois tipos de licença principais. Isso tem menos acesso do que o [!UICONTROL Plan], mas pode criar e fazer atualizações no sistema. Isso é mais habilidades do que os tipos de licença do [!UICONTROL External], do [!UICONTROL Reviewer] ou do [!UICONTROL Requester].</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] visão geral das licenças</a>.</p> <p>O trabalho pode se referir ao número de [!UICONTROL Horas Planejadas] para um projeto, tarefa ou problema. Para obter mais informações, consulte o campo "[!UICONTROL trabalho]" nesta tabela. </p> <p>Dica: Em um relatório de problema, adicionar um dos campos [!UICONTROL Horas planejadas] adiciona a variável <code>work </code>para o relatório. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estrutura de detalhamento do trabalho]</td> 
   <td>Uma estrutura hierárquica das tarefas a serem executadas pela equipe de projeto com base no relacionamento pai/filho.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Esforço de trabalho] </td> 
   <td> 
    <p>Um gerente de projeto pode decidir usar esse campo em vez de [!UICONTROL Horas Planejadas] para estimar o esforço necessário para concluir uma tarefa. Este campo fica visível somente quando as seguintes condições são atendidas:</p> 
     <ul> 
      <li> <p>A tarefa tem um [!UICONTROL Simple Duration Type]. </p> <p>Dica: Se você atualizar a tarefa [!UICONTROL Duration Type] para qualquer outro tipo, esse campo ficará oculto. </p> </li> 
      <li>O gerenciador de projeto habilitou o campo [!UICONTROL Usar Esforço de Trabalho] para calcular automaticamente a tarefa [!UICONTROL Horas Planejadas] no projeto. </li> 
     </ul> 
     <p>Para obter informações sobre como usar o [!UICONTROL Work Effort] em vez de [!UICONTROL Planned Hours] para estimar o esforço da tarefa, consulte <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Visão geral do esforço de trabalho</a>. </p> 
     <p>É possível exibir esse campo em relatórios e listas de tarefas.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Item de trabalho]</td> 
   <td> <p>Este campo se refere às tarefas ou aos problemas em [!DNL Workfront]. </p> <p>O relatório do [!UICONTROL Work Item] exibe informações sobre tarefas e problemas. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mistura de gerenciamento de trabalho]</td> 
   <td>Um [!UICONTROL Work Performance Indicator] (WPI) da proporção de trabalho alocada para executar sua empresa em vez de alterar sua empresa. A WPI de combinação ajuda você a entender, em um nível organizacional, se sua estratégia tem alguma alocação de trabalho real aplicada a ela.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabalho Management Resource]</td> 
   <td>Designação de uma pessoa no sistema que está qualificada para receber trabalho ou rastrear tempo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Função e responsabilidades do gerenciamento de trabalho]</td> 
   <td>Definir os proprietários e participantes para gerenciar o escopo, a execução e as aprovações da emissão, tarefa, projeto, programa ou portfólio designado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL SLA de gerenciamento de trabalho]</td> 
   <td>Uma métrica quantificável acordada por todas as partes interessadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parte interessada do gerenciamento de trabalho]</td> 
   <td>Uma coleção de usuários com interesse específico nos resultados de uma solicitação de trabalho.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pontos de contato do gerenciamento de trabalho]</td> 
   <td>Registros digitalizados de comunicação entre as partes interessadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicadores de desempenho do trabalho] </td> 
   <td> <p>Combine taxa, capacidade, velocidade, qualidade e envolvimento.</p> <p>O WPI é um acrônimo comum para [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Processo de trabalho]</td> 
   <td> <p>O método no qual o trabalho é recebido, priorizado e executado. A forma como você executa o trabalho normalmente é chamada de "fluxo de trabalho" ou "plano de projeto" (uma lista de tarefas com datas, relacionamentos do antecessor e assim por diante). </p> <p>Exemplos de um processo de trabalho podem ser a produção de um único ativo ou o delivery de uma campanha de vários ativos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modelo de fluxo de trabalho]</td> 
   <td>No relatório [!UICONTROL Proof Approval], este campo exibe todos os modelos de fluxo de trabalho anexados a uma prova. Se não houver modelos anexados, a coluna ficará em branco.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Tempo de trabalho]</td> 
   <td>

<p>Representa a porcentagem do tempo equivalente em tempo total ([!UICONTROL FTE]) que o usuário está disponível para o trabalho real, sem incluir a sobrecarga. [!UICONTROL Tempo de trabalho] deve ser um número decimal até 1 e não pode ser 0. Por exemplo, uma disponibilidade de 20% para o trabalho real seria de 0,2.</p>
   </p>O padrão do campo é 1, indicando que um usuário gasta todo o [!UICONTROL FTE] em um trabalho real relacionado ao projeto.  </p>
   <p>O sistema usa esse número para calcular a disponibilidade do usuário para o trabalho real relacionado ao projeto. </p>
   <p> As exceções de agendamento e o tempo limite também podem afetar a capacidade do usuário. </p>
   <p>Para obter mais informações sobre como criar programações no Workfront, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar um agendamento</a>. </p>
    <p>A Workfront calcula a disponibilidade de um usuário dependendo das preferências do Gerenciamento de Recursos na área [!UICONTROL Configuração]. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configurar preferências do Gerenciamento de recursos</a>. </p> 
   <p>Você pode atualizar o [!UICONTROL Work Time] de um usuário ao editar ou criar o usuário. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Editar o perfil de um usuário</a></p> 
   <b>DICA</b> 
   <p>Defina o valor [!UICONTROL Tempo de trabalho] como 1 para indicar que o usuário está disponível para trabalho relacionado ao projeto e todo o seu equivalente em tempo integral.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo de trabalho]</td> 
   <td>Na documentação do Workfront, esse termo é usado para descrever o tempo alocado para o trabalho, de acordo com um agendamento.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>Em um projeto, tarefa ou relatório de emissão, o uso da seguinte instrução no modo de texto exibe o número de Horas Planejadas do projeto, tarefa ou problema seguido da palavra "Horas":</p>
   <p></p><p></p>
    <p>Para obter informações sobre como usar o modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Visão geral da sintaxe do modo de texto</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
