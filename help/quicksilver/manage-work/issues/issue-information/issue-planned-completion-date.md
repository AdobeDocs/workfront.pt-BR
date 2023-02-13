---
product-area: projects
navigation-topic: issue-information
title: Visão geral do problema Data de conclusão planejada
description: A Data de conclusão planejada de um problema é a data na qual o problema deve ser concluído.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Visão geral do problema Data de conclusão planejada

A Data de conclusão planejada de um problema é a data na qual o problema deve ser concluído.

Você pode especificar a Data de conclusão planejada de um problema ou deixar que o Adobe Workfront calcule o valor dependendo de determinados critérios. 

As Datas de Conclusão Planejadas dos problemas não afetam a Data de Conclusão Planejada do projeto. Somente as Datas de conclusão planejadas das tarefas afetam a Data de conclusão planejada do projeto. Para obter mais informações sobre a Data de Conclusão Planejada do projeto, consulte [Definir a data de conclusão planejada do projeto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>A Data de conclusão planejada de um problema difere da Data de confirmação da emissão ou da Data de conclusão projetada do problema das seguintes maneiras:
>
>* A Data da Confirmação é a data pela qual a pessoa atribuída à emissão estima manualmente que ela terá concluído a emissão. Para obter mais informações, consulte os seguintes artigos:
   * [Visão geral da data de confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [Interações entre a Data de Confirmação e a Data de Conclusão Planejada](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* A Data de conclusão projetada é uma data calculada pela Workfront que leva em conta fatores externos para determinar uma data real para quando o problema pode ser realisticamente concluído. Para obter mais informações, consulte [Visão geral da data de conclusão projetada para projetos, tarefas e problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## Definir manualmente a Data de conclusão planejada de um problema

Você deve ter o acesso Editar a Problemas e as permissões Gerenciar no problema para atualizar a Data de conclusão planejada do problema.

Você pode definir manualmente a Data de conclusão planejada de um problema nas seguintes áreas do Workfront:

* Na caixa Editar ocorrência ou na área Detalhes da ocorrência ao criar ou editar um problema. Para obter mais informações, consulte [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md).
* Na área inicial, se a Data de conclusão planejada for exibida ao visualizar um problema. Para obter mais informações, consulte [Atualizar ou editar um item de trabalho na área Início](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* No cabeçalho da edição. Para obter mais informações, consulte [Novos cabeçalhos de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* Em uma lista de problemas ou relatório quando o campo Data de conclusão planejada for exibido na visualização.

   Para obter mais informações, consulte [Editar problemas em uma lista](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Como o Workfront calcula automaticamente a Data de conclusão planejada para um problema

Quando o Workfront calcula a Data de conclusão planejada de um problema automaticamente, o seguinte pode influenciar a data:

* Data de início planejada

   A Data de entrada e a Data inicial planejada devem corresponder em um problema ao criar o problema pela primeira vez.

* A Duração padrão conforme configurado na seção Detalhes da fila do projeto. Para obter mais informações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Se a Duração padrão for 0 dias, a Data de conclusão planejada corresponderá à Data inicial planejada do problema.

* Agendamento do projeto

Quando definida automaticamente, a Data de conclusão planejada é determinada com base no seguinte cálculo: 

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Exemplo:** Por exemplo, se sua tarefa tiver uma data de início de sexta-feira, 14 de janeiro e a Duração padrão for 5 dias, a Data de conclusão planejada será sexta-feira, 21 de janeiro, se a Programação do projeto for segunda-feira a sexta-feira por 8 horas por dia.

As seguintes situações existem:

* Se o projeto não tiver um agendamento, o agendamento padrão do sistema Workfront será considerado. Para obter mais informações, consulte [Visão geral dos agendamentos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* Se o Agendamento for de segunda a sexta-feira das 9h às 1 P.M. (4 horas por dia) e as Horas típicas de seu sistema Workfront por dia de trabalho forem de 8 horas, a Data de conclusão planejada será 27 de janeiro.

>[!TIP]
A Workfront considera as Exceções de Programação, como feriados e fins de semana, ao calcular as Datas de Conclusão Planejadas.

 
