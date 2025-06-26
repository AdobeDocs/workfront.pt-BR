---
content-type: reference
navigation-topic: workfront-navigation
title: 'Glossário da terminologia  [!DNL Adobe Workfront] '
description: O  [!DNL Adobe Workfront] glossário lista termos comumente usados em [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] interface, relatórios ou você tenta entender o significado dos [!DNL Workfront] conceitos definidos na  [!DNL Workfront] documentação.
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 594f224e11b0e7708ed555410b7c331741113791
workflow-type: tm+mt
source-wordcount: '21141'
ht-degree: 0%

---


# Glossário da terminologia [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Este artigo deve ser usado como referência para entender os termos que você pode encontrar no aplicativo [!DNL Adobe Workfront], na documentação [!DNL Workfront] ou quando, em geral, falar sobre o planejamento e o gerenciamento do trabalho. Estamos atualizando estas informações no momento e, como resultado, esta tabela pode não estar completa. Removeremos esse aviso de isenção de responsabilidade quando considerarmos essas informações exaustivas.

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
   <td>[!UICONTROL Nível de Acesso]</td> 
   <td>Um perfil de usuário que determina como um usuário pode interagir com diferentes objetos e ferramentas no Workfront.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa Ativa]</td> 
   <td>Uma tarefa incompleta em um projeto atual que não é impedida de ser trabalhada por uma tarefa predecessora e não tem uma restrição de tarefa com uma data de início planejada futura. Em outras palavras, pode ser trabalhada hoje.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Atividade]</td> 
   <td>Em [!DNL Workfront Goals], uma atividade é um indicador de progresso para uma meta. Pode ser uma barra de progresso que você atualiza manualmente ou um projeto associado à meta. Não é possível exibir atividades em um relatório e não é possível acessá-las por meio da API [!DNL Workfront]. Para obter informações sobre atividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introdução a resultados e atividades nas Metas do Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo Real]</td> 
   <td> <p>Para tarefas e problemas, esse é o custo associado às horas reais registradas em relação à taxa de Custo por hora do recurso atribuído à tarefa ou problema. Para projetos, esse é um total de todos os [!UICONTROL Custos Reais] de tarefas e problemas no projeto. Para obter informações, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo Efetivo de Despesa]</td> 
   <td> <p>A soma dos [!UICONTROL Valores Reais] para todas as despesas registradas para um projeto ou uma tarefa.</p> <b>EXEMPLO </b>
   <p>Se você criar uma despesa para a Tarefa 1 e inserir $600,00 no campo [!UICONTROL Valor Efetivo], o [!UICONTROL Custo Efetivo da Despesa] para essa tarefa será de $600,00. </p> 
   <p>Para um projeto, [!DNL Workfront] usa a seguinte fórmula para calcular o [!UICONTROL Custo Efetivo da Despesa]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas efetivas]</td> 
   <td> <p>Em um relatório de projeto, tarefa ou problema, as [!UICONTROL Horas Reais] são a soma de todas as horas registradas no projeto, tarefa ou problema após maio de 2021.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span> Se, a partir da guia [!UICONTROL Atualizações] para a Tarefa 1, você clicar em 'Tempo de Log' e inserir 25 horas, as Horas Reais da Tarefa 1 = 25 horas. </p> <p>[!DNL Workfront] calcula [!UICONTROL Horas efetivas] para tarefas pai ou projetos usando as seguintes fórmulas:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project + [!UICONTROL Actual Hours] logged on issues in the project</code>  </p> </li> 
    </ul> 
   <p>Consulte também <strong>Horas efetivas herdadas</strong>.
    <p>Para obter mais informações, consulte <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Exibir Horas Efetivas</a>.</p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo Real do Trabalho]</td> 
   <td> <p>O [!UICONTROL Custo Efetivo] associado à mão de obra investida em uma tarefa ou um projeto. </p> <p>Para uma tarefa, [!DNL Workfront] calcula o [!UICONTROL Custo Real do Trabalho] usando a seguinte fórmula:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Se a tarefa tiver um [!UICONTROL Tipo de Custo] de [!UICONTROL Usuário por Hora], [!DNL Workfront] usará a taxa de usuários. Se a tarefa tiver um [!UICONTROL Tipo de Custo] de [!UICONTROL Função por Hora], [!DNL Workfront] usará a taxa de funções de trabalho para calcular o [!UICONTROL Custo Real do Trabalho]. </p> <p>Para um projeto, [!DNL Workfront] usa a seguinte fórmula para calcular o [!UICONTROL Custo Real do Trabalho]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Por exemplo, se um usuário registrar 5 horas para uma tarefa com um [!UICONTROL Usuário por Hora] [!UICONTROL Tipo de Custo] e sua taxa horária for de $100, o [!UICONTROL Custo Real do Trabalho] será de $500.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Receita Real] </td> 
   <td> <p>A [!UICONTROL Receita Efetiva] de um projeto ou tarefa é a quantidade de dinheiro associada às [!UICONTROL Horas Efetivas] do projeto ou tarefa. </p> <p>Para obter informações sobre o rastreamento da receita em [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão Geral de Faturamento e Receita</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Início Real]</td> 
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
   <td>Metodologia do [!UICONTROL Agile]</td> 
   <td>Um tipo de metodologia baseada na evolução colaborativa de necessidades e soluções com equipes multifuncionais. Ele estimula a flexibilidade e a mudança com base em uma linha do tempo fixa.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Equipe Agile]</td> 
   <td>Difere de uma equipe tradicional porque ela tira o trabalho potencial de uma lista de pendências e trabalha nela dentro de um período definido, o que é chamado de [!UICONTROL Iteration].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Todas as Minhas Equipes]</td> 
   <td> <p>Quando isso for referenciado nos [!UICONTROL filtros], este campo exibirá usuários que pertencem a qualquer uma das equipes às quais o usuário conectado pertence ou itens de trabalho atribuídos a qualquer uma das equipes às quais o usuário conectado pertence. </p> <p>Recomendamos usar esse campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório que exibirá informações diferentes dependendo de quem faz logon para visualizá-lo, já que as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de Alocação]</td> 
   <td> <p>Esse campo pode ser encontrado nos seguintes tipos de relatórios:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Projeto] (Dados Financeiros)</li> 
     <li>[!UICONTROL Hora Orçada]</li> 
    </ul> <p>Para um relatório <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Project (Financial Data)]: </p> 
    <ul> 
     <li>Crie este relatório ao tentar entender <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> a quantidade de [!UICONTROL Horas Planejadas] que está atribuída aos seus recursos.</li> 
     <li> <p>A [!UICONTROL Data de Alocação] é o primeiro dia (domingo) de uma semana em que a alocação de uma [!UICONTROL Função de Trabalho] para uma tarefa é iniciada. Um recurso ([!UICONTROL Função de Trabalho]) pode ter quantas [!UICONTROL Datas de Alocação] tiver semanas durante a [!UICONTROL Duração] das tarefas às quais está atribuído. Se as tarefas estenderem-se por vários meses, o primeiro dia de um mês também poderá se tornar uma [!UICONTROL Data de Alocação], se estiver dentro da [!UICONTROL Duração] da tarefa.</p> <p>Por exemplo, você pode ter uma [!UICONTROL Função de trabalho] atribuída a uma tarefa que se estende por 3 semanas e tem 90 [!UICONTROL Horas planejadas]. Essas horas são distribuídas de maneira uniforme durante a duração da tarefa, o que faz com que todos os dias atribuam 6 [!UICONTROL Horas planejadas] à sua função de trabalho:</p> <p><em> [!UICONTROL Horas Planejadas Diárias] = [!UICONTROL Total de Horas Planejadas]/ Número de [!UICONTROL Dias de Trabalho] durante a [!UICONTROL Duração] da tarefa </em> </p> <p>Como resultado, há três [!UICONTROL Datas de Alocação], uma para cada domingo de cada semana durante a [!UICONTROL Duração] da tarefa, cada uma com um determinado número de [!UICONTROL Horas Planejadas] associadas a elas.<br>Se a tarefa começar no meio da última semana de um mês e terminar duas semanas após o início de um novo mês, ela terá quatro [!UICONTROL Datas de Alocação]: uma para cada domingo de cada semana durante a [!UICONTROL Duração] da tarefa e uma para o primeiro dia do novo mês.</p> <p>Para aproveitar essas informações ao máximo, recomendamos que você crie um relatório de Projeto <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> (Dados Financeiros) e adicione um agrupamento de matriz para a [!UICONTROL Allocation Date] e, em seguida, agrupe os resultados semanalmente, mensalmente, trimestralmente ou anualmente para obter os dados mais precisos.<br>Para obter informações sobre como criar um agrupamento de matriz, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Criar um relatório de matriz</a>.</p> </li> 
    </ul> <p>As informações financeiras são preenchidas nos relatórios do [!UICONTROL Project (Financial Data)] somente quando os dados associados a elas tiverem menos de 5 anos. Por exemplo, se uma função de trabalho foi alocada para uma tarefa em janeiro de 2015 e hoje é setembro de 2021, um campo financeiro como [!UICONTROL Data de Alocação] para a função de trabalho não será preenchido no relatório [!UICONTROL Projeto (Dados Financeiros)]. </p> 
    <div> 
     <p>Para um relatório de [!UICONTROL Budgeted Hour]:</p> 
     <ul> 
      <li>Crie este relatório ao tentar entender a quantidade de [!UICONTROL Horas Orçadas] que está alocada para seus recursos ou projetos no Planejador de Recursos.</li> 
      <li> <p>A [!UICONTROL Data de Alocação] é o primeiro dia (um domingo) da semana para o qual você orçou as horas no [!UICONTROL Resource Planner]. </p> <p><b>DICA</b></p> <p>Se uma semana se estender por dois meses, ela gerará duas linhas no relatório: uma correspondente ao primeiro dia da semana (domingo da primeira semana que está durante o primeiro mês), e a segunda linha exibirá o primeiro dia do segundo mês. </p> <p>Por exemplo, se você fizer um orçamento de 8 horas para um usuário para a semana de 30 de junho (domingo) a 6 de julho (sábado), as duas linhas mostrarão uma [!UICONTROL Data de Alocação] de 30 de junho e 1º de julho. </p> </p> <p>Para obter informações sobre recursos de orçamento no [!DNL Resource Planner], consulte o artigo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Recursos de orçamento no [!DNL Resource Planner] usando as exibições [!UICONTROL Project] e [!UICONTROL Role]</a>.</p> <p>Para obter informações sobre como criar um relatório de [!UICONTROL Budgeted Hour], consulte <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Relatório: Budgeted Hour</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anúncios]</td> 
   <td> <p>Uma forma de comunicar aos usuários informações dentro do sistema. Esta informação frequentemente vem do [!DNL Workfront] para o administrador ou do administrador para o usuário. </p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Enviar comunicados</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Integração de Aplicativos]</td> 
   <td>Um aplicativo geralmente representa um conector para um aplicativo de software, mas também pode representar funções especiais que manipulam dados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisão do Aprovador]</td> 
   <td> <p>No relatório [!UICONTROL Aprovação de prova], esse campo exibe decisões de aprovação de prova para provas que não estão mais ativas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estágio de Aprovador]</td> 
   <td>No [!UICONTROL Relatório de Aprovação de Prova], esse campo exibe informações sobre um estágio atual de provas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aprovação]</td> 
   <td> <p>Um determinado item de trabalho, como uma tarefa, um documento ou uma folha de horas, pode exigir que um supervisor ou outro usuário faça logoff no item de trabalho. Esse processo de aprovação é chamado de aprovação. </p> <p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Visão geral do processo de aprovação</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de aprovação]</td> 
   <td>No relatório [!UICONTROL Aprovação de prova], esse campo exibe a data em que uma prova foi aprovada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aprovador]</td> 
   <td>Um usuário ou função de trabalho que deve aprovar um determinado item de trabalho, ou o usuário que aprova entradas de horas em folhas de horas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuído A]</td> 
   <td> <p>Em um relatório de [!UICONTROL Tarefa ou Problema], esse campo exibe o Proprietário da tarefa ou o problema, ou o [!UICONTROL Atribuído Principal]. Também é possível filtrar ou agrupar por esse campo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuição]</td> 
   <td>Um usuário, função de trabalho ou equipe atribuída a um problema ou tarefa. Projetos, portfólios ou programas não podem ter atribuições.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuições]</td> 
   <td> <p>Em um relatório de [!UICONTROL Tarefa] ou [!UICONTROL Problema], esse campo exibe uma lista de todas as entidades (usuários, funções de trabalho, equipes) atribuídas à tarefa ou problema. Você pode filtrar por esse campo usando os campos [!UICONTROL Atribuição Usuários] e [!UICONTROL Atribuição Funções]. Você pode filtrar pela equipe atribuída à tarefa ou problema usando o campo Equipe. Não é possível agrupar um relatório por este campo.</p> <p>Os itens de trabalho colocados na [!UICONTROL Lixeira] continuarão a ser exibidos em alguns relatórios que se referem ao objeto [!UICONTROL Atribuição] onde um modificador de filtro [!DNL OR] é usado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Funções de Atribuição]</td> 
   <td>
   <p>Em um relatório de [!UICONTROL Tarefa] ou [!UICONTROL Problema], esse campo exibe informações sobre as funções de trabalho atribuídas às tarefas ou problemas. Este campo exibe [!UICONTROL Proprietários Primários], bem como outras funções de trabalho atribuídas a tarefas ou problemas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status de Atribuição]</td> 
   <td> <p>Em um relatório de atribuição, tarefa ou problema, o [!UICONTROL Status da Atribuição] exibe se os usuários atribuídos a um item de trabalho clicaram no botão [!UICONTROL Trabalhar Nele] ou [!UICONTROL Concluído] para aceitar ou concluir o trabalho. Existem os seguintes [!UICONTROL Status de Atribuição]:</p> 
    <ul> 
     <li><b>[!UICONTROL Solicitado]</b>: o usuário foi atribuído à tarefa ou problema, mas não clicou no botão [!UICONTROL Trabalhar Nele] para começar a trabalhar nele ainda.</li> 
     <li><b>[!UICONTROL Trabalhando]</b>: o usuário clicou no botão [!UICONTROL Trabalhando Nele] e está trabalhando no item no momento. </li> 
     <li><b>[!UICONTROL Concluído]</b>: o usuário clicou no botão [!UICONTROL Concluído] e concluiu seu trabalho no item. </li> 
    </ul> <p>Para obter mais informações, consulte a visão geral do botão <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Trabalhar Nele] e [!UICONTROL Concluído]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Equipes de Atribuição]</td> 
   <td>
   <p>Em um relatório de [!UICONTROL tarefa] ou [!UICONTROL problema], esse campo exibe informações sobre as equipes atribuídas às tarefas ou problemas. O campo exibe [!UICONTROL Proprietários principais], bem como outras equipes atribuídas a tarefas ou problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuários de Atribuição]</td> 
   <td>
   <p>Em um relatório de [!UICONTROL Tarefa] ou [!UICONTROL Problema], esse campo exibe informações sobre os usuários atribuídos às tarefas ou problemas. Este campo exibe [!UICONTROL Proprietários principais], bem como outros usuários atribuídos a tarefas ou problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atributo]</td> 
   <td>Um atributo é uma característica de um objeto [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Área de Auditoria]</td> 
   <td> <p>Auditorias são mensagens do sistema que registram uma ação que aconteceu no Workfront. Os seguintes tipos de auditoria são registrados:</p> 
    <ul> 
     <li>[!UICONTROL Alteração de Escopo]</li> 
     <li>[!UICONTROL Ação de Anexo]</li> 
     <li>[!UICONTROL Edição Geral]</li> 
     <li>[!UICONTROL Alteração de Status]</li> 
     <li>[!UICONTROL Observação]</li> 
     <li>[!UICONTROL Entrada Combinada]</li> 
     <li>[!UICONTROL Entrada de Erro]</li> 
     <li>[!UICONTROL Alteração de Status]</li> 
     <li>[!UICONTROL Alteração de Assinatura]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trilha de Auditoria]</td> 
   <td>A coleção de notas gerada automaticamente por eventos que são rastreados por meio das Alterações Gravadas ([!UICONTROL Áreas de Auditoria]). Cada nota registra quem fez a ação, o que fizeram e quando fizeram.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automático E Em Alteração]</td> 
   <td> <p>Um dos tipos [!UICONTROL Atualização de Projeto]. Isso recalculará as linhas do tempo projetadas e planejadas do projeto quando o processo de recálculo noturno for executado e quando qualquer atualização for feita no projeto ou nas tarefas dentro do projeto. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecionar o Tipo de Atualização do projeto </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Disponibilidade</p></td> 
   <td> <p>Esse termo é usado em relação à "disponibilidade de usuário" ou "disponibilidade de recurso" e ilustra a quantidade de tempo que o recurso (usuário ou função de trabalho) está disponível para trabalhar. </p> 
   <p>O Workfront calcula a disponibilidade de usuários usando vários campos e dependendo de quais configurações das preferências de Gerenciamento de recursos estão no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências de Gerenciamento de Recursos</a>. </p>
   <p>Para obter mais informações sobre a disponibilidade de recursos, consulte <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introdução ao Gerenciamento de Recursos</a></p>
   Como alternativa, a "capacidade" também é usada para se referir à disponibilidade de recursos. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Somente Automático]</td> 
   <td> <p>Um dos tipos [!UICONTROL Atualização de Projeto]. Isso recalculará as linhas de tempo projetadas e planejadas quando o processo noturno de recálculo for executado.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecionar o Tipo de Atualização do projeto</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Trabalho "Business as usual" que contribui para a execução das principais metas diárias de negócios.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Lista de Pendências]</td> 
   <td>A área em um ambiente ágil onde novos problemas são mantidos até que estejam prontos para serem trabalhados.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Linha de Base]</td> 
   <td>Uma fonte de dados para medir as iterações em um ambiente ágil.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Despesa Faturável]</td> 
   <td> <p>Uma despesa marcada como faturável para o cliente. Pode ser uma despesa planejada ou uma despesa real.</p> <p>Os campos Custo de Despesas Faturáveis Planejados e Custo Efetivo de Despesas Faturáveis estão disponíveis para serem adicionados a exibições e relatórios. Eles não aparecem nas páginas de detalhes do projeto ou da tarefa.</p>
   <p>Você pode encontrar esses campos nos seguintes tipos de relatórios:</p>
   <ul>
   <li>Linha de base</li>
   <li>Modelo</li>
   <li>Projeto (Dado Financeiro)</li>
   </ul>
   <p>Para obter mais informações sobre como marcar uma despesa como faturável, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Gerenciar despesas do projeto</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Registro de Cobrança]</td> 
   <td> <p>Registra a receita, as horas ou as despesas que podem ser faturadas. Essas informações podem ser usadas para criar faturas em um sistema de contabilidade externo.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Criar registros de cobrança</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Status do registro de cobrança</td> 
   <td> <p>Em um relatório de Registro de cobrança ou de Hora, o Status de um registro de cobrança indica se o registro de cobrança foi Faturado ou Não Faturado. Não é possível excluir um projeto ou editar um horário associado a um registro de cobrança faturado. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Criar registros de cobrança</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Identidade Visual]</td> 
   <td><p>O processo de personalizar o [!DNL Workfront] para dar à interface uma aparência que espelhe a empresa, usando suas cores e logotipos.</p><p><strong>OBSERVAÇÃO</strong><br>Se sua organização foi integrada no [!DNL Adobe Experience Cloud], a identidade visual não está disponível.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navegação Estrutural]</td> 
   <td> <p>A área na parte superior da página que mostra a localização hierárquica de onde o usuário está no aplicativo.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Para obter mais informações, consulte <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Visão geral da navegação estrutural</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status de Orçamento]</td> 
   <td> <p>Este campo está obsoleto. Qualquer informação que este campo possa exibir está relacionada a um recurso que [!DNL Workfront] removeu e o campo não pode ser atualizado. </p> <p>Este campo mostra se o projeto foi adicionado ao [!UICONTROL Capacity Planner] e se o cálculo de orçamento foi concluído para ele. O [!UICONTROL Capacity Planner] foi removido de [!DNL Workfront]. </p> 
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
   <td>[!UICONTROL Detalhamento]</td> 
   <td> <p>No Workfront Planning, é possível exibir registros conectados na exibição de linha do tempo de um registro usando o recurso Detalhamento. </p>
   <p>Detalhar os registros por suas conexões permite visualizar as linhas do tempo de outros registros conectados e entender como elas podem afetar o desempenho e os prazos de conclusão de seus registros. </p>
   <p>Os registros conectados são exibidos aninhados em seus respectivos registros. </p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/planning/views/manage-the-timeline-view.md">Gerenciar a exibição da linha do tempo</a>. </p>
   </td> 
    </tr>

<tr> 
   <td>[!UICONTROL Data de Término Orçada]</td> 
   <td> <p>Este campo está obsoleto. Qualquer informação que este campo possa exibir está relacionada a um recurso que [!DNL Workfront] removeu. Este campo não pode ser atualizado. </p>
   <p> Este campo ainda está visível em relatórios e listas do [!UICONTROL project].</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo Orçado]</td>

<td> <p>Esse é o custo associado aos recursos de orçamento de um projeto. </p>
   <p>O campo é exibido nas seguintes áreas de [!DNL Workfront] sob os seguintes nomes:</p>
   <ul>
   <li><strong>[!UICONTROL Custo Orçado]</strong>: no painel [!UICONTROL Resumo de Business Case]</li>
   <li><strong>[!UICONTROL Custo]</strong>: nas áreas [!UICONTROL Utilização] ao exibir informações pelo [!UICONTROL Custo]</li>
   <li><strong>[!UICONTROL Custo Orçado do Projeto]</strong>: em listas e relatórios</li>
   </ul>   
    <p>O [!UICONTROL Custo Orçado] do projeto é calculado usando a seguinte fórmula:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Para obter mais informações sobre como calcular o [!UICONTROL Custo Orçado] e compreender vários nomes para este conceito em [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcular Custo Orçado do Projeto</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas Orçadas]</td> 
   <td> <p>As horas orçadas para os recursos para o trabalho que precisam completar nos projetos. Este campo se refere às horas orçadas na área [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case] (ou no [!UICONTROL Resource Planner]) para o projeto ou para os recursos do projeto.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Entender o [!UICONTROL Custo do Trabalho Orçado] e [!UICONTROL Horas Orçadas] para projetos</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Para obter informações sobre como estimar Usuários no [!DNL Resource Planner], consulte o artigo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Recursos de orçamento no [!DNL Resource Planner] usando as exibições [!UICONTROL Project] e [!UICONTROL Role]</a>. </p> 
    <p>As horas orçadas na área [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case] ou do [!UICONTROL Resource Planner] são exibidas nas seguintes áreas de [!DNL Workfront] e sob os seguintes nomes:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL Horas Orçadas] nome para exibição</strong></td> 
        <td><strong>Áreas de [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Horas]</td> 
        <td>Área de [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>O [!UICONTROL Resource Planner] foi visualizado por [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Horas Orçadas]</td> 
        <td> <p>Exibição do relatório de utilização [!UICONTROL Hours]</p> <p>Para obter mais informações sobre o relatório [!UICONTROL Utilização], consulte o artigo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Visão Geral do Relatório [!UICONTROL Utilização de Recursos]</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Horas]</td> 
        <td> <p>Relatório de [!UICONTROL Hora Orçada]</p><p>O objeto [!UICONTROL Budgeted Hour] no relatório Budgeted Hour se refere às informações relacionadas a uma ferramenta de gerenciamento de recursos obsoleta. Somente o Bud ". O campo "Horas" neste relatório refere-se às horas orçadas na área do [!UICONTROL Resource Planner] ou do [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case] do projeto. </p> <p>Para obter mais informações sobre como criar um relatório, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Planejador de recursos Horas Orçadas] </td> 
        <td> <p>Encontrado nos seguintes relatórios:</p>
        <ul>
        <li>Relatório do [!UICONTROL Project]
        <li>Relatório de Projeto [!UICONTROL (Dados Financeiros)]
        <li>Relatório de [!UICONTROL Tarefa]
        <li>Relatório de [!UICONTROL Problema]
        <li>Relatório de [!UICONTROL Hora Orçada]</li>
        </ul>
         <p>Para obter mais informações sobre como criar um relatório, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Qualquer outra menção de [!UICONTROL Budgeted Hours] em [!DNL Adobe Workfront] se refere às horas orçadas usando recursos obsoletos que foram removidos do Workfront. Esses são campos somente para visualização e não são atualizados com as informações atuais quando você usa as ferramentas atuais de orçamento de recursos. </p>
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
   <td>[!UICONTROL Custo do Trabalho Orçado]</td> 
   <td> <p>Esse é o custo associado às horas que você, como Gerente de recursos, destina ao orçamento das suas funções de trabalho para o trabalho que precisam para concluir nos projetos. </p> <p>O [!UICONTROL Custo do Trabalho Orçado] em um relatório de projeto é calculado usando a seguinte fórmula:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Este campo pode referir-se ao seguinte:</p> 
    <ul> 
     <li> <p>Custos de mão de obra exibidos na área [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case] ou no [!UICONTROL Resource Planner] associados ao custo de funções de trabalho em um projeto. Para obter informações sobre como calcular o [!UICONTROL Custo do Trabalho Orçado], consulte o artigo <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Entender Custo do Trabalho Orçado] e [!UICONTROL Horas Orçadas] para projetos</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Custos de mão de obra exibidos na área [!UICONTROL Resource Budgeting] do [!UICONTROL Business Case] que refletem os [!UICONTROL People Costs] estimados em uma iniciativa vinculada ao projeto do [!DNL Scenario Planner] quando você usa o Planejador de cenários para orçar seus recursos de projeto. Para obter informações sobre iniciativas, consulte <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Visão geral das iniciativas no Planejador de cenários</a>. </p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">A visão geral</a> de [!DNL Scenario Planner]. </p> </li> 
     <p>Ela é exibida nas seguintes áreas de sob os seguintes nomes:</p>
   <ul>
   <li><strong>[!UICONTROL Custo do Trabalho Orçado]</strong>: na área [!UICONTROL Orçamento de Recursos] do [!UICONTROL Business Case].
   <li><strong>[!UICONTROL Custo Orçado]</strong>: no relatório [!UICONTROL Utilização] exibição [!UICONTROL Custo]
   <p>Para obter mais informações, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Exibir informações sobre a utilização de recursos </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: no Projeto [!DNL Resource Planner] ou nas exibições [!DNL Role], ao visualizar pelo Custo
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: nos seguintes relatórios: 
   <ul>
    <li>Relatório do [!UICONTROL Project]</li>
    <li>Relatório de Projeto [!UICONTROL (Dados Financeiros)]</li>
    <li>Relatório de [!UICONTROL Tarefa]</li>
    <li>Relatório de [!UICONTROL Problema]</li>
    <li>Relatório de [!UICONTROL Hora Orçada]</li> 
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
   <td>[!UICONTROL Data de Início Orçada]</td> 
  <td> <p>Este campo está obsoleto. Qualquer informação que este campo possa exibir está relacionada a um recurso que [!DNL Workfront] removeu. Este campo não pode ser atualizado.</p>
  <p>Estas áreas foram removidas de [!DNL Workfront]. </p> 
  <p>O campo ainda está visível nos relatórios e listas do [!UICONTROL project].</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gráfico de Burndown]</td> 
   <td>Um gráfico de linhas que fornece uma representação visual do trabalho concluído e restante.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>Ferramenta usada para avaliar se um projeto deve ser movido do status [!UICONTROL Idea] para o status [!UICONTROL Planning]. Em outras palavras, um [!UICONTROL business case] ajuda a organização a decidir se vale a pena iniciar e concluir o projeto ou não, especialmente ao comparar projetos com outros em um portfólio.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Criar um [!UICONTROL Business Case] para um projeto </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas Orçadas do Business Case]</td> 
   <td> <p>Este campo está obsoleto. Qualquer informação que este campo possa exibir está relacionada a um recurso que [!DNL Workfront] removeu. Este campo não pode ser atualizado.</p> <p>Este campo ainda está visível em listas e relatórios de projeto e de [!UICONTROL tarefa]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuição Calculada]</td> 
   <td> <p>Uma das tarefas [!UICONTROL Tipos de Duração] . Isso calculará a porcentagem de um dia de trabalho de 8 horas em que o usuário atribuído à tarefa será alocado na tarefa, com base na [!UICONTROL Duration] da tarefa e no [!UICONTROL Trabalho necessário].</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Tarefa [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabalho Calculado]</td> 
   <td> <p>Um dos [!UICONTROL Tipos de Duração] da tarefa. Isso calculará o [!UICONTROL Trabalho necessário] em uma tarefa, considerando a [!UICONTROL Duração] e as porcentagens de usuário [!UICONTROL Atribuição] (que se baseiam em um dia de trabalho de 8 horas).</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Tarefa [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendário]</td> 
   <td> <p>No Workfront, um relatório de calendário é um relatório dinâmico no qual os usuários podem visualizar a data e outros detalhes importantes de um evento, incluindo a data de vencimento, o status do trabalho e o usuário ao qual o evento é atribuído.</p> <p> Para obter mais informações sobre relatórios de calendário, consulte <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Visão geral dos relatórios de calendário</a>.</p>
   <p> No Workfront Planning, uma exibição de Calendário é um tipo de exibição para um tipo de registro que exibe registros em um calendário. Você deve ter uma licença adicional para acessar o Workfront Planning. </p>
    </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Pode Iniciar]</td> 
   <td> <p>Este campo indica se uma tarefa está pronta para ser iniciada. Se o início estiver pronto para ser trabalhado, o campo [!UICONTROL Pode Iniciar] na tarefa será definido como [!UICONTROL Verdadeiro]. </p> <p>Para obter mais informações, consulte a visão geral "<a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">"[!UICONTROL Pode Iniciar]" para tarefas</a>.</p> 
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
   <td> <p>Um tempo disponível do recurso quando ele pode ser alocado para trabalho. Consulte "Disponibilidade". </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Categoria]</p> </td> 
   <td> <p>Uma categoria é um formulário personalizado. Você pode criar relatórios para esse objeto e também pode mostrá-lo em outros relatórios de objeto. Nem todos os objetos podem ter um formulário ou categoria personalizada. Os seguintes objetos podem ter um formulário personalizado: <br></p> 
    <ul> 
     <li>[!UICONTROL Projeto]</li> 
     <li>[!UICONTROL Tarefa]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Documento]</li> 
     <li>[!UICONTROL Despesa]</li> 
     <li>[!UICONTROL Programa]</li> 
     <li>[!UICONTROL Usuário]</li> 
     <li>[!UICONTROL Empresa]</li> 
     <li>[!UICONTROL Iteração]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da Categoria]</td> 
   <td> <p>Quando adicionada como uma coluna à exibição de qualquer um dos seguintes objetos, ela exibe uma lista de todos os formulários personalizados associados a esses objetos:</p> 
    <ul> 
     <li>[!UICONTROL Projeto]</li> 
     <li>[!UICONTROL Tarefa]<br></li> 
     <li>[!UICONTROL Problema]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Documento]<br></li> 
     <li>[!UICONTROL Despesa]<br></li> 
     <li>[!UICONTROL Programa]<br></li> 
     <li>[!UICONTROL Usuário]<br></li> 
     <li>[!UICONTROL Empresa]</li> 
     <li>[!UICONTROL Iteração]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gerenciamento de Alterações]</td> 
   <td>Uma área de prática focada na definição, compreensão e adaptação do trabalho planejado a alterações nos fatores de escopo, programação, custo e recursos.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ordem de Alteração]</td> 
   <td>Um tipo de problema relacionado a um projeto que descreve uma alteração solicitada no escopo acordado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alterar Somente]</td> 
   <td>Um dos [!UICONTROL Tipos de Atualização] do projeto. Ela só atualiza as linhas do tempo do [!UICONTROL Projeto Projetado] e do [!UICONTROL Planejado] quando são feitas atualizações nas tarefas ou quando são realizadas edições no projeto ou nas tarefas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordem de Alteração]</td> 
   <td> <p>Um dos tipos de [!UICONTROL Issue], geralmente indicando que uma quantidade não planejada de trabalho deve ser feita antes que o projeto possa ser concluído.</p> <p>Para obter mais informações sobre os tipos de [!UICONTROL Issue], consulte a seção "Tipos de problema padrão" no artigo <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Personalizar tipos de problema padrão</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa Filho]</td> 
   <td>Uma tarefa que seja uma [!UICONTROL Subtarefa] de uma [!UICONTROL Tarefa Pai] ([!UICONTROL Tarefa Resumo]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filhos]</td> 
   <td>A coleção de [!UICONTROL Subtarefas] para uma [!UICONTROL Tarefa Pai] ([!UICONTROL Tarefa Resumo]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] e [!UICONTROL Training]</td> 
   <td>Módulos de aprendizado, certificações, padrões ou uma comunidade de prática.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Confirmar]</td> 
   <td>Uma ferramenta de comunicação para que os usuários definam expectativas em relação aos materiais de entrega da tarefa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de Confirmação]</td> 
   <td>Uma ferramenta de comunicação para o usuário definir expectativas em relação aos materiais de entrega da tarefa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comunicação] e [!UICONTROL Relatório]</td> 
   <td>Padrões para revisar as exceções e condições de um projeto, programa ou portfólio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Empresa]</td> 
   <td> <p>Uma [!UICONTROL Company] é uma unidade organizacional em [!DNL Workfront]. </p> 
   <p> Você pode associar um usuário ou um projeto a uma empresa. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Criar e editar empresas</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de conclusão]</td> 
   <td> <p>A data em que um projeto, tarefa ou problema está definido para ser concluído. Há vários tipos de [!UICONTROL Datas de conclusão] em [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Data de Término Real]. Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Visão geral do projeto [!UICONTROL Data de Término Efetivo] </a>.</li> 
     <li>[!UICONTROL Data de conclusão planejada]. Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Definir a [!UICONTROL Data de Conclusão Planejada]</a> e <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Visão geral da tarefa [!UICONTROL Data de Conclusão Planejada]</a>.</li> 
     <li>[!UICONTROL Data de Término Projetada]. Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Visão geral da [!UICONTROL Data de Conclusão Projetada] para projetos, tarefas e problemas</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dia de Término]</td> 
   <td>O dia, relativo ao início do [!UICONTROL Template], em que uma [!UICONTROL Template Task] ou um [!UICONTROL Template] deve estar concluído.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de conclusão]</td> 
   <td> <p>Isso indica como um projeto será marcado como [!UICONTROL Concluído]. Ele pode ter dois valores:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: um usuário deve alterar o status do projeto para [!UICONTROL Concluído].</li> 
     <li>[!UICONTROL Automático]: o status do projeto será alterado automaticamente para [!UICONTROL Concluído] quando todas as tarefas do projeto estiverem 100% Concluídas e todos os problemas estiverem fechados.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condição]</td> 
   <td> <p>Representação visual do progresso de uma tarefa, problema ou projeto.</p> <p>Para projetos, a condição pode ser definida manualmente pelo proprietário do projeto ou pode ser definida automaticamente por [!DNL Workfront], com base no status de progresso do projeto. </p> <p>Os valores possíveis para a condição do projeto são:</p> 
    <ul> 
     <li>[!UICONTROL No Destino]</li> 
     <li>[!UICONTROL Em Risco]</li> 
     <li>[!UICONTROL Com Problema]</li> 
    </ul> <p>Para obter mais informações sobre as condições do projeto, consulte o artigo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Visão Geral da [!UICONTROL Condição do Projeto] e [!UICONTROL Tipo de Condição]</a>.</p>
     <p>Você pode associar condições de tarefas e problemas a um número que pode ser exibido em relatórios. As listas abaixo exibem os nomes e números padrão para condições de tarefas e problemas. O administrador do sistema pode atualizar os nomes das condições e adicionar novas condições com números diferentes. Depois que um número é associado a uma condição, ele não pode ser editado.  </p> 
     <p>Para tarefas, a condição é definida manualmente pelo proprietário da tarefa. Os valores possíveis para a condição da tarefa são:</p> 
    <ul> 
     <li>[!UICONTROL Indo Bem] (0)<br></li> 
     <li> [!UICONTROL Algumas Preocupações] (1)<br></li> 
     <li>[!UICONTROL Principais Bloqueios] (2)</li> 
    </ul> <p>Para obter mais informações sobre as condições da tarefa, consulte o artigo <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Atualizar [!UICONTROL Condição] para tarefas e problemas</a>.</p> <p>Para ocorrências, a condição é definida manualmente pelo proprietário da ocorrência. Os valores possíveis para a condição de ocorrência são:<br></p> 
    <ul> 
     <li>[!UICONTROL Indo Bem] (0)<br></li> 
     <li>[!UICONTROL Algumas Preocupações] (1)<br></li> 
     <li>[!UICONTROL Principais Bloqueios] (2)</li> 
    </ul> 
   <p><b>Nota</b></p>
    <p>Quando o campo [!UICONTROL Condição] é acompanhado nos relatórios de [!UICONTROL Entrada de Diário], [!UICONTROL Novo] e [!UICONTROL Valores de Número Antigos] exibem o número associado à condição em vez de seu nome. Se uma condição não tiver sido originalmente definida para uma tarefa ou um problema e você atualizá-la posteriormente, a entrada do diário que captura a atualização exibirá o [!UICONTROL Old Number Value] do campo [!UICONTROL Condition] como -2.147.483.648. Consulte também "[!UICONTROL Novo valor numérico]", "[!UICONTROL Valor numérico antigo]" e "[!UICONTROL Entrada de diário]" neste artigo. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atualização de Condição]</td> 
   <td> <p>Este campo mostra a condição atual de tarefas, projetos ou problemas. Esta opção mostra as atualizações mais recentes que os proprietários de tarefas, projetos ou problemas forneceram no campo [!UICONTROL Atualizar Status], juntamente com a nova condição.</p> <p>Comentários feitos em atualizações de condição não são exibidos na coluna [!UICONTROL Atualização de Condição]; somente a atualização principal é exibida.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Tipos de registro conectados]</td> 
   <td> <p>No Workfront Planning, é possível criar uma conexão entre uma das seguintes opções: </p>
   <ul>
   <li>Dois tipos de registro</li>
   <li>Um tipo de registro e um tipo de objeto Workfront</li>
   <li>Um tipo de registro e um ativo do Adobe Experience Manager</li></ul>
   <p>A conexão de tipos de registro permite exibir informações de um registro ou tipo de objeto em outro tipo de registro.</p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/planning/architecture/connect-record-types-overview.md">Visão geral dos tipos de registros conectados</a>  </p>
  <p>O Workfront Planning exige uma licença adicional. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Registros Conectados]</td> 
   <td> <p>No Workfront Planning, depois de conectar dois tipos de registro, você pode conectar dois registros individuais desses tipos uns aos outros.  </p>
   <p>A conexão de registros permite exibir informações de um registro ou objeto de outro aplicativo em outro registro.</p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/planning/records/connected-records-overview.md">Visão geral dos registros conectados</a>. </p>

<p>O Workfront Planning exige uma licença adicional. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Conexões]</td> 
   <td> <p>No Workfront Planning, as conexões podem se referir a tipos de registros conectados ou a registros conectados. O Workfront Planning exige uma licença adicional.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Data de Restrição]</td> 
   <td> <p>Se você estiver usando uma [!UICONTROL Restrição de Tarefa] vinculada a uma data específica, como [!UICONTROL Deve Iniciar em], essa data específica se tornará a [!UICONTROL Data de Restrição] da tarefa.</p> <p>As restrições de tarefa a seguir atualizam o campo [!UICONTROL Constraint Date]:</p> 
    <ul> 
     <li>[!UICONTROL Deve Iniciar Em]</li> 
     <li>[!UICONTROL Deve Terminar Em]</li> 
     <li>[!UICONTROL Não Iniciar Depois De]</li> 
     <li>[!UICONTROL Não Iniciar Antes De]</li> 
    </ul> <p><b>DICA</b></p>   
     <ul> 
      <li> <p>Uma tarefa com uma [!UICONTROL Restrição] de [!UICONTROL Datas Fixas] não tem [!UICONTROL Data de Restrição]. </p> </li> 
      <li> <p> A [!UICONTROL Data de Restrição] só é visível em um relatório ou exibição personalizada.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dia de Restrição]</td> 
   <td> <p>Se você estiver usando uma Restrição de Tarefa em uma tarefa de modelo vinculada a um dia específico, como Deve Iniciar em, esse dia específico se tornará o Dia de Restrição da tarefa de modelo.</p> <p>As restrições de tarefa a seguir atualizam o campo [!UICONTROL Constraint Day]:</p> 
    <ul> 
     <li>[!UICONTROL Deve Iniciar Em]</li> 
     <li>[!UICONTROL Deve Terminar Em]</li> 
     <li>[!UICONTROL Não Iniciar Depois De]</li> 
     <li>[!UICONTROL Não Iniciar Antes De]</li> 
    </ul> <p><b>DICA</b></p> <p>  O [!UICONTROL Dia de Restrição] só é visível em um relatório ou exibição personalizada. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Restrição]</td> 
   <td> <p>A tendência de agendamento de uma tarefa. Por exemplo, [!UICONTROL Assim que Possível] agendará uma tarefa para iniciar assim que possível, e [!UICONTROL Não Terminar Depois Que] agendará uma tarefa para ser concluída até a [!UICONTROL Data de Restrição] e não depois.</p> <p>Para obter mais informações, consulte a visão geral <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL Restrição de Tarefa]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menu Contextual]</td> 
   <td>Um menu, localizado no lado esquerdo da tela, no qual os itens são alterados para se correlacionarem com o conteúdo ativo. Por exemplo, quando um usuário está visualizando um projeto, o [!UICONTROL Menu Contextual] exibirá links para informações e ferramentas relacionadas ao projeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converteu Originador de Problema]</td> 
   <td>Um campo em um relatório de projeto ou tarefa que mostra informações sobre o usuário que é o [!UICONTROL Contato Principal] de um problema quando o problema é convertido em um projeto ou tarefa. O campo também é exibido na seção [!UICONTROL Detalhes do projeto], onde é exibido o nome do [!UICONTROL Contato Principal] do problema convertido. Consulte também "[!UICONTROL Contato Principal]" neste artigo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custo]</td> 
   <td> <p>O valor monetário que você deve gastar ao concluir um projeto, tarefa ou problema. </p> <p>Você pode rastrear vários tipos de custos de mão de obra, despesas e riscos relacionados ao projeto.Para obter informações sobre o rastreamento de custos no [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/track-costs.md">Rastrear custos</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Custo]</td> 
   <td>Para uma tarefa, o [!UICONTROL Tipo de Custo] determina como a tarefa acumulará custos. Alguns exemplos incluem [!UICONTROL Horas Fixas], [!UICONTROL Horas Usuários Horas Fixas] e [!UICONTROL Horas Usuários Horas Fixas]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependências entre Projetos]</td> 
   <td> <p>Uma tarefa de um projeto depende de uma tarefa de um projeto diferente.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Criar predecessores entre projetos</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Dados Personalizados]</td> 
   <td> <p>Dados exclusivos de uma organização. As organizações podem personalizar o aplicativo [!DNL Workfront] criando formulários e campos personalizados. Essas informações personalizadas podem gerar relatórios para KPIs, auditoria e mix de demanda. </p> <p>[!UICONTROL Dados Personalizados] podem ser vinculados a:</p> 
    <ul> 
     <li>[!UICONTROL Projetos]</li> 
     <li>[!UICONTROL Tarefas]</li> 
     <li>[!UICONTROL Usuários]</li> 
     <li>[!UICONTROL Empresas]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Documentos]</li> 
     <li>[!UICONTROL Despesas]</li> 
     <li>[!UICONTROL Portfólio]</li> 
     <li>[!UICONTROL Programas]</li> 
     <li>[!UICONTROL Iterações]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Dados Personalizado]</td> 
   <td>A opção para especificar se um Campo de Dados Personalizados  será armazenado no banco de dados como Texto, Data, Número ou Moeda.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Exibição Personalizada]</td> 
   <td>O tipo de exibição de campo de um campo personalizado. Os exemplos incluem [!UICONTROL Suspenso], [!UICONTROL Campo de Texto], [!UICONTROL Área de Texto], [!UICONTROL Botões de Opção], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campo Personalizado]</td> 
   <td>Para dados Personalizados que permitem ao usuário selecionar entre várias opções, esses são os valores a partir dos quais um usuário pode selecionar. As Opções Personalizadas são válidas somente na [!UICONTROL Lista Suspensa], [!UICONTROL Lista Suspensa de Seleção Múltipla], [!UICONTROL Botões de Opção] e [!UICONTROL Caixas de Seleção].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rótulo de Formulário Personalizado]</td> 
   <td>Ao usar um Tipo de exibição personalizado com Opções personalizadas, esse é o texto da interface do usuário que será exibido no menu suspenso, nas Caixas de seleção ou nos Botões de opção dessa Opção personalizada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor personalizado]</td> 
   <td>Ao usar um campo Personalizado com Opções Personalizadas, este é o valor que será armazenado no banco de dados para uma Opção específica.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de Exibição Personalizado]</td> 
   <td>Uma definição dos campos de dados ou colunas que são exibidos para cada objeto em uma lista.</td> 
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
   <th>Nome do objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Painéis]</td> 
   <td> <p> É possível adicionar esse campo em um relatório ou em uma exibição do objeto Relatório para exibir os painéis nos quais o relatório está listado em uma lista. </p> <p> Também é possível usar esse campo para filtrar relatórios listados em um painel específico. </p> <p> Para obter mais informações sobre como incluir informações do painel em relatórios de objetos de relatório, consulte a seção "Entendendo quais relatórios estão listados em painéis" no artigo <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Acessar e organizar relatórios</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Dados]</td> 
   <td>Consulte "[!UICONTROL Tipo de Dados Personalizado]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dias Atrasados]</td> 
   <td> <p>Este campo mostra uma diferença de data entre [!UICONTROL Início Planejado] e [!UICONTROL Hoje] se a [!UICONTROL Data de Conclusão Real] estiver ausente.</p> <p>Também mostra uma diferença de data entre [!UICONTROL Conclusão Real] e [!UICONTROL Conclusão Planejada], quando uma [!UICONTROL Data de Conclusão Real] está presente.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Agenda Padrão]</td> 
   <td> <p>Horas de trabalho padrão personalizáveis a serem atribuídas a usuários e projetos dentro de uma organização. </p> <p>Calendários são usados para calcular as datas planejadas, de início e de conclusão das tarefas atribuídas aos usuários.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Produto]</td> 
   <td>Bens ou serviços quantificáveis que devem ser fornecidos após a conclusão de um projeto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gerenciamento de Demanda]</td> 
   <td>Pontuação e priorização dos processos de admissão.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Metas de Departamento]</td> 
   <td>Metas exclusivas de um departamento específico que se concentram em melhorar as métricas operacionais no departamento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependência]</td> 
   <td>O vínculo entre duas tarefas que exigem que uma tarefa altere o status antes que a outra também possa alterar o status.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Dependência]</td> 
   <td> <p>O tipo de relacionamento de agendamento entre uma tarefa e sua predecessora. Um exemplo é [!UICONTROL Finish-Start], que requer que a primeira tarefa seja Finalizada antes que a segunda possa ser iniciada.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Visão geral dos tipos de dependência de tarefa</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Documento]</td> 
   <td>Qualquer arquivo anexado a um objeto em [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Versão do Documento]</td> 
   <td> <p>Sempre que o mesmo documento for carregado no mesmo objeto, um número de versão será atribuído a ele. Os usuários podem exibir e alterar várias opções de uma versão anterior de um documento.</p> <p>Para obter mais informações, consulte <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Gerenciar versões de documentos</a>.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Data de Conclusão]</td> 
   <td> <p>A data em que uma tarefa ou um problema deve ser concluído. A Data de Vencimento de uma tarefa ou problema é a mesma data que a Data de Conclusão Planejada.</p>
    <p>A Data de Conclusão da tarefa e do problema está visível nas listas de tarefas e problemas e nos relatórios.</p> 
    <p>Consulte também Data de conclusão planejada nesta tabela. 
    </td> 
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duração]</td> 
   <td> <p>A janela de tempo alocada para a conclusão de um problema de tarefa ou projeto (conforme determinado pelo número de dias entre o [!UICONTROL Início Planejado] e a Conclusão Planejada).</p> 
    <ul> 
     <li>Para tarefas, a Duração é um campo editável se o Tipo de duração da tarefa não for Simples. Se o Tipo de Duração da tarefa for Simples, ou se a Restrição de Tarefa for Datas Fixas, a Duração será um cálculo executado pelo Workfront.</li> 
     <li>Para problemas, a Duração é sempre um campo editável e deve representar uma estimativa de um número de dias que exigiriam que o problema fosse resolvido.</li> 
     <li>Para projetos, a Duração é um cálculo executado por [!DNL Workfront] e representa a diferença em dias entre o Início Planejado da tarefa mais antiga e a [!UICONTROL Conclusão Planejada] da tarefa mais recente no projeto.</li> 
    </ul> <p>Para obter mais informações sobre a diferença entre a [!UICONTROL Duração] e a [!UICONTROL Duração Planejada] para tarefas, consulte o artigo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Diferença entre a [!UICONTROL Duração Planejada] e a [!UICONTROL Duração] para tarefas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duração em Minutos]</td> 
   <td>Este campo exibe as mesmas informações que o campo [!UICONTROL Duration] em minutos em vez de dias. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duração por Ocorrência]</td> 
   <td> <p>Isso é exibido nas caixas [!UICONTROL Detalhes da tarefa] e [!UICONTROL Editar tarefa] de um pai de tarefas recorrentes. Ela exibe a duração de cada tarefa recorrente. Para obter informações sobre como criar tarefas recorrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Criar tarefas recorrentes</a>. </p> <p> <span>As durações modificadas em tarefas recorrentes individuais não exibem o valor indicado neste campo.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Tipo de Duração]</td> 
   <td> <p>Um campo de tarefa que indica como o trabalho necessário para concluir a tarefa é alocado aos atribuídos na duração da tarefa. Ela representa a relação entre a [!UICONTROL Duração] da tarefa, o [!UICONTROL Trabalho Necessário] e o tempo, ou [!UICONTROL Alocação], que os recursos atribuídos devem gastar na tarefa para concluí-la. </p> <p>Este campo aparece na guia [!UICONTROL Detalhes] de uma tarefa. </p> <p>As opções para o Tipo de duração de uma tarefa são:</p> 
    <ul> 
     <li>[!UICONTROL Atribuição calculada]</li> 
     <li>[!UICONTROL Trabalho Calculado]</li> 
     <li>[!UICONTROL Controlado pelo Esforço]</li> 
     <li>[!UICONTROL Simples]</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Tarefa [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> 
    --&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Unidade de Duração]</td> 
   <td>A unidade usada para medir o tempo em uma pesquisa de energia.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Controlado pelo Esforço]</td> 
   <td>A relação entre o número de usuários e o tempo que a tarefa levará para ser concluída. À medida que você adiciona mais usuários, o tempo total agendado para a conclusão da tarefa diminui, mas a duração da tarefa permanece a mesma. Por exemplo, se uma tarefa estiver descascando um barril de amendoim, adicionar mais pessoas diminuirá o tempo agendado, mas a duração em pessoas-dias permanecerá a mesma.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo Decorrido]</td> 
   <td> <p>[!UICONTROL Tempo decorrido] é uma unidade de tempo para a [!UICONTROL Duração] de uma tarefa. É o tempo entre a [!UICONTROL Data de Início Planejada] e a [!UICONTROL Data de Conclusão Planejada] de uma tarefa que inclui feriados, finais de semana e folga. Em outras palavras, o tempo decorrido é a passagem de dias do calendário. </p> <p>[!DNL Workfront] O oferece suporte às seguintes unidades de tempo decorrido para a duração da tarefa:</p> 
    <ul> 
     <li> <p>[!UICONTROL Minutos Corridos]</p> </li> 
     <li> <p>[!UICONTROL Horas Decorridas]</p> </li> 
     <li> <p>[!UICONTROL Dias Decorridos]</p> </li> 
     <li> <p>[!UICONTROL Semanas Corridas]</p> </li> 
     <li> <p>[!UICONTROL Meses Decorridos]</p> </li> 
    </ul> <p>Para obter mais informações sobre a duração da tarefa, incluindo o tempo decorrido, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Tarefa [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de Término]</td> 
   <td> <p> Em um relatório [!UICONTROL Rate], esta é a data em que termina uma nova taxa de cobrança para uma função de trabalho no nível do projeto. As horas associadas ao projeto antes dessa data são multiplicadas por essa taxa de faturamento para calcular a receita do projeto. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Envolvimento]</td> 
   <td>O [!UICONTROL Indicador de Desempenho de Trabalho] (WPI) que indica quando o compromisso e a crença na tarefa, projeto, equipe ou organização estão diminuindo. Isso indica que você precisa agir para reviver essa crença e compromisso. O WPI seria medido fazendo-se perguntas simples, "Você entendeu o que se esperava de você? O trabalho atribuído a você fez alguma diferença para a organização? Você fez um ótimo trabalho?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Metas Empresariais]</td> 
   <td>Metas multifuncionais que contribuem para as métricas das metas da empresa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Evento]</td> 
   <td>Qualquer alteração em um projeto ou tarefa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Manipulador de Eventos]</td> 
   <td>Tarefas automatizadas que ocorrem quando Eventos ocorrem. Um exemplo comum é uma notificação por email automatizada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notificação de Eventos]</td> 
   <td>Email gerado por um manipulador de eventos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Despesas]</td> 
   <td>Um custo não mão de obra em tarefas ou projetos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Externo]</td> 
   <td> <p>Normalmente, esse é um tipo de licença ou um usuário com essa licença. Um usuário com esse tipo de licença só tem a capacidade de revisar informações no sistema. Não podem participar ativamente no trabalho.</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] visão geral das licenças</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sistema Externo]</td> 
   <td>Qualquer serviço ou software armazenado e controlado fora do sistema de registro designado.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Campo]</td> 
   <td><p>Qualquer objeto do Workfront ou as informações associadas a ele, conforme exibido no banco de dados. </p>
   <p>Por exemplo, "projeto", "usuário", "hora" são objetos do Workfront e campos. "Name", "status", "owner", "start date" são campos do Workfront associados aos objetos acima. </p>

<p>Quando se referem a objetos, os termos "objetos" e "campos" podem ser usados alternadamente.</p>
   <p>No escopo dos relatórios, os "campos" se referem aos objetos ou às informações sobre o objeto que você deseja capturar no relatório.</p>

<p><b>Nota</b></p>

<p>Nos relatórios text-more, os campos se referem aos objetos ou suas informações conforme aparecem no banco de dados.</p>
   <p>Às vezes, o nome que você vê na interface do usuário é diferente do nome do campo no banco de dados. Por exemplo, "issue" é o nome do objeto na interface do Workfront, mas "opTask" é o nome do objeto (ou do campo) no banco de dados do Workfront. </p> 
   <p> É importante usar o campo como ele aparece no banco de dados ao gravar um relatório em modo de texto, exibir, filtrar ou agrupar, ou ao criar um campo calculado.</p>

<p>Para obter mais informações, consulte <a href="../../../wf-api/general/api-explorer.md">API Explorer</a> e <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Visão geral do Modo de Texto</a>.</p>

<p>Por padrão, o Workfront vem com um conjunto de campos que definem os objetos e suas informações. Você também pode criar campos personalizados para definir objetos, mas não pode criar objetos personalizados.</p>

<p>No Workfront Planning, é possível criar campos personalizados para todos os tipos de registro. Os tipos de registro do Workfront vêm com um número muito limitado de campos. É necessário criar todos os campos do zero e associá-los aos tipos de registro. Para obter informações, consulte <a href="/help/quicksilver/planning/fields/fields-overview.md">Visão geral do campo</a>. </p> <p>O Workfront Planning exige uma licença adicional. </p>   
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filtro]</td> 
   <td> <p>Um dos blocos principais de um relatório ou um elemento de lista que define quais informações são exibidas na tela. Para obter mais informações sobre elementos de relatórios, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de relatórios: filtros, exibições e agrupamentos</a>.</p> <p>O Filtro determina os resultados que são exibidos em um relatório ou em uma lista do painel [!DNL Workfront], como projetos, tarefas ou problemas.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Gerenciamento de Trabalho Financeiro]</td> 
   <td>Processo para gerenciar dados de custos de mão de obra, despesas e receita em [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo Fixo]</td> 
   <td>Você pode definir uma quantia fixa de custo para um projeto. Isso faz parte do [!UICONTROL Custo Planejado] do projeto que representa a quantidade de dinheiro necessária para concluir o projeto. Para obter informações sobre custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Receita Fixa]</td> 
   <td>Você pode definir uma quantia fixa de receita para um projeto. Isso faz parte da [!UICONTROL Receita Planejada] do projeto que representa a quantidade de dinheiro que você pode obter se concluir o projeto. Para obter informações sobre receita, consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão Geral de Faturamento e Receita</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sinalizadores]</td> 
   <td> <p> Este campo é igual ao dos [!UICONTROL Ícones de Status], mas só está disponível para os seguintes modos de exibição: </p> 
    <ul> 
     <li> [!UICONTROL Modelos] </li> 
     <li> [!UICONTROL Despesas] </li> 
    </ul> <p> Para obter mais informações, consulte o artigo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ícones de status internos em Exibições</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta]</td> 
   <td>Pastas são usadas para organizar documentos ou relatórios associados a um objeto.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (Equivalente a Tempo Integral)</td> 
   <td>Este é o Equivalente de Tempo Integral que indica a quantidade de tempo em que um recurso está disponível para trabalho. 
   O campo [!UICONTROL FTE] é exibido nas seguintes áreas: 
  <ul>
   <li> Perfil do usuário, ao editar ou criar o usuário </li>
   <li> [!UICONTROL Planejador de Recursos] </li>
   <li> [!UICONTROL Scenario Planner] (requer licença adicional para o Planejador de cenários do Workfront) </li>
   <li> Listas de usuários e relatórios </li> </ul>

<p>O [!UICONTROL FTE] deve ser um número decimal até 1 e não pode ser 0. </p>
   <p> Um [!UICONTROL FTE] de 1 (que é o padrão para o campo [!UICONTROL FTE] de um usuário, conforme definido em seu perfil) significa que um recurso (usuário ou função) trabalha o número inteiro de horas, com base no agendamento que calcula sua disponibilidade. </p>
   <p>O administrador do Workfront decide qual programação usar para determinar a disponibilidade do usuário.  </p>
   <ul>
   <li> Quando a [!UICONTROL Default Schedule] é usada, o Workfront usa o [!UICONTROL FTE] do usuário encontrado no perfil para calcular a disponibilidade. </li>
   <li> Quando a Agenda do Usuário é usada, o Workfront usa a folga do usuário, o valor da [!UICONTROL Tempo de Trabalho] e as horas da [!UICONTROL Agenda Padrão] para calcular o [!UICONTROL FTE] do usuário. </li> </ul>

<p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências de Gerenciamento de Recursos</a>.  </p>
   <p>Para obter mais informações sobre como criar agendas em [!DNL Workfront], consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar uma agenda</a>. </p>

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
   <th>Nome do objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Gráfico de Gantt]</td> 
   <td> <p>Uma linha do tempo visual das datas do projeto em uma visão de calendário baseada nas datas planejadas ou projetadas, à medida que as tarefas do projeto são agendadas no momento.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Meta]</td> 
   <td><p>Há dois conceitos de metas em [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Metas do projeto</b>: um conjunto de objetivos comerciais acordados pelos participantes relevantes de um projeto. As metas do projeto fazem parte do Business Case de um projeto. </p> <p>Não é possível exibir metas do projeto em listas ou relatórios, mas você pode acessá-las por meio da API. </p> <p>Para obter informações sobre as metas do projeto de Business Case, consulte <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Criar metas de Business Case </a>. </p> </li> 
     <li> <p><b>Metas estratégicas</b>: uma meta estratégica é um objetivo que você cria para planejar sua estratégia de trabalho para um período específico. Você pode criar esses tipos de metas usando o [!DNL Workfront Goals]. Sua organização deve adquirir uma licença adicional e você deve ter acesso a esse recurso para poder criar metas estratégicas. [!DNL Workfront Goals] estão disponíveis somente com uma licença adicional.</p> 
     <p>Para obter mais informações, consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] visão geral </a>. </p> 
     <p>Você pode exibir metas estratégicas em um relatório de meta ou projeto e acessá-las por meio da API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Hierarquia de Meta]</td> 
   <td> <p>Nos relatórios de [!UICONTROL Meta] e [!UICONTROL Projeto], este é um campo de coleção que mostra as metas na hierarquia às quais uma meta estratégica pertence quando se alinha a outras metas. As metas são separadas por um delimitador de. </p> <p>Somente os pais da meta e a meta são exibidos neste campo. As metas secundárias não são exibidas. </p> <p>Para obter informações sobre como alinhar metas no [!DNL Workfront Goals], consulte a <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Visão geral do alinhamento de metas em [!DNL Workfront Goals]</a>. </p> 
   <p>Este campo só estará visível se sua organização tiver comprado [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] visão geral </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Pontuação de Sucesso da Meta]</td> 
   <td> Em um [!UICONTROL Project report], esse campo era usado para fazer referência às metas de nível de projeto associadas ao Caso [!UICONTROL Business]. No momento, esse campo está obsoleto e não está associado a nenhuma funcionalidade.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Metas] </td> 
   <td> <p>Em um relatório de [!UICONTROL Project], este é um campo de coleção que exibe todas as metas estratégicas associadas a um projeto. As metas são separadas por vírgulas.</p> <p>Este campo só estará visível se sua organização tiver comprado [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] visão geral</a>. Para obter mais informações sobre metas estratégicas e metas do projeto no [!DNL Workfront], consulte "[!UICONTROL Meta]" neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Preferências de Interface Global]</td> 
   <td>Configurações de interface que afetam todos os usuários. As [!UICONTROL Preferências de Interface Global] podem ser substituídas pelas [!UICONTROL Preferências de Interface de Usuário].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Grupo]</td> 
   <td> <p>Um conjunto de usuários (possivelmente do mesmo departamento ou unidade de negócios) que têm acesso aos mesmos objetos. Além dos usuários, os grupos podem ser associados a portfólios, programas, projetos, <span> modelos de projeto, </span> empresas, equipes, agendamentos, modelos de layout e perfis de quadro de horários.</p> <p>Você também pode conceder permissões a objetos por grupo. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Visão geral dos grupos</a>.</p> <p>Em uma lista ou relatório de objetos de um dos tipos a seguir, você pode usar o campo [!UICONTROL Group] para listar quais objetos desse tipo estão associados a um grupo específico: usuário, portfólio, programa, projeto, <span>modelo de projeto</span>, empresa, equipe, agendamento, modelo de layout ou perfil de folha de horas.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Administrador de Grupo]</td> 
   <td> <p>Usuários que gerenciam os objetos, o acesso e os usuários dos grupos de usuários designados.</p> <p> Em um relatório do [!UICONTROL Group], esse campo exibe os nomes dos usuários designados como [!UICONTROL Group Administrators] no Grupo. Para obter mais informações sobre Administradores de Grupo, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Grupo com Acesso de Administração]</td> 
   <td> <p> Em um [!UICONTROL Modelo de layout], [!UICONTROL Perfil de folha de horas] ou [!UICONTROL Relatório de agendamento], esse campo exibe os Grupos cujos Administradores de Grupo têm acesso para modificar o modelo. Você também pode filtrar esse relatório por esse campo. </p> <p> Para obter mais informações, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Agrupamento]</td> 
   <td> <p>Um elemento de relatório usado para categorizar informações em uma lista por um critério comum.</p> <p>Para obter mais informações, consulte a seção "[!UICONTROL Groupings]" no artigo <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de relatório: filtros, exibições e agrupamentos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de Transferência]</td> 
   <td> <p>A data em que uma tarefa se torna disponível para trabalho. A [!UICONTROL Data de Transferência] é um cálculo e não pode ser definida manualmente. <br>Para obter mais informações sobre a [!UICONTROL Data de Transferência], consulte o artigo <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL Data de Transferência da Tarefa] visão geral</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>Um nome alternativo para descrever a área [!UICONTROL Solicitações] de [!DNL Workfront]. Você pode usar a área [!UICONTROL Solicitações] para processar tíquetes de suporte ao cliente, solicitações de projeto, tíquetes de suporte técnico etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proprietário]</td> 
   <td>Em um relatório [!UICONTROL Hour], o [!UICONTROL Proprietário] é o usuário ao qual as horas são atribuídas. Isso é diferente do usuário que está realmente registrando o horário. Às vezes, essas duas entidades podem ser dois usuários diferentes. <br>Para obter mais informações sobre o tempo de registro para outro usuário, consulte o artigo <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Tempo de registro</a>.</td> 
  </tr>

<tr> 
   <td>Status de Hora</td> 
   <td> <p>Um atributo definido pela Workfront para as Horas efetivas que os usuários registram para tarefas, problemas ou projetos. </p>

As entradas de horas podem ter um dos seguintes status no Workfront:
<ul>
   <li><b>Enviado</b>: as horas foram registradas em um projeto, tarefa ou problema. Eles fazem parte de um registro de cobrança ou ainda não foram adicionados a um registro de cobrança.</li>
   <li><b>Aprovado</b>: as horas foram registradas e aprovadas pelo Proprietário do Projeto. Eles fazem parte de um registro de cobrança ou ainda não foram adicionados a um registro de cobrança.</li> 
   <li><b>Não Aprovado</b>: as horas foram registradas e rejeitadas pelo Proprietário do Projeto. Eles fazem parte de um registro de cobrança ou ainda não foram adicionados a um registro de cobrança.</li>
   <li><b>Faturado</b>: as horas foram registradas, adicionadas a um registro de cobrança e o status do registro de cobrança foi marcado como Faturado. Elas não precisavam ser aprovadas pelo Proprietário do projeto.</li>
   <li><b>Faturado e Aprovado</b>: as horas foram registradas, aprovadas pelo Proprietário do projeto e o status do registro de cobrança foi marcado como Faturado.</li>
   </ul>

<p>Quando as horas fazem parte de um registro de cobrança, o Status da Hora indica se as horas foram aprovadas ou se o Registro de cobrança ao qual pertencem foi faturado. O Status de Hora de uma entrada de hora é visível apenas em uma lista de horas ou relatório. </p>

<p>Para obter mais informações sobre como adicionar horas a registros de cobrança, consulte a seção "Adicionar horas a registros de cobrança" no artigo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Criar registros de cobrança</a>.</p>

<p>Para obter mais informações sobre o tempo de aprovação de projetos, consulte <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Solicitar tempo para ser aprovado para um projeto</a>.</p>

<p><b>DICA</b></p>

<p>As Horas Gerais que não estão conectadas diretamente a itens de trabalho não exibem um Status de Hora. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Tipo de Hora]</td> 
   <td> <p>Um atributo que pode ser definido para Horas efetivas que os usuários registram para tarefas, problemas ou projetos. Este também é um atributo para as horas registradas que não estão diretamente vinculadas ao trabalho, como [!UICONTROL Férias] e [!UICONTROL Folga].</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Gerenciar tipos de horas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>A ID é um indicador alfanumérico associado a cada objeto em [!DNL Workfront]. Identifica exclusivamente cada objeto no banco de dados [!DNL Workfront]. Você pode visualizar a ID de qualquer objeto em um relatório ou uma lista para cada objeto. </p> <p><b>DICA</b></p>   <p>Você também pode exibir a ID no URL da página do objeto. Por exemplo, ao acessar a página [!UICONTROL Detalhes do projeto], a ID de um projeto pode se parecer com o número descrito na URL a seguir:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL IMS]</td> 
   <td>Sistema Identity Management. O Adobe IMS exige que você faça logon no Workfront por meio da Adobe, em vez de usar seu nome de usuário e senha da Workfront.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Metas Individuais]</td> 
   <td>Metas individuais que contribuem para as métricas das metas da equipe, mas não relacionadas ao desenvolvimento pessoal ou de carreira.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Acesso Herdado]</td> 
   <td>Função de compartilhamento que permite que o acesso se propague do objeto para outro. Por exemplo, o acesso herdado do usuário do projeto definido nos registros do programa e do portfólio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Iniciativa]</td> 
   <td> <p>No [!DNL Workfront Scenario Planner], você pode dividir um plano em várias iniciativas para facilitar o gerenciamento do plano. <span>Você pode criar um relatório da [!UICONTROL Initiative] e acessar informações da [!UICONTROL Initiative] em um relatório do [!UICONTROL Project].</span></p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">A visão geral</a> de [!DNL Scenario Planner]. </p> <p>O relatório [!DNL Initiative] não está visível na instância [!DNL Workfront], a menos que a empresa tenha comprado uma licença [!DNL Workfront Scenario Planner]. Não é possível acessar [!UICONTROL Iniciativas] por meio da API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Função de Trabalho Iniciativa]</span> </td> 
   <td> <p><span>O tipo de relatório [!UICONTROL Função de Trabalho da Iniciativa] exibe informações sobre as funções de trabalho associadas a uma iniciativa de plano no [!DNL Workfront Scenario Planner].</span> </p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">A visão geral</a> de [!DNL Scenario Planner]. </p> <p><span>Este tipo de relatório não é visível na instância [!DNL Workfront], a menos que a empresa tenha comprado uma licença [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Horas da Função de Trabalho da Iniciativa]</span> </td> 
   <td> <p><span> Em um relatório de [!UICONTROL Função de Trabalho da Iniciativa], é exibido o número de horas associado a uma função de trabalho em uma iniciativa.</span> </p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">A visão geral</a> de [!DNL Scenario Planner]. </p> <p>Este campo e o tipo de relatório da [!UICONTROL Função de Trabalho da Iniciativa] não estão visíveis na instância [!DNL Workfront], a menos que a empresa tenha comprado uma licença [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contagem de Funções de Trabalho da Iniciativa]</td> 
   <td> <p>Em um relatório de [!UICONTROL Função de Trabalho da Iniciativa], é exibido o número de funções de trabalho específicas associadas a uma iniciativa.</p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">A visão geral</a> de [!DNL Scenario Planner]. </p> <p>Este campo e o tipo de relatório da [!UICONTROL Função de Trabalho da Iniciativa] não estão visíveis na instância [!DNL Workfront], a menos que a empresa tenha comprado uma licença [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data da Última Publicação da Iniciativa]</td> 
   <td> <p>Um campo em um relatório de [!UICONTROL Initiative], [!UICONTROL Initiative Job Role] e [!UICONTROL Project] que exibe a data em que uma iniciativa de plano foi publicada pela última vez em um projeto. É possível publicar iniciativas para criar projetos ou atualizar projetos vinculados às iniciativas.</p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">A visão geral</a> de [!DNL Scenario Planner]. </p> <p><span>Para obter informações sobre como publicar iniciativas, consulte</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publicar cenários para criar e atualizar projetos no [!DNL Workfront Scenario Planner]</a>. Este campo não está visível na instância [!DNL Workfront], a menos que a empresa tenha comprado uma licença [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pesquisa em Linha]</td> 
   <td>Uma pesquisa realizada, no processo de preencher um formulário, para localizar possíveis entradas para um campo específico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuração de Interface]</td> 
   <td>A área do aplicativo que permite definir Exibições personalizadas, Filtros, Agrupamentos, Controles de lista etc.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL É o Objetivo da Empresa]</p></td> 
   <td> <p>Em [!DNL goal reports], exibe um valor "[!UICONTROL True]/ [!UICONTROL False]" para cada meta estratégica para indicar se sua organização está atribuída à meta como seu proprietário. </p> 
   <p>Este campo só estará visível se sua organização tiver comprado [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] visão geral </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problema]</td> 
   <td> <p>Um item de trabalho não planejado que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Ele é triado e avaliado para consideração adicional do esforço de trabalho</p> <p>Um [!UICONTROL Problema] também pode ser uma solicitação de [!UICONTROL Help Desk]. [!UICONTROL Pedidos de Alteração], [!UICONTROL Pedidos] e [!UICONTROL Bugs] também são [!UICONTROL Problemas].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gerenciamento de Problemas]</td> 
   <td> <p>O processo e as regras que regem a definição de tipos de problemas e o processo de roteamento, triagem ou tráfego associado a cada tipo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Proprietário de Problema]</td> 
   <td>A equipe ou os usuários responsáveis por testar e concluir um problema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteração]</td> 
   <td>Um período no qual uma equipe produz um conjunto predefinido de materiais de entrega.</td> 
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
   <td>[!UICONTROL Função de Trabalho]</td> 
   <td> <p>Usado para identificar as funções e responsabilidades diárias de um usuário. Funções de trabalho podem ser atribuídas a itens de trabalho para identificar a habilidade necessária para concluir um processo de trabalho sem atribuí-lo a um usuário específico. </p> <p>Um usuário pode ter mais de uma função. Os exemplos incluem Designer gráfica ou consultor.</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Entrada de Diário]</p> </td> 
   <td> <p>Um objeto reportável que informa informações sobre atualizações do sistema para campos rastreados que aparecem na área [!UICONTROL Atualizações] de projetos, tarefas, problemas e outros objetos.</p> <p>Para saber mais, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Relatório na área Atualizações com um relatório de Entrada de Diário</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sinalizador Kanban]</td> 
   <td> <p>Em um Relatório de [!UICONTROL Tarefa] ou Relatório de [!UICONTROL Problema], o campo [!UICONTROL Sinalizador Kanban] exibe o status do sinalizador definido na matéria no quadro [!UICONTROL Kanban]. Os valores possíveis são [!UICONTROL On Track], [!UICONTROL Ready to Pull] e [!UICONTROL Is Blocked].</p> <p>Para obter mais informações sobre como definir o status do sinalizador em matérias no [!UICONTROL Kanban story board], consulte  o artigo <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Use sinalizadores em matérias no [!UICONTROL Kanban board]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPIs</td> 
   <td>Um valor mensurável que demonstra quão efetivamente uma empresa está atingindo os principais objetivos de negócios.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Defasagem]</td> 
   <td>Tempo decorrido após a [!UICONTROL Data de conclusão planejada] da tarefa predecessora ter passado até que a tarefa dependente possa começar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipos de Defasagem]</td> 
   <td> <p>O método de cálculo do [!UICONTROL Lag]. Pode ser:</p> 
    <ul> 
     <li>[!UICONTROL Dias] (dias úteis)</li> 
     <li>[!UICONTROL Dias do Calendário] (ignorar feriados)</li> 
     <li>[!UICONTROL Porcentagem]</li> 
     <li>[!UICONTROL Dia da Semana]</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Visão geral dos Tipos de Defasagem</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniatura Grande]</td> 
   <td> <p> Em uma lista ou relatório do [!UICONTROL Document], é exibida uma visualização do documento em miniatura. </p> <p>Selecione <strong>[!UICONTROL Miniatura Grande]</strong> para exibir uma miniatura de 400 pixels de largura no relatório.</p> <p>O tamanho da miniatura é ajustado quando você modifica a largura da coluna em uma lista ou relatório.</p> <p>Consulte também "[!UICONTROL Miniatura]" neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Últimos 10 Visualizadores]</td> 
   <td> <p>Em uma lista de relatórios, esse campo exibe os nomes de até 10 usuários que visualizaram o relatório mais recentemente.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Exibir uso de relatório</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última Nota de Condição]</td> 
   <td> <p>Este campo exibe a última atualização inserida em um objeto pelo proprietário do objeto. Esta é a atividade ou interação mais recente do proprietário em um objeto.</p> <p>A coluna [!DNL Last Condition Note] estará vazia se o texto da última nota de um objeto tiver sido excluído. Quando uma nova nota é inserida no objeto, ela se torna a última nota e é exibida novamente na coluna. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data da Última Atualização Financeira]</td> 
   <td>Em um relatório de [!UICONTROL project], este campo captura a data e a hora em que as finanças do projeto foram calculadas e atualizadas pela última vez. Para obter informações sobre finanças do projeto, consulte <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Visão geral das finanças do projeto</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última Nota]</td> 
   <td> <p>Este campo exibe a última atualização inserida em um objeto por qualquer usuário. Esta é a atividade ou interação mais recente em um objeto.</p> <p>A coluna [!UICONTROL Última Nota] estará vazia se o texto da última nota de um objeto tiver sido excluído. Quando uma nova nota é inserida no objeto, ela se torna a última nota e é exibida novamente na coluna.</p>
   <p>Quando este campo é adicionado a um relatório de [!UICONTROL Tarefa], as atualizações são deixadas em objetos filho — como problemas, subtarefas, documentos, etc. — da tarefa não são exibidas nessa coluna.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizado pela Última Vez por]</td> 
   <td> <p>Em uma lista de relatórios, esse campo exibe informações sobre o usuário que visualizou o relatório por último.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Exibir uso de relatório</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data da Última Visualização]</td> 
   <td> <p>Em uma lista de relatórios, esse campo exibe a data em que o relatório foi exibido por último.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Exibir uso de relatório</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Modelo de Layout]</td> 
   <td>Definido pelo Administrador do sistema ou Administrador de grupo para identificar as guias e os relatórios exibidos no espaço de trabalho de um determinado usuário.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de layout]</td> 
   <td>Em conjunto com [!UICONTROL Custom Views], o [!UICONTROL Layout Type] especifica o tipo de [!UICONTROL Custom View]. Atualmente, somente a Lista está disponível. Futuramente, o [!UICONTROL Detail] (a exibição [!UICONTROL Detail] de um objeto) poderá se tornar disponível.</td> 
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
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas Atuais Herdadas]</td> 
   <td> <p>Em um relatório de projeto, tarefa ou problema, as [!UICONTROL Horas Reais Herdadas] são a soma de todas as horas registradas no projeto, tarefa ou problema a qualquer momento, inclusive antes de maio de 2021.</p>  
   <p>As Horas Reais Herdadas são exibidas como Horas Reais em uma área de detalhes de projeto, tarefa ou problema. </p>
   <p>Consulte também <strong>Horas efetivas</strong>.
    <p>Para obter mais informações, consulte <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Exibir Horas Efetivas</a>.</p>
    </td> 
  </tr>  <tr> 
   <td>[!UICONTROL Tipo de Licença]</td> 
   <td>O tipo de licença alocada para um [!UICONTROL Access Level]. Ele é [!UICONTROL Usuário Completo], [!UICONTROL Usuário Limitado] ou [!UICONTROL Solicitante].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plano de Limite de Licença]</td> 
   <td> <p>Em uma exibição ou relatório do [!UICONTROL Group], este campo mostra o número máximo de licenças do [!UICONTROL Plan] que podem ser atribuídas a usuários que têm o respectivo grupo designado como seu [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabalho de Limite de Licença]</td> 
   <td> <p>Em uma exibição ou relatório do [!UICONTROL Group], este campo mostra o número máximo de licenças do [!UICONTROL Work] que podem ser atribuídas a usuários que têm o respectivo grupo designado como seu [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuário Limitado]</td> 
   <td>Um Tipo de Licença que permite a criação de um [!DNL Access Level] que contenha privilégios somente para visualização, com a capacidade de enviar problemas, inserir observações e carregar documentos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Controles de Lista]</td> 
   <td> <p>Parte da [!UICONTROL Interface Setup] que permite vincular Filtros, Visualizações e Agrupamentos personalizados a Usuários individuais ou globalmente a todos os Usuários.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Campos de pesquisa]</td> 
   <td> <p>No Workfront Planning, depois de estabelecer a conexão entre dois tipos de registro e vincular registros individuais, é possível fazer referência aos campos dos registros vinculados no registro a partir do qual você está se conectando.</p>
   <p>Por exemplo, se você conectar um tipo de registro de Campanha a um tipo de objeto Projeto do Workfront, será possível exibir o campo Orçamento dos projetos conectados nos registros da campanha. O campo Budget project é um campo de pesquisa de projetos em uma campanha.</p> <p>Os valores dos campos de pesquisa são preenchidos automaticamente nos registros dos quais estão conectados.</p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/planning/records/connected-records-overview.md">Visão geral dos registros conectados</a>.</p>
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
   <td>[!UICONTROL Somente Manual]</td> 
   <td> <p>Um dos [!UICONTROL Tipos de Atualização] de um [!UICONTROL Project]. Esta configuração permite que as linhas de tempo [!UICONTROL Projeto Projetado] e [!UICONTROL Planejado] sejam atualizadas apenas quando "[!UICONTROL Linhas de Tempo Recalculadas]" for clicado. Projetos configurados dessa maneira serão ignorados durante o processo noturno de recálculo e quando o projeto ou as tarefas no projeto forem atualizadas.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecionar o projeto [!UICONTROL Tipo de Atualização] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL -ME]</td> 
   <td> <p>Refere-se ao usuário conectado no momento. </p> <p>Recomendamos usar esse campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório que exibirá informações diferentes dependendo de quem faz logon para visualizá-lo, já que as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Máximo de Usuários]</td> 
   <td> <p>Este campo está obsoleto. Qualquer informação que este campo possa exibir está relacionada a um recurso que [!DNL Workfront] removeu e o campo não pode ser atualizado. </p> <p>Em versões anteriores do [!DNL Workfront], você poderia atualizar este campo ao criar ou editar uma função de trabalho. Ele exibiu o número total de usuários que podem ser associados a uma função em cada projeto. Um valor zero é permitido para um número ilimitado de usuários que podem ser atribuídos em um projeto. </p>O campo ainda está visível em alguns relatórios e listas, mas as informações exibidas não podem ser atualizadas. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Etapa]</td> 
   <td> <p>Um marcador que pode ser associado a uma tarefa para indicar que um ponto-chave no projeto foi atingido quando a tarefa for concluída. Geralmente, você pode usar marcos para mostrar um evento significativo, como a conclusão de uma fase do projeto ou um conjunto de atividades críticas. As [!UICONTROL Marcos] são normalmente associadas a tarefas pai. Você deve criar marcos antes de anexá-los a tarefas. Para obter informações sobre etapas, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Criar um caminho de etapas</a> e <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Associar etapas a tarefas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Caminho de Etapas]</td> 
   <td>Uma coleção de [!UICONTROL marcos]. [!UICONTROL Caminhos de Etapas] são usados em projetos para distinguir projetos com certos tipos de [!UICONTROL Etapas] de projetos com um conjunto diferente de [!UICONTROL Etapas].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Tarefa de Etapa]</td> 
   <td>Uma tarefa sinalizada para indicar um evento reportável a ser medido.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Módulo]</td> 
   <td>Uma única etapa em um cenário em [!DNL Workfront Fusion] que executa alguma função com base no aplicativo associado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Minha Função Primária]</td> 
   <td> <p>Quando referenciado em filtros, exibe os usuários que têm a mesma [!UICONTROL Primary Role] do usuário conectado ou itens de trabalho atribuídos à [!UICONTROL Primary Role] do usuário conectado.</p> <p>Recomendamos usar esse campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório que exibirá informações diferentes dependendo de quem faz logon para visualizá-lo, já que as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Minha Equipe Doméstica]</td> 
   <td> <p>Quando referenciado em filtros, este campo exibe os usuários que pertencem à [!UICONTROL Equipe Inicial] do usuário conectado ou os itens de trabalho atribuídos à [!UICONTROL Equipe Inicial] do usuário conectado. </p> <p>Recomendamos usar esse campo em um filtro para tornar os relatórios mais genéricos ao compartilhá-los com outros usuários. Dessa forma, você pode criar apenas um relatório que exibirá informações diferentes dependendo de quem faz logon para visualizá-lo, já que as informações são sempre personalizadas para o usuário conectado. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Convenção de nomenclatura]</td> 
   <td>Um conjunto de regras em toda a organização que usa dados para criar nomes de projetos, tarefas e materiais de entrega.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Integração Nativa]</td> 
   <td>Uma integração que não requer codificação manual ou configuração de API. Também chamada de integração "pronta para uso".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menu de Navegação]</td> 
   <td>O painel superior central do aplicativo que tem links para as áreas principais do [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL Novo Valor de Número]</td> 
   <td>Em um relatório de [!UICONTROL Lançamento], é exibido o valor atualizado de um campo que substitui o [!UICONTROL Valor Velho de Número].
   Para obter mais informações, consulte "[!UICONTROL Valor Velho de Número]" neste artigo.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Despesa Não Faturável]</td> 
   <td> <p>Uma despesa que não está marcada como faturável para o cliente. Pode ser uma despesa planejada ou uma despesa real.</p> <p>Os campos Custo de Despesas Não Faturáveis Planejadas e Custo Efetivo de Despesas Não Faturáveis estão disponíveis para serem adicionados a exibições e relatórios. Eles não aparecem nas páginas de detalhes do projeto ou da tarefa.</p>
   <p>Você pode encontrar esses campos nos seguintes tipos de relatórios:</p>
   <ul>
   <li>Linha de base</li>
   <li>Modelo</li>
   <li>Projeto (Dado Financeiro)</li>
   </ul>
   <p>Para obter mais informações sobre como marcar uma despesa como faturável, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Gerenciar despesas do projeto</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Dia Não Útil]</td> 
   <td>Um dia que não está alocado para a conclusão de atribuições. Normalmente, é um dia de férias, feriado ou fim de semana. O termo é exibido no explorador de API. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Observação]</td> 
   <td>Foi feito um comentário ou uma atualização em um objeto [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto de Nota]</td> 
   <td> <p>Isso exibe o texto de uma atualização inserida por um usuário em qualquer objeto. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Número de Metas Vinculadas]</td> 
   <td> <p>Em um relatório de [!UICONTROL Project], esse é o número de metas estratégicas associadas ao projeto. Para obter informações sobre como associar projetos a metas estratégicas, consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Adicionar projetos a metas em [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Para obter informações sobre metas estratégicas, consulte também "[!UICONTROL Meta]" neste artigo.</p> 
   <p>Este campo só estará visível se sua organização tiver comprado [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Adicionar projetos a metas em [!UICONTROL Metas do Adobe Workfront]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Objeto]</td> 
   <td> <p>As informações exibidas em [!DNL Adobe Workfront] são representadas por objetos armazenados no banco de dados [!DNL Workfront]. Os objetos são o que direciona as informações no Workfront. Alguns exemplos de objetos são:</p> 
    <ul> 
     <li>[!UICONTROL Portfólio]</li> 
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
     <li>[!UICONTROL Horas]</li> 
     <li>[!UICONTROL Taxas de Cobrança]</li> 
     <li>[!UICONTROL Modelos]</li> 
     <li>[!UICONTROL Modelos de tarefa]</li>

<p><b>Nota</b></p>
  <p>Esta lista não é extensa. </p>

</ul> <p>Para obter mais informações, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Entender objetos na [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipos de Objeto]</td> 
   <td>Se você criar um relatório ou uma lista contendo todos os formulários personalizados, poderá usar esse campo como uma exibição ou um filtro para ver quais tipos de objeto estão associados a cada formulário. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Valor Velho de Número]</td> 
   <td>Em um relatório de [!UICONTROL Journal Entry], é exibido o valor original de um campo antes de ele ser atualizado. Depois que o valor de um campo for atualizado, ele será exibido como o [!UICONTROL Novo Valor de Número] em um relatório de [!UICONTROL Entrada de Diário]. Para obter mais informações, consulte também "[!UICONTROL Novo Valor de Número]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Somente na alteração]</td> 
   <td> <p>Um dos Tipos de [!UICONTROL Project Update]. Quando selecionado, as linhas do tempo [!UICONTROL Projeto Projetado] e [!UICONTROL Planejado] são atualizadas apenas quando uma atualização ou alteração é feita no projeto ou em uma tarefa dentro do projeto. Ele não atualiza o projeto todas as noites.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecionar o Tipo de Atualização do projeto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa de Operação]</td> 
   <td> <p>O nome do [!UICONTROL Problema] no banco de dados [!DNL Workfront], usado em relatórios do modo de texto ou dados personalizados calculados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abrir]</td> 
   <td>Um problema ou tarefa que não está completa, mas sendo trabalhada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organograma]</td> 
   <td>Abreviação de Organograma. Este é um gráfico que mostra a hierarquia de uma organização. Ele também está na guia na tela de detalhes do [!UICONTROL Usuário] que exibe e permite configurar as relações entre [!UICONTROL Empresa] e [!UICONTROL Relatório] do [!UICONTROL Usuário].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuração Organizacional]</td> 
   <td>Isso define [!UICONTROL Empresas], [!UICONTROL Grupos] e [!UICONTROL Perfis de Segurança] para sua organização.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Outros Grupos]</td> 
   <td> <p>Em um relatório ou exibição que lista usuários, esse campo exibe todos os grupos dos quais cada usuário é membro. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Substituir Moeda]</span> </td> 
   <td> 
    <div> 
     <p>Em um relatório de [!UICONTROL Função de Trabalho], esta é a moeda associada a uma função de trabalho. É uma substituição da [!UICONTROL Moeda Base] conforme estabelecido na área [!UICONTROL Setup] pelo administrador [!DNL Workfront]. </p> 
     <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Substituir Cobrança/Hora da Moeda]</span> </td> 
   <td> 
    <div> 
     <p>Em um relatório [!UICONTROL Função de Trabalho], essa é a taxa de cobrança por hora da função de trabalho usando a [!UICONTROL Substituir Moeda] selecionada da função de trabalho.</p> 
     <p> Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Substituir Custo/ Hora da Moeda]</span> </td> 
   <td> 
    <div> 
     <p>Em um relatório [!UICONTROL Função de Trabalho], essa é a taxa de custo por hora da função de trabalho usando a [!UICONTROL Substituir Moeda] selecionada da função de trabalho. </p> 
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
     <p>Em um relatório de [!UICONTROL Meta], é exibido o tipo de proprietário atribuído a uma meta estratégica. A seguir estão os tipos de proprietário de meta:</p> 
     <ul> 
      <li> <p>[!UICONTROL Usuário]</p> </li> 
      <li> <p>[!UICONTROL Equipe] </p> </li> 
      <li> <p>[!UICONTROL Grupo]</p> </li> 
     </ul> 
     <p>Nenhum valor é exibido nesse campo quando o proprietário da meta é sua organização. </p> 
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
   <th>Nome do objeto</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Parâmetro]</td> 
   <td> <p>Um [!UICONTROL parâmetro] é um campo personalizado. Você pode criar um relatório para todos os parâmetros ou campos personalizados em seu sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pai]</td> 
   <td>Em um relatório, este campo mostra informações sobre o pai do objeto. Por exemplo, em um relatório de [!UICONTROL issue], ele pode mostrar informações sobre a tarefa ou o projeto em que o problema está registrado; em um relatório de tarefa, ele pode mostrar informações sobre a tarefa pai direta ou sobre o projeto. Para obter mais informações sobre quais objetos podem ter pais em [!DNL Workfront], consulte a seção "Interdependência e hierarquia de objetos" no artigo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Entender objetos em [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Defasagem Pai]</td> 
   <td>O tempo que deve decorrer entre o início da [!UICONTROL Tarefa Pai] e o Início da [!UICONTROL Subtarefa].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa Pai]</td> 
   <td>Também conhecida como [!UICONTROL Summary Task]. Esta é uma tarefa que tem Subtarefas (também chamada de [!UICONTROL Tarefas Filhas]). A [!UICONTROL Duration], o [!UICONTROL Trabalho Necessário] e o [!UICONTROL Porcentagem Concluída] da Tarefa Pai são calculados a partir das Subtarefas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Recursos de Meio Período]</td> 
   <td>Um usuário licenciado que tem menos capacidade do que o agendamento padrão definido no sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Porcentagem Concluída]</td> 
   <td> <p>Um campo de projeto, tarefa ou problema que mostra qual porcentagem do trabalho associado à tarefa, projeto ou problema foi concluída.</p> <p>Você pode atualizar esse campo manualmente para problemas e tarefas de trabalho. </p> <p>Para projetos e tarefas pai, esse campo é um acúmulo de todas as tarefas de trabalho e você não pode atualizá-lo manualmente. </p> <p>Para obter mais informações, consulte Visão geral do <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Projeto [!UICONTROL Porcentagem Concluída]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permissão]</td> 
   <td> <p>Direitos concedidos a um usuário em um objeto, normalmente fornecidos para que ele possa concluir o trabalho no item ou visualizá-lo. Você pode conceder permissões para:</p> 
    <ul> 
     <li>[!UICONTROL Projetos]</li> 
     <li>[!UICONTROL Tarefas]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Portfólio]</li> 
     <li>[!UICONTROL Programas]</li> 
     <li>[!UICONTROL Relatórios]</li> 
     <li>[!UICONTROL Painéis]</li> 
     <li>[!UICONTROL Documentos]</li> 
     <li>[!UICONTROL Forms Personalizado]</li> 
     <li>[!UICONTROL Exibições]</li> 
     <li>[!UICONTROL Filtros]</li> 
     <li>[!UICONTROL Agrupamentos]</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral das permissões de compartilhamento em objetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plano]</td> 
   <td> <p>Este é um tipo de licença completa no sistema [!DNL Workfront]. Os usuários devem ter este recurso para acessar todos os recursos no [!DNL Workfront].</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] visão geral das licenças</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plano] (no [!DNL Scenario Planner])</td> 
   <td> <p>Um plano é o objeto principal ao trabalhar com o Planejador de cenários [!DNL Workfront]. Você pode destacar a estratégia para o futuro próximo e de longo prazo de sua empresa, identificar cada resultado de alto nível e adicioná-lo como um plano ao Planejador de cenários do [!DNL Workfront]. </p> <p>Você não pode exibir planos do [!DNL Scenario Planner] em um relatório e não pode acessá-los por meio da API do [!DNL Workfront]. </p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">A visão geral</a> de [!DNL Scenario Planner]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planejado]</td> 
   <td> <p>O período dentro do qual algo está programado para ocorrer. Ao criar projetos, tarefas ou problemas no [!DNL Workfront], você estabelece as datas planejadas de início e término, bem como o período planejado durante o qual elas ocorrem. Esses valores representam sua intenção original ou estimativa de quanto tempo um item deve levar para ser concluído. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefício Planejado]</td> 
   <td>Esta é uma entrada manual para o Gerente de projetos para estimar se a conclusão de um projeto traria algum benefício monetário para a organização. A especificação desse valor pode fazer parte da montagem de um [!UICONTROL Business Case] para o projeto. Você deve ter permissões [!UICONTROL Manage] para o projeto para atualizar esse valor.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Horas Orçadas Planejadas]</td> 
   <td> <p>Em um relatório de [!UICONTROL Hora Orçada], é exibido o número de horas orçadas para projetos ou [!UICONTROL Funções de Trabalho] no [!UICONTROL Resource Planner]. </p> <p>Para obter informações sobre projetos ou funções de orçamento no [!UICONTROL Resource Planner], consulte o artigo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Recursos de orçamento no [!UICONTROL Resource Planner] usando os modos de exibição [!UICONTROL Project] e [!UICONTROL Role]</a>. Para obter informações sobre o relatório [!UICONTROL Budgeted Hours], consulte o artigo <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Relatório: Budgeted Hour</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de Término Planejada]</td> 
   <td> <p>Você pode definir manualmente a [!UICONTROL Data de conclusão planejada] de uma tarefa, projeto ou problema para uma data de sua escolha. Se você não definir a [!UICONTROL Data de Conclusão Planejada], [!DNL Workfront] a definirá automaticamente. Quando definida automaticamente, a [!UICONTROL Data de conclusão planejada] é: [!UICONTROL Data de início planejada] + [!UICONTROL Duração]</p> <p>Para obter mais informações, consulte os seguintes artigos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Visão geral da tarefa [!UICONTROL Data de Término Planejada]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Definir a [!UICONTROL Data de Término Planejada]</a> do projeto </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo Planejado]</td> 
   <td> <p>Um total do [!UICONTROL Custo de Trabalho Planejado] e do [!UICONTROL Custo de Despesas Planejado] do projeto. Isso não inclui o [!UICONTROL Custo de Risco Planejado] no projeto.  </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Alinhamento de Data Planejada]</td> 
   <td> <p>Este é um indicador automático que o Workfront atribui a projetos, tarefas e problemas para mostrar quando um item será concluído em relação à Data de conclusão planejada. </p>
   <p>A seguir estão os valores possíveis para o indicador de Alinhamento de Data Planejada: </p>
<ul>
<li>Será terminado na data planejada de término</li>
<li>Será terminado antes da data planejada de término</li>
<li>Será terminado depois da data planejada de término</li></ul>
<p>O Alinhamento da data planejada está visível em listas e relatórios de projetos, tarefas e problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Duração Planejada]</td> 
   <td> <p>A [!UICONTROL Duração Planejada] de uma tarefa geralmente é a mesma [!UICONTROL Duração] da tarefa. Representa a diferença em dias entre o [!UICONTROL Início Planejado] e as [!UICONTROL Datas de Conclusão Planejadas] da tarefa. </p> <p>Quando a tarefa tem um Tipo [!UICONTROL Duration] de [!UICONTROL Effort Driven], a Duração Planejada  pode ser diferente da Duração  da tarefa, com base nos recursos atribuídos a ela. </p> <p>Por exemplo, se uma tarefa com um tipo [!UICONTROL Duração] de [!UICONTROL Controlado por Esforço] tiver uma [!UICONTROL Duração] de 3 dias e você atribuir um recurso com um agendamento de tempo integral à tarefa, a [!UICONTROL Duração Planejada] também será de 3 dias. Se você atribuir três recursos com um agendamento de tempo integral à mesma tarefa, a [!UICONTROL Duration] permanecerá 3 dias, mas a Duration Planned será de 1 dia. A [!UICONTROL Duração Planejada] também altera as datas de [!UICONTROL Início Planejado] e [!UICONTROL Conclusão Planejada] da tarefa, para refletir a nova [!UICONTROL Duração Planejada]. Como resultado, a linha do tempo do projeto também é afetada. </p> <p>Para obter mais informações sobre a diferença entre a [!UICONTROL Duração] e a [!UICONTROL Duração Planejada] para tarefas, consulte o artigo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Diferença entre a [!UICONTROL Duração Planejada] e a [!UICONTROL Duração] para tarefas</a>.</p> <p>Projetos e problemas não têm uma [!UICONTROL Duração Planejada]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Duração Planejada em Minutos]</td> 
   <td> <p>A [!UICONTROL Duração planejada em minutos] de um projeto ou problema é a [!UICONTROL Duração] do projeto ou problema em minutos. </p> <p>As tarefas não têm um campo [!UICONTROL Planned Duration Minutes]. </p> <p>[!UICONTROL Modelos de Tarefa] têm um campo [!UICONTROL Duração Planejada em Minutos] que exibe a [!UICONTROL Duração Planejada] da tarefa em minutos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo de Despesas Planejado]</td> 
   <td> <p>A soma dos [!UICONTROL Valores Planejados] de todas as despesas registradas para um projeto ou uma tarefa.</p> <p><b>EXEMPLO</b></p>
   <p>Se você criar uma despesa para a Tarefa 1 e inserir $600,00 no campo [!UICONTROL Quantia Planejada], o [!UICONTROL Custo de Despesas Planejadas] para essa tarefa será de $600,00. </p> 
   <p>Para um projeto, [!DNL Workfront] usa a seguinte fórmula para calcular o [!UICONTROL Custo de Despesa Planejado]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Horas Planejadas]</td> 
   <td> <p>Este campo aparece nas áreas [!UICONTROL projetos], [!UICONTROL tarefas] e problemas, relatórios de projetos, tarefas ou problemas, e ferramentas de gerenciamento de recursos como o [!UICONTROL Planejador de Recursos], [!UICONTROL Balanceador de Carga de Trabalho] e o relatório [!UICONTROL Utilização]. </p> <p>Ela mostra o número de horas que o Proprietário do projeto estima que cada tarefa ou problema deve levar para ser concluído. Para projetos, geralmente é um pacote das [!UICONTROL Horas planejadas] das tarefas no projeto. </p> <p>O campo [!UICONTROL Horas Planejadas] pode exibir informações diferentes dependendo de onde você as exibe. Para obter informações sobre as Horas Planejadas, consulte <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">visão geral das Horas Planejadas</a>.</p> <p>As Horas Planejadas são armazenadas em minutos no banco de dados [!DNL Workfront]. Ao escrever cálculos usando esse campo, certifique-se de considerar o fato de que as horas são exibidas como minutos.<br></p> <p>Por padrão, as Horas Planejadas são distribuídas igualmente a todos os dias dentro da duração de um item de trabalho e também igualmente para todos os recursos atribuídos à tarefa. Os usuários podem atualizar o número diário de Horas Planejadas para um item de trabalho ou as Horas Planejadas individuais para cada destinatário.</p> <p>A atualização desse campo é diferente para projetos, tarefas e problemas: </p> 
    <ul> 
     <li> <p>Para ocorrências, você pode atualizar manualmente esse campo. As horas planejadas de problemas não são adicionadas às horas planejadas do projeto. </p> <p><b>DICA</b></p> <p>Em um relatório de problemas, um dos campos [!UICONTROL Horas planejadas] é substituído pelo campo [!UICONTROL Trabalho]. O campo exibe o número de Horas planejadas da ocorrência. Para obter mais informações, consulte os campos "trabalho" ou "[!UICONTROL Trabalho]" nesta tabela. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Para tarefas, você pode atualizar manualmente esse campo quando o [!UICONTROL Tipo de Duração] da tarefa for [!UICONTROL Atribuição Calculada] ou [!UICONTROL Simples]. Este campo é calculado por [!DNL Workfront] quando o [!UICONTROL Tipo de Duração] da tarefa é [!UICONTROL Trabalho Calculado] ou [!UICONTROL Esforço Controlado].<br>Para obter informações sobre a [!UICONTROL Duração da Tarefa], consulte o artigo <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Tarefa [!UICONTROL Duração] e [!UICONTROL Tipo de Duração]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Para projetos, [!DNL Workfront] calcula as Horas Planejadas adicionando todas as Horas Planejadas de todas as tarefas do projeto. </p> </li> 
    </ul> <p><b>DICA</b></p> <p>Você pode exibir [!UICONTROL Trabalho necessário] nos relatórios do [!UICONTROL projeto], [!UICONTROL tarefa] ou [!UICONTROL problemas] também usando o modo de texto e referenciando campos adicionais. Para obter mais informações, consulte os campos "<code>work</code>", "[!UICONTROL Work]" e "<code>workRequiredExpression</code>" nesta tabela. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo de Trabalho Planejado]</td> 
   <td> 
    <p>Para uma tarefa, a taxa horária do usuário ou função multiplicada pelo número de horas atribuídas ao usuário ou função.</p> <p>Para um projeto, é um total de todos os [!UICONTROL Custos de Trabalho Planejados] de todas as tarefas.</p> <p>A taxa de uso do usuário ou da função depende do Tipo de Custo selecionado para determinada tarefa. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md">Rastrear custos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Receita Planejada]</td> 
   <td> <p>Tarefas e projetos podem exibir um valor para a [!UICONTROL Receita Planejada] em [!DNL Workfront]. A [!UICONTROL Receita Planejada] representa a quantidade de dinheiro associada às [!UICONTROL Horas Planejadas] das tarefas no projeto. Para projetos, também pode incluir a [!UICONTROL Receita fixa] do projeto. </p> <p>Para tarefas, esta é a receita associada às [!UICONTROL Horas Planejadas] de tarefas. As Horas Planejadas de todas as tarefas são acumuladas até as Horas Planejadas do projeto para contribuir com o cálculo do projeto [!UICONTROL Horas Planejadas]. </p> 
   <p>[!DNL Workfront] calcula a [!UICONTROL Receita Planejada] para tarefas e projetos usando as seguintes fórmulas:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>A [!UICONTROL Receita Planejada] do projeto exibida na área [!UICONTROL Detalhes do Projeto] e nos relatórios do projeto é diferente da Receita Planejada exibida no relatório [!UICONTROL Utilização]. </p> <p>A [!UICONTROL Receita Planejada] na área [!UICONTROL Detalhes do Projeto] reflete a receita da tarefa, bem como a Receita Fixa do projeto. A [!UICONTROL Receita Planejada] no [!UICONTROL Relatório de Utilização] exibe a [!UICONTROL Receita Planejada] associada somente às tarefas do projeto. </p> 
     <p><b>EXEMPLO</b></p>  
      <p>Se o projeto tiver uma tarefa com 10 horas, atribuída a um Consultor com uma taxa horária de US$ 20, e o projeto tiver US$ 100 [!UICONTROL Receita Fixa], o relatório [!UICONTROL Utilização] exibirá US$ 200 para [!UICONTROL Receita Planejada] (a [!UICONTROL Receita Planejada] associada às horas na tarefa). A seção [!UICONTROL Detalhes do Projeto] exibe US$ 300 (a [!UICONTROL Receita Planejada] da tarefa e a Receita Fixa do projeto.) </p> 
    <p>Para obter informações sobre o rastreamento da receita em [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Visão Geral de Faturamento e Receita</a>. </p> 
    <p>Para obter informações sobre os cálculos de [!UICONTROL Receita Planejada] no [!UICONTROL Relatório de Utilização], consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Exibir informações sobre a utilização de recursos </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo de Risco Planejado]</td> 
   <td> <p>O total do [!UICONTROL Custo Potencial] de todos os riscos no projeto considerando sua Probabilidade de ocorrência. Esse valor não está incluído no [!UICONTROL Custo Planejado] do projeto.</p> <p>O [!UICONTROL Custo de Risco Planejado] de um projeto é calculado pela seguinte fórmula:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Perfil de Portal]</td> 
   <td>Uma coleção de Guias e Seções definida pelo administrador que é exibida no [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seção do Portal]</td> 
   <td>Um componente de uma guia em uma página de portal ou painel. Geralmente, um único Relatório, Gráfico, Calendário ou lista de informações principais.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Guia Portal]</td> 
   <td>Uma guia em um portal ou painel que contém até três seções do portal.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Uma coleção de projetos com características unificadoras. Esses projetos geralmente competem pelos mesmos recursos, orçamento ou período. Você pode dividir Portfólios em Programas e associar os projetos aos Programas antes que eles sejam adicionados a uma Portfolio.</p> <p>Para obter mais informações sobre portfólios, consulte <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Visão geral do Portfolio em [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Gerenciamento Portfolio]</td> 
   <td>Uma área de prática focada no gerenciamento de uma coleção ou de programas e esforços de projeto relacionados.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Otimizer]</td> 
   <td>Uma ferramenta [!DNL Workfront] para auxiliar na avaliação e priorização de projetos em um portfólio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Proprietário do Portfolio]</td> 
   <td>A parte interessada responsável pela definição de prioridades e pelo orçamento de um portfólio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custo de Risco Potencial]</td> 
   <td>Este é um campo de projeto que você pode localizar em listas e relatórios. Mostra o custo potencial para os riscos associados ao projeto, caso ocorram. Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular Custo do Risco Potencial </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessora]</td> 
   <td> <p>Uma tarefa que deve ser concluída antes da conclusão de uma tarefa dependente. Também é uma tarefa marcada como uma [!UICONTROL Dependência] para outra tarefa. Predecessores permitem que o planejador defina a lógica de dependência de sequência, como iniciar uma tarefa após a conclusão de outra tarefa.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Visão geral dos predecessores da tarefa</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Empresa Primária]</td> 
   <td>A Empresa à qual o usuário pertence conforme designado nas configurações do usuário. Empresas também podem ser associadas a projetos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contato Primário]</td> 
   <td><p>O [!UICONTROL Contato Primário] é o criador de um problema e é automaticamente designado por [!DNL Workfront] quando alguém cria o problema. Você pode atualizar manualmente esse campo se tiver [!DNL Manage] permissões para o problema. Um problema pode ter apenas um contato principal.</p> 
   <p>Se você alterar o Contato principal, o usuário originalmente designado como contato principal ainda terá acesso à ocorrência pela [!UICONTROL Manager].</p>
   <p>Ao converter um problema em uma tarefa ou projeto, o usuário designado como o [!UICONTROL Contato Principal] do problema se torna o [!UICONTROL Originador do problema convertido] do projeto ou tarefa. Se o [!UICONTROL Contato Principal] do problema for atualizado depois que o problema for convertido, o [!UICONTROL Originador do Problema Convertido] será preservado como o [!UICONTROL Contato Principal] do problema no momento em que a conversão ocorrer. Consulte também "[!UICONTROL Originador de problema convertido]" neste artigo.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Prioridade]</td> 
   <td>Um valor que pode ser atribuído a uma tarefa, problema ou projeto para designar a importância dele. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Privado]</td> 
   <td>Em uma [!UICONTROL Note] ou [!UICONTROL Document], essa opção torna esse objeto oculto para a maioria dos visualizadores. Para uma Fila de solicitação de ajuda privada, somente os usuários na Equipe do projeto podem enviar problemas para essa fila (ou projeto) por meio da área [!UICONTROL Solicitações].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Perfil]</td> 
   <td>Todas as informações sobre uma conta de usuário.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Programa]</td> 
   <td> <p>Um subconjunto em um portfólio, em que projetos semelhantes podem ser agrupados para alcançar um benefício bem definido.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gerenciamento de Programas]</td> 
   <td>Gerenciamento de dependências entre projetos, riscos, problemas, requisitos e soluções para manter a integridade do programa e obter os benefícios definidos do programa.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Proprietário de Programa]</td> 
   <td>A parte interessada responsável por supervisionar e organizar atividades para garantir que as metas do projeto se alinhem aos objetivos da empresa.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progresso]</span> </td> 
   <td> <p>Em um relatório de [!UICONTROL Meta], é exibida a porcentagem de quão perto uma meta estratégica está de ser concluída. A porcentagem do progresso é exibida como um número. Para obter informações sobre metas estratégicas, consulte também "[!UICONTROL Meta]" nesta tabela.</p> <p>Este campo só estará visível se sua organização tiver comprado [!DNL Workfront] Metas. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Adicionar projetos a metas no [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status de Progresso]</td> 
   <td> <p>Em um relatório de Projeto, Tarefa e Meta, esse campo exibe o Status do Andamento dos projetos, tarefas ou metas estratégicas. Para obter mais informações, consulte os seguintes artigos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Visão geral do Status de Progresso do Projeto</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Visão geral do status de progresso da tarefa</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Visão geral do progresso e da condição da meta em [!DNL Adobe Workfront Goals]</a> </p>
     <p>O relatório [!UICONTROL Goal] e o [!UICONTROL Progress Status] para o campo [!DNL goals] só estarão visíveis se sua organização tiver comprado [!DNL Workfront Goals]. Para obter informações sobre metas estratégicas em [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] visão geral</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Projeto]</td> 
   <td> <p>Uma grande quantidade de trabalho que deve ser concluída dentro de um período específico e deve usar um orçamento e número de recursos específicos. Para torná-lo gerenciável, divida o projeto em uma série de tarefas. Concluir todas as tarefas resulta na conclusão do projeto. Para obter informações sobre o planejamento de um projeto, consulte <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Planejar uma visão geral do projeto</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Horas Planejadas de Atribuição de Projeto]</td> 
   <td> <p>Em um relatório de [!UICONTROL Função de Trabalho da Iniciativa], é exibido o número de [!UICONTROL Horas Planejadas] associado a uma função de trabalho atribuída a tarefas ou problemas no projeto. Este campo e o tipo de relatório da [!UICONTROL Função de Trabalho da Iniciativa] não são exibidos na instância [!DNL Workfront], a menos que a empresa tenha comprado uma licença [!DNL Workfront Scenario Planner]. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">A visão geral</a> de [!DNL Workfront Scenario Planner]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Detalhes do Projeto]</td> 
   <td>Os detalhes do status atual de um Projeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo orçado do projeto]</td> 
   <td> <p> Este é o [!UICONTROL Custo Orçado] de um projeto como ele é exibido em listas e relatórios.</p><p>Consulte também "[!UICONTROL Custo Orçado]" neste artigo.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gerenciamento de Projeto]</td> 
   <td>Um conjunto de políticas que regem os limites para criação de projetos, categorização e nomenclatura dos projetos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Sobrecarga de Projeto]</td> 
   <td>Em um relatório [!UICONTROL Hour], esse campo é reservado para informações financeiras vinculadas às horas registradas com o tipo de hora do [!UICONTROL Project Time]. Os projetos podem ter suas próprias taxas de cobrança e, se uma hora for registrada diretamente em um projeto, essas taxas serão usadas nos cálculos. Com base nas configurações do projeto, os projetos também podem ter moedas diferentes e pode haver uma conversão de moeda para essas horas. O objeto [!UICONTROL Project Overhead] permite que [!DNL Workfront] obtenha essas informações.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proprietário do Projeto]</td> 
   <td>O usuário responsável pelo gerenciamento do escopo, linha do tempo e atribuições de um projeto. O aprovador padrão para ordens de alteração, alterações financeiras e materiais para distribuição.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planejamento de Projeto]</td> 
   <td>Processos para desenvolver e manter o cronograma do projeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Patrocinador de Projeto]</td> 
   <td>Um perfil de parte interessada designado com o qual cada usuário deve se relacionar. Em [!DNL Workfront], eles são designados como [!UICONTROL Níveis de Acesso]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Equipes de Projeto]</td> 
   <td> <p>A coleção de usuários ou funções atribuídos a um projeto</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Visão geral da Equipe do Projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rastreamento de projeto]</td> 
   <td>Os dados usados para medir a integridade e o escopo de um projeto</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projetado]</td> 
   <td> <p>Uma estimativa do carimbo de data e hora de quando o trabalho será concluído com base nas horas planejadas e na porcentagem concluída de uma tarefa, problema ou projeto.</p> <p>Refere-se às datas ou à [!UICONTROL Duração] de tarefas, problemas ou projetos. Normalmente, ela designa datas e durações mais verdadeiras à vida útil dos itens de trabalho, depois que algum trabalho já foi concluído ou algum tempo passou. </p> <p>Por exemplo, a [!UICONTROL Data de Conclusão Projetada] de uma tarefa é a data em que [!DNL Workfront] estima que a tarefa será concluída, com base em quanto trabalho foi feito até agora, quantas pessoas estão atribuídas a ela e quanto tempo passou desde a data de início.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Prazo de Prova]</td> 
   <td> <p>Em relatórios que contêm o objeto [!UICONTROL Versão do documento] (como um relatório [!UICONTROL Versão do documento] e um relatório [!UICONTROL Aprovação da prova]), esse campo exibe o dia da semana, a data, a hora do dia e o ano do prazo de prova.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisão de Prova]</td> 
   <td> <p>Em relatórios que contêm o objeto [!UICONTROL Versão do Documento] (como um relatório [!UICONTROL Versão do Documento])  e [!UICONTROL Aprovação de Prova]), esse campo exibe o status de decisão da prova (pendente, alterações necessárias ou aprovado)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da Prova]</td> 
   <td> <p>Em relatórios que contêm o objeto [!UICONTROL Versão do Documento] (como um relatório [!UICONTROL Versão do Documento] e um relatório [!UICONTROL Aprovação de Prova]), esse campo exibe o nome da prova.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Páginas de Prova]</td> 
   <td> <p>Em relatórios que contêm o objeto [!UICONTROL Versão do Documento] (como um relatório [!UICONTROL Versão do Documento] e um relatório [!UICONTROL Aprovação de Prova]), esse campo exibe o número de páginas incluídas na prova.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progresso de Prova]</td> 
   <td> <p>Em relatórios que contêm o objeto [!UICONTROL Versão do Documento] (como um relatório [!UICONTROL Versão do Documento] e um relatório [!UICONTROL Aprovação da Prova]), exibe o status do progresso da prova ([!UICONTROL Enviado], [!UICONTROL Aberto], [!UICONTROL Comentado], [!UICONTROL Decisão Tomada]).</p> <p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Visão geral do progresso da prova</a> em <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Visão geral do progresso e do status da prova</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Prova]</td> 
   <td>Um processo de revisão no qual um ou mais usuários marcam e comentam o conteúdo que deve ser alterado em uma imagem, um documento de texto, um vídeo ou conteúdo interativo da Web.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Público]</td> 
   <td>Em uma [!UICONTROL Observação] ou [!UICONTROL Documento], essa opção torna esse objeto acessível a outros usuários ou até mesmo a pessoas de fora do [!DNL Workfront]. Para uma [!UICONTROL Fila de Solicitações de Ajuda], [!UICONTROL Público] significa que todos os usuários que podem enviar problemas a um projeto podem enviá-los por meio da área [!UICONTROL Solicitações].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Qualidade]</td> 
   <td>A percepção da qualidade do trabalho na organização.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fila]</td> 
   <td>Também chamada de Fila de Help Desk ou [!UICONTROL Fila de solicitação de ajuda]. Este é um projeto que foi publicado na área [!UICONTROL Solicitações] para permitir que os usuários enviem problemas para ele. Normalmente, filas são criadas para tópicos específicos, como [!UICONTROL Bugs], [!UICONTROL Solicitações de Projeto], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propriedades da Fila]</td> 
   <td>Essas configurações definem regras de envio de problemas para um projeto que está sendo publicado na área [!UICONTROL Solicitações].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tópico de Fila]</td> 
   <td> <p>Uma propriedade em uma [!UICONTROL Fila de solicitação de ajuda] que permite que os usuários enviem um problema para selecionar um Tópico. Os tópicos podem:</p> 
    <ul> 
     <li>Ser associado a um Formulário de Dados Personalizado.</li> 
     <li>Atribua a ocorrência automaticamente a um usuário, função ou equipe por meio do conjunto de Regras de Encaminhamento no Tópico selecionado.</li> 
     <li>Mova o problema para um projeto ou fila diferente por meio do conjunto de regras de roteamento no tópico selecionado.</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Criar tópicos da fila</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Classificação]</td> 
   <td> <p>Em um relatório de [!UICONTROL Nível de Acesso], você pode indicar manualmente uma [!UICONTROL Classificação] do [!UICONTROL Nível de Acesso]. Isso o ajuda, como administrador do [!DNL Workfront], a identificar visualmente o nível de complexidade associado a cada Nível de Acesso. Por exemplo, você pode fornecer números mais baixos para Níveis de Acesso mais complexos ([!UICONTROL Plano] nível) e números mais altos para Níveis de Acesso menos complexos ([!UICONTROL Solicitante] nível). Não é possível classificar os Níveis de Acesso padrão. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pronto]</td> 
   <td> <p>Este campo em um relatório de tarefa indica se uma tarefa [!UICONTROL Agile] foi marcada como [!UICONTROL Ready] na lista de pendências. Esse sinalizador se aplica somente a tarefas do [!UICONTROL Agile], que são tarefas atribuídas a uma equipe do [!UICONTROL Agile]. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Registro]</td> 
   <td> <p>No Workfront Planning, um registro é uma instância exclusiva de um tipo de registro.</p>
<p>Depois de adicionar um tipo de registro a um espaço de trabalho, você pode começar a adicionar registros desse tipo na página do tipo de registro.</p>
<p>Por exemplo, "Campanha" pode ser um tipo de registro e "Campanha de verão para EMEA" é um registro do tipo de registro Campanha.</p>
<p>Para obter informações sobre como criar registros, consulte <a href="/help/quicksilver/planning/records/create-records.md">Criar registros</a>. </p> <p>O Workfront Planning exige uma licença adicional. </p></td> 
  </tr>


<tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>O tipo de objeto do Workfront Planning.</p>
<p>Diferentemente do Workfront, onde os tipos de objeto são predefinidos, no Workfront Planning você pode criar seus próprios tipos de objeto. Os tipos de objeto do Workfront Planning são chamados de tipos de registro.</p>
<p>Por exemplo, no Workfront, os tipos de objeto de Programa, Portfolio, Projeto, Tarefa ou Problema já foram criados.</p>
<p>No Workfront Planning, é possível criar qualquer tipo de registro que atenda aos workflows da organização. Posteriormente, é possível definir como os tipos de registro se relacionam entre si ou as dependências do formulário.</p> Para obter informações sobre como criar tipos de registro, consulte <a href="/help/quicksilver/planning/architecture/create-record-types.md">Criar tipos de registro</a>. </p> <p>O Workfront Planning exige uma licença adicional. </p></td> 
  </tr>

<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Frequência de Recorrência]</td> 
   <td> <p>Um campo exibido na caixa [!UICONTROL Detalhes da Tarefa] ou [!UICONTROL Editar Tarefa] de um pai de tarefas recorrentes. É a frequência com que as tarefas na recorrência ocorrem. Para obter informações sobre como criar tarefas recorrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Criar tarefas recorrentes</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número de Referência]</td> 
   <td> <p>Projetos, tarefas e problemas são associados automaticamente a um número de referência exclusivo à medida que são criados. Você pode exibir o [!UICONTROL Número de Referência] na página [!UICONTROL Detalhes] de projetos, tarefas ou problemas, ou em uma lista ou relatório. </p> <p><b>DICA</b><p><br>É possível adiar para números de referência quando dois itens têm o mesmo nome, pois os números de referência são sempre exclusivos. </p> <p>[!DNL Workfront] O gera automaticamente números de referência sequenciais no nível do sistema. Cada projeto, tarefa ou problema recebe o próximo número disponível na sequência. <br></p> <p>Por exemplo, se o Usuário A criar uma tarefa, [!DNL Workfront] poderá atribuir automaticamente a tarefa o Número de Referência 100. Se o Usuário B criar um problema logo após isso, [!DNL Workfront] atribuirá o problema ao Número de Referência 101. Não é possível editar manualmente os Números de Referência. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema de Rejeição]</td> 
   <td>Em um relatório de projeto ou de tarefa, esse é o problema criado quando a aprovação do projeto ou da tarefa é rejeitada. Para obter informações sobre problemas de rejeição, consulte o artigo <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Criar um processo de aprovação para itens de trabalho</a>. </td> 
  </tr>

<tr>
  <td>Tipos de relacionamento</td>
  <td><p>Os objetos do Workfront são sempre conectados uns aos outros usando um dos seguintes tipos de relacionamento:</p>

<ul><li> <b>De um para muitos</b>: nesta relação, um objeto pode ser conectado a vários outros objetos de tipos diferentes. Por exemplo, um projeto pode ter várias tarefas. A relação projeto-tarefas é uma relação um para muitos. Não é possível exibir essa relação em um relatório usando a interface Padrão. Você deve usar os relatórios do modo de texto para exibir relações de um para muitos.</li>
  <li><b>Um para um</b>: nesta relação, um objeto só pode ser conectado a outro objeto de um tipo diferente. Por exemplo, um projeto só pode ter um Grupo. A relação Projeto-Grupo é uma relação um para um. Você pode exibir relações um para um entre objetos em um relatório Padrão.</li>
  <li><b>De muitos para um</b>: nesta relação, vários objetos podem ser conectados somente a um outro objeto de um tipo diferente. Por exemplo, várias tarefas podem ser conectadas ao mesmo projeto. A relação tarefas-projeto é uma relação muitos para um. Você pode exibir relações muitos para um entre objetos em um relatório Padrão. </li>
  <li><b>Muitos para muitos</b>: nesta relação, vários objetos do mesmo tipo podem ser conectados a vários objetos de um tipo diferente. Por exemplo, vários usuários podem pertencer a várias Outras equipes, e as equipes podem pertencer a vários usuários. Não é possível exibir essa relação em um relatório usando a interface Padrão. Você deve usar os relatórios do modo de texto para exibir relacionamentos muitos para muitos. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Custo de Risco Restante]</td> 
   <td> <p>Um campo de projeto que mostra a diferença entre o [!UICONTROL Custo de Risco Planejado] de um projeto e o total de todos os [!UICONTROL Custos Reais] de todos os riscos do projeto. </p> <p>O [!UICONTROL Custo de Risco Restante] de um projeto é calculado usando a seguinte fórmula:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Replanejamento]</td> 
   <td>Alterar as datas de um projeto para reparar ou superar problemas. Por exemplo, um projeto que esteve suspenso por vários meses precisaria ser replanejado para refletir datas precisas. Esta é uma operação manual para ajustar as datas do projeto ou as datas das tarefas. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Relatório]</td> 
   <td>Um gráfico ou tabela que contém informações sobre um determinado objeto [!DNL Workfront] e seus atributos relacionados.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Solicitação]</td> 
   <td> <p>Um tipo de problema que é colocado em uma única fila centralizada e não está relacionado a um esforço de trabalho em andamento.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Fila de Solicitações]</td> 
   <td>O backlog de problemas gerenciado por um processo de tráfego e triagem.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Solicitar velocidade]</td> 
   <td>Tempo total do ciclo de trabalho para entrada e conclusão de uma solicitação.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Solicitante]</td> 
   <td>Normalmente, é um tipo de licença. Um usuário com uma licença de Solicitante pode enviar solicitações para que um novo trabalho ocorra no sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo Reservado]</td> 
   <td>Dias especificados no Tempo pessoal do usuário, indicando que o usuário não estará disponível para trabalho. Consulte "[!UICONTROL Dias Não Úteis]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver Problema]</td> 
   <td> <p>Em um relatório de problemas, use esse campo em exibições ou filtros para se referir ao problema que resolve o problema. </p> <p>Para obter informações sobre como exibir objetos de resolução em relatórios, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Exibir informações sobre Objeto Resolvível e de Resolução em um relatório</a> em <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral de Objetos Resolvíveis e de Resolução </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver Projeto]</td> 
   <td> <p>Em um relatório de problemas, use esse campo em exibições ou filtros para se referir ao projeto que resolve o problema. </p> <p>Para obter informações sobre como exibir objetos de resolução em relatórios, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Exibir informações sobre Objeto Resolvível e de Resolução em um relatório</a> em <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral de Objetos Resolvíveis e de Resolução </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver Tarefa]</td> 
   <td> <p>Em um relatório de problemas, use esse campo em exibições ou filtros para se referir à tarefa que resolve o problema. </p> <p>Para obter informações sobre como exibir objetos de resolução em relatórios, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Exibir informações sobre Objeto Resolvível e de Resolução em um relatório</a> em <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral de Objetos Resolvíveis e de Resolução </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurso]</td> 
   <td>Usuários ou funções que existem em [!DNL Workfront] e são atribuídos a Equipes de Projeto, tarefas e problemas. Eles são responsáveis por concluir o trabalho associado a projetos, tarefas ou problemas. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Gerenciamento de Recursos]</td> 
   <td> <p>O [!UICONTROL Gerenciamento de Recursos] é um conjunto de ferramentas corporativas que permite prever com precisão o uso dos recursos com base em sua disponibilidade, de forma que o trabalho necessário seja concluído no prazo e dentro do orçamento. </p> <p>Com as ferramentas de Gerenciamento de recursos, você pode planejar a capacidade a longo prazo e as necessidades de programação a curto prazo para seus recursos. </p> <p>Para obter informações sobre o Gerenciamento de Recursos no [!DNL Workfront], consulte <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introdução ao Gerenciamento de Recursos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL IDs do Gerenciador de Recursos]</td> 
   <td><p>Em um relatório de projeto, você pode usar essa opção ao criar um filtro para localizar um gerenciador de recursos específico. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gerentes de Recursos]</td> 
   <td> <p>Em um relatório de projeto ou exibição de lista, este é um campo informativo que mostra os usuários designados para executar atividades de gerenciamento de recursos no projeto.  Quando você usa "" em um relatório, uma lista de gerenciadores de recursos é exibida, com cada gerenciador de recursos no projeto separado por vírgula. Você pode designar até 30 gerentes de recursos em um determinado projeto.</p> <p>Para obter mais informações, consulte o artigo <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Designar Gerentes de Recursos para um projeto ou modelo </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Planejador de recursos Horas Orçadas] </td> 
   <td>As horas orçadas para o projeto e os recursos associados a ele no [!UICONTROL Resource Planner]. Consulte também "[!UICONTROL Horas Orçadas]" neste artigo. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Planejador de Recursos] </td> 
   <td>Uma ferramenta avançada do [!DNL Workfront] que permite exibir e gerenciar recursos entre projetos, funções de trabalho ou usuários. Para obter informações, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Visão geral do Planejador de recursos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planejador de recursos Custo do trabalho orçado]</td> 
   <td> <p>Este é o custo associado às horas orçadas para as funções de trabalho do projeto que usam o Planejador de recursos. </p> <p>Consulte também "Custo do trabalho orçado" neste artigo. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Conjuntos de Recursos]</td> 
   <td> <p>Conjuntos de recursos são coleções de usuários que podem ser associados a um projeto. Os usuários no mesmo Conjunto de recursos geralmente pertencem ao mesmo departamento, têm habilidades semelhantes ou complementares ou são financiados pelo mesmo orçamento. Você pode associar vários Conjuntos de recursos a um projeto ou a um usuário. Um conjunto de recursos pode ser atribuído exclusivamente a um projeto ou compartilhado por vários projetos.</p> 
   <p>Para obter mais informações sobre pools de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Visão geral dos pools de recursos </a>.</p> 
   <p>Nos relatórios de projetos, os Conjuntos de recursos mostram todos os conjuntos associados a um projeto. Este objeto não pode ser usado em um agrupamento.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilização de Recursos]</td> 
   <td>Um Relatório que exibe o número de horas disponíveis durante um determinado período e o número de horas agendadas para cada usuário no relatório. Isso também é calculado em [!UICONTROL Average Hours Per Day] e uma porcentagem de alocação.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Resultado]</td> 
   <td>Em [!DNL Workfront Goals], um resultado é um indicador de progresso para uma meta. Pode ser um número, um valor percentual ou um valor de moeda que você atualiza manualmente. Não é possível exibir resultados em um relatório e você não pode acessá-los por meio da API [!DNL Workfront]. Para obter informações sobre atividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introdução a resultados e atividades nas Metas do Adobe Workfront</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Receita]</td> 
   <td>Uma quantia faturável para a tarefa ou projeto. A quantidade pode ser por hora, fixa ou uma combinação de ambos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Receita]</td> 
   <td>O tipo de receita determina como a tarefa acumulará receita. Alguns exemplos incluem [!UICONTROL Horas Fixas], [!UICONTROL Função Horas por Hora] e [!UICONTROL Função Horas por Hora c/Cap]. Para obter informações sobre o rastreamento da receita em [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão Geral de Faturamento e Receita</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revisor]</td> 
   <td>Normalmente, é um tipo de licença. Um usuário com uma licença de [!UICONTROL Reviewer] pode revisar e aprovar itens de trabalho no sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risco]</td> 
   <td> <p>Isso pode se referir aos seguintes conceitos em [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>Um campo em um projeto que indica o risco que um projeto pode ter. Você pode priorizar a execução de seus projetos com base no nível de risco. Os projetos podem ter os seguintes níveis de risco:</p> <p>- [!UICONTROL Muito Baixo]</p> <p>- [!UICONTROL Baixo]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL Alto]</p> <p>- [!UICONTROL Muito Alto]</p> <p>Os níveis de riscos que você indica para um projeto não podem ser personalizados. </p> <p> Para obter informações sobre como atualizar o Risco de um projeto, consulte a seção "Configurações do Projeto" do artigo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar projetos</a>. É possível exibir o campo de risco de um projeto em relatórios. </p> </li> 
     <li> <p>Um evento que pode ocorrer durante a vida útil de um projeto e que identifica um impacto potencial no custo, escopo ou programação do projeto. Você define riscos potenciais para um projeto e associa uma probabilidade de ocorrência ou um custo à medida que cria o Business Case do projeto. Para obter informações sobre como adicionar riscos ao Business Case do projeto, consulte "Criar e editar riscos em projetos". </p> <p>Não é possível exibir riscos definidos no [!UICONTROL Business Case] nos relatórios. Você só pode exibir vários tipos de Custos de Risco em relatórios e listas. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custo de Risco]</td> 
   <td> <p>O custo associado aos riscos em um projeto. A seguir estão os custos de risco associados aos projetos que você pode exibir nos relatórios:</p> 
    <ul> 
     <li> <p>[!UICONTROL Custo Real]: um campo em um risco que mostra o custo real do risco que ocorreu. Além de relatórios e listas, é possível localizá-los na caixa [!UICONTROL Editar Risco] ao editar ou criar um risco. </p> <p>Para custos de projetos, tarefas ou problemas, consulte "[!UICONTROL Custo Real]" neste artigo. </p> </li> 
     <li> <p>[!UICONTROL Custo de Risco Planejado]: um campo no projeto que mostra um total de todos os [!UICONTROL Custos de Risco Potenciais] do projeto. Consulte também "[!UICONTROL Custo de Risco Planejado]" neste artigo. </p> <p>Para obter informações sobre Custo de Risco Potencial, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular Custo de Risco Potencial </a>. </p> </li> 
     <li> <p>[!UICONTROL Custo de Risco Restante]: um campo no projeto que exibe a diferença entre o total dos [!UICONTROL Custos Reais] de todos os riscos e o [!UICONTROL Custo de Risco Planejado]. Consulte também "Custo de risco restante" neste artigo. </p> </li>
    </ul> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Gerenciamento de Riscos]</td> 
   <td>Processos para identificar, reduzir e monitorar o risco.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Função]</td> 
   <td>Consulte "[!UICONTROL Função de trabalho]" neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Roteamento]</td> 
   <td>Atribuição ou movimentação automática de um problema, geralmente devido a um Tópico da Fila ou por ser a Rota Padrão (Regra de Roteamento) para a fila.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Regra de Roteamento]</td> 
   <td>Uma configuração em projetos e tópicos de fila que atribui automaticamente um problema a um usuário, função ou equipe, ou move o problema para outro projeto ou tópico de fila. As Regras de Encaminhamento geralmente são usadas com as Filas de Solicitações de Ajuda para atribuir automaticamente os problemas recebidos.</td> 
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
   <td>[!UICONTROL Pesquisa Salva]</td> 
   <td>Uma pesquisa para a qual os critérios de pesquisa foram salvos. As Pesquisas salvas facilitam a execução das mesmas novamente sem precisar inserir os critérios de pesquisa novamente.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Cenário] (em [!DNL Workfront Fusion]) </td> 
   <td> <p>Um cenário é composto por uma série de etapas (módulos) que indicam como os dados devem ser transferidos e transformados entre aplicativos/serviços.</p> <p>Para obter informações sobre cenários em [!DNL Workfront Fusion], consulte <a href="https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview">[!DNL Adobe Workfront Fusion] visão geral do cenário</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cenário] (no [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>No [!DNL Scenario Planner], um cenário é uma cópia de um plano. </p> <p>O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">A visão geral</a> de [!DNL Scenario Planner]. </p> <p>Para obter informações sobre como criar cenários, consulte <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Criar e comparar cenários de planejamento no [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Agenda]</td> 
   <td>A programação de trabalho semanal, incluindo horários de trabalho, combinada com Dias de folga (como Feriados) e dias de exceção (como um dia de trabalho de sábado). Você pode associar cronogramas a projetos e usuários.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Isenção de Agendamento]</td> 
   <td>Também conhecido como [!UICONTROL Modified Shift]. Dias programados, em contraste com os horários de trabalho semanais regulares, conforme definidos pelo horário. Por exemplo, um sábado agendado para funcionar, quando o Agendamento estiver configurado para trabalhar somente de segunda a sexta-feira, seria uma [!UICONTROL Isenção de agendamento].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Relatório Agendado]</td> 
   <td> <p>Ao criar um relatório de relatórios, você pode exibir informações sobre os agendamentos do relatório, se ele estiver agendado para entrega usando o campo [!UICONTROL Relatório Agendado]. Este campo mostra vários valores, um para cada agendamento de cada relatório, em uma lista com marcadores. Para obter mais informações sobre o agendamento de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Visão geral da entrega de relatórios</a>.</p> <p>Como esse campo mostra vários valores, ele não pode ser usado em um agrupamento. Você pode acessá-lo somente em um filtro ou em uma visualização. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alteração de Escopo]</td> 
   <td>Uma [!UICONTROL Trilha de Auditoria] que, se estiver ativa, gera uma observação sempre que uma alteração for feita no Escopo de um projeto ou tarefa, como quando uma [!UICONTROL Duração da Tarefa] ou os [!UICONTROL Predecessores] são alterados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seção]</td> 
   <td>Uma área na tela, com seu próprio cabeçalho, criada para organizar os Dados personalizados para fins de exibição.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quebra de Seção]</td> 
   <td>Uma lacuna ou borda entre seções.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Segurança]</td> 
   <td>As configurações que permitem que um usuário interaja com determinados objetos no sistema e não com outros. Consulte também "[!UICONTROL Níveis de Acesso]" neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Instalação]</td> 
   <td>A área em que os administradores podem definir as configurações e preferências do sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gravidade]</td> 
   <td> <p>[!UICONTROL Gravidade] é uma indicação da probabilidade de um item afetar a conclusão do trabalho. Por exemplo, um problema com alta [!UICONTROL Gravidade] pode bloquear completamente a conclusão de uma tarefa, mas um problema com baixa [!UICONTROL Gravidade] pode ser meramente superficial.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Atualizar gravidade do problema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severidades]</td> 
   <td>Consulte "[!UICONTROL Gravidade]" neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Compartilhamento]</td> 
   <td>A ação de permitir que outros usuários exibam ou editem um item específico em [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data do Slack]</td> 
   <td>Em uma exibição de tarefa ou relatório, a [!UICONTROL Data de Slack] exibe a data exata em que uma tarefa poderia definitivamente afetar a [!UICONTROL Data de conclusão] do projeto. Para obter informações sobre a [!UICONTROL Data Slack] de uma tarefa, consulte <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Visão geral da Data Slack da Tarefa</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atribuições Inteligentes]</td> 
   <td> <p>Ao atribuir tarefas ou problemas a usuários, o [!DNL Workfront] faz recomendações ([!UICONTROL Atribuições Inteligentes]) sobre quem são os melhores usuários para concluir o trabalho, com base no tempo disponível para concluí-lo e sua relação com o projeto.</p> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Visão geral das atribuições inteligentes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Indica o objeto pai de outro objeto. Por exemplo, um documento anexado a uma tarefa tem o nome da tarefa no campo [!UICONTROL Source] de um relatório ou exibição [!UICONTROL Document]; um problema registrado em um projeto tem o nome do projeto no campo [!UICONTROL Source] de um relatório ou exibição de Problema. </p> 
   <p>Os relatórios a seguir exibem uma coluna Source, na qual você pode exibir informações sobre o objeto pai:</p>
  <ul><li>Relatórios de problemas</li>
    <li>Relatórios de horas</li>
    <li>Relatórios de documentos </li>
    </ul>
   <p>Se os usuários não tiverem permissões para o objeto principal de um problema, hora ou documento, a coluna Source do relatório será exibida vazia, mesmo quando o relatório estiver configurado para exibição ou para ser entregue com os direitos de acesso de outro usuário. </p>
   <p> Para mostrar informações sobre o objeto pai no relatório, recomendamos adicionar uma coluna para o objeto pai, onde você pode exibir o nome do objeto pai. </p>
    <p>Por exemplo, você pode adicionar qualquer um dos itens a seguir a um relatório com uma coluna Source: </p>
    <ul><li>As colunas Nome do projeto, Nome da tarefa ou Nome do problema em um documento ou relatório de horas.</li>
    <li>As colunas Nome do projeto ou Nome da tarefa para um relatório de problemas. </li> </ul>
    Para obter mais informações, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Executar e entregar um relatório com direitos de acesso de outro usuário</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de Início]</td> 
   <td> <p>A Data em que o trabalho em um item está definido para iniciar. Há várias Datas de Início em [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Planejado]</li> 
     <li>[!UICONTROL Real]</li> 
     <li>[!UICONTROL Projetado] </li> 
    </ul> <p>Em um [!UICONTROL Rate report], esta é a data em que uma nova taxa de cobrança para uma função de trabalho no nível do projeto começa. As horas associadas ao projeto que estão após essa data são multiplicadas por essa taxa de faturamento para calcular a receita no projeto. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Um indicador usado para sinalizar uma posição de fluxo de trabalho de um item de trabalho ou de uma meta estratégica.</p> <p>Para projetos, o [!UICONTROL Status] é uma configuração no projeto que indica se o projeto é:</p> 
    <ul> 
     <li>[!UICONTROL Atual]</li> 
     <li>[!UICONTROL Em Espera] </li> 
     <li>[!UICONTROL Concluído] </li> 
     <li>[!UICONTROL Desativado]</li> 
    </ul> <p>Para obter mais informações sobre o Status de um projeto, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Acessar a lista de status de projetos do sistema</a>.</p>
    <p>Para tarefas, o [!UICONTROL Status] é uma configuração na tarefa que indica se a tarefa é:</p> 
    <ul> 
     <li>[!UICONTROL Novo]</li> 
     <li>[!UICONTROL Em Andamento]</li> 
     <li>[!UICONTROL Concluído]</li> 
    </ul> <p>Para obter mais informações sobre o Status da tarefa, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Acessar a lista de status de tarefa do sistema</a></p> <p>Para problemas, o [!UICONTROL Status] é uma configuração no problema que indica se esse problema é:</p> 
    <ul> 
     <li>[!UICONTROL Novo]</li> 
     <li>[!UICONTROL Em Andamento]</li> 
     <li>[!UICONTROL Aguardando Comentários]</li> 
     <li>[!UICONTROL Em Espera]</li> 
     <li>[!UICONTROL Resolvido]</li> 
     <li>[!UICONTROL Não Resolverá]</li> 
     <li>[!UICONTROL Não Pode Duplicar]</li> 
     <li>[!UICONTROL Confirmado Concluído]</li> 
     <li>[!UICONTROL Reaberto]</li> 
    </ul> <p>Para obter mais informações sobre Status de Problemas, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acessar a lista de status de problemas do sistema</a>.</p> 
    <p>Para metas estratégicas, o [!UICONTROL Status] é uma configuração na meta que indica se a meta é:</p> 
     <ul> 
      <li>[!UICONTROL Ativo]</li> 
      <li>[!UICONTROL Rascunho]</li> 
      <li>[!UICONTROL Inativo]</li> 
      <li>[!UICONTROL Fechado]</li> 
     </ul> 
     <p>Para obter mais informações sobre metas estratégicas, consulte também "[!UICONTROL Meta]" ou "[!UICONTROL Metas]" neste artigo. </p> 
     <p>Para metas estratégicas, este campo estará visível somente se sua organização tiver comprado o [!DNL Workfront Goals]. Para obter informações sobre como gerenciar metas estratégicas usando o [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] visão geral</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alteração de Status]</td> 
   <td>Uma [!UICONTROL trilha de auditoria]. Uma nota é gerada quando um usuário altera o Status do projeto, tarefa ou problema.</td> 
  </tr> 
  <tr> 
   <td>Ícones de Status</td> 
   <td> <p>Você pode adicionar o campo [!UICONTROL Status Icons] interno como uma coluna em suas visualizações para melhorar a visibilidade em pontos-chave sobre seus objetos, como:</p> 
    <ul> 
     <li>Um objeto tem documentos anexados</li> 
     <li>Um objeto está associado a um processo de aprovação</li> 
     <li>Um objeto tem observações adicionais associadas a ele</li> 
     <li>Uma despesa é faturável ou reembolsável </li> 
     <li>Uma tarefa está em um caminho crítico</li> 
     <li>Um usuário pertence a uma empresa, equipe ou está localizado em um fuso horário diferente </li> 
    </ul> <p>Você pode adicionar o campo [!UICONTROL Ícones de Status] nas exibições dos seguintes objetos: </p> 
    <ul> 
     <li>[!UICONTROL Tarefas]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Projetos]</li> 
     <li>[!UICONTROL Modelos de Tarefa]</li> 
     <li>[!UICONTROL Modelos]</li> 
     <li>[!UICONTROL Despesas]</li> 
     <li>[!UICONTROL Documentos]</li> 
     <li>[!UICONTROL Usuários]</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ícones de Status Internos em Exibições</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atualização de Status]</td> 
   <td> <p>Em um relatório de projeto, tarefa ou problema, este campo mostra a atualização de status mais recente que os proprietários do objeto forneceram na área '[!UICONTROL Atualizações]'. Para projetos, isso significa que os comentários feitos pelo Proprietário do projeto e, para tarefas e problemas, significa que os comentários feitos pelos atribuídos.</p> 
   <p> Comentários feitos ao atualizar o status de um objeto não são exibidos na coluna [!UICONTROL Atualização de Status].</p> <p>Para mostrar os status '[!UICONTROL New],' '[!UICONTROL In Process],' e '[!UICONTROL Complete]', use a coluna [!UICONTROL Status].</p> <p>Para obter mais informações sobre status, consulte o artigo <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Atualizar status da tarefa</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td>Consulte "[!UICONTROL Status]" neste artigo.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Um gráfico que representa o status das histórias (tarefas na metodologia ágil) e como elas estão progredindo em direção à conclusão.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>Uma métrica usada para medir a dificuldade ou a complexidade de uma história. As equipes Agile podem escolher se desejam usar Horas ou Pontos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Pontos de História]</td> 
   <td>Uma métrica usada para medir a dificuldade ou a complexidade de uma história. As equipes Agile podem escolher se desejam usar Horas ou Pontos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Estratégico]</td> 
   <td>Trabalho de longo prazo que altera a organização ou como ela funciona.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Alinhamento Estratégico]</td> 
   <td>Medir e alinhar metas da empresa em portfólios e programas.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Isso é usado nas colunas do relatório ao usar a interface do Modo de texto. </p>
   <p>O <code>[!UICONTROL stretch]</code> é usado para identificar quais colunas ocupam espaço extra não necessário para a exibição. A largura da interface do usuário do espaço de trabalho para um usuário típico é de cerca de 850 pixels. Isso significa que, se você tiver uma visualização com quatro
   colunas (150 pixels cada) em que a visualização ocupa 600 de 850 pixels. Há 250 pixels extras na interface do usuário que serão adicionados às colunas com uma porcentagem de ampliação fornecida. </p>
   <p>O alongamento de uma coluna é aplicado quando você usa a linha de código adicional: <code>[!UICONTROL usewidths=true]</code> para pelo menos uma das colunas na exibição. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Assinantes]</td> 
   <td> <p>Usuários que assinam projetos, tarefas ou problemas.</p> <p>Quando você usa esse campo em um relatório, uma lista de assinantes é exibida, com cada assinante separado por vírgula.</p> <p>Para obter mais informações, consulte o artigo <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Assinar itens em [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa Resumo]</td> 
   <td>Consulte "[!UICONTROL Tarefa pai]" neste artigo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtarefa]</td> 
   <td>Uma tarefa filho, localizada em uma tarefa pai.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Governança do Sistema]</td> 
   <td>Um conjunto de políticas que controla as alterações e a manutenção de um sistema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Integração do Sistema]</td> 
   <td>Processo que consiste em ligar, física ou funcionalmente, diferentes sistemas informáticos e diferentes aplicações informáticas, a fim de atuar como um todo coordenado.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Tarefa]</td> 
   <td> <p>Uma atividade que deve ser executada como uma etapa para atingir uma meta final (concluir o projeto).</p>

<p>As tarefas são unidades de trabalho menores que concluem um projeto, o que representa uma unidade de trabalho maior.</p>
   <p>Tarefas nunca podem existir independentemente. Eles sempre fazem parte de um projeto. </p>
   <p>Para obter mais informações sobre tarefas, consulte <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Visão geral das tarefas</a>.</p> 
   <p>Para obter informações sobre como criar tarefas, consulte <a href="/help/quicksilver/manage-work/tasks/create-tasks/create-tasks-in-project.md">Criar tarefas em um projeto</a>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atributo de Tarefa]</td> 
   <td>Outros campos ou objetos associados a uma tarefa e indicam determinados detalhes sobre a tarefa. Alguns exemplos são [!UICONTROL Data de conclusão planejada] e [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Restrição de Tarefa]</td> 
   <td>Consulte "[!UICONTROL Tipo de restrição]" e "[!UICONTROL Data de restrição]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gerenciamento de Tarefas]</td> 
   <td>Um conjunto de políticas que governa os limites para a criação, atribuição, fechamento e visibilidade de tarefas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Proprietário da Tarefa]</td> 
   <td>A equipe ou usuário responsável pela estimativa de esforço e conclusão da tarefa</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Equipe]</td> 
   <td> <p>Uma coleção de usuários que trabalham para metas ou objetivos de negócios semelhantes. Esses usuários podem ser atribuídos coletivamente a um item de trabalho, atribuindo a equipe ao item de trabalho.</p> <p>Para obter mais informações sobre Equipes, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Visão geral das equipes</a>.</p> <p>Os projetos podem ter uma [!UICONTROL Equipe de Projeto], que contém todos os usuários ou funções associados ao trabalho no projeto.</p> <p>Para obter mais informações sobre Equipes de Projeto, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral da Equipe de Projeto</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Modelo]</td> 
   <td> <p>Os modelos de projeto são estruturas genéricas dos projetos mais repetíveis. Você pode definir tarefas, colocar em fila tópicos, formulários personalizados, anexar documentos ou aprovações ao criar um modelo de projeto para economizar tempo quando precisar criar um novo projeto. </p> <p>Você pode anexar modelos a projetos existentes ou usá-los para criar novos projetos. Todas as informações especificadas no modelo são transferidas para os projetos criados que o utilizam. </p> <p>Para obter mais informações sobre modelos, consulte <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Visão geral do modelo de projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modelo de Tarefa]</td> 
   <td>Uma tarefa que faz parte de um modelo. Modelos de Tarefa se tornam Tarefas no projeto criado usando o modelo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>Uma [!UICONTROL Observação] e sua coleção de respostas relacionadas a um tópico específico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniatura]</td> 
   <td> <p> Em uma lista ou relatório do [!UICONTROL Document], é exibida uma visualização do documento em miniatura. </p> <p> Selecionar <strong>[!UICONTROL Miniatura]</strong>  para exibir uma miniatura de 33 a 66 pixels de largura no relatório. </p> <p>O tamanho da miniatura é ajustado quando você modifica a largura da coluna em uma lista ou relatório.</p> <p>Consulte também "[!UICONTROL Miniatura grande]" neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo livre]</td> 
   <td>É possível criar um relatório de [!UICONTROL Folga] para exibir quando os usuários indicaram folga em seus perfis. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planilha de Horas]</td> 
   <td> <p>Um cartão de ponto que permite aos usuários inserir as horas reais que eles gastaram trabalhando em projetos, tarefas ou problemas, ou as horas que eles gastaram em outras atividades não relacionadas ao trabalho, como reuniões ou treinamento. Além de informar a quantidade de tempo que você gastou trabalhando, você também pode indicar se o tempo está relacionado ao trabalho ou se é uma quantidade de tempo indireto, usando Tipos de Hora para definir suas entradas de tempo. Para obter informações sobre folhas de horas, consulte <a href="../../../timesheets/timesheets/timesheets-overview.md">Visão geral sobre folhas de horas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Perfil de Planilha de Horas]</td> 
   <td> <p>Um [!UICONTROL Perfil de Planilha de Horas] é um modelo que [!DNL Workfront] usa para criar automaticamente planilhas de horas para os usuários associados a elas. </p> <p>Você pode definir várias configurações que serão aplicadas a cada folha de horas quando ela for criada. Algumas dessas configurações são: a frequência com que a folha de horas deve ser criada (semanalmente, a cada duas semanas, duas vezes por mês ou mensalmente), o dia de início da folha de horas, os aprovadores de folha de horas, os [!UICONTROL Tipos de horas] disponíveis que os usuários podem associar às horas registradas.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL ID do Pai Superior] </td> 
   <td> <p>Esse campo permite identificar e filtrar dados sobre um grupo de nível superior e seus subgrupos em uma lista ou relatório.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do Pai Superior] </td> 
   <td> <p>Este campo permite a identificação de dados sobre um grupo de nível superior e seus subgrupos em uma [!UICONTROL Exibir] para uma lista ou relatório.</p> <p>Também é possível fazer isso usando o campo [!UICONTROL ID do pai superior].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Horas Totais]</td> 
   <td> <p>Em um [!UICONTROL project report], esse campo exibe a soma arredondada de todas as horas do projeto, na última vez que as finanças do projeto foram calculadas. [!UICONTROL Horas efetivas] reflete as horas exatas registradas no projeto. Normalmente, as [!UICONTROL Horas efetivas] devem corresponder às [!UICONTROL Horas totais]. Se [!UICONTROL Total de Horas] parecer significativamente diferente do campo [!UICONTROL Horas Reais], você deverá Recalcular as Finanças no projeto.</p> <p>Para obter mais informações sobre como recalcular as finanças do projeto, consulte o artigo <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Recalcular as finanças do projeto</a>.</p> <p>Em uma exibição de folha de horas [!UICONTROL Padrão], esse campo se refere ao total de horas registradas para itens para as datas exibidas em uma folha de horas. O campo [!UICONTROL Total de Horas] para folhas de horas nessa exibição interna faz referência ao campo "[!UICONTROL hoursDuration]" que calcula dinamicamente a diferença em horas entre as datas de Início e Término da folha de horas. Isso é usado para exibir a coluna [!UICONTROL Horas totais] em vermelho se o usuário registrar mais tempo do que as horas disponíveis no intervalo de tempo da folha de horas. Para obter mais informações, consulte <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Exibir total de horas na folha de horas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de Acompanhamento]</td> 
   <td> <p>Um atributo de uma tarefa. Isso determina como e quando as linhas do tempo Projetadas serão atualizadas para uma tarefa. Por exemplo:</p> 
    <ul> 
     <li>[!UICONTROL Usuário Deve Atualizar] requer que uma tarefa seja atualizada manualmente. Caso contrário, ele se tornará [!UICONTROL Atrasado] e [!UICONTROL Atrasado].</li> 
     <li>A [!UICONTROL Preenchimento Automático] concluirá automaticamente uma tarefa quando a Data de Conclusão ou a [!UICONTROL Data de Conclusão Planejada] tiver passado.</li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Visão geral do modo de rastreamento de tarefas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Acionador]</td> 
   <td>Um evento que inicia um cenário.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa de Problema]</td> 
   <td>Uma tarefa incompleta com uma condição de [!UICONTROL Atrasado], [!UICONTROL Atrasado na Agenda] ou [!UICONTROL em Risco].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarefa Não Atribuída]</td> 
   <td>Uma tarefa que não está atribuída a nenhum usuário, função ou equipe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Atualização]</td> 
   <td> <p>Uma configuração em um projeto que determina quando a linha do tempo do Projeto será recalculada. O [!UICONTROL Tipo de Atualização] pode ter os seguintes valores:</p> 
    <ul> 
     <li>[!UICONTROL Automático e Mediante Alteração]</li> 
     <li>[!UICONTROL Somente Automático]</li> 
     <li>[!UICONTROL Somente Manual] </li> 
    </ul> <p>Para obter mais informações, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecionar o Tipo de Atualização do projeto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuário]</td> 
   <td>Uma conta criada em [!DNL Workfront] para permitir que uma pessoa faça logon e interaja com o sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Delegação de Usuário]</p> </td> 
   <td> <p>Um objeto reportável que informa a você:</p> 
    <ul> 
     <li>Quais usuários delegaram as aprovações de tarefas, problemas e projetos</li> 
     <li>Quais usuários tiveram as aprovações de tarefas, problemas e projetos delegadas a eles</li> 
     <li>Quando estas delegações começam e terminam</li> 
    </ul> <p>Para saber mais, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Criar um relatório de delegação de usuário</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface do Usuário]</td> 
   <td>Todos os aspectos visuais e interativos do aplicativo [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Preferências de Interface do Usuário]</td> 
   <td>[!UICONTROL Configuração da Interface do Usuário]. Os administradores do [!DNL Workfront] podem alterar essas configurações para personalizar aspectos da interface do usuário.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilização]</td> 
   <td>A disponibilidade de um usuário ou função com base na programação atribuída, PTO e carga de trabalho atual.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilização de Usuário]</td> 
   <td> <p>Uma pesquisa combinada a um relatório que mostra como os Usuários (Recursos) são alocados ou superalocados. Consulte "[!UICONTROL Utilização de Recursos]" neste artigo.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

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
   <td>[!UICONTROL Velocidade]</td> 
   <td>Uma medida do tempo total do ciclo de trabalho (quanto tempo leva para concluir um trabalho) e a frequência com que o trabalho é feito no tempo originalmente comprometido (proporção trabalho-para-comprometimento).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Exibir]</td> 
   <td> <p>As exibições se referem a um elemento de relatório que permite modificar as colunas em um relatório ou em uma lista de objetos.</p> 
   <p> Visualização também se refere ao direito de um usuário de visualizar apenas informações em um objeto, de acordo com seu nível de acesso ou em um nível de compartilhamento de permissões nesse objeto.</p> 
   <p>No Workfront Planning, os registros são exibidos na página tipo de registro em um dos seguintes tipos de exibição:</p>
   <ul><li>Tabela</li>
   <li>Linha do tempo</li>
   <li>Calendário</li></ul>
   <p>No Workfront Planning, as exibições incluem os filtros, agrupamentos, classificações e outras configurações aplicadas aos registros na tela.</p> <p>Para obter informações, consulte <a href="/help/quicksilver/planning/views/manage-record-views.md">Gerenciar exibições de registros</a>.</p>   
   <p>O Workfront Planning exige uma licença adicional.</p>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibir Ícones]</td> 
   <td> <p> Esse campo é igual aos Ícones de Status, mas só está disponível para as seguintes exibições: </p> 
    <ul> 
     <li> [!UICONTROL Documentos] </li> 
    </ul> <p> Para obter mais informações, consulte o artigo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ícones de status internos em Exibições</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibe o Mês Passado]</td> 
   <td> <p>Em uma lista de relatórios, é exibido o número de vezes que o relatório foi visualizado durante o último mês.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Exibir uso de relatório</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibe o Trimestre Passado]</td> 
   <td>Em uma lista de relatórios, é exibido o número de vezes que o relatório foi visualizado durante o último trimestre.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Exibir uso de relatório</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibições Ano Passado]</td> 
   <td>Em uma lista de relatórios, é exibido o número de vezes que o relatório foi visualizado durante o último ano.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Exibir uso de relatório</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibe Este Mês]</td> 
   <td> <p>Em uma lista de relatórios, é exibido o número de vezes que o relatório foi visualizado durante este mês.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Exibir uso de relatório</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibe Este Trimestre]</td> 
   <td>Em uma lista de relatórios, é exibido o número de vezes que o relatório foi visualizado durante esse trimestre.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Exibir uso de relatório</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exibe Este Ano]</td> 
   <td>Em uma lista de relatórios, é exibido o número de vezes que o relatório foi visualizado durante este ano.<br>Para obter mais informações sobre o uso em listas de relatórios, consulte o artigo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Exibir uso de relatório</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> Em um relatório, ao usar a interface [!UICONTROL Text Mode], a linha de código em que é possível especificar a largura de cada coluna em pixels. O Workfront fornece uma largura sugerida para cada campo,
No entanto, dependendo do tipo de campo e do formato, talvez você queira fazer ajustes.
Você deve usar a linha de código <code>[!UICONTROL usewidths=true]</code> adicional para aplicar a largura especificada para a coluna. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>Em um relatório de projeto, tarefa ou problema, usando a seguinte instrução no modo de texto, as Horas Planejadas do projeto, tarefa ou problema são exibidas:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Para obter informações sobre como usar o modo texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Visão geral da sintaxe do modo texto</a>. </p> 
   <p><b>DICA</b> 
   <p>Em um relatório de problemas, a adição de um dos campos [!UICONTROL Planned Hours] adiciona o campo <code>work </code> ao relatório. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabalho]</td> 
   <td> <p>Um dos dois tipos de licença principais. Este plano tem menos acesso do que o [!UICONTROL Plan], mas pode criar e fazer atualizações no sistema. Um usuário com uma licença de Trabalho tem mais habilidades do que um titular de licença [!UICONTROL Externo], [!UICONTROL Revisor] ou [!UICONTROL Solicitante].</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] visão geral das licenças</a>.</p> <p>O trabalho pode se referir ao número de [!UICONTROL Horas Planejadas] para um projeto, tarefa ou problema. Para obter mais informações, consulte o campo "[!UICONTROL work]" nesta tabela. </p> <p><b>DICA</b></p> <p> Em um relatório de problemas, a adição de um dos campos [!UICONTROL Planned Hours] adiciona o campo <code>work </code> ao relatório. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estrutura de Detalhamento de Trabalho]</td> 
   <td>Uma estrutura hierárquica das tarefas a serem executadas pela equipe do projeto com base no relacionamento pai/filho.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Esforço de trabalho] </td> 
   <td> 
    <p>Um gerente de projeto pode decidir usar esse campo em vez de [!UICONTROL Horas planejadas] para estimar o esforço necessário para concluir uma tarefa. Este campo fica visível somente quando as seguintes condições são atendidas:</p> 
     <ul> 
      <li> <p>A tarefa tem um [!UICONTROL Tipo de Duração Simples]. </p> <p><b>DICA</b></p> <p> Se você atualizar a tarefa [!UICONTROL Tipo de Duração] para qualquer outro tipo, esse campo ficará oculto. </p> </li> 
      <li>O gerente de projeto habilitou o [!UICONTROL Usar esforço de trabalho] para calcular automaticamente o campo de tarefa [!UICONTROL Horas planejadas] no projeto. </li> 
     </ul> 
     <p>Para obter informações sobre como usar o [!UICONTROL Esforço de trabalho] em vez das [!UICONTROL Horas planejadas] para estimar o esforço da tarefa, consulte <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Visão geral do esforço de trabalho</a>. </p> 
     <p>Você pode exibir esse campo em relatórios e listas de tarefas.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Item de Trabalho]</td> 
   <td> <p>Este campo se refere a tarefas ou problemas em [!DNL Workfront]. </p> <p>O relatório do [!UICONTROL Item de Trabalho] exibe informações sobre tarefas e problemas. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Combinação de gerenciamento de trabalho]</td> 
   <td>Um [!UICONTROL Indicador de Desempenho de Trabalho] (WPI) da proporção de trabalho alocada para administrar sua empresa versus alterar sua empresa. O WPI de combinação ajuda você a entender, em um nível organizacional, se sua estratégia tem alguma alocação de trabalho real aplicada a ela.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurso de Gerenciamento de Trabalho]</td> 
   <td>Uma designação de uma pessoa no sistema que está qualificada para receber trabalho ou tempo de rastreamento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Função e Responsabilidades de Gerenciamento de Trabalho]</td> 
   <td>Definir os proprietários e os participantes para gerenciar o escopo, a execução e as aprovações da ocorrência, tarefa, projeto, programa ou portfólio designado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL SLA de gerenciamento de trabalho]</td> 
   <td>Uma métrica quantificável acordada por todas as partes interessadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Participante no Gerenciamento de Trabalho]</td> 
   <td>Uma coleção de usuários com interesse adquirido nos resultados de uma solicitação de trabalho.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pontos de contato de gerenciamento de trabalho]</td> 
   <td>Registros digitalizados da comunicação entre as partes interessadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicadores de Desempenho de Trabalho] </td> 
   <td> <p>Taxa de combinação, capacidade, velocidade, qualidade e envolvimento.</p> <p>WPI é um acrônimo comum para [!UICONTROL Indicador de desempenho de trabalho].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Processo de Trabalho]</td> 
   <td> <p>O método no qual o trabalho é recebido, priorizado e executado. A maneira como você executa o trabalho normalmente é chamada de "fluxo de trabalho" ou "plano de projeto" (uma lista de tarefas com datas, relações de predecessoras e assim por diante). </p> <p>Exemplos de um processo de trabalho podem ser a produção de um único ativo ou a entrega de uma campanha com vários ativos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modelo de fluxo de trabalho]</td> 
   <td>No relatório [!UICONTROL Aprovação de prova], esse campo exibe todos os modelos de fluxo de trabalho anexados a uma prova. Se não houver modelos anexados, a coluna ficará em branco.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Horário de Trabalho]</td> 
   <td>

<p>Representa a porcentagem de tempo Equivalente ao Tempo Integral ([!UICONTROL FTE]) em que o usuário está disponível para o trabalho real, sem incluir a sobrecarga. [!UICONTROL Horário de Trabalho] deve ser um número decimal até 1 e não pode ser 0. Por exemplo, uma disponibilidade de 20% para o trabalho real seria de 0,2.</p>
   </p>O padrão do campo é 1, indicando que um usuário gasta todo o [!UICONTROL FTE] no trabalho real relacionado ao projeto.  </p>
   <p>O sistema usa esse número para calcular a disponibilidade do usuário para o trabalho real relacionado ao projeto. </p>
   <p> Exceções de agendamento e folga também podem afetar a capacidade do usuário. </p>
   <p>Para obter mais informações sobre como criar agendas no Workfront, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar uma agenda</a>. </p>
    <p>O Workfront calcula a disponibilidade de um usuário dependendo das preferências de Gerenciamento de recursos na área [!UICONTROL Setup]. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configurar preferências de Gerenciamento de Recursos</a>. </p> 
   <p>É possível atualizar o [!UICONTROL Horário de Trabalho] de um usuário ao editá-lo ou criá-lo. Para obter informações, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Editar perfil de um usuário</a></p> 
   <b>DICA</b> 
   <p>Defina o valor de [!UICONTROL Tempo de trabalho] para 1, de modo a indicar que o usuário está disponível para trabalhos relacionados ao projeto em todo o seu equivalente de tempo integral.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Horário de trabalho]</td> 
   <td>Na documentação do Workfront, esse termo é usado para descrever o tempo alocado para trabalhar, de acordo com um agendamento.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>Em um relatório de projeto, tarefa ou problema, usar a seguinte instrução no modo de texto exibe o número de Horas planejadas do projeto, tarefa ou problema seguido da palavra "Horas":</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Para obter informações sobre como usar o modo texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Visão geral da sintaxe do modo texto</a>. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Workspace] </td> 
   <td> <p>No Workfront Planning, um espaço de trabalho é uma coleção de tipos de registro que define o ciclo de vida operacional de uma determinada organização. Um espaço de trabalho é o quadro de trabalho de uma unidade organizacional.</p>
   <p>O Workfront Planning exige uma licença adicional. </p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/planning/architecture/create-workspaces.md">Criar espaços de trabalho</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


