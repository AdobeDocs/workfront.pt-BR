---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '''Visão geral do tipo de duração: Esforço orientado"'
description: Impulsionado pelo esforço é um tipo de duração que pode ser definido para uma tarefa no Adobe Workfront. Para obter informações gerais sobre Tipos de duração no Workfront, consulte Visão geral da duração da tarefa e Tipo de duração.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# Visão geral do Tipo de duração: Esforço orientado

Impulsionado pelo esforço é um tipo de duração que pode ser definido para uma tarefa no Adobe Workfront. Para obter informações gerais sobre Tipos de duração no Workfront, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Visão Geral do Tipo de Duração Orientada pelo Esforço

Seu Workfront ou um administrador de grupo pode definir o Tipo de duração padrão do seu sistema ou grupo como Orientado por Esforço. Nesse caso, todas as novas tarefas serão criadas com esse Tipo de duração. Para obter informações sobre como alterar sua tarefa e emitir preferências como parte de suas preferências de projeto no nível do sistema ou no nível do grupo, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Neste cenário, há o risco de encurtar arbitrariamente o plano do projeto, a menos que você, como gerente do projeto, tenha tempo para considerar se a tarefa é realmente uma tarefa Orientada a Esforço.

Use Esforço direcionado para:

* Determine a Duração planejada com base no número de recursos disponíveis para trabalhar na tarefa. Duração é igual a Horas Planejadas. Duração Planejada é igual a Horas Planejadas dividido pelo número de designados.

   O nível de esforço aplicado à tarefa determina a divisão do trabalho e a Duração.

* Rastreie o número total de horas gastas em uma tarefa quando vários recursos são atribuídos.

   À medida que os recursos são adicionados, a Duração planejada da tarefa diminui. (O princípio de &quot;muitas mãos fazem a luz funcionar&quot; ilustra o efeito que esse Tipo de duração tem na Duração planejada de uma tarefa.)

As seções a seguir fornecem informações mais detalhadas sobre como o Workfront calcula a Duração planejada de uma tarefa Orientada por Esforço e o efeito que a adição de recursos tem na tarefa com esse Tipo de duração.

## Visão geral da fórmula Tipo de Duração Orientada pelo Esforço

A fórmula para calcular a Duração Planejada de uma tarefa com um Tipo de Duração Orientada pelo Esforço depende da porcentagem de alocação de cada recurso atribuído à tarefa. No caso de uma tarefa Orientada ao Esforço, o Workfront calcula as Horas Planejadas da tarefa e elas são sempre as mesmas da Duração da tarefa:

```
Planned Hours (in hours) = Duration (in days)
```

É possível ajustar manualmente a Duração da tarefa.

A Workfront parte do princípio de que há 8 horas de trabalho em um dia útil. O administrador do Workfront ou de grupo define as horas por dia de trabalho com a configuração Horas típicas por dia de trabalho nas Preferências do projeto em Configurar. Para obter mais informações sobre como alterar sua tarefa e emitir preferências como parte das preferências do projeto no nível do sistema, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>O Workfront considera o Schedule para cada recurso atribuído à tarefa para determinar a porcentagem de alocação para cada recurso da tarefa. Para obter informações sobre como criar e atribuir agendamentos a usuários, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Considere os seguintes cenários:

* [Os recursos são alocados 100% para a tarefa](#resources-are-allocated-100-to-the-task)
* [Os recursos são alocados para várias porcentagens de tempo na tarefa](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Os recursos são alocados 100% para a tarefa {#resources-are-allocated-100-to-the-task}

Essa fórmula pressupõe que todos os recursos sejam alocados 100% para a tarefa.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Este cálculo pressupõe que o número de horas em um dia de trabalho normal é de 8. A equação inclui esse valor para que a Duração planejada seja exibida em dias.

### Os recursos são alocados para várias porcentagens de tempo na tarefa {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Como cada recurso atribuído pode ter um nível exclusivo de alocação, a fórmula real leva esses valores de alocação em consideração:

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Este cálculo pressupõe que o número de horas em um dia de trabalho normal é de 8. A equação inclui esse valor para que a Duração planejada seja exibida em dias.

## O efeito de adicionar mais recursos a uma tarefa

Ao adicionar ou remover destinatários a uma tarefa com o Tipo de duração determinado pelo esforço, a Duração e as Horas planejadas não são alteradas. No entanto, a Duração planejada muda.

No exemplo a seguir, as Horas típicas por dia de trabalho são definidas como 8 nas Preferências do projeto na configuração do sistema. Como a duração é de 3 dias, as Horas Planejadas são definidas como 24 (3 dias x 8 horas por dia de trabalho = 24 Horas Planejadas).

>[!NOTE]
>
>Ao usar a Restrição de tarefa de datas fixas, a Duração planejada permanece a mesma ao adicionar ou remover destinatários e, em vez disso, a Duração e as Horas planejadas são ajustadas. Ao usar qualquer Restrição de tarefa diferente de Datas fixas, a Duração planejada é ajustada.

A tabela a seguir ilustra como a Duração planejada muda com a adição de recursos à tarefa:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>Número de Atributos (cada 100% alocado)</strong> </p> </th> 
   <th> <p><strong>Duração</strong> </p> </th> 
   <th> <p><strong>Horas planejadas</strong> </p> </th> 
   <th><strong>Duração Planejada</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 Dias</p> </td> 
   <td> <p>24 Horas</p> <p>(3 Dias x 8 Horas por Dia de Trabalho = 24 Horas Planejadas)</p> </td> 
   <td> <p>3 Dias</p> <p>(24 Horas Planejadas / 1 Destinatário = 3 Dias)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 Dias</p> </td> 
   <td> <p>24 Horas</p> <p>(3 Dias x 8 Horas por Dia de Trabalho = 24 Horas Planejadas)</p> </td> 
   <td> <p>1,5 Dias</p> <p>(24 Horas Planejadas / 2 Atributos = 12 Horas ou 1,5 Dias)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 Dias</p> </td> 
   <td> <p>24 Horas</p> <p>(3 Dias x 8 Horas por Dia de Trabalho = 24 Horas Planejadas)</p> </td> 
   <td> <p>1 dia</p> <p>(24 Horas Planejadas / 3 Destinatários = 8 Horas ou 1 Dia)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Altere o Tipo de duração de uma tarefa para Impulsionado

Para obter informações sobre como alterar o Tipo de duração de uma tarefa, consulte [Atualizar o Tipo de duração de uma tarefa](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
