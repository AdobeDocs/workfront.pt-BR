---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral da data de conclusão planejada da tarefa
description: A Data de Conclusão Planejada de uma tarefa é a data na qual a tarefa é definida como concluída.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 1%

---

# Visão geral da data de conclusão planejada da tarefa

A Data de Conclusão Planejada de uma tarefa é a data na qual a tarefa é definida como concluída.

Você pode especificar a Data de conclusão planejada de uma tarefa, ou pode deixar que o Adobe Workfront a calcule dependendo de determinados critérios. 

As Datas de conclusão planejadas das tarefas em um projeto determinam a Data de conclusão planejada de um projeto quando o projeto é agendado a partir da Data inicial. Para obter mais informações sobre a Data de Conclusão Planejada do projeto, consulte [Definir a data de conclusão planejada do projeto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>A Data de Conclusão Planejada de uma tarefa é diferente da Data de Confirmação da tarefa ou da Data de Conclusão Projetada da tarefa das seguintes maneiras:
>
>* A Data de Confirmação é a data pela qual a pessoa atribuída à tarefa estima manualmente que ela terá concluído a tarefa. Para obter mais informações, consulte os seguintes artigos:
   * [Visão geral da data de confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [Interações entre a Data de Confirmação e a Data de Conclusão Planejada](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* A Data de Conclusão Projetada é uma data calculada pela Workfront e considera atrasos na tarefa, linhas do tempo da tarefa ou seus antecessores e outros fatores para determinar uma data da vida real para quando a tarefa pode ser realisticamente concluída. Para obter mais informações, consulte [Visão geral da data de conclusão projetada para projetos, tarefas e problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## Definir manualmente a Data de conclusão planejada de uma tarefa

Você deve ter o acesso Editar às Tarefas e as permissões Gerenciar na tarefa para atualizar a Data de conclusão planejada da tarefa.

Definir a Data de Conclusão Planejada de uma tarefa depende do tipo de Restrição de Tarefa que você atribui à tarefa. 

Você pode definir manualmente a Data de conclusão planejada nas seguintes áreas do Workfront:

* Na caixa Editar tarefa, ao criar ou editar uma tarefa. Para obter mais informações, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* Na área Detalhes da tarefa. Para obter mais informações, consulte [Gerenciar informações da tarefa na área Visão geral de detalhes da tarefa](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* Na área Inicial, se a Data de Conclusão Planejada for exibida ao visualizar uma tarefa. Para obter mais informações, consulte [Atualizar ou editar um item de trabalho na área Início](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* No cabeçalho da tarefa. Para obter mais informações, consulte [Novos cabeçalhos de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* Em uma lista de tarefas ou relatório quando o campo Data de Conclusão Planejada é exibido na exibição.

   Para obter mais informações, consulte [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Você pode especificar manualmente a Data de Conclusão Planejada ao selecionar qualquer uma das seguintes Restrições de Tarefa: 

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
   <td> <p>Precisa Terminar Em</p> <p>Não Terminar Depois De</p> <p>Não Terminar Antes De</p> </td> 
   <td> <p><span class="s1">A Data de início planejada é ajustada para manter a Duração igual.</span> </p> </td> 
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

   Para obter mais informações sobre Restrições de Tarefa, consulte o artigo [Visão geral da restrição de tarefa](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relação entre predecessores de tarefa

   Para obter mais informações sobre predecessores de tarefas, consulte o artigo [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Data de conclusão do projeto, quando o projeto é agendado a partir da data de conclusão.
* O horário de descarregamento do Destinatário Principal da tarefa.

   Quando o Destinatário Principal tiver tempo de folga programado durante a duração da tarefa, as datas planejadas da tarefa se ajustarão adequadamente quando a **Considere o tempo limite do usuário nas durações da tarefa** é selecionada para a variável **Tempo do usuário desligado** campo. Os novos projetos herdam essa configuração da área Preferências do projeto , mas você pode editar a configuração no nível do projeto.

   Por exemplo, se uma tarefa com uma Restrição do Mais Rápido Possível estiver programada para iniciar em 1° de junho e ser concluída em 3 de junho, e o Destinatário principal tiver o 2 de junho marcado para Tempo de Desativação, a Data de Conclusão Planejada será 4 de junho.

   Para obter informações sobre o **Tempo do usuário desligado** , consulte os artigos [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

* O tempo associado às Configurações de aprovação se a tarefa estiver associada a uma aprovação. Para obter mais informações, consulte [Definir configurações de aprovação global](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Quando definida automaticamente, a Data de conclusão planejada é determinada com base no seguinte cálculo: 

```
Planned Completion Date = Planned Start Date + Duration
```

Por exemplo, se sua tarefa tiver uma data de início de 16 de setembro e uma Duração de 10 dias, a Data de conclusão planejada será 26 de setembro.

>[!NOTE]
 O Tipo de atualização do projeto deve ser definido como Automático e Ativado ou Automaticamente para que as Horas e a Duração Planejadas sejam ajustadas automaticamente.\
Para obter mais informações sobre o Tipo de atualização, consulte o artigo [Selecione o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
