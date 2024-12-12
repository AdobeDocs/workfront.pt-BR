---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Acompanhar Custos
description: Você pode rastrear custos de projetos, tarefas e problemas no Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '2480'
ht-degree: 0%

---

# Rastrear custos

<!-- Audited: 02/2024 -->

Você pode rastrear custos de projetos, tarefas e problemas no Adobe Workfront.

## Como a Workfront calcula custos

Para rastrear custos, você deve associar usuários e funções de trabalho a taxas de custo por hora.

As taxas de custo por hora são quantias de custos por unidade de trabalho associadas a funções de trabalho ou usuários. Multiplicar as taxas pelas horas gastas no trabalho gera custos para seus projetos, tarefas ou problemas.

Existem os seguintes cenários:

* Se o Tipo de Custo de suas tarefas for Hora do Usuário, a taxa horária do usuário calculará os custos da tarefa e do projeto.

  Para obter informações sobre como associar usuários a taxas de custo, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Se o Tipo de Custo de suas tarefas for Função por hora, a taxa horária da função de trabalho calculará os custos da tarefa e do projeto.

  Para obter informações sobre como associar funções de trabalho a taxas de custo, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* O Workfront calcula somente o Custo Efetivo para ocorrências e as ocorrências não têm um Tipo de Custo. Para obter mais informações, consulte a seção [Como o Workfront rastreia os custos de problemas](#how-workfront-tracks-costs-for-issues) neste artigo.

>[!TIP]
>
>Não é possível substituir taxas de custo para projetos. Depois de estabelecer a taxa de custo por hora em um usuário ou função de trabalho, essa taxa calcula todos os custos no sistema.

## Índices de desempenho de custo do Workfront

O Workfront calcula vários índices de desempenho de custo para projetos para que os projetos possam ser rastreados com relação à eficiência de custo.\
Para obter mais informações sobre o cálculo de índices de custo-desempenho, consulte:

* [Calcular Índice de Desempenho de Custo (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Calcular CSI (Índice de Desempenho de Agendamento de Custos)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Calcular Índice de Desempenho de Agendamento (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Como o Workfront rastreia custos de tarefas e projetos

Os tipos de custos são calculados de forma diferente para tarefas e para projetos.

### Como o Workfront rastreia custos {#how-workfront-tracks-costs}

É possível rastrear vários tipos de custos para tarefas e projetos no Workfront. Os custos gerais são calculados pela seguinte fórmula:

`Costs = Labor Costs + Expense Costs`

* **Custos de mão de obra** estão associados às horas em tarefas e projetos e às taxas de Custo por hora dos recursos associados a tarefas. Geralmente, o Workfront calcula os seguintes custos de mão de obra:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Custos de trabalho planejados</td> 
     <td> <p>Elas são calculadas usando a seguinte fórmula:</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Custos de trabalho orçados</td> 
     <td> <p>Elas são calculadas usando a seguinte fórmula:</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Custos Reais do Trabalho</td> 
     <td> <p>Elas são calculadas usando a seguinte fórmula:</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> </td> 
    </tr> 
   </tbody> 
  </table>

  Para obter mais informações, consulte a seção [Como o Workfront calcula os custos planejados, orçados e reais](#how-workfront-calculates-planned-budgeted-and-actual-costs) neste artigo.

* **Custos de Despesas** estão associados a despesas em projetos e tarefas.\
  Ao criar um projeto, você pode definir despesas planejadas para todo o projeto. Além disso, você pode associar despesas a tarefas novas ou existentes. Para obter informações, consulte [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Custos fixos** são definidos como uma quantidade fixa de custo para um projeto. Isso é parte do Custo planejado do projeto, que representa a quantidade de dinheiro necessária para concluir o projeto.

  >[!TIP]
  >
  >Ao anexar um modelo a um projeto, o Custo Fixo de um modelo é adicionado ao Custo Fixo do projeto. Para obter informações, consulte [Visão geral de anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Como o Workfront calcula os custos planejados, orçados e reais {#how-workfront-calculates-planned-budgeted-and-actual-costs}

O Workfront calcula o Custo Planejado e o Custo Efetivo para cada tarefa individual em um projeto. O Workfront usa esses cálculos para tarefas individuais para calcular o Custo Planejado e o Custo Efetivo do projeto.

#### Custo Planejado {#planned-cost}

O Custo Planejado de um projeto é o custo associado ao trabalho planejado (Horas Planejadas) no projeto.

O Custo Planejado de um projeto é calculado pela seguinte fórmula:

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

Por exemplo, você tem as seguintes despesas na guia Despesas de uma tarefa: uma despesa de US$ 100 Marketing e uma despesa administrativa de US$ 50. Na guia Finanças, você seleciona o tipo de custo de Hora em hora do usuário. Um usuário é atribuído à tarefa e a taxa horária do usuário é de US$ 15. O usuário é designado para trabalhar 5 horas nesta tarefa. Na guia Expenses (Despesas) do projeto, você tem um custo planejado de US$ 100 para uma despesa chamada Consulting. Você também tem um custo fixo de US$ 200 para o projeto.

O Custo Planejado do projeto é calculado da seguinte maneira:

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

A taxa horária na fórmula considera quaisquer alterações de data de efetivação da taxa.

#### Custo Orçado {#budgeted-cost}

O Custo Orçado de um projeto é o custo associado ao trabalho orçado (Horas Orçadas) no projeto.

O Custo Orçado do projeto é o mesmo que o Custo Planejado do projeto se as duas condições a seguir forem atendidas:

* As horas planejadas das tarefas no projeto correspondem às horas orçadas (no Planejador de recursos).
* O tipo de faturamento das tarefas é Função por hora.

O Custo Orçado do projeto é calculado usando a fórmula abaixo, se as seguintes condições forem atendidas:

* As horas planejadas das tarefas no projeto não correspondem às horas orçadas (no Planejador de recursos).
* O tipo de faturamento das tarefas é Função por hora.

Quando as condições acima são atendidas, o Workfront calcula o Custo orçado do projeto usando a seguinte fórmula:

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### Custo Efetivo {#actual-cost}

O Custo Real de um projeto é o custo associado ao trabalho real (Horas registradas) no projeto.

O Custo Real é calculado usando a seguinte fórmula:

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

Por exemplo, você tem as seguintes despesas na guia Despesas de uma tarefa: uma despesa de Marketing com um Custo Efetivo de $110, e uma despesa Administrativa com um Custo Efetivo de $40. Você seleciona o tipo de custo Função por hora e atribui a função de trabalho Consultor à tarefa. A taxa da função de trabalho do consultor é de US$ 15 por hora e há 6 horas registradas na tarefa para a função de trabalho Consultor. Há uma despesa de Consultoria associada ao projeto (na guia Despesas ), com um Custo real de US$ 100 e um usuário com uma taxa de Custo por hora de US$ 20 em seus registros de perfil de usuário de 10 horas no projeto. Você também tem um custo fixo de US$ 200 para o projeto.

O Custo Efetivo do projeto é calculado da seguinte forma:

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

A taxa horária na fórmula considera quaisquer alterações de data de efetivação da taxa.

>[!NOTE]
>
>O Custo Efetivo de Despesas do projeto é calculado da seguinte forma:
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>Esses custos não são duplicados no cálculo do Custo Real. Por exemplo, se um Custo Fixo é parte do Custo Efetivo de Despesas do projeto, ele não é adicionado separadamente ao Custo Efetivo.

>[!NOTE]
>
>Ao registrar o tempo em um projeto, os seguintes cenários existem ao calcular o Custo Efetivo do Trabalho para o projeto:
>
>* Por padrão, o Workfront usa a taxa de Custo por hora do usuário para calcular o Custo Efetivo do Trabalho.
>* Se o usuário que registra a hora não estiver associado a nenhum custo, o Workfront usará a taxa Custo por hora da função principal do usuário.
>* Se o administrador do Workfront habilitou a configuração **Atribuir funções de trabalho a entradas de hora manualmente** na área Preferências de folhas de horas e horas da Configuração e o tempo de logon do usuário no projeto seleciona uma função diferente para associar a esse tempo, o Custo Efetivo do projeto é calculado com base na função especificada quando as horas foram registradas. Para obter informações sobre como habilitar o tempo de log para uma função de trabalho específica, consulte o artigo [Configurar preferências de horas e folha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

### Como o Workfront calcula os tipos de custo para tarefas {#how-workfront-calculates-cost-types-for-tasks}

O Custo Planejado e Efetivo das tarefas e seus Custos de Mão-de-Obra são determinados pelo Tipo de Custo de cada tarefa.

Você pode configurar o Tipo de custo para tarefas individuais dentro do projeto. Cada tipo de custo afeta os valores de Custo Planejado e Custo Efetivo.

Para obter informações sobre como modificar o Tipo de Custo de uma tarefa, consulte [Atualizar Tipo de Custo da tarefa](../../../manage-work/tasks/task-information/update-task-cost-type.md).

A tabela a seguir descreve os Tipos de Custo da tarefa disponíveis no Workfront:

<table style="table-layout:auto">
 <col> 
 <col> 
<tbody> 
  <tr> 
   <td> <p><strong>Tipo de Custo da Tarefa</strong> </p> </td> 
   <td> <p><strong>Descrição</strong> </p> </td> 
  </tr>
  <tr> 
   <td> <p>Horas por Valor da Hora do Recurso</p> </td> 
   <td> <p>Esse é o Tipo de Custo padrão quando você cria uma tarefa.</p> <p>O <strong>Custo Planejado</strong> é calculado pela seguinte fórmula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Onde o Custo de Trabalho Planejado é calculado por:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Nota: <p>Considere os seguintes impactos do uso do Tipo de Custo por Hora do Usuário e do cálculo do Custo Planejado:</p> 
     <ul> 
      <li>Se você atribuir vários recursos a uma tarefa, o Workfront ajustará cálculos para o Custo Planejado com base na porcentagem da tarefa atribuída a cada recurso.</li>
      <li>Para taxas de custo de efetivação da data, o custo de Trabalho Planejado é a soma dos custos planejados de cada período coberto na tarefa.</li>
      <li>O valor do campo Custo Planejado pode diferir dependendo se você exibe o Custo Planejado da própria tarefa ou do relatório de Utilização.<br><strong>Ao exibir o Custo Planejado da própria tarefa:</strong> o campo Custo Planejado leva em consideração o campo Custo/Hr definido no nível da Função de Trabalho (quando o campo Custo/Hr não foi definido no nível do usuário).<br><strong>Ao exibir o Custo Planejado do relatório de Utilização no projeto:</strong> o campo Custo Planejado não leva em consideração o campo Custo/Hr definido no nível de Função de Trabalho. Em vez disso, se você quiser que o relatório de Utilização considere o campo Custo/Hr definido no nível de Função do Cargo, defina o Tipo de Custo na tarefa como Função por Hora. </li> 
     </ul> </p> <p>O <strong>Custo Efetivo</strong> é calculado pela seguinte fórmula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Onde o Custo Efetivo do Trabalho é calculado por:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>Por exemplo, um usuário tem uma taxa de Custo por hora de US$ 20 em seu perfil. Quando registram 5 horas para uma tarefa, o Custo de Mão de Obra Real é de US$ 100 para essa tarefa. Se o usuário não tiver uma taxa de Custo por hora associada a ele, o Custo real será calculado com base na taxa de Custo por hora da função de trabalho principal. Se eles não tiverem uma função de trabalho ou se a taxa de Custo por hora de sua função de trabalho não estiver definida, o Custo Real da tarefa será zero. </p> <p>Nota: Os Custos Reais são calculados com base na taxa de Custo por Hora do usuário que está registrando o tempo, independentemente de quem está atribuído à tarefa. Além disso, a taxa horária de faturamento na fórmula considera quaisquer alterações de data de efetivação da taxa.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor da Hora do Perfil</p> </td>
   <td> <p>O <strong>Custo Planejado</strong> é calculado pela seguinte fórmula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Onde o Custo de Trabalho Planejado da Tarefa é calculado por:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Nota: Se você atribuir vários recursos a uma tarefa, o Workfront ajustará cálculos para Horas Planejadas com base na porcentagem da tarefa atribuída a cada recurso. Além disso, a taxa horária na fórmula considera quaisquer alterações de data de efetivação da taxa.</p> <p>O <strong>Custo Efetivo</strong> é calculado pela seguinte fórmula: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Onde o Custo Efetivo do Trabalho da Tarefa é calculado por:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Por exemplo, uma tarefa é atribuída a uma função de trabalho ou a um usuário com uma função de trabalho para a qual a taxa de Custo por hora é de $20. Quando um usuário registra 5 horas para uma tarefa, o Custo Efetivo da Mão-de-Obra é de US$ 100 para essa tarefa. Se o usuário atribuído à tarefa não tiver uma função de trabalho associada a ele na tarefa, o Custo Efetivo será calculado com base na taxa de Custo por Hora da Função de Trabalho Principal. Se eles não tiverem uma função de trabalho ou se a taxa de Custo por hora de sua função de trabalho não estiver definida, o Custo Real da tarefa será zero. </p> <p>Observação: as Horas Reais de uma tarefa de Função por Hora são calculadas com base nas funções de trabalho dos usuários associados à tarefa, não nas funções associadas ao usuário que está registrando o horário. Além disso, a taxa horária de faturamento na fórmula considera quaisquer alterações de data de efetivação da taxa.</p> <p>Se o administrador do Workfront habilitou a configuração <strong>Atribuir funções de trabalho a entradas de hora manualmente</strong> na área Preferências de folhas de horas e horas na Configuração e o tempo de logon do usuário na tarefa seleciona uma função diferente para associar a esse tempo, o Custo real de uma função por hora da tarefa é calculado com base na função especificada quando as horas foram registradas. Para obter informações sobre como habilitar o tempo de log para uma função de trabalho específica, consulte o artigo <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurar preferências de horas e folha de horas</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor de Hora Fixo</p> </td> 
   <td> <p>O <strong>Custo Planejado</strong> é calculado pela seguinte fórmula:</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Onde o Custo de Mão-de-Obra da Tarefa é calculado por:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p>O <strong>Custo Efetivo</strong> é calculado pela seguinte fórmula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Onde o Custo Efetivo da Mão-de-Obra da Tarefa é calculado por:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Esse tipo de custo não considera usuários individuais ou funções de trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Sem Custo</p> </td> 
   <td> <p>Esse Tipo de Custo não afeta custos. Se uma tarefa-pai tiver esse Tipo de Custo, as subtarefas com outro Tipo de Custo serão calculadas de acordo com seus Tipos de Custo individuais, e o custo da tarefa-pai será afetado adequadamente. </p> <p>Quando um usuário sem acesso a dados financeiros ou um usuário sem permissões financeiras em um modelo cria um projeto a partir desse modelo, esse é o Tipo de Custo padrão para as tarefas no projeto.</p> <p>Para obter informações sobre acesso a Dados Financeiros, consulte o artigo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acesso a dados financeiros</a>.</p> <p>Para obter informações sobre permissões financeiras em objetos, consulte o artigo <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Compartilhar permissões financeiras em um objeto</a>.</p> <p>Para obter informações sobre como criar projetos a partir de modelos, consulte o artigo <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Criar um projeto usando um modelo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Como o Workfront rastreia custos de problemas {#how-workfront-tracks-costs-for-issues}

Os problemas não têm e não afetam os seguintes tipos de custos em um projeto:

* Custo Planejado
* Custo Orçado

Problemas, no entanto, podem ter um **Custo Efetivo**, o que também afeta o Custo Efetivo do projeto.

A tabela a seguir explica como o Custo Efetivo é calculado para ocorrências, dependendo do tipo de atribuição na ocorrência:

<table style="table-layout:auto"> 
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td> <p>Atribuição de usuário</p> <p> </p> </td> 
   <td colspan="3"> <p>O <strong>Custo Efetivo</strong> é calculado pela seguinte fórmula:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>A taxa de custo por hora do usuário que está registrando o tempo é considerada aqui, independentemente de quem está atribuído ao problema. </p> <p>Se o usuário que registra o tempo não tiver uma taxa de Custo por hora em seu perfil, a taxa de Custo por hora de sua função de trabalho principal calcula o Custo real do problema.</p> <p>Se o usuário que está registrando o horário não tiver função em seu perfil ou nenhuma taxa associada a ele, as Horas efetivas serão calculadas usando a taxa de Custo por hora da Função de trabalho principal da Destinatária principal na ocorrência. Se essa função não tiver uma taxa definida, o custo real do problema será zero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Atribuição de Função</p> <p> </p> </td> 
   <td colspan="3"> <p>O <strong>Custo Efetivo</strong> é calculado pela seguinte fórmula:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>A taxa de custo por hora do usuário que registra o tempo na ocorrência é considerada aqui, independentemente da função atribuída à ocorrência. </p> <p>Se o usuário que registra a hora não tiver uma taxa de Custo por hora associada a ele, a taxa de Custo por hora da função principal calcula o Custo real do problema.</p><p>Se o usuário que está registrando o horário não tiver função em seu perfil ou nenhuma taxa associada a ele, o custo real do problema será zero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Sem atribuição</p> <p> </p> </td> 
   <td colspan="3"> <p>O <strong>Custo Efetivo</strong> é calculado pela seguinte fórmula:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Se o usuário que registra a hora não tiver uma taxa de Custo por hora associada ao perfil, a taxa de Custo por hora da função de trabalho principal calcula o Custo real da ocorrência. </p> <p>Se o usuário que está registrando o tempo não tiver nenhuma função de trabalho associada ao seu perfil ou se a Função de trabalho principal não tiver uma taxa de Custo por hora definida, o Custo real do problema será zero. </p> </td> 
  </tr> 
 </tbody> 
</table>
