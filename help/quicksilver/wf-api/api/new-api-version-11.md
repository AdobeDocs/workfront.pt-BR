---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 11
description: ReportableBudgedHour foi adicionado à API do Adobe Workfront como um recurso para Relatórios. Ele apresenta campos de referência, campos principais e campos padrão que estão ausentes em BudgetedHour.
author: Becky
feature: Workfront API
role: Developer
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '3573'
ht-degree: 2%

---

# Novidades da API versão 11

* [Recursos Adicionados](#added-resources)
* [Recursos Removidos](#removed-resources)
* [Recursos modificados](#modified-resources)

## Recursos adicionados {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [HorasOrçadasRelatáveis](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">accessID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">acessador</li> 
     <li style="font-weight: bold;">cliente</li> 
     <li style="font-weight: bold;">usuário  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principais</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">cliente  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principais</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">restrictLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">cliente  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de coleção</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">additionalRules</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principais</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### HorasOrçadasRelatáveis {#reportablebudgetedhour}

ReportableBudgedHour foi adicionado à API do Adobe Workfront como um recurso para Relatórios. Ele apresenta campos de referência, campos principais e campos padrão que estão ausentes em BudgetedHour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>A Data de Alocação é o primeiro dia (um domingo) da semana para o qual você orçou as horas no Planejador de Recursos.</p> </li> 
     <li> <p style="font-weight: bold;">budgetedHours </p> <p>As horas orçadas são horas que o gerente de recursos elabora para o trabalho que os recursos precisam concluir nos projetos</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>A Workfront ID exclusiva atribuída a um objeto específico de Horas orçadas reportáveis.</p> </li> 
     <li style="font-weight: bold;">plannedBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>A Workfront ID exclusiva atribuída a um projeto específico.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>A Workfront ID exclusiva atribuída a uma Função de trabalho específica.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>A ID exclusiva do Workfront atribuída a um usuário específico.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">projeto</p> <p>O Projeto ao qual uma ReportableBudgetedHour está associada.</p> </li> 
     <li> <p style="font-weight: bold;">função</p> <p>A Função de Trabalho à qual uma ReportableBudgetedHour está associada.</p> </li> 
     <li> <p style="font-weight: bold;">usuário</p> <p>O Usuário ao qual uma ReportableBudgetedHour está associada.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principais</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">name</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos padrão</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">name</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Operações</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">CONTAGEM</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">RELATÓRIO </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Recursos removidos {#removed-resources}

Nenhum recurso foi removido para a API v11.

## Recursos modificados {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">PermissõesDeNívelDeAcesso</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">SolicitaçãoDeAcesso</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">RegraDeAcesso</a> </li> 
     <li><a href="#approval" class="MCXref xref">Aprovação</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">Atribuição</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">TarefaDaLinhaDeBase</a> </li> 
     <li><a href="#category" class="MCXref xref">Categoria</a> </li> 
     <li><a href="#company" class="MCXref xref">Empresa</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">Cliente</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">PreferênciasDoCliente</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">Documento</a> </li> 
     <li><a href="#iteration" class="MCXref xref">Iteração</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">Modelo de layout</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">CaminhoEtapas</a> </li> 
     <li><a href="#note" class="MCXref xref">Nota</a> </li> 
     <li><a href="#optask" class="MCXref xref">TarefaOp</a> </li> 
     <li><a href="#parameter" class="MCXref xref">Parâmetro</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio</a> </li> 
     <li><a href="#program" class="MCXref xref">Programa</a> </li> 
     <li><a href="#project" class="MCXref xref">Projeto</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">AprovaçãoDeProva</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">DefiniçãoDaFila</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">TempoReservado</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">FiltroDoPlanejadorDeRecursos</a> </li> 
     <li><a href="#risk" class="MCXref xref">Risco</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">RelatórioAgendado</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">Tarefa</a> </li> 
     <li><a href="#team" class="MCXref xref">Equipe</a> </li> 
     <li><a href="#template" class="MCXref xref">Modelo</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">AtribuiçãoModelo</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TarefaModelo</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">Planilha de horas</a> </li> 
     <li><a href="#update" class="MCXref xref">Atualização</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">AnotaçãoUsuário</a> </li> 
     <li><a href="#work" class="MCXref xref">Trabalho </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### PermissõesDeNívelDeAcesso {#accesslevelpermissions}

Um objeto AccessLevelPermissions representa um conjunto de permissões. Esse conjunto de permissões pode ser associado a um Nível de acesso.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> <p>Os campos a seguir adicionaram o possível valor BUDGETING_INFORMATION. Isso permite que os usuários com permissão editem prioridades e horas de orçamento no planejador.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Solicitação de acesso {#accessrequest}

Se um usuário não tiver acesso a um objeto no Workfront necessário, ele poderá solicitar acesso a esse objeto. O objeto AccessRequest representa essa solicitação.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">ação</p> <p>Adição do possível valor BUDGETING_INFORMATION. Isso permite que os usuários com permissão editem prioridades e horas de orçamento no planejador.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Regra de acesso {#accessrule}

Um objeto AccessRule representa um conjunto de regras em níveis de acesso personalizados que determina como os usuários podem compartilhar projetos criados por eles.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> <p>Os campos a seguir adicionaram o possível valor BUDGETING_INFORMATION. Isso permite que os usuários com permissão editem prioridades e horas de orçamento no planejador.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aprovação {#approval}

Um determinado item de trabalho, como uma tarefa, um documento ou uma folha de horas, pode exigir que um supervisor ou outro usuário faça logoff no item de trabalho. Um objeto de Aprovação representa a ação de desconectar em um item de trabalho.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos diretos<p style="font-weight: normal;">Os campos a seguir adicionaram os validadores AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Esses validadores especificam que as datas em objetos associados não podem ser definidas antes de 1900 ou depois de 2200.</p>
    <ul>
     <li style="font-weight: bold;">atualCompletionDate</li>
     <li style="font-weight: bold;">atualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">Os seguintes campos foram adicionados à API pública para maior transparência no cálculo da EAC (Estimativa no término).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Também conhecido como Valor Agregado, o Custo Orçado do Trabalho Realizado (COTR) é uma métrica de desempenho do projeto que representa o custo orçado da quantidade da tarefa que foi realmente concluída no momento em que essa métrica é calculada. Para tarefas, COTR = Percentual de Término Real x Orçamento da Tarefa. Para Projetos, BCWP = SUM(valores BCWP de todas as tarefas pai e individual).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Também conhecido como Valor Planejado, o Custo Orçado do Trabalho Agendado (BCWS) é uma métrica de desempenho do projeto que representa o custo orçado da quantidade da tarefa que deveria ter sido concluída no momento em que essa métrica é calculada. Para tarefas, BCWS = Percentual de Término Planejado x Orçamento da Tarefa. Para projetos, BCWS = SUM(valores BCWS de todas as tarefas pai e individual).</p></li>
    </ul><p style="font-weight: normal;">Os campos a seguir adicionaram o valor possível ET. Esse valor representa a unidade de tempo Meses decorridos, que se refere aos meses sem considerar fins de semana ou feriados.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Os seguintes campos adicionaram o sinalizador MOEDA</p>
    <ul>
     <li style="font-weight: bold;">custoOrçadoProjeto</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Os campos a seguir foram removidos do objeto Aprovação.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">O campo a seguir foi adicionado ao objeto Aprovação.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Removido do objeto de Aprovação  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de coleção</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Adicionado ao objeto Approval.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

Um objeto ApprovalPath é uma ramificação dentro de um Processo de Aprovação. Os Caminhos de Aprovação são baseados no status do objeto ao qual o Processo de Aprovação está associado.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Adição do possível valor ET. Esse valor representa a unidade de tempo Meses decorridos, que se refere aos meses sem considerar fins de semana ou feriados.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

Um objeto ApprovalProcess é uma Aprovação de várias etapas que pode ser associada a um Projeto, Tarefa ou Problema.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Este campo foi adicionado e é um parâmetro booleano que tem um valor true se um objeto estiver ativo e false se não for. Os objetos definidos como Ativos aparecem em menus suspensos e campos de digitação antecipada e podem ser anexados a outros objetos. Objetos não definidos como Ativos não são visíveis em menus suspensos e campos de digitação antecipada para anexar a outros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos padrão</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Atribuição {#assignment}

Um objeto de atribuição representa a conexão entre um item de trabalho e o usuário, equipe ou grupo atribuído para trabalhar nele.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">Adição do possível valor ET. Esse valor representa a unidade de tempo Meses decorridos, que se refere aos meses sem considerar fins de semana ou feriados.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TarefaDaLinhaDeBase {#baselinetask}

Linhas de Base são instantâneos de como era o desempenho de um projeto em um determinado momento. Eles armazenam informações importantes sobre o projeto, como datas importantes, progresso, valores de custo e receita. Quando você cria uma linha de base, as informações sobre a tarefa também são capturadas nas tarefas dessa linha de base.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Adição do possível valor ET. Esse valor representa a unidade de tempo Meses decorridos, que se refere aos meses sem considerar fins de semana ou feriados.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categoria {#category}

Um objeto de Categoria é um formulário personalizado. Você pode criar relatórios para esse objeto e também pode mostrá-lo em outros relatórios de objeto.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Este campo foi adicionado e é um parâmetro booleano que tem um valor true se um objeto estiver ativo e false se não for. Os objetos definidos como Ativos aparecem em menus suspensos e campos de digitação antecipada e podem ser anexados a outros objetos. Objetos não definidos como Ativos não são visíveis em menus suspensos e campos de digitação antecipada para anexar a outros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos padrão</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Empresa {#company}

Um objeto Company representa uma organização que consiste em uma coleção de pessoas. As empresas estão associadas a um usuário ou projeto.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Este campo foi adicionado e é um parâmetro booleano que tem um valor true se um objeto estiver ativo e false se não for. Os objetos definidos como Ativos aparecem em menus suspensos e campos de digitação antecipada e podem ser anexados a outros objetos. Objetos não definidos como Ativos não são visíveis em menus suspensos e campos de digitação antecipada para anexar a outros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos padrão</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Ações</td> 
   <td> <p style="font-weight: normal;">As seguintes ações foram adicionadas ao objeto CustomEnum</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Consultas</td> 
   <td> <p>As seguintes consultas foram adicionadas ao objeto CustomEnum</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Cliente {#customer}

Um objeto Customer representa uma organização que usa uma instância do Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">Valores possíveis adicionados: </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ (Condições do Projeto)</li> 
       <li style="font-weight: normal;">CONDITION_TASK (Condições de Tarefa)</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK (Condições de Emissão)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>Ações</td> 
   <td> <p style="font-weight: normal;">As ações a seguir foram adicionadas ao objeto Cliente</p> 
    <ul> 
     <li style="font-weight: bold;">goalsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### PreferênciasDoCliente {#customerpreferences}

Um objeto CustomerPreferences representa o conjunto de preferências que um cliente definiu para sua instância do Workfront.

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Valores possíveis adicionados:</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy (Requisitos de complexidade de senha)</li> 
       <li style="font-weight: normal;"> senha:senha.comprimentoMínimo (tamanho mínimo da senha)</li> 
       <li style="font-weight: normal;">senha:mobileSessionTimeout (Tempo Limite da Sessão Móvel)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (Tempo livre do usuário)</li> 
       <li style="font-weight: normal;">folha de horas:default.timesheet.manualrole (função de controle Manual)</li> 
       <li style="font-weight: normal;">prova:defaultNonRecipientRole (config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">prova:defaultNonRecipientGuestRole (config.proofhq.defaultnonrecipientguestrole)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Ações</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Documento {#document}

Um objeto Documento representa um arquivo (como material escrito, imagens ou outras formas de informação).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Ações</td> 
   <td> <p>As ações a seguir foram adicionadas ao objeto Documento.</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Iteração {#iteration}

Um objeto de Iteração representa uma única Iteração Agile. Iterações são períodos discretos usados para planejar e concluir histórias Agile.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> <p>Os campos a seguir foram adicionados ao objeto de Iteração.</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">pontos concluídos</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Modelo de Layout {#layout-template}

Um objeto de Modelo de layout representa uma disposição específica de elementos de layout, como o menu principal, o painel de navegação ou a área da página inicial. Os modelos de layout podem ser atribuídos a usuários, equipes, grupos ou funções de trabalho.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">Este campo foi adicionado e é um parâmetro booleano que tem um valor true se um Modelo de layout estiver definido para mostrar carimbos de data e hora para datas de vencimento na Lista de trabalho e no Calendário, e false se estiver definido para ocultar carimbos de data e hora.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos padrão</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CaminhoEtapas {#milestonepath}

Uma etapa é um marcador em uma indicação de tarefa que é um ponto-chave no projeto. Geralmente usado para indicar um evento significativo, como a conclusão de uma fase do projeto ou um conjunto de atividades críticas. Um objeto MilestonePath é uma coleção de marcos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Este campo foi adicionado e é um parâmetro booleano que tem um valor true se um objeto estiver ativo e false se não for. Os objetos definidos como Ativos aparecem em menus suspensos e campos de digitação antecipada e podem ser anexados a outros objetos. Objetos não definidos como Ativos não são visíveis em menus suspensos e campos de digitação antecipada para anexar a outros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos padrão</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Nota {#note}

Um objeto Note é um comentário ou uma atualização feita em um objeto Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> <p>Os campos a seguir foram adicionados ao objeto Nota.</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de coleção</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>curtidas</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Um objeto OpTask é comumente conhecido como um Problema. Um problema é um item de trabalho que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Um problema também pode ser uma solicitação de Help Desk. Pedidos de alteração, solicitações e bugs também são problemas.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos diretos<p style="font-weight: normal;">Os campos a seguir adicionaram os validadores AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Esses validadores especificam que as datas em objetos associados não podem ser definidas antes do ano 1900 ou depois de 2200.</p>
    <ul>
     <li style="font-weight: bold;">atualCompletionDate</li>
     <li style="font-weight: bold;">atualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">Os campos a seguir foram adicionados ao OpTask.</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">O Workfront ID exclusivo de um objeto do Quadro Kanban.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">Percentual Concluído é um parâmetro que retornará a quantia concluída de uma ocorrência, como uma porcentagem.</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">trabalho  </li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de coleção</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de Busca</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>trabalho</p> <p style="font-weight: normal;">Removido</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos padrão</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Ações</td> 
   <td> <p>As seguintes ações foram adicionadas ao objeto OpTask</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parâmetro {#parameter}

Um objeto Parameter é um campo personalizado.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Adição do valor possível TYAH (Typeahead).</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">Este campo foi adicionado e se refere ao código de objeto de um objeto referenciado. Códigos de objeto para todos os objetos podem ser encontrados no <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfólio {#portfolio}

Um objeto Portfolio é uma coleção de projetos que competem pelos mesmos recursos, normalmente dinheiro ou pessoas para concluí-los.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>descrição</p> <p style="font-weight: normal;">Adição do validador MAX_LENGTH, que especifica que o comprimento da descrição não é superior a 4000 caracteres.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programa {#program}

Um objeto de Programa é um subconjunto em um portfólio, no qual projetos semelhantes podem ser agrupados.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>descrição</p> <p style="font-weight: normal;">Adição do validador MAX_LENGTH, que especifica que o comprimento da descrição não é superior a 4000 caracteres.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Este campo foi adicionado e é um parâmetro booleano que tem um valor true se um objeto estiver ativo e false se não for. Os objetos definidos como Ativos aparecem em menus suspensos e campos de digitação antecipada e podem ser anexados a outros objetos. Objetos não definidos como Ativos não são visíveis em menus suspensos e campos de digitação antecipada para anexar a outros objetos.  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">Adição do validador MAX_LENGTH, que especifica que o comprimento do nome não é superior a 255 caracteres.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos padrão</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projeto {#project}

Os projetos são itens de trabalho no Workfront e um elemento principal da maneira como o Workfront ajuda as pessoas a trabalhar. Um objeto Projeto representa um grupo de tarefas com uma meta comum e específica.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos diretos<p style="font-weight: normal;">Os campos a seguir adicionaram os validadores AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Esses validadores especificam que as datas em objetos associados não podem ser definidas antes do ano 1900 ou depois de 2200.</p>
    <ul>
     <li style="font-weight: bold;">atualCompletionDate</li>
     <li style="font-weight: bold;">atualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">Os seguintes campos foram adicionados à API pública para maior transparência no cálculo da EAC (Estimativa no término).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Também conhecido como Valor Agregado, o Custo Orçado do Trabalho Realizado (COTR) é uma métrica de desempenho do projeto que representa o custo orçado da quantidade da tarefa que foi realmente concluída no momento em que essa métrica é calculada. Para tarefas, COTR = Percentual de Término Real x Orçamento da Tarefa. Para Projetos, BCWP = SUM(valores BCWP de todas as tarefas pai e individual).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Também conhecido como Valor Planejado, o Custo Orçado do Trabalho Agendado (BCWS) é uma métrica de desempenho do projeto que representa o custo orçado da quantidade da tarefa que deveria ter sido concluída no momento em que essa métrica é calculada. Para tarefas, BCWS = Percentual de Término Planejado x Orçamento da Tarefa. Para projetos, BCWS = SUM(valores BCWS de todas as tarefas pai e individual).</p></li>
    </ul><p style="font-weight: normal;">Os seguintes campos adicionaram o sinalizador MOEDA</p>
    <ul>
     <li style="font-weight: bold;">custoOrçadoProjeto</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">O campo a seguir foi removido do objeto Project.</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de coleção</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AprovaçãoDaProva {#proofapproval}

Um objeto ProofApproval representa uma aprovação que está diretamente conectada a uma prova.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitingDecision</p> <p style="font-weight: normal;">Este campo foi adicionado, e é um parâmetro booleano que tem um valor de true se uma prova estiver aguardando uma decisão e false se não estiver.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Um objeto QueueDef representa uma Fila, que é um Projeto publicado na área Help Desk para permitir que os usuários enviem Problemas a ele.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> <p>Os campos a seguir adicionaram o possível valor BUDGETING_INFORMATION. Isso permite que os usuários com permissão editem prioridades e horas de orçamento no planejador.</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### TempoReservado {#reservedtime}

Um objeto ReservedTime representa dias especificados no Tempo pessoal de um usuário, indicando que o usuário não estará disponível para trabalho.

O recurso ReservedTime adicionou o sinalizador REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> <p>Os campos a seguir removeram o sinalizador NOT_GROUPABLE.</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>O campo a seguir foi removido do objeto ReservedTime.</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>tarefa</p> <p style="font-weight: normal;">Removido  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Operações</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>EDITAR</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### FiltroDoPlanejadorDeRecursos {#resourceplannerfilter}

Um objeto ResourcePlannerFilter é um conjunto de regras que determinam quais itens serão exibidos no Planejador de recursos.

O recurso ResourcePlannerFilter adicionou o sinalizador SHARABLE. Não houve outras alterações no objeto.

### Risco {#risk}

Um objeto de Risco representa um evento possível que pode impedir que um projeto seja concluído no prazo ou dentro do orçamento. Os riscos são adicionados aos projetos na fase de planejamento para identificar possíveis obstáculos antes da aprovação de qualquer trabalho.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> <p>Os seguintes campos foram adicionados ao objeto Risk:</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">A ID do usuário que criou originalmente o objeto.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>A data em que um objeto foi enviado por um usuário no Workfront.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>O parâmetro Última data de atualização retornará a data em que a Última atualização foi feita em um objeto,</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>ID da Última Atualização realizada por é um parâmetro que retornará a ID do último Usuário que atualizou o objeto.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> <p style="font-weight: normal;">Os seguintes Campos de referência foram adicionados ao objeto Risco.</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RelatórioAgendado {#scheduledreport}

Um objeto ScheduledReport representa um relatório que foi configurado para ser agendado para entrega.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">Foram adicionados os seguintes valores possíveis:</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Um objeto ScoreCardQuestion representa uma pergunta que foi adicionada a um Scorecard. Essas perguntas geralmente são determinadas pelo gerente de Portfolio, e suas respostas permitem que o gerente entenda como um projeto se alinha com as metas do portfólio.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Valor adicionado possível TYAH (Typeahead)  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tarefa {#task}

Um objeto Tarefa representa um item de trabalho que deve ser executado como uma etapa para atingir uma meta final (concluir um Projeto).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos diretos<p style="font-weight: normal;">Os campos a seguir adicionaram os validadores AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Esses validadores especificam que as datas em objetos associados não podem ser definidas antes do ano 1900 ou depois de 2200.</p>
    <ul>
     <li style="font-weight: bold;">atualCompletionDate</li>
     <li style="font-weight: bold;">atualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">Os seguintes campos foram adicionados à API pública para maior transparência no cálculo da EAC (Estimativa no término).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Também conhecido como Valor Agregado, o Custo Orçado do Trabalho Realizado (COTR) é uma métrica de desempenho do projeto que representa o custo orçado da quantidade da tarefa que foi realmente concluída no momento em que essa métrica é calculada. Para tarefas, COTR = Percentual de Término Real x Orçamento da Tarefa. Para Projetos, BCWP = SUM(valores BCWP de todas as tarefas pai e individual).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Também conhecido como Valor Planejado, o Custo Orçado do Trabalho Agendado (BCWS) é uma métrica de desempenho do projeto que representa o custo orçado da quantidade da tarefa que deveria ter sido concluída no momento em que essa métrica é calculada. Para tarefas, BCWS = Percentual de Término Planejado x Orçamento da Tarefa. Para projetos, BCWS = SUM(valores BCWS de todas as tarefas pai e individual).</p></li>
    </ul><p style="font-weight: normal;">Os campos a seguir adicionaram o valor possível ET. Esse valor representa a unidade de tempo Meses decorridos, que se refere aos meses sem considerar fins de semana ou feriados.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">O campo a seguir foi removido do objeto Tarefa.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">O campo a seguir foi adicionado ao objeto Tarefa.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Removido  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de coleção</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Equipe {#team}

Um objeto Equipe é uma coleção de Usuários que pode ser atribuída a um item de trabalho.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">Este campo foi adicionado ao objeto Equipe. O Tipo de estimativa ágil determina como a carga de trabalho de uma história é estimada. Se estimado em horas, esse é o número de Horas planejadas que são adicionadas à história. Se estimado em pontos, cada ponto adicionará um número de Horas planejadas à história com base em como os pontos são definidos (o padrão é 8 horas). Os valores possíveis para o Tipo de estimativa Agile são:</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS (pontos da história)</li> 
       <li style="font-weight: normal;">HORAS (Horas)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS (Horas como Pontos)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Modelo {#template}

Um objeto Modelo representa um padrão para um Projeto. Os projetos podem ser criados a partir de Modelos para economizar tempo. Um Modelo contém uma Equipe e Tarefas, que serão copiadas para um Projeto quando o Modelo for usado.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Este campo foi adicionado e é um parâmetro booleano que tem um valor true se um objeto estiver ativo e false se não for. Os objetos definidos como Ativos aparecem em menus suspensos e campos de digitação antecipada e podem ser anexados a outros objetos. Objetos não definidos como Ativos não são visíveis em menus suspensos e campos de digitação antecipada para anexar a outros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de coleção</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriority</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos padrão</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AtribuiçãoModelo {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">Adição do possível valor ET. Esse valor representa a unidade de tempo Meses decorridos, que se refere aos meses sem considerar fins de semana ou feriados.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TarefaModelo {#templatetask}

Um objeto TemplateTask representa uma Tarefa que faz parte de um Template. Modelos de Tarefa se tornam Tarefas no Projeto onde o Modelo é usado.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> <p style="font-weight: normal;">Os campos a seguir adicionaram o valor possível ET. Esse valor representa a unidade de tempo Meses decorridos, que se refere aos meses sem considerar fins de semana ou feriados.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de coleção</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriority</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Planilha de horas {#timesheet}

Um objeto de Planilha de Horas representa um cartão de ponto virtual que permite aos Usuários inserir as horas reais trabalhadas para Tarefas, Projetos e Tipos de Horas Gerais.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos principais</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">Removido</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Atualizar {#update}

Os itens de trabalho no Workfront podem ser atualizados para manter os usuários informados sobre o status atual. Um objeto Update representa uma dessas atualizações. As atualizações podem ser inseridas por usuários ou criadas pelo sistema do Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">Adição de um valor possível referenceObjectCustomData (enum.updatetypeenum.referenceobjectcustomdata)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Consultas</td> 
   <td> <p style="font-weight: normal;">As consultas a seguir foram adicionadas ao objeto Update.</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos de coleção</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Ações</td> 
   <td> <p style="font-weight: normal;">As ações a seguir foram adicionadas ao objeto Usuário.</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Consultas</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserNote {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Ações</td> 
   <td> <p style="font-weight: normal;">As ações a seguir foram adicionadas ao objeto Usuário.</p> 
    <ul> 
     <li style="font-weight: bold;">confirmMyNotifications</li> 
     <li style="font-weight: bold;">unconfirmationAllObjectsTypeCount  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Consultas</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Trabalho  {#work}

Um objeto Trabalho é uma interface comum que tanto Tarefa quanto OpTask herdam e compartilha código comum entre os dois.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos diretos<p style="font-weight: normal;">Os campos a seguir adicionaram os validadores AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Esses validadores especificam que as datas em objetos associados não podem ser definidas antes do ano 1900 ou depois de 2200.</p>
    <ul>
     <li style="font-weight: bold;">atualCompletionDate</li>
     <li style="font-weight: bold;">atualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">Os seguintes campos foram adicionados à API pública para maior transparência no cálculo da EAC (Estimativa no término).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Também conhecido como Valor Agregado, o Custo Orçado do Trabalho Realizado (COTR) é uma métrica de desempenho do projeto que representa o custo orçado da quantidade da tarefa que foi realmente concluída no momento em que essa métrica é calculada. Para tarefas, COTR = Percentual de Término Real x Orçamento da Tarefa. Para Projetos, BCWP = SUM(valores BCWP de todas as tarefas pai e individual).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Também conhecido como Valor Planejado, o Custo Orçado do Trabalho Agendado (BCWS) é uma métrica de desempenho do projeto que representa o custo orçado da quantidade da tarefa que deveria ter sido concluída no momento em que essa métrica é calculada. Para tarefas, BCWS = Percentual de Término Planejado x Orçamento da Tarefa. Para projetos, BCWS = SUM(valores BCWS de todas as tarefas pai e individual).</p></li>
    </ul><p style="font-weight: normal;">Os campos a seguir adicionaram o valor possível ET. Esse valor representa a unidade de tempo Meses decorridos, que se refere aos meses sem considerar fins de semana ou feriados.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">O campo a seguir foi removido do objeto Trabalho.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">O campo a seguir foi adicionado ao objeto Trabalho.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Removido  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de coleção</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
