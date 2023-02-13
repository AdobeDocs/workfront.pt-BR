---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Visão geral do tipo de duração: Trabalho Calculado'
description: O Trabalho Calculado é um Tipo de Duração que pode ser definido para uma tarefa no Adobe Workfront. Para obter informações gerais sobre Tipos de duração no Workfront, consulte Visão geral da duração da tarefa e Tipo de duração.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# Visão geral do Tipo de duração: Trabalho Calculado

O Trabalho Calculado é um Tipo de Duração que pode ser definido para uma tarefa no Adobe Workfront. Para obter informações gerais sobre Tipos de duração no Workfront, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Visão Geral do Tipo de Duração Calculada do Trabalho

O Trabalho Calculado determina a quantidade de esforço (Horas Planejadas) necessária para a tarefa ser concluída. Recomendamos usar o Tipo de duração do trabalho calculado quando os recursos atribuídos à tarefa forem alocados para toda a duração da tarefa.

Sua Workfront ou um administrador de grupo pode definir o Tipo de duração padrão do sistema ou grupo como Trabalho calculado. Nesse caso, todas as novas tarefas serão criadas com esse Tipo de duração. Para obter informações sobre como alterar sua tarefa e emitir preferências como parte de suas preferências de projeto no nível do sistema ou no nível do grupo, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

À medida que os recursos são adicionados a uma tarefa, um gerente de projeto pode esperar ver o esforço planejado aumentar. Para ilustrar, uma reunião de planejamento de uma hora com três recursos representa três horas totais de trabalho necessárias e uma reunião de planejamento de uma hora com dez recursos representa dez horas de trabalho necessárias. Isso pressupõe que cada recurso seja alocado para a tarefa com alocação de 100%.

## Revise a fórmula para calcular o Trabalho Necessário ao usar o Tipo de Duração de Trabalho Calculada

Quando você usa o Tipo de duração do trabalho calculado em uma tarefa, o Workfront calcula a quantidade de Trabalho para cada tarefa usando as duas fórmulas a seguir. As fórmulas diferem dependendo do percentual de tempo que cada recurso é alocado à tarefa e de quantos recursos você atribuiu a cada tarefa:

* Fórmula simplificada: Supondo que você tenha um recurso atribuído à tarefa e ele esteja alocado à tarefa por 100% do tempo disponível, o valor Work Required para cada tarefa será calculado usando a seguinte fórmula:

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Fórmula complexa: Se você atribuir cada recurso com várias alocações, a fórmula leva essas alocações em conta e contabiliza essas variações:

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Revise o efeito de adicionar ou remover recursos da tarefa

Ao adicionar ou remover destinatários a uma tarefa com o tipo de duração do Trabalho Calculado, a Duração pode ser editada manualmente. À medida que os destinatários são adicionados ou removidos da tarefa, as Horas Planejadas são alteradas.

No exemplo a seguir, as Horas típicas por dia de trabalho são definidas como 8 nas Preferências do projeto em Configurar. Cada tarefa tem uma Duração de 1 dia. Conforme o número de destinatários muda, as Horas Planejadas mudam com base no número de destinatários em uma determinada tarefa:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Número de Atributos (cada 100% alocado)</strong> </p> </th> 
   <th> <p><strong>Duração</strong> </p> </th> 
   <th> <p><strong>Horas planejadas</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 dia</p> </td> 
   <td> <p>8 Horas</p> <p>(1 Dia x 8 Horas por Dia de Trabalho x 1 Destinatário = 8 Horas Planejadas)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 dia</p> </td> 
   <td> <p>16 Horas</p> <p>(1 Dia x 8 Horas por Dia de Trabalho x 2 Destinatários = 16 Horas Planejadas)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 dia</p> </td> 
   <td> <p>24 Horas</p> <p>(1 Dia x 8 Horas por Dia de Trabalho x 3 Destinatários = 24 Horas Planejadas)</p> </td> 
  </tr> 
 </tbody> 
</table>

Nesse caso, cada destinatário é 100% alocado para a tarefa Trabalho calculado.

![](assets/calcwork-350x71.png)

## Alterar o Tipo de duração de uma tarefa para Trabalho calculado

Para obter informações sobre como alterar o Tipo de duração de uma tarefa, consulte [Atualizar o Tipo de duração de uma tarefa](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
