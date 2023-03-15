---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Visão Geral da Duração da Tarefa e do Tipo de Duração
description: A Duração da tarefa é a diferença entre a Data de Conclusão Planejada e a Data Inicial Planejada da tarefa. A Duração indica o período de tempo disponível para a tarefa ser concluída.
author: Alina
feature: Work Management
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 2%

---

# Visão Geral da Duração da Tarefa e do Tipo de Duração

A Duração da tarefa é a diferença entre a Data de Conclusão Planejada e a Data Inicial Planejada da tarefa. A Duração indica o período de tempo disponível para a tarefa ser concluída.

O Tipo de duração de uma tarefa identifica a relação entre o número de recursos atribuídos a uma tarefa, o esforço total e a Duração total da tarefa.

## Visão geral da Duração da tarefa

>[!NOTE]
>
>Ao considerar o tempo de folga do Destinatário Principal em um projeto, as datas planejadas da tarefa podem se ajustar, mas a Duração da tarefa permanece a mesma. Para obter informações sobre como considerar o tempo limite do Destinatário Principal ao planejar um projeto, consulte  [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Se as Datas de Início Real e Conclusão Real da tarefa não estiverem incluídas na programação do projeto, do destinatário principal ou da Programação Padrão, a Duração da tarefa será zero.

**Exemplo:** Se você tiver um agendamento que começa às 9h00 e termina às 12h00 e uma tarefa agendada para iniciar às 14h00 e terminar às 16h00, a Duração da tarefa será zero.

Veja a seguir dois cenários que existem ao calcular a duração no Adobe Workfront.

* Se a tarefa for atribuída a um usuário, o Workfront usará uma das programações a seguir, nesta ordem exata para calcular a Duração:

   1. A Workfront considera o agendamento do usuário.
   1. Se o usuário não estiver associado a um agendamento, a Workfront leva em consideração o agendamento do projeto.
   1. Se o projeto não estiver associado a um agendamento, a Workfront considerará o Agendamento padrão do seu sistema. Para obter informações sobre programações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Se a tarefa for atribuída a vários usuários:

   A Workfront leva em conta a programação do projeto ou a do destinatário principal.

   O administrador do Workfront determina qual programação a Workfront usa quando uma tarefa é atribuída a vários usuários. Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   As etapas são semelhantes ao primeiro cenário, depois de entender qual programação a Workfront usa para calcular a Duração.

## Unidades de tempo para duração da tarefa

Você pode indicar a Duração da tarefa no tempo regular e no tempo decorrido entre as Datas de Início Planejado e de Conclusão Planejada.

Ao atualizar a Duração das tarefas em uma lista, você pode usar as seguintes abreviações para indicar unidades de tempo no Workfront:

| Unidade de tempo | Abreviação |
|---|---|
| Minutos | M |
| Horas | H |
| Dias. Este é o padrão. | E |
| Semanas | Q |
| Meses | T |
| Minutos corridos | EM |
| Horas corridas | EH |
| Dias corridos | ED |
| Semanas corridas | EW |
| Meses decorridos | ET |

{style="table-layout:auto"}

**Exemplo:** Se quiser indicar que a Duração de uma tarefa é 3 Dias de Atraso, digite &quot;3 ED&quot; no campo Duração em uma lista de tarefas .  Você também pode selecionar a opção preferencial para a Unidade de duração de tempo no menu suspenso disponível ao editar uma tarefa ou na seção Detalhes da tarefa . Para obter informações sobre edição de tarefas, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Considere o seguinte ao indicar a Duração de uma tarefa:

* Tempo decorrido é uma unidade de tempo para a Duração de uma tarefa. É o tempo entre a Data inicial planejada e a Data de conclusão planejada de uma tarefa que inclui feriados, finais de semana e tempo limite. Por outras palavras, o tempo decorrido é a passagem dos dias de calendário.
* O tempo normal leva em consideração feriados, finais de semana e tempo de folga e os exclui da Duração da tarefa.

* Quando você indica a Duração de uma tarefa em semanas, a Workfront calcula a Duração em dias e horas com base nas configurações Típicas de dias de trabalho por semana e Típicas de horas por dia de trabalho definidas pelo administrador da Workfront na área Preferências do projeto da Configuração.
* O Workfront usa a duração padrão de 4 semanas para um mês ao calcular a Duração em meses.

## Visão geral do Tipo de duração da tarefa

O Gerenciamento do Tipo de duração de uma tarefa permite definir atribuições de recursos consistentes com base nas necessidades da tarefa.

O Tipo de duração ajuda a responder as seguintes perguntas:

* Quão ocupados vamos estar?
* Qual é o tamanho do trabalho?
* Quanto tempo vai demorar?

![duration_type_triangle.png](assets/duration-type-triangle-350x245.png)

## Definir Tipos de Duração

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row">Tipo de Duração </th> 
   <th scope="col"> <p><strong>Função</strong> </p> </th> 
   <th scope="col"> <p><strong>Como os recursos afetam isso</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Atribuição Calculada</strong> </p> </th> 
   <td scope="col"> <p>Calcula a porcentagem de alocação para cada destinatário em uma tarefa. </p> <p>Ao escolher esse Tipo de duração, você pode inserir Duração individual e Horas planejadas para a tarefa. O Workfront divide as Horas Planejadas pelo número de horas dentro da Duração da tarefa e, em seguida, pelo número de recursos atribuídos à tarefa para calcular a alocação para cada destinatário.</p> <p>Para obter informações mais detalhadas, consulte <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Visão geral do Tipo de duração: Atribuição calculada</a>.</p> </td> 
   <td scope="col">Duração e Horas Planejadas não são alteradas ao adicionar ou remover destinatários à tarefa. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Trabalho Calculado</strong> </p> </th> 
   <td scope="col"> <p>Determina as Horas Planejadas (quantidade de esforço) necessárias para a tarefa ser concluída.</p> <p>Normalmente usado quando os recursos atribuídos à tarefa são alocados para toda a Duração da tarefa.</p> <p>Ao escolher esse Tipo de duração, você tem a capacidade de inserir uma Duração individual para a tarefa. O Workfront calcula as Horas Planejadas da tarefa multiplicando o número de dias na Duração pelo número de horas de trabalho na programação e pelo número de destinatários da tarefa. </p> <p>Você pode alterar manualmente a porcentagem de alocação de cada destinatário para a tarefa, o que reduzirá a quantidade de Horas Planejadas.</p> <p>Para obter informações mais detalhadas, consulte <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Visão geral do Tipo de duração: Trabalho Calculado</a>.</p> </td> 
   <td scope="col"> <p>As Horas planejadas aumentam quando os destinatários são adicionados à tarefa. </p> <p>As Horas Planejadas diminuem quando os destinatários são removidos da tarefa.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p>Controlado pelo empenho</p> </th> 
   <td scope="col"> <p>Determina as Horas Planejadas com base no número de recursos.</p> <p>Ao escolher esse Tipo de duração, você tem a capacidade de inserir uma Duração individual para a tarefa. O Workfront calcula as Horas Planejadas da tarefa multiplicando o número de dias na Duração pelo número de horas de trabalho na programação e dividindo esse número pelo número de destinatários da tarefa. </p> <p>Você pode alterar manualmente a porcentagem de alocação de cada destinatário para a tarefa, mas o número de Horas Planejadas permanece o mesmo.</p> <p>Para obter informações mais detalhadas, consulte <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Visão geral do Tipo de duração: Esforço orientado</a>.</p> </td> 
   <td scope="col"> <p>As horas planejadas aumentam quando os destinatários são removidos da tarefa.</p> <p>As horas planejadas diminuem quando os destinatários são adicionados à tarefa. </p> <p>A Duração não muda, independentemente das alterações no número de destinatários ou de seu cronograma. </p> <p>Duração é igual a Horas Planejadas. Duração Planejada é igual a Horas Planejadas dividido pelo número de designados.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Simples</strong> </p> </th> 
   <td scope="col"> <p>Determina as Horas Planejadas e a Duração (que são as mesmas, para esse Tipo de Duração) com base no número de horas que cada destinatário está alocado. </p> <p>A Workfront calcula as Horas Planejadas adicionando as horas alocadas planejadas para cada destinatário. </p> <p>Você pode alterar manualmente a quantidade de horas alocadas por cada destinatário, e o número de Horas Planejadas e a quantidade de Duração são alterados de acordo. Se você escolher um número total de horas alocadas para todos os destinatários, esse número será dividido igualmente entre cada destinatário.</p> <p>Para obter informações mais detalhadas, consulte <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Visão geral do Tipo de duração: Simples</a>.</p> </td> 
   <td scope="col"> <p>As horas são distribuídas uniformemente entre os destinatários se você escolher um número total de horas alocadas. No entanto, como gerente de projeto, você pode ajustar manualmente as horas de cada destinatário. </p> <p>Você pode editar as Horas Planejadas e a Duração de uma tarefa com um Tipo de Duração Simples em linha ou no nível da tarefa. </p> <p>Se uma equipe ágil for atribuída a uma tarefa, o Tipo de duração será automaticamente definido como Simples e não poderá ser alterado. A duração da tarefa de uma equipe ágil deve ser superior a 0 minutos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## O Tipo de duração de novas tarefas

O Tipo de duração de uma nova tarefa corresponde ao Tipo de duração configurado no sistema. O Tipo de duração padrão é Atribuição calculada. O administrador do Workfront ou um administrador de grupo pode atualizar o Tipo de duração padrão do sistema ou do grupo associado ao projeto. Para obter mais informações, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Alterar o Tipo de duração de uma tarefa

Para obter informações sobre como alterar o Tipo de duração de uma tarefa, consulte [Atualizar o Tipo de duração de uma tarefa](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
