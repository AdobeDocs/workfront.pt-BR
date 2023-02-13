---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral das Horas Planejadas
description: As Horas Planejadas associadas a uma tarefa, ocorrência ou projeto representam o tempo necessário para os usuários atribuídos concluírem a tarefa, emissão ou projeto.
author: Alina
feature: Work Management
exl-id: 0b86c760-691a-436e-9beb-31e9ac36440a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2888'
ht-degree: 0%

---

# Visão geral das Horas Planejadas

As Horas Planejadas associadas a uma tarefa, ocorrência ou projeto representam o tempo necessário para os usuários atribuídos concluírem a tarefa, emissão ou projeto.

## Considerações sobre as horas planejadas no Adobe Workfront

* As Horas Planejadas são associadas principalmente aos itens de trabalho (tarefas e problemas) no Adobe Workfront. As Horas Planejadas dos itens de trabalho são acumuladas até as Horas Planejadas de seus projetos.
* Por padrão, o Workfront distribui a tarefa e emite as Horas Planejadas igualmente para todos os dias na Duração da tarefa ou do problema.
* Quando os usuários e as funções são atribuídos a tarefas e problemas, as Horas Planejadas das tarefas e problemas são associadas às atribuições de usuário ou função.
* Você deve definir o valor de Horas Planejadas para tarefas e problemas se quiser usar as ferramentas de Gerenciamento de Recursos no Workfront.
* Você pode modificar o valor de Horas Planejadas em tarefas somente para alguns Tipos de Duração.

   Para obter mais informações sobre como modificar Horas Planejadas em tarefas relacionadas ao Tipo de Duração das tarefas, consulte a seção [Atualizar a tarefa Horas Planejadas com base no Tipo de Duração](#update-task-planned-hours-based-on-duration-type) neste artigo.

* Você pode modificar o valor de Horas Planejadas em problemas a qualquer momento.
* Não é possível modificar o valor de Horas Planejadas de projetos ou tarefas pai, pois elas são um total calculado de todas as Horas Planejadas de todas as suas tarefas e subtarefas.
* O gerenciamento de alocações de usuários usando ferramentas de gerenciamento de recursos pode alterar o número de Horas Planejadas de tarefas, problemas, projetos e as atribuições associadas aos itens de trabalho.

## Horas Planejadas em Tarefas x Horas Planejadas em Projetos {#planned-hours-on-tasks-vs-planned-hours-on-projects}

Horas Planejadas das tarefas acumuladas até as Horas Planejadas do projeto. As Horas Planejadas dos problemas nem sempre se acumulam nas Horas Planejadas do projeto.

Esta seção descreve as diferenças entre a tarefa e as Horas Planejadas do projeto. Também descreve onde você pode visualizar o problema Horas Planejadas que são acumuladas no projeto.

* [Horas Planejadas em Tarefas](#planned-hours-on-tasks)
* [Horas previstas em projetos](#planned-hours-on-projects)

### Horas Planejadas em Tarefas {#planned-hours-on-tasks}

As Horas Planejadas de uma tarefa indicam a quantidade de tempo estimado que o trabalho real na tarefa pode demorar. Por padrão, o Workfront distribui a quantidade total de horas planejadas uniformemente para cada dia dentro da duração de cada tarefa. A quantidade diária de horas planejadas se torna as alocações diárias da tarefa. Se a tarefa for atribuída a vários recursos, cada recurso receberá uma quantidade igual de horas diárias, por padrão.

Usando o Balanceador de Carga de Trabalho, você pode modificar as alocações diárias dos usuários atribuídos às tarefas. Isso também pode atualizar as Horas Planejadas da tarefa quando o Tipo de Duração da tarefa for Simples. Para obter mais informações, consulte a seção &quot;Atualizar tarefa Horas Planejadas ao gerenciar alocações de usuários&quot; no artigo [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Quando uma tarefa contém subtarefas, as Horas Planejadas da tarefa pai são a soma de todas as Horas Planejadas em qualquer subtarefa. Não é possível atualizar as Horas Planejadas de uma tarefa pai.

>[!NOTE]
>
>Ao contrário das Horas Planejadas, as Horas Reais em uma tarefa pai são horas registradas diretamente na tarefa pai. Eles não representam uma soma das Horas Reais das tarefas filho.\
>Para obter mais informações sobre Horas Reais, consulte [Exibir Horas Reais](../../../manage-work/tasks/task-information/actual-hours.md).

### Horas previstas em projetos {#planned-hours-on-projects}

Não é possível editar a quantidade de Horas Planejadas em um projeto. As Horas Planejadas em um projeto são uma soma calculada de todas as Horas Planejadas de todas as tarefas no projeto.

Se os problemas são incluídos no cálculo para Horas Planejadas depende do local no projeto em que você está visualizando Horas Planejadas. Você pode visualizar o projeto Horas Planejadas nos seguintes locais em um projeto:

* **Detalhes do projeto** **seção** ****e **Editar projeto**caixa **:**Somente as Horas Planejadas para as tarefas do projeto são consideradas. As Horas Planejadas para os problemas no projeto não são consideradas ao visualizar o número total de Horas Planejadas para o projeto na seção Detalhes do projeto ou na caixa Editar projeto .

* **O **Balanceador de carga de trabalho: Somente as Horas Planejadas associadas às tarefas visíveis no Balanceador de Carga de Trabalho são exibidas no Balanceador de Carga de Trabalho para projetos. As alocações diárias do usuário podem alterar o projeto diariamente Horas Planejadas no Balanceador de Carga de Trabalho.
* **Seção de utilização :** As Horas Planejadas associadas aos usuários atribuídos às tarefas e os problemas no projeto são considerados ao visualizar o número total de Horas Planejadas para o projeto na seção Utilização .
* **Painel de alocação de funções** na lista de tarefas : As Horas Planejadas para as tarefas e os problemas no projeto que são atribuídos a uma função de trabalho ou a um usuário associado a uma função de trabalho são exibidos nesta área. As Horas Planejadas associadas a tarefas e problemas que não foram atribuídos ou atribuídos a equipes não são exibidas nessa área. Para obter mais informações, consulte [Visualizar horas planejadas do projeto no painel Alocação de funções](../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md).

## Distribuição de Horas Planejadas durante a Duração de uma tarefa

Por padrão, o Workfront distribui as Horas Planejadas uniformemente na Duração de uma tarefa, alocando um número igual de Horas Planejadas para cada dia da tarefa, de acordo com a disponibilidade do agendamento do projeto.

Por exemplo, se uma tarefa estiver definida para iniciar às 16 horas e o agendamento tiver uma hora restante no primeiro dia da tarefa, o Workfront colocará uma Hora planejada no primeiro dia da tarefa Duração e dividirá o restante das Horas planejadas igualmente entre o resto dos dias na tarefa Duração.

>[!NOTE]
>
>As Horas Planejadas por Dia ou a alocação diária é a alocação de Horas Planejadas para cada dia durante a Duração da tarefa. Se a tarefa tiver uma atribuição, esse número representa as Horas Planejadas por Dia por atribuição. Se a tarefa tiver várias atribuições, as Horas Planejadas por Dia por atribuição serão diferentes das Horas Planejadas por Dia para a tarefa. Não há representação visual no Workfront para as Horas Planejadas por Dia por atribuição, para tarefas com várias atribuições.

 

## Localizar e entender os valores de Horas Planejadas

Você pode encontrar valores de Horas Planejadas em várias áreas do Workfront. 

O número de Horas Planejadas exibidas é originário dos itens de trabalho no projeto ou é calculado de forma diferente, dependendo da área e do objeto em que você os exibe.

Você pode localizar Horas Planejadas nas seguintes áreas do Workfront:

* [A seção Detalhes de um projeto, tarefa ou problema](#the-details-section-of-a-project-task-or-issue)
* [A caixa Editar tarefa ou Editar ocorrência](#the-edit-task-or-edit-issue-box)
* [Relatórios](#reports)
* [As áreas de agendamento](#the-scheduling-areas)
* [O Balanceador de Carga de Trabalho](#the-workload-balancer)
* [O Planejador de recursos](#the-resource-planner)
* [O relatório Utilização](#the-utilization-report)
* [O painel Alocação de funções](#The%C2%A0Role)

### A seção Detalhes de um projeto, tarefa ou problema {#the-details-section-of-a-project-task-or-issue}

![](assets/planned-hours-on-details-for-project-nwe-350x138.png)

As Horas Planejadas na seção Detalhes de uma tarefa, emissão ou projeto são o total de Horas Planejadas associado ao respectivo item.

Para obter mais informações sobre as Horas Planejadas do projeto, consulte o [Horas Planejadas em Tarefas x Horas Planejadas em Projetos](#planned-hours-on-tasks-vs-planned-hours-on-projects) neste artigo.

### A caixa Editar tarefa ou Editar ocorrência {#the-edit-task-or-edit-issue-box}

![](assets/planned-hours-on-edit-task-box-nwe-350x70.png)

As Horas Planejadas na caixa Editar de uma tarefa ou emissão são o total de Horas Planejadas do respectivo item.

Para obter mais informações sobre as Horas Planejadas do projeto, consulte o [Horas Planejadas em Tarefas x Horas Planejadas em Projetos](#planned-hours-on-tasks-vs-planned-hours-on-projects) neste artigo.

Para tarefas, você pode editar a quantidade de Horas Planejadas somente para determinados Tipos de Duração. Para obter mais informações, consulte [Atualizar a tarefa Horas Planejadas com base no Tipo de Duração](#update-task-planned-hours-based-on-duration-type) neste artigo.

Você pode exibir a alocação individual de Horas Planejadas para cada usuário ou função de trabalho atribuída à tarefa ou ocorrência na área Atribuições.

### Relatórios {#reports}

![](assets/planned-hours-on-task-repot-nwe-350x99.png)

Você pode adicionar o campo Horas Planejadas no projeto, na tarefa e nos relatórios de emissão.

A coluna Horas Planejadas é incluída na exibição Padrão de uma lista de tarefas, por padrão.

As Horas Planejadas em uma tarefa, edição ou relatório de projeto são o total de Horas Planejadas do respectivo item, conforme são exibidas na seção Detalhes ou na caixa Editar dos itens.

Para obter informações sobre como criar relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

>[!NOTE]
>
>Se você criar um relatório de Projeto (Dados Financeiros) e o agrupar por data, as Horas Planejadas poderão exibir uma parte das Horas Planejadas do projeto, dependendo da linha do tempo das tarefas no projeto. Por padrão, o Workfront distribui as Horas Planejadas de tarefas igualmente para cada dia da Duração da tarefa. As Horas Planejadas de um determinado período correspondem à distribuição igual definida pelo Workfront para esse período no relatório Projeto (Dados Financeiros).

### As áreas de agendamento  {#the-scheduling-areas}

![](assets/task-detail-expanded-in-scheduler-with-planned-hours-and-adjusted-daily-allocations-nwe-350x323.png)

As Horas Planejadas para tarefas e problemas são exibidas nas áreas de Agendamento no campo Horas Planejadas .

Você pode visualizar a alocação diária de Horas Planejadas para cada usuário atribuído a uma tarefa ou a um problema nas áreas de Agendamento.

O valor da hora diária representa um dos seguintes itens: 

* o valor padrão igualmente distribuído pela Workfront para cada dia da Duração das tarefas ou emissões
* a alocação diária ajustada gerenciada pelos gerentes de recursos.

   Para obter informações sobre como ajustar alocações diárias nas ferramentas de Agendamento, consulte [Gerenciar alocações de usuários nas áreas de Agendamento](../../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

### O Balanceador de Carga de Trabalho {#the-workload-balancer}

![](assets/planned-hours-on-wb-expanded-with-pti-info-nwe-350x114.png)

As seguintes Horas Planejadas para tarefas, problemas e projetos são exibidas no Balanceador de Carga de Trabalho à direita da tarefa, do problema ou do nome do projeto:

* Para tarefas e problemas, as Horas Planejadas associadas a elas são exibidas.
* Para projetos, um total de Horas Planejadas das tarefas e problemas visíveis na tela é exibido.

   >[!TIP]
   O Balanceador de Carga de Trabalho não exibe todas as Horas Planejadas de um projeto como visíveis na área Detalhes do projeto.

Você pode visualizar a alocação diária de Horas Planejadas para cada usuário atribuído a uma tarefa ou a um problema no Balanceador de Carga de Trabalho.

A quantidade diária de Horas Planejadas representa um dos seguintes itens: 

* o valor padrão igualmente distribuído pela Workfront para cada dia da Duração das tarefas, emissões ou do projeto
* a alocação diária ajustada gerenciada pelos gerentes de recursos.

   Para obter informações sobre como ajustar alocações diárias no Balanceador de Carga de Trabalho , consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

### O Planejador de recursos {#the-resource-planner}

![](assets/planned-hours-on-all-objects-in-resource-planned-expanded-nwe-350x204.png)

O Planejador de Recursos exibe Horas Planejadas para projetos, tarefas, problemas.

Você pode exibir alocações semanais de Horas Planejadas para os usuários e funções de cargo associadas aos itens de trabalho na coluna PLN do Planejador de Recursos.

>[!TIP]
Os ajustes diários de alocação no Balanceador de Carga de Trabalho influenciam as alocações semanais para tarefas e problemas no Planejador de Recursos.

O número de Horas Planejadas para cada objeto varia de acordo com a exibição aplicada ao Planejador de Recursos. Para obter mais informações, consulte [Visão geral de horas, FTE e informações de custo nas exibições Projeto e Função do Planejador de Recursos](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

A quantidade semanal de horas planejadas de tarefas e problemas representa um dos seguintes: 

* o valor semanal padrão igualmente distribuído pela Workfront para cada dia da Duração das tarefas ou emissões
* a alocação semanal ajustada gerenciada pelos gerentes de recursos no Balanceador de Carga de Trabalho.

   Para obter informações sobre como ajustar alocações diárias no Balanceador de Carga de Trabalho , consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

O valor semanal para projetos, usuários e funções é influenciado pelas quantidades semanais de Horas Planejadas para as tarefas e problemas associados a elas.

### O relatório Utilização {#the-utilization-report}

As Horas Planejadas do projeto são aquelas associadas às atribuições em cada tarefa e emissão.

>[!IMPORTANT]
Observe que as Horas Planejadas no relatório Utilização estão associadas às atribuições e não às próprias tarefas e problemas. As Horas Planejadas no relatório Utilização nem sempre correspondem às Horas Planejadas nas tarefas e problemas do projeto. No entanto, as Horas Planejadas correspondem às horas associadas às atribuições em tarefas e problemas.

Você pode exibir os seguintes tipos de Horas Planejadas no relatório Utilização:

* o total de Horas Planejadas de todas as atribuições no projeto durante a vida geral dos projetos incluídos
* o total de Horas Planejadas de todas as atribuições somente para o intervalo de datas especificado (você pode especificar uma semana ou um mês individual).

   Quando a alocação diária do usuário para horas tiver sido ajustada usando o Balanceador de Carga de Trabalho, as Horas Planejadas para um intervalo de datas específico podem ser afetadas se as datas selecionadas no relatório Utilização contiverem apenas uma parte da Duração de uma tarefa ou ocorrência. Para obter informações sobre como ajustar alocações diárias para usuários, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Para obter mais informações, consulte [Exibir informações de utilização de recursos](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

### O painel Alocação de funções

As Horas Planejadas no painel Alocação de Função representam o número de Horas Planejadas associadas a cada função de trabalho atribuída às tarefas ou problemas no projeto durante a duração total do projeto. O número corresponde à função Horas Planejadas do Planejador de Recursos.

>[!TIP]
Observe que as Horas Planejadas associadas aos usuários não são exibidas no painel Alocação de função .

Para obter mais informações, consulte [Mostrar alocação de função para projetos e iniciativas no Balanceador de Carga de Trabalho](../../../scenario-planner/show-role-allocation-workload-balancer.md).

## Atualizar a tarefa Horas Planejadas com base no Tipo de Duração {#update-task-planned-hours-based-on-duration-type}

Você pode atualizar o total de Horas Planejadas nas tarefas ao editar tarefas somente se as tarefas tiverem um determinado Tipo de Duração.

Os seguintes cenários existem:

* Você pode modificar Horas Planejadas para tarefas somente ao usar a Atribuição Calculada ou os Tipos de Duração Simples ao editar uma tarefa.

   Para obter mais informações sobre o Tipo de Duração da Atribuição Calculada, consulte [Visão geral do Tipo de duração: Atribuição calculada](../../../manage-work/tasks/taskdurtn/calculated-assignment.md).

   Para obter mais informações sobre o Tipo de duração simples, consulte [Visão geral do Tipo de duração: Simples](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).

* Você pode atualizar a tarefa Horas Planejadas no Balanceador de Carga de Trabalho somente para tarefas de Tipo de Duração Simples quando gerencia as alocações de usuários para tarefas. Para obter informações sobre o gerenciamento de alocações de usuários no Balanceador de Carga de Trabalho, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
* Não é possível modificar Horas Planejadas para tarefas com um Tipo de Duração do Esforço Orientado ou Calculado. Nesses casos, o Workfront determina as Horas Planejadas com base na Duração da tarefa; no entanto, nesse caso, as Horas Planejadas são sempre iguais à Duração (em horas) e não são afetadas pela alocação de porcentagem dos recursos atribuídos.

   Para obter mais informações sobre o Tipo de Duração Orientada pelo Esforço, consulte [Visão geral do Tipo de duração: Esforço orientado](../../../manage-work/tasks/taskdurtn/effort-driven.md).

   Para obter mais informações sobre o Tipo de duração do trabalho calculado, consulte [Visão geral do Tipo de duração: Trabalho Calculado](../../../manage-work/tasks/taskdurtn/calculated-work.md).

## Atualizar a tarefa Horas Planejadas ao gerenciar alocações de usuários

Você pode atualizar Horas Planejadas para tarefas ao atualizar manualmente as alocações de usuário ou função de trabalho para tarefas. Isso é possível somente quando as tarefas têm um Tipo de duração Simples.

Para obter mais informações, consulte [Visão geral do Tipo de duração: Simples](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).

Você pode atualizar a alocação geral de usuários e funções atribuídos à tarefa ou as alocações diárias do usuário ao usar o Balanceador de Carga de Trabalho.

Para obter informações sobre como gerenciar alocações gerais de usuários e funções de trabalho para tarefas, consulte [Gerenciar horas de alocação de usuários e funções em tarefas](../../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md).

Para obter informações sobre como gerenciar alocações diárias para tarefas, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Os seguintes cenários existem ao atualizar manualmente as alocações de funções de usuário ou de trabalho para tarefas:

* Quando você não tiver atualizado manualmente as alocações de usuário individual ou de função para acionar uma alteração na tarefa Horas Planejadas, as Horas Planejadas permanecerão inalteradas quando você adicionar, remover ou substituir atribuições na tarefa. Ao adicionar uma nova atribuição à tarefa, as alocações individuais são redistribuídas entre todos os destinatários.
* Quando você atualizou manualmente as alocações para acionar uma alteração na tarefa Horas Planejadas, as Horas Planejadas diminuem quando você remove atribuições da tarefa. Elas permanecem inalteradas quando você substitui uma atribuição.
* Quando você atualizou manualmente as alocações para acionar uma alteração na tarefa Horas Planejadas e adicionou uma atribuição à tarefa, a nova atribuição é alocada 0 horas por padrão. Você deve atualizar manualmente a alocação para a tarefa, o que pode afetar as Horas Planejadas.
* Quando você não tiver atualizado manualmente as alocações para acionar uma alteração na tarefa Horas Planejadas e remover todas as atribuições na tarefa, as Horas Planejadas permanecerão inalteradas.
* Ao atualizar manualmente as alocações para acionar uma alteração na tarefa Horas Planejadas e remover todas as atribuições na tarefa, as Horas Planejadas também são removidas e as Horas Planejadas da tarefa se tornam 0.

>[!NOTE]
Por exemplo, se uma tarefa tiver 10 Horas Planejadas e você tiver dois destinatários, cada um terá 5 horas alocadas cada, por padrão.
* Se você não atualizar a alocação de usuário individual ou as alocações diárias usando o Balanceador de Carga de Trabalho e remover qualquer ou todos os destinatários da tarefa, a tarefa Horas Planejadas permanecerá 10 horas.
* Se você alterar manualmente as alocações das atribuições para 4 e 6 horas, respectivamente, e remover o usuário alocado para 6 horas, bem como sua função de trabalho, a tarefa Horas Planejadas será atualizada para 4 horas. Se você também remover o usuário alocado para 4 horas, mas manter a função de trabalho associada ao usuário removido, as Horas Planejadas da tarefa permanecerão 4 horas. Se você remover o último usuário alocado a 4 horas, bem como sua função de trabalho e a tarefa não for atribuída, a tarefa Horas Planejadas da tarefa se tornará 0.





## Atualizar tarefa Horas Planejadas automaticamente usando Esforço de Trabalho

Quando você usa Esforço de trabalho para estimar o esforço necessário para que uma tarefa seja concluída, a quantidade de Horas planejadas para as tarefas é atualizada automaticamente. Isso é possível somente para tarefas com um Tipo de duração simples.

Para obter informações sobre o uso do Esforço de Trabalho para estimar o esforço da tarefa, consulte [Visão geral do esforço de trabalho](../../../manage-work/tasks/task-information/work-effort.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this issue has the explanation of how Planned Hours should work - from Vazgen and Anna: https://hub.workfront.com/issue/6217dced00730b7034c4b808339a35ce/</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Details of their comments: </p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Anna Asatryan</p>
<p>3/22/2022 At 3:16 PM</p>
<p>&nbsp;</p>
<p>to Mark Paul, Corrie Butler, Arman Simonyan, Gagik Khalatyan, Alina Wilson, Artur Sargsyan, Vazgen Babayan, Anna Asatryan</p>
<p>I have done some rough calculations on what the planned hours/revenues should look like Book.xlsx . And if we look, for example at the 2 users highlighted in one of the screenshots their planned hours look way off from what the calculation looks like in the spreadsheet (i.e. equally distributed allocation). When looking at the Workload balancer (the second screenshot), as an example for the user Yashas Mitta, I can see that the allocation has been modified. Obviously the utilization report calculates the allocations based on the modified contouring using the new work per day calculation. The project financial report uses the old, equal distribution of allocation along the full duration of the task. Hence. there is a difference when grouping per periods.</p>
<p>Vazgen Babayan</p>
<p>I believe we will need to prioritise syncing the project financial data report with the new work per day.</p>
<p>Alina Wilson</p>
<p>@Anna Asatryan , do you have a definition of what we should say in documentation (glossary, for example) for how the Planned Hours (or Planned Revenue) is calculated, keeping in mind that we don't document the concept of "workPerDay". We call them "daily allocations", for example, but let me know if that's accurate, too.</p>
<p>Vazgen Babayan</p>
<p>Last Thursday at 3:13 PM</p>
<p>I think an important note here is that regardless the calculation, even if the both views used the same formula, they will not display the same data, because the underlying data sources are different. The Financial Data report does not respect user-entered allocations in Workload Balancer at this moment. So there will be a clear discrepancy, as Anna showed in her message. My recommendation for communication will be to explain that the data sources are different so there can be a mismatch in data and that we will look into addressing that on our roadmap.</p>
<p>Alina Wilson</p>
<p>So far, I hear you guys say this (with my questions for confirmation/ comments in bold):</p>
<p>- the utilization report calculates the allocations based on the modified contouring using the new work per day calculation (so this is what we see in the Workload Balancer, right?)</p>
<p>- the project financial report uses the old, equal distribution of allocation along the full duration of the task (this is before the daily allocations for example were modified in the WB, right?)</p>
<p>I have these additional questions:</p>
<p>- what does the Project Details show? Which Planned Hours, for instance - because earlier, we had a question about this also. - which numbers?</p>
<p>- what does any Planned Hours/ Planned Revenue field that can be pulled in any other report (outside of Financial Data and Utilization reports) show? - which numbers?</p>
<p>- are there any other areas I am not thinking of that we need to document, @Corrie Butler</p>
<p>I will try to document all the possible areas where these display but please help. Thanks!</p>
<p>Vazgen Babayan</p>
<p>Last Saturday at 3:41 PM</p>
<ul>
<li> <p>Confirming the first two points </p> </li>
</ul>
<p>For the following questions</p>
<ul>
<li> <p>Project details show an aggregated sum of task planned hours. It doesn't have anything to do with the work per day because it always deals with total numbers for the whole duration of the Project/Task.</p> </li>
<li> <p>Same thing applies to the Planned Hours and Planned Revenue fields in reports - they show totals for the whole Project/Task duration and thus have no use of work per day.</p> </li>
<li> <p>Can't think of any other fields related to this right now.</p> </li>
<li> <p>In general, if I were to summarize the system behavior, it's as follows:</p> </li>
<li> <p>Every area that only deals with total numbers of Planned Hours / Planned Revenue, uses the numbers entered on the tasks. Those are Task / Project Details, reports exposing those fields.</p> </li>
<li> <p>Areas that deal with time-sensitive portions of Planned Hours / Planned Revenue, use work per day. Those are all Resource Management tools - Workload Balancer, Resource Planner, Utilization Report, importing projects via Scenario Planner.</p> </li>
<li> <p>All the areas in the second point support user-edited allocations made in Workload Balancer.</p> </li>
<li> <p>Scheduling area and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from Workload Balancer.</p> </li>
<li> <p>Scheduling will be removed this year, and we need to do work to move the Project Financial Data reports to the new work per day sometime after Q3.</p> </li>
</ul>
<p>Alina Wilson</p>
<p>@Vazgen Babayan , one clarifying question: when you say "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" - you mean that those use the system default which spreads the allocations evenly, correct? Because you can edit (daily) allocations in Scheduling tools, but it doesn't use that, correct? It uses the default of the daily allocation that the system figures out when dividing the Planned Hours by the number of days in the Duration. Please let me know. And thanks!</p>
<p>Anna Asatryan</p>
<p>Yesterday at 11:42 AM</p>
<p>@Alina Wilson , that's correct, when saying "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" Vazgen meant that it spreads the allocation evenly.</p>
<p>As for the scheduling, the allocation modification that's being done there isn't reflected anywhere else in the application other than in the Scheduling itself. That's probably one of the reasons it's being deprecated.</p>
</div>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <br> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: everything below is drafted because I replaced it with the table above)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can find the Planned Hours information on tasks, issues, or projects in the following locations:</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours in the Details  section  of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours in the Details  section  is identical for tasks, issues, and projects. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the Planned Hours value on the Details  section  of a task: </p>
<ol>
<li value="1">Go to a task for which you want to review the Planned Hours.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Overview</strong> area and notice the Planned Hours value.</p> <p>This value represents the time it would take the user assigned to the task to complete it. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3> </h3>
<p>The Planned Hours in the Edit box of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours while editing a task or an issue is identical. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the value of Planned Hours while editing a task:</p>
<ol>
<li value="1">Go to the task or issue you want to view Planned Hours for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> <p>The Planned Hours are located in the <strong>Overview</strong> section. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours column is included in the Standard view of a task list, by default. For issues and projects, you can add it to the view, when you are editing the view or when you build a report. </p>
<p>The Planned Hours in a task, issue, or project report are the total Planned Hours of the respective item as they display in the Details  section  or the Edit box of the items. </p>
<p>Adding the Planned Hours column to a project view is similar to building a view in a project report. </p>
<p>To show Planned Hours in a project report:</p>
<ol>
<li value="1"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Workfront, then click <strong>Reports</strong>. </p> </li>
<li value="2">Click <strong>New Report</strong>, then choose <strong>Project</strong> as your object.</li>
<li value="3">Click <strong>Add Column</strong>, and start typing <strong>Planned Hours</strong> when the <strong>Show in this column</strong> drop-down field is displayed. Select the field when it appears in the list.</li>
<li value="4"> <p>Click <strong>Save + Close</strong> to save the report. </p> <p>The Planned Hours column shows the total number of Planned Hours on each project. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Planned Hours in Resource Management tools</p> <note type="important">
When viewing Planned Hours in the Resource Management tools by a specific time frame, the daily allocations for each work item and the daily allocations for the resources assigned to the work items during that time frame can influence the daily Planned Hours of projects or work items.
</note>
<p>You can see the value of Planned Hours for your tasks, issues, or projects when using the following Resource Management tools:</p>
<ul>
<li> <p>Resource Planner</p> <p>For information about using the Resource Planner, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p> </li>
<li> <p>Utilization Report.</p> <p>For information about the utilization report, see <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Overview of the Resource Utilization report</a>.</p> </li>
<li>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Workload Balancer or Scheduling areas in the following sections:</p>
<ul>
<li>Scheduling or Workload Balancer sections in the Resourcing area</li>
<li>Scheduling or Workload Balancer section at the project level</li>
<li>Schedule or Workload Balancer section at the team level</li>
</ul>
</div> <p>For information about scheduling resources, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p> <p>For information about the Workload Balancer, see <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Overview of the Workload Balancer</a>. </p> </li>
<li> <p><b>Role Allocation panel</b> in the project  task list or  Workload Balancer: The Planned Hours for the tasks and the issues on the project that are assigned to a job role or a user associated with a job role are taken into account in this area. For more information, see <a href="../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md" class="MCXref xref">View project Planned Hours in the Role Allocation panel</a>. </p> </li>
</ul>
</div>
-->
