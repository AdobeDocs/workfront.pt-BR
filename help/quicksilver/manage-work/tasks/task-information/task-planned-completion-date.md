---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral da Data de conclusão planejada da tarefa
description: A Data de conclusão planejada de uma tarefa é a data na qual a tarefa está definida para ser concluída.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 1%

---

# Visão geral da Data de conclusão planejada da tarefa

A Data de conclusão planejada de uma tarefa é a data na qual a tarefa está definida para ser concluída.

Você pode especificar a Data de conclusão planejada de uma tarefa ou deixá-la a cargo do Adobe Workfront para calculá-la, dependendo de determinados critérios. 

As Datas de conclusão planejadas das tarefas em um projeto determinam a Data de conclusão planejada de um projeto quando ele estiver programado a partir da Data inicial. Para obter mais informações sobre a Data de Conclusão Planejada do projeto, consulte [Definir a Data de Conclusão Planejada do projeto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>A Data de conclusão planejada de uma tarefa difere da Data de confirmação da tarefa ou da Data de conclusão projetada da tarefa das seguintes maneiras:
>
>* A Data de Compromisso é a data pela qual a pessoa atribuída à tarefa estima manualmente que ela terá concluído a tarefa. Para obter mais informações, consulte os seguintes artigos:
>
>   * [Visão geral da Data de confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interações entre a Data de Confirmação e a Data de Conclusão Planejada](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* A Data de conclusão projetada é uma data calculada pela Workfront e leva em conta atrasos da tarefa, linhas do tempo da tarefa ou de suas predecessoras e outros fatores para determinar uma data da vida real para quando a tarefa pode ser concluída realisticamente. Para obter mais informações, consulte [Visão geral da Data de conclusão projetada para projetos, tarefas e problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Definir manualmente a Data de conclusão planejada de uma tarefa

Você deve ter acesso para Editar a Tarefas e Gerenciar permissões na tarefa para poder atualizar a Data de conclusão planejada da tarefa.

Definir a Data de conclusão planejada de uma tarefa depende do tipo de Restrição de tarefa que você atribui à tarefa. 

Você pode definir manualmente a Data de conclusão planejada nas seguintes áreas do Workfront:

* Na caixa Editar tarefa, ao criar ou editar uma tarefa. Para obter informações, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* Na área Detalhes da tarefa. Para obter informações, consulte [Gerenciar informações da tarefa na área Visão Geral de Detalhes da Tarefa](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* Na área Início, se a Data de conclusão planejada for exibida durante a visualização de uma tarefa. Para obter informações, consulte [Atualizar ou editar um item de trabalho na área Página Inicial](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* No cabeçalho da tarefa. Para obter informações, consulte [Novos cabeçalhos de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* Em uma lista de tarefas ou relatório quando o campo Data de conclusão planejada é exibido na exibição.

  Para obter informações, consulte [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Você pode especificar manualmente a Data de Conclusão Planejada ao selecionar qualquer uma das seguintes Restrições de Tarefa: 

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
   <td> <p>Precisa Terminar Em</p> <p>Não Terminar Depois De</p> <p>Não Terminar Antes De</p> </td> 
   <td> <p><span class="s1">A Data de Início Planejada é ajustada para manter a Duração igual.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Datas Fixas</p> </td> 
   <td> <p>A Duração é ajustada para manter a Data inicial planejada igual.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Como o Workfront calcula automaticamente a Data de conclusão planejada para uma tarefa

Quando é calculado automaticamente pelo sistema, o seguinte pode influenciar a Data de conclusão planejada de uma tarefa:

* Restrição de Tarefa

  Para obter mais informações sobre Restrições de Tarefa, consulte o artigo [Visão geral sobre Restrições de Tarefa](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relacionamento de predecessora da tarefa

  Para obter mais informações sobre predecessores de tarefas, consulte o artigo [Visão geral dos predecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Data de conclusão do projeto, quando o projeto é agendado a partir da Data de conclusão.
* O horário de folga do Principal Responsável da tarefa.

  Quando o Destinatário Principal tiver uma folga agendada durante a duração da tarefa, as datas planejadas da tarefa serão ajustadas de acordo quando a configuração **Considerar folga do usuário nas durações da tarefa** for selecionada para o campo **Tempo de folga do usuário**. Novos projetos herdam essa configuração da área Preferências do projeto, mas você pode editar a configuração no nível do projeto.

  Por exemplo, se uma tarefa com uma Restrição o Mais Breve Possível estiver programada para iniciar em 1° de junho e terminar em 3 de junho, e o Destinatário principal tiver o dia 2 de junho marcado para Folga, a Data de conclusão planejada da tarefa será 4 de junho.

  Para obter informações sobre a preferência **Tempo de folga do usuário**, consulte os artigos [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

* A quantidade de tempo associada às Configurações de aprovação se a tarefa estiver associada a uma aprovação. Para obter mais informações, consulte [Definir configurações de aprovação global](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Quando definida automaticamente, a Data de conclusão planejada é determinada com base no seguinte cálculo: 

```
Planned Completion Date = Planned Start Date + Duration
```

Por exemplo, se sua tarefa tiver uma data de início de 16 de setembro e uma Duração de 10 dias, a Data de conclusão planejada será 26 de setembro.

>[!NOTE]
>
> O Tipo de atualização do projeto deve ser definido como Automático e Mediante alteração ou Automaticamente para que as Horas planejadas e a Duração sejam ajustadas automaticamente.\
>Para obter mais informações sobre o Tipo de Atualização, consulte o artigo [Selecionar o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
