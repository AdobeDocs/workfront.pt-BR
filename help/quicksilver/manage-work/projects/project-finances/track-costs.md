---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Rastrear custos
description: Você pode acompanhar os custos de projetos, tarefas e problemas no Adobe Workfront.
author: Alina
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: 7e78ca8c8ea7f037b55b06e7452ac5c562b99eca
workflow-type: tm+mt
source-wordcount: '2418'
ht-degree: 1%

---

# Rastrear custos

Você pode acompanhar os custos de projetos, tarefas e problemas no Adobe Workfront.

## Como a Workfront calcula custos

Para rastrear custos, você deve associar usuários e funções de trabalho a taxas de custo por hora.

As taxas de custo por hora são quantias de custos por unidade de trabalho associadas a funções de trabalho ou usuários. Multiplicar as taxas pelas horas gastas no trabalho gera custos para seus projetos, tarefas ou problemas.

Os seguintes cenários existem:

* Se o Tipo de Custo de suas tarefas for Por Hora do Usuário, a taxa horária do usuário calculará os custos da tarefa e do projeto.

   Para obter informações sobre como associar usuários a taxas de custo, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Se o Tipo de Custo de suas tarefas for Função por hora, a taxa por hora da função da tarefa calculará os custos da tarefa e do projeto.

   Para obter informações sobre como associar funções de cargo a taxas de custo, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* A Workfront calcula somente o Custo Real para problemas e problemas não têm um Tipo de Custo. Para obter mais informações, consulte a seção [Como o Workfront acompanha os custos de problemas](#how-workfront-tracks-costs-for-issues) neste artigo.

>[!TIP]
>
>Não é possível substituir as taxas de custo de projetos. Depois de estabelecer a taxa de custo por hora em um usuário ou função de cargo, essa taxa calcula todos os custos no sistema.

## Índices de desempenho de custo da Workfront

A Workfront calcula uma série de índices de desempenho de custo para projetos, de modo que os projetos possam ser rastreados para oferecer eficiência de custos.\
Para obter mais informações sobre o cálculo de índices de custo-desempenho, consulte:

* [Calcular Índice de Desempenho de Custo (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Calcular CSI (Cost Schedule Performance Index, Índice de Desempenho da Programação de Custo)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Calcular o Índice de Desempenho da Programação (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Como o Workfront rastreia os custos de tarefas e projetos

* [Como a Workfront acompanha os custos](#how-workfront-tracks-costs)
* [Como o Workfront calcula os Custos Planejados, Orçados e Reais](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [Como a Workfront calcula os Tipos de Custo para tarefas](#how-workfront-calculates-cost-types-for-tasks)

### Como a Workfront acompanha os custos  {#how-workfront-tracks-costs}

Você pode rastrear vários tipos de Custos para tarefas e projetos no Workfront. Os custos gerais são calculados pela seguinte fórmula:

```
Costs = Labor Costs + Expense Costs
```

* **Custos da mão de obra** estão associados às horas em tarefas e projetos e às taxas de Custo por Hora dos recursos associados às tarefas. Geralmente, a Workfront calcula os seguintes custos de mão de obra:

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Custos planejados de mão de obra</td> 
     <td> <p>Eles são calculados usando a seguinte fórmula:</p><pre>Custos Planejados da Mão de Obra = Horas Planejadas * Custo por Hora</pre> </td> 
    </tr> 
    <tr> 
     <td>Custos de mão de obra orçados</td> 
     <td> <p>Eles são calculados usando a seguinte fórmula:</p><pre>Custos de Mão-de-Obra Orçados = Horas Orçamentadas * Taxa de Custo por Hora</pre> </td> 
    </tr> 
    <tr> 
     <td>Custos reais de mão de obra</td> 
     <td> <p>Eles são calculados usando a seguinte fórmula:</p><pre>Custos Reais da Mão-de-Obra = Horas Reais * Taxa de Custo por Hora</pre> </td> 
    </tr> 
   </tbody> 
  </table>

   Para obter mais informações, consulte o [Como o Workfront calcula os Custos Planejados, Orçados e Reais](#how-workfront-calculates-planned-budgeted-and-actual-costs) neste artigo.

* **Custos de Despesas** estão associados a Despesas em projetos e tarefas.\
   Ao criar um projeto, você pode definir as despesas planejadas para todo o projeto. Além disso, é possível associar despesas com tarefas novas ou existentes. Para obter mais informações, consulte [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Custos fixos** são definidas como uma quantia fixa de custo para um projeto. Isso faz parte do Custo Planejado do projeto, que representa a quantia de dinheiro que você precisa para concluir o projeto.

   >[!TIP]
   >
   >Ao anexar um modelo a um projeto, o Custo Fixo de um modelo é adicionado ao Custo Fixo do projeto. Para obter mais informações, consulte [Visão geral de anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Como o Workfront calcula os Custos Planejados, Orçados e Reais {#how-workfront-calculates-planned-budgeted-and-actual-costs}

A Workfront calcula o Custo Planejado e o Custo Real de cada tarefa individual em um projeto. A Workfront usa esses cálculos para tarefas individuais para calcular o Custo Planejado e o Custo Real do projeto.

* [Custo Planejado](#planned-cost)
* [Custo Orçado](#budgeted-cost)
* [Custo Efetivo](#actual-cost)

#### Custo Planejado {#planned-cost}

O Custo Planejado de um projeto é o custo associado ao trabalho planejado (Horas Planejadas) no projeto.

O Custo Planejado de um projeto é calculado pela seguinte fórmula:

```
Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project
```

Por exemplo, você tem as seguintes despesas na guia Expenses de uma tarefa: uma despesa de marketing de US$ 100 e uma despesa administrativa de US$ 50. Na guia Finanças, é possível selecionar o tipo de custo por hora do usuário. Um usuário é atribuído à tarefa e a taxa horária do usuário é de US$ 15. O usuário é atribuído para trabalhar 5 horas nessa tarefa. Na guia Expenses do projeto, você tem um Custo Planejado de $100 para uma despesa chamada Consulting. Você também tem um Custo Fixo de $200 para o projeto.

O Custo Planejado do projeto é calculado da seguinte maneira:

```
$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525
```

#### Custo Orçado {#budgeted-cost}

O Custo Orçamentado de um projeto é o custo associado ao trabalho orçado (Horas Orçamentadas) no projeto.

O custo orçamentado do projeto é o mesmo que o custo planejado do projeto se as duas condições seguintes forem cumpridas:

* As Horas Planejadas das tarefas no projeto correspondem às Horas Orçadas (no Planejador de Recursos)
* O Tipo de Faturamento da tarefa é Função por hora.

O Custo Orçamentado do projeto é calculado usando a fórmula abaixo se as seguintes condições forem atendidas:

* As Horas Planejadas das tarefas no projeto não correspondem às Horas Orçadas (no Planejador de Recursos)
* O Tipo de Faturamento das tarefas é Função por hora.

Quando as condições acima são atendidas, a Workfront calcula o Custo Orçado do projeto usando a seguinte fórmula:
<pre>Custo do Projeto Orçado = Custo da Mão-de-Obra Orçada + Custo da Despesa Orçada de todas as tarefas + Custo da Despesa Orçada do Projeto</pre>

#### Custo Efetivo {#actual-cost}

O Custo Real de um projeto é o custo associado ao trabalho real (Horas registradas) no projeto.

O Custo Real é calculado usando a seguinte fórmula:

```
Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project
```

Por exemplo, você tem as seguintes despesas na guia Expenses de uma tarefa: uma despesa de Marketing com um Custo Real de $110 e uma despesa Administrativa com um Custo Real de $40. Você seleciona o tipo de custo Função por hora e atribui a função de trabalho Consultor à tarefa. A taxa da função de consultor é de US$ 15 por hora e há 6 horas registradas na tarefa para a função de Consultor. Há uma despesa de Consultoria associada ao projeto (na guia Despesas), com um Custo Real de $100 e um usuário com uma taxa de Custo por Hora de $20 em seus logs de perfil de usuário de 10 horas no projeto. Você também tem um Custo Fixo de $200 para o projeto.

O Custo Real do projeto é calculado da seguinte forma:

```
$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740
```

>[!NOTE]
>
>O Custo Real de Despesa do projeto é calculado da seguinte maneira:
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>Esses custos não são duplicados no cálculo de Custo Real. Por exemplo, se um Custo Fixo fizer parte do Custo de Despesa Real do projeto, ele não será adicionado separadamente ao Custo Real.

>[!NOTE]
>
>Ao registrar o tempo em um projeto, os seguintes cenários existem ao calcular o Custo Real da Mão de Obra para o projeto:
>
>* Por padrão, o Workfront usa a taxa de Custo por Hora do usuário para calcular o Custo Real da Mão de obra.
>* Se o usuário que está registrando a hora não estiver associado a nenhum custo, o Workfront usará a taxa de Custo por Hora da Função Principal do usuário.
>* Se o administrador da Workfront ativou a variável **Atribuir Funções de Trabalho a entradas de hora manualmente** na área Folhas de Horas e Preferências de Horas e o tempo de logon do usuário no projeto seleciona uma função diferente para associar a esse tempo, o Custo Real do projeto é calculado com base na função especificada quando as horas foram registradas. Para obter informações sobre como ativar o tempo de registro para uma função de trabalho específica, consulte o artigo [Configurar preferências de hora e folha de ponto](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).


### Como a Workfront calcula os Tipos de Custo para tarefas {#how-workfront-calculates-cost-types-for-tasks}

O Custo Planejado e Real das tarefas e seus Custos de Mão-de-Obra são determinados pelo Tipo de Custo de cada tarefa.

Você pode configurar o Tipo de custo para tarefas individuais no projeto. Cada tipo de custo afeta os valores de Custo Planejado e Custo Real.

Para obter informações sobre como modificar o Tipo de Custo de uma tarefa, consulte [Atualizar Tipo de Custo da Tarefa](../../../manage-work/tasks/task-information/update-task-cost-type.md).

A tabela a seguir descreve a tarefa disponível Tipos de Custo no Workfront:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo de Custo da Tarefa</strong> </p> </th> 
   <th> <p><strong>Descrição</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Horas por Valor da Hora do Recurso</p> </td> 
   <td> <p>Esse é o Tipo de Custo padrão ao criar uma tarefa.</p> <p><strong>Custo Planejado</strong> é calculada pela seguinte fórmula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Quando o Custo da Mão de obra Planejada for calculado por:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Nota:   <p>Considere os seguintes impactos de usar o Tipo de Custo por Hora do Usuário e calcular o Custo Planejado:</p> 
     <ul> 
      <li>Se você atribuir vários recursos a uma tarefa, o Workfront ajusta cálculos para o Custo Planejado com base na porcentagem da tarefa atribuída a cada recurso.</li> 
      <li>O valor do campo Custo Planejado pode ser diferente dependendo se você exibir o Custo Planejado da própria tarefa ou do relatório Utilização.<br><strong>Ao exibir o Custo Planejado da própria tarefa:</strong> O campo Custo Planejado considera o conjunto de campos Custo/Hora no nível da Função da Ordem de Produção (quando o campo Custo/Hora não tiver sido definido no nível do usuário).<br><strong>Ao exibir o Custo Planejado do relatório Utilização no projeto:</strong> O campo Custo Planejado não leva em consideração o campo Custo/Hora definido no nível Função da Ordem de Produção. Em vez disso, se desejar que o relatório Utilização considere o campo Custo/Hora definido no nível Função da Ordem de Produção, você deve definir o Tipo de Custo na tarefa como Função por Hora. </li> 
     </ul> </p> <p><strong>Custo real</strong> é calculada pela seguinte fórmula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Quando o Custo Real da Mão-de-Obra é calculado por:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>Por exemplo, um usuário tem uma taxa de Custo por hora de US$ 20 em seu perfil. Quando eles registram 5 horas para uma tarefa, o Custo Real da Mão de Obra é de $100 para essa tarefa. Se o usuário não tiver uma taxa de Custo por Hora associada a ele, o Custo Real será calculado com base na taxa de Custo por Hora de sua Função de Trabalho Principal. Se eles não tiverem uma função de cargo ou a taxa de Custo por Hora da função de cargo não estiver definida, o Custo Real da tarefa será zero. </p> <p>Observação: Os Custos reais são calculados com base na taxa de Custo por hora do usuário que está registrando o tempo, independentemente de quem está atribuído à tarefa. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor da Hora do Perfil</p> </td> 
   <td> <p><strong>Custo Planejado</strong> é calculada pela seguinte fórmula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Onde o Custo da Mão de obra Planejada da Tarefa é calculado por:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Observação: Se você atribuir vários recursos a uma tarefa, o Workfront ajusta cálculos para as Horas Planejadas com base na porcentagem da tarefa atribuída a cada recurso.</p> <p><strong>Custo real</strong> é calculada pela seguinte fórmula: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Onde o Custo Real da Mão de obra da Tarefa é calculado por:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Por exemplo, uma tarefa é atribuída a uma função de trabalho ou a um usuário com uma função de trabalho para a qual a taxa de Custo por Hora é de $20. Quando um usuário faz 5 horas por uma tarefa, o Custo Real da Mão de Obra é de $100 por essa tarefa. Se o usuário atribuído à tarefa não tiver uma função de trabalho associada a ela na tarefa, o Custo Real será calculado com base na taxa de Custo por Hora da Função de Trabalho Principal. Se eles não tiverem uma função de cargo ou a taxa de Custo por Hora da função de cargo não estiver definida, o Custo Real da tarefa será zero. </p> <p>Nota:   <p> As Horas Reais de uma Tarefa de Função por Hora calculam com base nas funções de trabalho dos usuários associados à tarefa, não nas funções associadas ao usuário que está registrando o tempo.</p> <p>Se o administrador da Workfront ativou a variável <strong>Atribuir Funções de Trabalho a entradas de hora manualmente</strong> na área Folhas de Horas e Preferências de Horas, e o tempo de log do usuário na tarefa seleciona uma função diferente para associar a esse tempo, o Custo Real de uma Função Por Hora calcula com base na função especificada quando as horas eram registradas. Para obter informações sobre como ativar o tempo de registro para uma função de trabalho específica, consulte o artigo <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurar preferências de hora e folha de ponto</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor de Hora Fixo</p> </td> 
   <td> <p><strong>Custo Planejado</strong> é calculada pela seguinte fórmula:</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Onde o Custo da Mão-de-Obra da Tarefa é calculado por:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Custo real</strong> é calculada pela seguinte fórmula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Onde o Custo Real da Mão-de-Obra é calculado por:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Esse tipo de custo não leva em conta usuários individuais ou funções de trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Sem Custo</p> </td> 
   <td> <p>Esse Tipo de Custo não afeta Custos. Se uma tarefa pai tiver esse Tipo de Custo, as subtarefas com outro Tipo de Custo serão calculadas de acordo com seus Tipos de Custo individuais e o Custo da tarefa pai será afetado adequadamente. </p> <p>Quando um usuário sem acesso a dados financeiros ou um usuário sem permissões financeiras em um modelo cria um projeto a partir desse modelo, esse é o Tipo de custo padrão para as tarefas no projeto.</p> <p>Para obter informações sobre o acesso a Dados Financeiros, consulte o artigo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acesso aos dados financeiros</a>.</p> <p>Para obter informações sobre permissões financeiras em objetos, consulte o artigo <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Compartilhar permissões financeiras em um objeto</a>.</p> <p>Para obter informações sobre como criar projetos a partir de modelos, consulte o artigo <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Criar um projeto usando um modelo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because this was moved to its own how-to article linked above. Could be removed after some time.) </p>
<p>To configure the Cost Type of an individual task:</p>
<ol>
<li value="1">Go to the task where you want to configure the Cost Type. </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then expand the <strong>Finance</strong> area. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Double click <strong>Cost Type</strong> and select the cost type that you want to apply to the task. </p> </li>
<li value="4">Click <strong>Save.</strong></li>
</ol>
</div>
-->

## Como o Workfront acompanha os custos de problemas {#how-workfront-tracks-costs-for-issues}

Problemas não afetam os seguintes tipos de custos em um projeto e não os afetam:

* Custo Planejado
* Custo Orçado

Problemas podem, no entanto, ter uma **Custo real** que também afeta o custo real do projeto.

A tabela a seguir explica como o Custo Real é calculado para problemas, dependendo do tipo de atribuição na emissão:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">Emitir Custo Real</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Atribuição de Usuário</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Custo real</strong> é calculada pela seguinte fórmula:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>A taxa de Custo por hora do usuário que está registrando o tempo é considerada aqui, independentemente de quem está atribuído ao problema. </p> <p>Se o usuário que registra a hora não tiver uma taxa de Custo por Hora em seu perfil, a taxa de Custo por Hora de sua Função de Trabalho Principal calculará o Custo Real do problema. Se o usuário que está registrando o horário não tiver nenhuma função em seu perfil ou taxa associada a ele, as Horas Reais serão calculadas usando a taxa de Custo por Hora da Função de Trabalho Principal do Destinatário Principal sobre o problema. Se essa função não tiver taxa definida, o Custo Real da emissão será zero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Atribuição de Função</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Custo real</strong> é calculada pela seguinte fórmula:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>A taxa de Custo por hora do usuário que registra o tempo no problema é considerada aqui, independentemente da função atribuída ao problema. </p> <p>Se o usuário que estiver registrando o tempo não tiver uma taxa de Custo por Hora associada a ele, a taxa de Custo por Hora de sua Função Principal calculará o Custo Real do problema.<br>Se o usuário que estiver registrando o horário não tiver nenhuma função em seu perfil ou taxa associada a ele, o Custo Real do problema será zero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Sem atribuição</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Custo real</strong> é calculada pela seguinte fórmula:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Se o usuário que registra a hora não tiver uma taxa de Custo por Hora associada ao perfil, a taxa de Custo por Hora da Função de Trabalho Principal calculará o Custo Real do problema. </p> <p>Se o usuário que está registrando o horário não tiver nenhuma função de trabalho associada ao perfil ou se a Função de Trabalho Principal não tiver uma taxa de Custo por Hora definida, o Custo Real do problema será zero. </p> </td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td colspan="4"> 
    <div> <MadCap:conditionalText data-mc-conditions="">
       If your Workfront administrator enabled the 
      <strong>Assign Job Roles to hour entries manually</strong> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the issue selects a different role to associate with this time, the Actual Cost of the issue calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article 
      <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>. 
     </MadCap:conditionalText> 
    </div> </td> 
  </tr> 
  -->
 </tbody> 
</table>
