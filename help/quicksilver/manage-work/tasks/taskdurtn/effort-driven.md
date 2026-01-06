---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Visão geral do tipo de duração: Controlado pelo esforço'
description: Orientado pelo esforço é um tipo de duração que você pode definir para uma tarefa no Adobe Workfront. Para obter informações gerais sobre Tipos de duração no Workfront, consulte Visão geral da duração da tarefa e Tipo de duração.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 1%

---

# Visão geral do tipo de duração: Controlado pelo esforço

Orientado pelo esforço é um tipo de duração que você pode definir para uma tarefa no Adobe Workfront. Para obter informações gerais sobre os Tipos de Duração no Workfront, consulte [Visão Geral da Duração e do Tipo de Duração da Tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Visão geral do tipo de duração orientada pelo esforço

O Workfront ou um administrador de grupo pode definir o Tipo de duração padrão do seu sistema ou grupo como Controlado pelo esforço. Nesse caso, todas as novas tarefas serão criadas com esse Tipo de Duração. Para obter informações sobre como alterar as preferências de tarefas e problemas como parte das preferências de projetos no nível do sistema ou do grupo, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Nesse cenário, há o risco de encurtar arbitrariamente o plano do projeto, a menos que você, como gerente do projeto, reserve um tempo para considerar se a tarefa é realmente uma tarefa orientada pelo esforço.

Use o Effort Driven para:

* Determine a Duração planejada com base no número de recursos disponíveis para trabalhar na tarefa. A duração é igual às Horas planejadas. A Duração Planejada é igual às Horas Planejadas divididas pelo número de atribuídos.

  O nível de esforço aplicado à tarefa determina a divisão do trabalho e a Duração.

* Rastreie o número total de horas gastas em uma tarefa quando vários recursos são atribuídos.

  À medida que os recursos são adicionados, a Duração planejada da tarefa diminui. (O princípio de &quot;muitas mãos fazem a luz funcionar&quot; ilustra o efeito que esse Tipo de duração tem na duração planejada de uma tarefa.)

As seções a seguir fornecem informações mais detalhadas sobre como o Workfront calcula a Duração planejada de uma tarefa orientada pelo esforço e o efeito que a adição de recursos tem na tarefa com esse Tipo de Duração.

## Visão geral da fórmula Tipo de Duração Conduzida pelo Esforço

A fórmula de cálculo da Duração Planejada para uma tarefa com um Tipo de Duração de Esforço Orientado depende da porcentagem de alocação de cada recurso atribuído à tarefa. No caso de uma tarefa orientada pelo esforço, o Workfront calcula as Horas planejadas da tarefa e elas são sempre as mesmas que a Duração da tarefa:

```
Planned Hours (in hours) = Duration (in days)
```

Você pode ajustar manualmente a Duração da tarefa.

A Workfront presume que há 8 horas de trabalho em um dia útil. O administrador do Workfront ou do grupo define as horas por dia de trabalho com a configuração Horas típicas por dia de trabalho nas Preferências do projeto em Configuração. Para obter mais informações sobre como alterar as preferências de tarefas e problemas como parte das preferências do projeto no nível do sistema, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>O Workfront considera a Programação para cada recurso atribuído à tarefa para determinar o percentual de alocação para cada recurso da tarefa. Para obter informações sobre como criar e atribuir agendas a usuários, consulte [Criar uma agenda](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Considere os seguintes cenários:

* [Os recursos estão alocados 100% para a tarefa](#resources-are-allocated-100-to-the-task)
* [Os recursos são alocados para várias porcentagens de tempo para a tarefa](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Os recursos são alocados 100% para a tarefa {#resources-are-allocated-100-to-the-task}

Essa fórmula pressupõe que todos os recursos estejam alocados 100% para a tarefa.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Esse cálculo pressupõe que o número de horas em um dia de trabalho normal seja 8. A equação inclui esse valor para que a Duração planejada seja exibida em dias.

### Os recursos são alocados para várias porcentagens de tempo para a tarefa {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Como cada recurso atribuído pode ter um nível exclusivo de alocação, a fórmula real leva em consideração esses valores de alocação:

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Esse cálculo pressupõe que o número de horas em um dia de trabalho normal seja 8. A equação inclui esse valor para que a Duração planejada seja exibida em dias.

## O efeito de adicionar mais recursos a uma tarefa

Ao adicionar ou remover atribuídos a uma tarefa com o Tipo de duração direcionado ao esforço, a Duração e as Horas planejadas não são alteradas. No entanto, a duração planejada não muda.

No exemplo a seguir, as Horas típicas por dia de trabalho estão definidas como 8 nas Preferências do projeto, na configuração do sistema. Como a duração é de 3 dias, as Horas planejadas são definidas como 24 (3 dias x 8 horas por dia de trabalho = 24 Horas planejadas).

>[!NOTE]
>
>Ao usar a Restrição de tarefa de datas fixas, a Duração planejada permanece a mesma ao adicionar ou remover atribuídos, e em vez disso, a Duração e as Horas planejadas são ajustadas. Ao usar qualquer Restrição de tarefa diferente de Datas fixas, a Duração planejada é ajustada.

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
   <th> <p><strong>Número de Atribuídos (cada 100% alocados)</strong> </p> </th> 
   <th> <p><strong>Duração</strong> </p> </th> 
   <th> <p><strong>Horas planejadas</strong> </p> </th> 
   <th><strong>Duração Planejada</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 dias</p> </td> 
   <td> <p>24 Horas</p> <p>(3 dias x 8 horas por dia de trabalho = 24 horas planejadas)</p> </td> 
   <td> <p>3 dias</p> <p>(24 Horas Planejadas / 1 Destinatário = 3 Dias)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 dias</p> </td> 
   <td> <p>24 Horas</p> <p>(3 dias x 8 horas por dia de trabalho = 24 horas planejadas)</p> </td> 
   <td> <p>1,5 dia</p> <p>(24 Horas Planejadas / 2 Atribuídos = 12 Horas ou 1,5 Dia)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 dias</p> </td> 
   <td> <p>24 Horas</p> <p>(3 dias x 8 horas por dia de trabalho = 24 horas planejadas)</p> </td> 
   <td> <p>1 dia</p> <p>(24 Horas Planejadas / 3 Atribuídos = 8 Horas ou 1 Dia)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Alterar o Tipo de Duração de uma tarefa para Controlado pelo Esforço

Para obter informações sobre como alterar o Tipo de Duração de uma tarefa, consulte [Atualizar o Tipo de Duração de uma tarefa](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
