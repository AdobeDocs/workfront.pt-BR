---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral da Data de Início Planejada da tarefa
description: A Data de Início Planejada de uma tarefa é a data em que você, como criador da tarefa, decide que o trabalho na tarefa deve começar. As datas das tarefas planejadas influenciam as datas e a linha do tempo do projeto. Para obter informações sobre a Data Inicial Planejada do projeto, consulte Visão Geral da Data Inicial Planejada do projeto.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: 0ff02569d3c7fb532a2faafc46fe4235ce77acd4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 2%

---

# Visão geral da Data de Início Planejada da tarefa

<!-- Audited: 6/2025 -->

A Data de Início Planejada de uma tarefa é a data em que você, como criador da tarefa, decide que o trabalho na tarefa deve começar. As datas das tarefas planejadas influenciam as datas e a linha do tempo do projeto. Para obter informações sobre a Data de Início Planejada do projeto, consulte [Visão Geral da Data de Início Planejada do projeto](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## A Data de Início Planejada de uma tarefa

Você pode especificar a Data de início planejada da tarefa ou deixá-la a cargo do Adobe Workfront para calculá-la, dependendo de determinados critérios. 

* [Definir manualmente a Data de Início Planejada de uma tarefa](#manually-set-the-planned-start-date-of-a-task)
* [Como a Data de Início Planejada é calculada para uma tarefa](#how-the-planned-start-date-is-calculated-for-a-task)

### Definir manualmente a Data de Início Planejada de uma tarefa {#manually-set-the-planned-start-date-of-a-task}

Definir a Data de Início Planejada de uma tarefa depende do tipo de Restrição de Tarefa que você atribui à tarefa. 

Você pode definir manualmente a Data de início planejada ao criar uma tarefa. Para obter mais informações, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Você pode especificar manualmente a Data de Início Planejada quando seleciona qualquer uma das seguintes Restrições de Tarefa: 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo de Restrição de Tarefa</strong> </p> </th> 
   <th> <p><strong>Efeito da Alteração Manual da Data de Término Planejada</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Precisa Iniciar Em</p> <p>Não Iniciar Antes De</p> <p>Não Iniciar Depois De</p> </td> 
   <td> <p><span class="s1">A Data de Conclusão Planejada é ajustada para manter a Duração igual.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Datas Fixas</p> </td> 
   <td> <p>A Duração é ajustada para manter a Data de conclusão planejada igual.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Como a Data de Início Planejada é calculada para uma tarefa {#how-the-planned-start-date-is-calculated-for-a-task}

Quando é calculado automaticamente pelo sistema, o seguinte pode influenciar a Data de início planejada de uma tarefa:

* A configuração da preferência Data inicial na área Tarefas e problemas em Configurar

  O administrador do Workfront ou do grupo pode determinar se uma nova tarefa inicia na mesma data que a Data de início planejada do projeto ou no dia em que você criou a tarefa.

  Para obter informações sobre preferências de tarefas e problemas, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Restrição de Tarefa

  Para obter mais informações sobre Restrições de Tarefa, consulte [Visão geral da Restrição de Tarefa](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relacionamento de predecessora da tarefa

  Para obter mais informações sobre predecessores de tarefas, consulte [Visão geral dos predecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Data de Início do Projeto, quando o projeto é agendado a partir da Data de Início.
* O horário de folga da Principal pessoa atribuída da tarefa.

  Quando o Principal responsável tiver uma folga programada durante a duração da tarefa, as datas planejadas da tarefa serão ajustadas de acordo quando a configuração Considerar a folga do usuário nas durações da tarefa for selecionada para o campo User Time Off. Novos projetos herdam essa configuração da área Preferências do projeto, mas você pode editar a configuração no nível do projeto.

  Por exemplo, se uma tarefa com uma Restrição o Mais Breve Possível estiver programada para iniciar em 1° de junho e terminar em 3 de junho, e o Destinatário principal tiver o dia 1° de junho marcado para folga, a tarefa Data de início planejada será marcada para 2° de junho.

  Para obter informações sobre a preferência Tempo livre do usuário, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

Quando definida automaticamente, a Data de Início Planejada é determinada com base no seguinte cálculo: 

```
Planned Start Date = Planned Completion Date - Task Duration
```

Por exemplo, se sua tarefa tiver uma Data de conclusão de 16 de setembro e uma duração de 10 dias, a Data de início planejada será 6 de setembro.

>[!NOTE]
>
> O Tipo de atualização do projeto também deve ser definido como Automático e Mediante alteração ou Automaticamente para que as Horas planejadas e a Duração sejam ajustadas automaticamente.\
>Para obter mais informações sobre o Tipo de Atualização, consulte [Selecionar o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
