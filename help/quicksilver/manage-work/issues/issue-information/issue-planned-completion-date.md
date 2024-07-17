---
product-area: projects
navigation-topic: issue-information
title: Visão geral da Data de conclusão planejada do problema
description: A data de conclusão planejada de uma ocorrência é a data até a qual a ocorrência deve terminar.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# Visão geral da Data de conclusão planejada do problema

A data de conclusão planejada de uma ocorrência é a data até a qual a ocorrência deve terminar.

Você pode especificar a Data de conclusão planejada de um problema ou deixá-la a cargo da Adobe Workfront para calculá-la, dependendo de determinados critérios. 

As datas de conclusão planejadas dos problemas não afetam a data de conclusão planejada do projeto. Somente as datas de conclusão planejadas das tarefas afetam a data de conclusão planejada do projeto. Para obter mais informações sobre a Data de Conclusão Planejada do projeto, consulte [Definir a Data de Conclusão Planejada do projeto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>A Data de conclusão planejada de um problema difere da Data de confirmação do problema ou da Data de conclusão projetada do problema das seguintes maneiras:
>
>* A Data de Compromisso é a data pela qual a pessoa atribuída à emissão estima manualmente que terá concluído a emissão. Para obter mais informações, consulte os seguintes artigos:
>
>   * [Visão geral da Data de confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interações entre a Data de Confirmação e a Data de Conclusão Planejada](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* A data de conclusão projetada é uma data calculada pela Workfront que leva em conta fatores externos para determinar uma data real para quando o problema pode ser realisticamente concluído. Para obter mais informações, consulte [Visão geral da Data de conclusão projetada para projetos, tarefas e problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Definir manualmente a Data de conclusão planejada de um problema

Você deve ter acesso para Editar problemas e Gerenciar permissões sobre o problema para poder atualizar a Data de conclusão planejada do problema.

Você pode definir manualmente a Data de conclusão planejada de um problema nas seguintes áreas do Workfront:

* Na caixa Editar problema ou na área Detalhes do problema ao criar ou editar um problema. Para obter informações, consulte [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md).
* Na área Página inicial, se a Data de conclusão planejada for exibida ao visualizar um problema. Para obter informações, consulte [Atualizar ou editar um item de trabalho na área Página Inicial](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* No cabeçalho do problema. Para obter informações, consulte [Novos cabeçalhos de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* Em uma lista de problemas ou relatório quando o campo Data de conclusão planejada é exibido na visualização.

  Para obter informações, consulte [Editar problemas em uma lista](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Como o Workfront calcula automaticamente a Data de conclusão planejada para um problema

Quando a Workfront calcula a Data de conclusão planejada de um problema automaticamente, o seguinte pode influenciar a data:

* Data de Início Planejada

  A Data de entrada e a Data inicial planejada devem corresponder a uma ocorrência quando você a cria pela primeira vez.

* A duração padrão conforme configurada na seção Detalhes da fila do projeto. Para obter informações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

  Se a Duração padrão for 0 dias, a Data de conclusão planejada corresponderá à Data inicial planejada do problema.

* Cronograma do Projeto

Quando definida automaticamente, a Data de conclusão planejada é determinada com base no seguinte cálculo: 

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Exemplo:** Por exemplo, se sua tarefa tiver uma data de início de sexta-feira, 14 de janeiro e a Duração padrão for 5 dias, a Data de conclusão planejada será sexta-feira, 21 de janeiro, se o Cronograma do projeto for de segunda a sexta-feira por 8 horas por dia.

As seguintes situações existem:

* Se o projeto não tiver um Cronograma, o Cronograma padrão do sistema Workfront será considerado. Para obter informações, consulte [Visão geral dos cronogramas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* Se a Programação for de segunda a sexta das 9h às 13h (4 horas por dia) e as horas típicas do seu sistema Workfront por dia de trabalho forem 8 horas, a Data de conclusão planejada será 27 de janeiro.

>[!TIP]
>
>O Workfront leva em consideração Exceções de programação, como feriados e finais de semana, ao calcular Datas de conclusão planejadas.

 
