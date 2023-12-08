---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Visão Geral da Duração da Tarefa e do Tipo de Duração
description: A Duração da tarefa é a diferença entre a Data de conclusão planejada e a Data inicial planejada da tarefa. A Duração indica o período disponível para a tarefa ser concluída.
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: 8f8a274eb872f78f888cf76b2d5fd3d39c6d6223
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 1%

---

# Visão Geral da Duração da Tarefa e do Tipo de Duração

A Duração da tarefa é a diferença entre a Data de conclusão planejada e a Data inicial planejada da tarefa. A Duração indica o período disponível para a tarefa ser concluída.

O Tipo de Duração de uma tarefa identifica a relação entre o número de recursos atribuídos a uma tarefa, o esforço total e a Duração total da tarefa.

## Visão geral da duração da tarefa

Se o Início Efetivo e as Datas de Término Efetivo da tarefa estiverem fora do cronograma do projeto, do responsável principal ou do Cronograma Padrão, a Duração da tarefa será zero.

**Exemplo:** Se você tiver uma programação que comece às 9h e termine às 12h e uma tarefa que esteja programada para iniciar às 14h e terminar às 16h, a Duração da tarefa será zero.

Veja a seguir dois cenários que existem ao calcular a duração no Adobe Workfront:

* Se a tarefa for atribuída a um Workfront de usuário, o usará um dos seguintes agendamentos, nesta ordem exata, para calcular a Duração:

   1. O Workfront considera a programação do usuário.
   1. Se o usuário não estiver associado a um agendamento, a Workfront levará em conta o agendamento do projeto.
   1. Se o projeto não estiver associado a um agendamento, a Workfront levará em conta o Agendamento padrão do seu sistema. Para obter informações sobre programações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Se a tarefa for atribuída a vários usuários:

   1. A Workfront considera a programação do projeto ou a do responsável principal.

  O administrador do Workfront determina qual programação o Workfront usa quando uma tarefa é atribuída a vários usuários. Para obter informações, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  As etapas são semelhantes ao primeiro cenário depois de entender qual agendamento o Workfront usa para calcular a Duração.

>[!NOTE]
>
>Ao considerar o tempo de folga do responsável principal em um projeto, as datas planejadas da tarefa podem ser ajustadas, mas a Duração da tarefa permanece a mesma. Para obter informações sobre como considerar a folga da Principal pessoa atribuída ao planejar um projeto, consulte  [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Unidades de tempo para a Duração da Tarefa

Você pode indicar a Duração da tarefa tanto no tempo normal quanto no tempo decorrido entre as Datas de Início Planejado e de Conclusão Planejada.

Ao atualizar a Duração das tarefas em uma lista, você pode usar as seguintes abreviações para indicar unidades de tempo no Workfront:

| Unidade de Tempo | Abreviação |
|---|---|
| Minutos | M |
| Horas | H |
| Dias. Este é o padrão. | E |
| Semanas | S |
| Meses | T |
| Minutos corridos | EM |
| Horas corridas | EH |
| Dias corridos | ED |
| Semanas corridas | NOVO |
| Meses decorridos | ET |

{style="table-layout:auto"}

**Exemplo:** Se você quiser indicar que a duração de uma tarefa é de 3 dias decorridos, digite &quot;3 ED&quot; no campo Duração em uma lista de tarefas .  Você também pode selecionar a opção preferida para a Unidade de tempo de duração no menu suspenso disponível ao editar uma tarefa ou na seção Detalhes da tarefa. Para obter informações sobre edição de tarefas, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Considere o seguinte ao indicar a Duração de uma tarefa:

* Tempo decorrido é uma unidade de tempo da Duração de uma tarefa. É o tempo entre a Data de Início Planejada e a Data de Conclusão Planejada de uma tarefa que inclui feriados, finais de semana e folga. Em outras palavras, o tempo decorrido é a passagem de dias do calendário.
* O tempo normal leva em conta feriados, fins de semana e folga e os exclui da Duração da tarefa.

* Quando você indica a Duração de uma tarefa em semanas, o Workfront calcula a Duração em dias e horas com base nas configurações de Dias de trabalho típicos por semana e Horas típicas por dia de trabalho definidas pelo administrador do Workfront na área Preferências do projeto da Configuração.
* O Workfront usa a duração padrão de 4 semanas para um mês ao calcular a Duração em meses.

## Visão geral do Tipo de duração da tarefa

O gerenciamento do Tipo de Duração de uma tarefa permite definir atribuições de recursos consistentes com base nas necessidades da tarefa.

O Tipo de duração ajuda a responder às seguintes perguntas:

* Quão ocupados vamos estar?
* Qual é o tamanho do trabalho?
* Quanto tempo vai demorar?

![duration_type_triangle.png](assets/duration_type_triangle.png)

## Definir Tipos de Duração

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row"><p><strong>Tipo de Duração</strong></p></th> 
   <th scope="col"> <p><strong>Função</strong> </p> </th> 
   <th scope="col"> <p><strong>Como os recursos afetam isso</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Atribuição Calculada</strong> </p> </th> 
   <td scope="col"> <p>Calcula a porcentagem de alocação para cada destinatário em uma tarefa. </p> <p>Ao escolher esse Tipo de duração, você pode inserir Duração individual e Horas planejadas para a tarefa. O Workfront divide as Horas planejadas pelo número de horas dentro da Duração da tarefa e, em seguida, pelo número de recursos atribuídos à tarefa para calcular a alocação para cada destinatário.</p> <p>Para obter informações mais detalhadas, consulte <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Visão geral do tipo de duração: atribuição calculada</a>.</p> </td> 
   <td scope="col">A duração e as horas planejadas não são alteradas ao adicionar ou remover atribuídos à tarefa. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Trabalho Calculado</strong> </p> </th> 
   <td scope="col"> <p>Determina as horas planejadas (quantidade de esforço) necessárias para a tarefa ser concluída.</p> <p>Normalmente usado quando os recursos atribuídos à tarefa são alocados para toda a duração da tarefa.</p> <p>Ao escolher esse Tipo de duração, você tem a capacidade de inserir uma Duração individual para a tarefa. O Workfront calcula as Horas planejadas para a tarefa multiplicando o número de dias na Duração pelo número de horas de trabalho no cronograma e pelo número de atribuídos à tarefa. </p> <p>Você pode alterar manualmente a porcentagem de alocação de cada destinatário para a tarefa, o que reduzirá a quantidade de Horas planejadas.</p> <p>Para obter informações mais detalhadas, consulte <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Visão geral do tipo de duração: trabalho calculado</a>.</p> </td> 
   <td scope="col"> <p>As Horas planejadas aumentam quando os atribuídos são adicionados à tarefa. </p> <p>As horas planejadas diminuem quando os atribuídos são removidos da tarefa.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Controlado pelo empenho</strong></p> </th> 
   <td scope="col"> <p>Determina as horas planejadas com base no número de recursos.</p> <p>Ao escolher esse Tipo de duração, você tem a capacidade de inserir uma Duração individual para a tarefa. O Workfront calcula as Horas Planejadas para a tarefa multiplicando o número de dias na Duração pelo número de horas de trabalho no cronograma e dividindo esse número pelo número de atribuídos à tarefa. </p> <p>Você pode alterar manualmente a porcentagem de alocação de cada destinatário para a tarefa, mas o número de Horas planejadas permanece o mesmo.</p> <p>Para obter informações mais detalhadas, consulte <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Visão geral do tipo de duração: Controlado pelo esforço</a>.</p> </td> 
   <td scope="col"> <p>As horas planejadas aumentam quando os atribuídos são removidos da tarefa.</p> <p>As horas planejadas diminuem quando os atribuídos são adicionados à tarefa. </p> <p>A duração não é alterada, independentemente das alterações no número de responsáveis ou em seu agendamento. </p> <p>A duração é igual às Horas planejadas. A Duração Planejada é igual às Horas Planejadas divididas pelo número de atribuídos.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Simples</strong> </p> </th> 
   <td scope="col"> <p>Determina as horas planejadas e a duração (que são as mesmas, para este tipo de duração) com base no número de horas para as quais cada destinatário é alocado. </p> <p>O Workfront calcula as Horas planejadas somando as horas alocadas planejadas para cada destinatário. </p> <p>Você pode alterar manualmente a quantidade de horas para a qual cada destinatário está alocado, e o número de Horas planejadas e a quantidade de Duração são alterados de acordo. Se você escolher um número total de horas alocadas para todos os designados, esse número será dividido igualmente entre cada designado.</p> <p>Para obter informações mais detalhadas, consulte <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Visão geral do tipo de duração: simples</a>.</p> </td> 
   <td scope="col"> <p>As horas são distribuídas uniformemente entre os designados se você escolher um número total de horas alocadas. No entanto, como gerente de projeto, você pode ajustar manualmente as horas para cada destinatário. </p> <p>Você pode editar as Horas planejadas e a Duração de uma tarefa com um Tipo de duração simples em linha ou no nível da tarefa. </p> <p>Se uma Equipe Ágil for atribuída a uma tarefa, o Tipo de duração será automaticamente definido como Simples e não poderá ser alterado. A duração da tarefa para uma Equipe Ágil deve ser maior que 0 minutos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## O tipo de duração das novas tarefas

O Tipo de Duração de uma nova tarefa corresponde ao Tipo de Duração configurado em seu sistema. O tipo de duração padrão é Atribuição calculada. O administrador do Workfront ou um administrador de grupo pode atualizar o Tipo de duração padrão para o seu sistema ou para o grupo associado ao projeto. Para obter informações, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Alterar o tipo de duração de uma tarefa

Para obter informações sobre como alterar o Tipo de Duração de uma tarefa, consulte [Atualizar o tipo de duração de uma tarefa](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
