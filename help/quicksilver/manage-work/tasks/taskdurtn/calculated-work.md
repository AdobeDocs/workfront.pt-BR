---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Visão Geral Do Tipo De Duração: Trabalho Calculado'
description: O Trabalho calculado é um Tipo de duração que pode ser definido para uma tarefa no Adobe Workfront. Para obter informações gerais sobre Tipos de duração no Workfront, consulte Visão geral da duração da tarefa e Tipo de duração.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 1%

---

# Visão geral do tipo de duração: trabalho calculado

O Trabalho calculado é um Tipo de duração que pode ser definido para uma tarefa no Adobe Workfront. Para obter informações gerais sobre os Tipos de Duração no Workfront, consulte [Visão Geral da Duração e do Tipo de Duração da Tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Visão geral do tipo de duração do trabalho calculado

O Trabalho Calculado determina a quantidade de esforço (Horas Planejadas) necessário para a tarefa ser concluída. Recomendamos que você use o Tipo de Duração do Trabalho Calculado quando os recursos atribuídos à tarefa forem alocados para toda a duração da tarefa.

O Workfront ou um administrador de grupo pode definir o Tipo de duração padrão do sistema ou grupo como Trabalho calculado. Nesse caso, todas as novas tarefas serão criadas com esse Tipo de Duração. Para obter informações sobre como alterar as preferências de tarefas e problemas como parte das preferências de projetos no nível do sistema ou do grupo, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

À medida que recursos são adicionados a uma tarefa, um gerente de projeto pode esperar que o esforço planejado aumente. Para ilustrar, uma reunião de planejamento de uma hora com três recursos representa três horas totais de trabalho necessário, e uma reunião de planejamento de uma hora com dez recursos representa dez horas de trabalho necessário. Isso pressupõe que cada recurso esteja alocado para a tarefa com 100% de alocação.

## Revise a fórmula de cálculo do Trabalho necessário ao usar o Tipo de duração do trabalho calculado

Quando você usa o Tipo de Duração do Trabalho Calculado em uma tarefa, o Workfront calcula a quantidade de Trabalho para cada tarefa usando as duas fórmulas a seguir. As fórmulas diferem dependendo da porcentagem de tempo que cada recurso está alocado para a tarefa e de quantos recursos você atribuiu a cada tarefa:

* Fórmula simplificada: supondo que você tenha um recurso atribuído à tarefa e que eles estejam alocados para a tarefa por 100% do tempo disponível, o valor Trabalho necessário para cada tarefa será calculado usando a seguinte fórmula:

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Fórmula complexa: se você atribuir cada recurso com várias alocações, a fórmula leva essas alocações em consideração e leva em conta essas variações:

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Revisar o efeito da adição ou remoção de recursos da tarefa

Ao adicionar ou remover atribuídos a uma tarefa com o tipo de duração Trabalho calculado, a Duração pode ser editada manualmente. À medida que os atribuídos são adicionados ou removidos da tarefa, as Horas planejadas são alteradas.

No exemplo a seguir, as Horas típicas por dia de trabalho estão definidas como 8 nas Preferências do projeto, em Configuração. Cada tarefa tem uma duração de 1 dia. À medida que o número de atribuídos muda, as Horas planejadas mudam com base no número de atribuídos em uma determinada tarefa:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Número de Atribuídos (cada 100% alocados)</strong> </p> </th> 
   <th> <p><strong>Duração</strong> </p> </th> 
   <th> <p><strong>Horas planejadas</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 dia</p> </td> 
   <td> <p>8 Horas</p> <p>(1 Dia x 8 Horas por Dia Útil x 1 Destinatário = 8 Horas Planejadas)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 dia</p> </td> 
   <td> <p>16 Horas</p> <p>(1 Dia x 8 Horas por Dia Útil x 2 Atribuídos = 16 Horas Planejadas)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 dia</p> </td> 
   <td> <p>24 Horas</p> <p>(1 Dia x 8 Horas por Dia Útil x 3 Atribuídos = 24 Horas Planejadas)</p> </td> 
  </tr> 
 </tbody> 
</table>

Nesse caso, cada destinatário é 100% alocado para a tarefa Trabalho calculado.

![](assets/calcwork-350x71.png)

## Alterar o tipo de duração de uma tarefa para Trabalho calculado

Para obter informações sobre como alterar o Tipo de Duração de uma tarefa, consulte [Atualizar o Tipo de Duração de uma tarefa](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Work</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
