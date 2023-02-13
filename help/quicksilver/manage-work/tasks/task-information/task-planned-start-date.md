---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral da data de início planejada da tarefa
description: A Data Inicial Planejada de uma tarefa é a data em que você, como o criador da tarefa, decide que o trabalho na tarefa deve ser iniciado. As datas da tarefa planejada influenciam as datas e a linha do tempo no projeto. Para obter informações sobre a Data Inicial Planejada do projeto, consulte Visão Geral da Data Inicial Planejada do projeto.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 2%

---

# Visão geral da data de início planejada da tarefa

A Data Inicial Planejada de uma tarefa é a data em que você, como o criador da tarefa, decide que o trabalho na tarefa deve ser iniciado. As datas da tarefa planejada influenciam as datas e a linha do tempo no projeto. Para obter informações sobre a Data Inicial Planejada do projeto, consulte [Visão geral da data de início planejada do projeto](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## A Data Inicial Planejada de uma tarefa

Você pode especificar a Data inicial planejada de uma tarefa ou pode deixar que o Adobe Workfront a calcule dependendo de determinados critérios. 

* [Definir manualmente a Data de início planejada de uma tarefa](#manually-set-the-planned-start-date-of-a-task)
* [Como a Data Inicial Planejada é calculada para uma tarefa](#how-the-planned-start-date-is-calculated-for-a-task)

### Definir manualmente a Data de início planejada de uma tarefa {#manually-set-the-planned-start-date-of-a-task}

Definir a Data Inicial Planejada de uma tarefa depende do tipo de Restrição de Tarefa que você atribui à tarefa. 

Você pode definir manualmente a Data inicial planejada ao criar uma tarefa, conforme descrito no artigo [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Você pode especificar manualmente a Data Inicial Planejada ao selecionar qualquer uma das seguintes Restrições de Tarefa: 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo de Restrição de Tarefa</strong> </p> </th> 
   <th> <p><strong>Efeito da alteração manual da data de conclusão planejada</strong> </p> </th> 
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

### Como a Data Inicial Planejada é calculada para uma tarefa {#how-the-planned-start-date-is-calculated-for-a-task}

Quando é calculado automaticamente pelo sistema, o seguinte pode influenciar a Data de início planejada de uma tarefa:

* A configuração de preferência Data de Início na área Tarefas e Problemas em Configurar

   Seu Workfront ou administrador de grupo pode determinar se uma nova tarefa começa na mesma data da Data de início planejada do projeto ou no dia em que você criou a tarefa.

   Para obter informações sobre as preferências de Tarefas e Problemas, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Restrição de Tarefa

   Para obter mais informações sobre Restrições de Tarefa, consulte o artigo [Visão geral da restrição de tarefa](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)

* Relação entre predecessores de tarefa

   Para obter mais informações sobre predecessores de tarefas, consulte o artigo [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Data de início do projeto, quando o projeto é agendado a partir da data de início.
* O horário de descarregamento do Destinatário Principal da tarefa.

   Quando o Destinatário Principal tiver tempo de folga programado durante a duração da tarefa, as datas planejadas da tarefa se ajustarão adequadamente quando a **Considere o tempo limite do usuário nas durações da tarefa** é selecionada para a variável **Tempo do usuário desligado** campo. Os novos projetos herdam essa configuração da área Preferências do projeto , mas você pode editar a configuração no nível do projeto.

   Por exemplo, se uma tarefa com uma Restrição do Mais Rápido Possível estiver programada para iniciar em 1° de junho e ser concluída em 3 de junho, e o Destinatário Principal tiver 1° de junho marcado para Tempo de Desativação, a tarefa Data de Início Planejado será 2 de junho.

   Para obter informações sobre o **Tempo do usuário desligado** , consulte os artigos  [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

Quando configurada automaticamente, a Data inicial planejada é determinada com base no seguinte cálculo: 

```
Planned Start Date = Planned Completion Date - Task Duration
```

Por exemplo, se sua tarefa tiver uma Data de conclusão de 16 de setembro e uma duração de 10 dias, a Data de início planejada será 6 de setembro.

>[!NOTE]
>
> O Tipo de atualização do projeto também deve ser definido como &quot;Automático e Em alteração&quot; ou &quot;Automaticamente&quot; para que as Horas e a Duração planejadas sejam ajustadas automaticamente.\
Para obter mais informações sobre o Tipo de atualização, consulte o artigo [Selecione o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
