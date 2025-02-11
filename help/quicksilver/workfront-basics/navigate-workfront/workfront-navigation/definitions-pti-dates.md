---
content-type: reference
navigation-topic: workfront-navigation
title: Visão geral das datas de Projeto, Tarefa e Problema em [!DNL Workfront]
description: Este artigo fornece definições para as datas mais comuns associadas a projetos, tarefas e problemas no [!DNL Adobe Workfront].
feature: Get Started with Workfront
author: Alina
exl-id: 3808200f-a573-4c39-8965-b254f69c893c
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '2357'
ht-degree: 3%

---

# Visão geral das datas de Projeto, Tarefa e Problema em [!DNL Workfront]

<!-- Audited: 05/2024 -->

<!--consider expanding on this article with ALL dates for PTIs - Hand off dates, Approval Dates, etc-->

<!-- there are dates below that need definition - ask Product-->

Este artigo fornece definições para as datas mais comuns associadas a projetos, tarefas e problemas no [!DNL Adobe Workfront]. As imagens incluídas aqui são exemplos de onde as datas são exibidas no Workfront e não são exaustivas. Há outras áreas que exibem as datas. Todas as datas também estão visíveis nos relatórios e listas de projetos, tarefas e problemas.

Para obter informações sobre relatórios e listas, consulte os seguintes artigos:

* [Introdução a listas em  [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)
* [Introdução a relatórios](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)

Para obter mais informações sobre campos de projeto, tarefa e problema, consulte [Glossário de [!DNL Adobe Workfront] terminologia](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).


## [!UICONTROL Data de Início Efetivo]

A [!UICONTROL Data de Início Efetivo] é a data em que um usuário começa realmente a trabalhar em um projeto, tarefa ou problema. A [!UICONTROL Data de Início Efetiva] fica vazia quando o projeto, tarefa ou problema é criado.

Você pode indicar manualmente quando o trabalho começou em uma tarefa ou um problema, ou a [!UICONTROL Data de Início Efetivo] é preenchida automaticamente quando o status da tarefa ou do problema muda de [!UICONTROL Novo] para [!UICONTROL Em Andamento] ou [!UICONTROL Concluído]. A [!UICONTROL Data de Início Efetivo] de um projeto coincide com a data em que a primeira tarefa do projeto começa.

>[!TIP]
>
>A [!UICONTROL Data de Início Efetivo] pode não corresponder à [!UICONTROL Data de Início Planejada] de um projeto, tarefa ou problema porque o usuário pode começar a trabalhar mais tarde ou antes da data planejada.

Para obter mais informações, consulte [Visão Geral do projeto [!UICONTROL Data de Início Efetivo]](../../../manage-work/projects/planning-a-project/project-actual-start-date.md).

>[!NOTE]
>
>A [!UICONTROL Data de Início] ou as restrições de Datas Fixas afetam a [!UICONTROL Data de Início Planejada] de uma tarefa, não a [!UICONTROL Data de Início Efetivo]. Isto atualizará a [!UICONTROL Data de Início Planejada] para uma data que você especificar. A [!UICONTROL Data de Início Efetivo] é atualizada independentemente da [!UICONTROL Data de Início Planejada], conforme descrito acima.

![Data de início efetiva na tarefa de edição](assets/actual-start-date-on-edit-task-highlighted-nwe-350x251.png)

![Data de início efetiva na tarefa](assets/actual-start-date-on-task-details-highlighted-nwe-350x191.png)

## [!UICONTROL Data de Término Efetivo]

A [!UICONTROL Data de Término Efetivo] é a data em que um usuário realmente conclui um projeto, tarefa ou problema. A [!UICONTROL Data de Término Efetivo] fica vazia quando o projeto, tarefa ou problema é criado.

Você pode indicar manualmente quando o trabalho é concluído em uma tarefa ou problema, ou a [!UICONTROL Data de Término Efetivo] é preenchida automaticamente quando qualquer uma das seguintes situações ocorrer:

* O status do projeto, da tarefa ou do problema muda para [!UICONTROL Concluído], [!UICONTROL Fechado] ou [!UICONTROL Resolvido].
* A porcentagem concluída da tarefa ou do projeto é 100%.

A [!UICONTROL Data de Término Efetivo] de um projeto coincide com a data em que você concluiu a última tarefa do projeto.

>[!TIP]
>
>A [!UICONTROL Data de Término Efetivo] pode não corresponder à [!UICONTROL Data de Término Planejada].

Para obter mais informações, consulte [Visão geral do projeto [!UICONTROL Data de Término Efetivo]](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

![Data de Término Efetivo em Detalhes](assets/actual-completion-date-task-details-highlighted-nwe-350x189.png)

## Data de conclusão do caminho de aprovação

A Data de conclusão do caminho de aprovação é a data em que a aprovação de um projeto, tarefa ou problema foi concedida e o status do item foi alterado.

A Data de conclusão do caminho de aprovação é visível em listas e relatórios de projetos, tarefas e problemas.

## Data de início do caminho de aprovação

A Data inicial do caminho de aprovação é a data em que o status do projeto, tarefa ou problema foi alterado para &quot;Aprovação pendente&quot; e a solicitação de aprovação do projeto foi enviada aos aprovadores.

A data de início do caminho de aprovação está visível em listas e relatórios de projetos, tarefas e problemas.

<!--## Auto Closure Date -->

## Data de conclusão orçada

Este é um campo obsoleto para projetos. Qualquer informação que este campo possa exibir em uma lista ou relatório está relacionada a um recurso que a Workfront removeu. Este campo não pode ser atualizado.

O campo fica visível nos relatórios e listas do projeto.

## Data de início orçada

Este é um campo obsoleto para projetos. Qualquer informação exibida neste campo está relacionada a um recurso removido pelo Workfront. Este campo não pode ser atualizado.

O campo fica visível nos relatórios e listas do projeto.

## [!UICONTROL Data de confirmação]

A [!UICONTROL Data de Confirmação] é a data na qual um usuário atribuído a uma tarefa ou problema confirma a conclusão da tarefa ou do problema. Isso é diferente da [!UICONTROL Data de conclusão planejada], pois é uma estimativa mais realista da data de conclusão fornecida somente pelo usuário responsável pelo trabalho. Para obter mais informações, consulte [[!UICONTROL Data de confirmação] visão geral](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

>[!NOTE]
>
>Alterar a [!UICONTROL Data de Confirmação] afeta a [!UICONTROL Data de Conclusão Projetada], mas não a [!UICONTROL Data de Conclusão Planejada] de uma tarefa ou um problema. O gerente de projeto pode usar as alterações feitas por um signatário na [!UICONTROL Data de Confirmação] para atualizar a [!UICONTROL Data de Conclusão Planejada] de uma tarefa ou um problema.

<!--## Completion Pending Date-->

## Data de Restrição

Se você estiver usando uma Restrição de Tarefa vinculada a uma data específica, essa data específica se tornará a Data de Restrição da tarefa.

As seguintes restrições de tarefa atualizam o campo Data de Restrição:

* Precisa Iniciar Em
* Precisa Terminar Em
* Não Iniciar Depois De
* Não Iniciar Antes De

>[!TIP]
>
>Uma tarefa com Restrição de Datas Fixas não tem Data de Restrição.
>

A Data de Restrição é visível em uma lista de tarefas ou relatório.

## Data de entrada do problema convertido

A data em que o problema que foi convertido no projeto ou na tarefa foi criada.

A Data de entrada do problema convertido está visível em listas de projetos e tarefas e relatórios.

## Data vencida

A data em que uma tarefa ou um problema deve ser concluído. A Data de Vencimento de uma tarefa ou problema é a mesma data que a Data de Conclusão Planejada.

A Data de Conclusão da tarefa e do problema está visível nas listas de tarefas e problemas e nos relatórios.

Para obter informações, consulte a seção [Data de conclusão planejada](#planned-completion-date) neste artigo.

## Concluir em

A data de conclusão do projeto. A data de conclusão de um projeto é igual à Data de conclusão planejada do projeto.

A data de conclusão do projeto está visível em listas e relatórios de projetos.

Para obter informações, consulte a seção [Data de conclusão planejada](#planned-completion-date) neste artigo.

## [!UICONTROL Data de entrada]

A [!UICONTROL Data de Entrada] é a data em que um projeto, tarefa ou problema foi criado em [!DNL Workfront].

A [!UICONTROL Data de Entrada] não influencia a linha do tempo de projetos, tarefas ou problemas, mas é importante para fins de rastreamento e relatórios. [!DNL Workfront] gera automaticamente a [!UICONTROL Data de Entrada] quando o objeto é criado e você não pode editá-lo manualmente.

![Data de entrada nos detalhes da tarefa](assets/entry-date-in-task-details-highlighted-nwe.png)

## Data de Vencimento Estimada

A data de conclusão estimada da tarefa e do projeto mostra uma data mais realista de quando o projeto ou a tarefa devem ser concluídos.

As datas estimadas estão mais de acordo com a realidade do projeto e da tarefa, uma vez que têm em conta o que influencia a conclusão efetiva do projeto ou da tarefa. As Datas de Vencimento Estimadas são semelhantes às Datas de Conclusão Projetadas.

Para obter mais informações, consulte [Visão geral das datas projetadas e estimadas](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md).

As Datas de Vencimento Estimadas do projeto e da tarefa estão visíveis nas listas de projetos e tarefas e nos relatórios.

## Data de Início Estimada

A Data de início estimada da tarefa e do projeto mostra uma data mais realista de quando o projeto ou a tarefa poderiam começar.

As datas estimadas estão mais de acordo com a realidade do projeto e da tarefa, uma vez que têm em conta o que influencia o início real do projeto ou da tarefa. As Datas de Início Estimadas são semelhantes às Datas de Início Projetadas.

Para obter mais informações, consulte [Visão geral das datas projetadas e estimadas](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md).

As Datas de início estimadas do projeto e da tarefa estão visíveis em listas de projetos e tarefas e relatórios.

<!--## Exchange Rate Date-->

## Data de Término Fixa

O solicitante ou proprietário do projeto identifica a Data de término fixa de um projeto ao concluir o Business Case. É a data na qual eles recomendam que o projeto seja concluído.

Trata-se de uma estimativa manual e não leva em conta o andamento real das tarefas no projeto.

A Data de término fixa de um projeto está visível na seção Business Case do projeto, bem como em listas e relatórios de projeto.

![Data final fixa](assets/fixed-end-date-business-case-highlight.png)

## Data de Início Fixa

O solicitante ou proprietário do projeto identifica a Data de início fixa de um projeto ao concluir o Business Case. É a data até a qual eles recomendam que o projeto tenha início.

Trata-se de uma estimativa manual e não leva em conta o andamento real das tarefas no projeto.

A Data de início fixa de um projeto está visível na seção Business Case do projeto, bem como em listas e relatórios de projeto.

![Data de início fixa](assets/fixed-start-date-business-case-highlight.png)

## Data de Transferência

A data em que uma tarefa se torna disponível para trabalho. Isso significa que todas as restrições, aprovações e dependências foram concluídas e os usuários podem começar a trabalhar na tarefa.

A Data de Transferência é um cálculo e não pode ser definida manualmente.

Para obter mais informações sobre a Data de Transferência, consulte [Visão geral da Data de Transferência da Tarefa](/help/quicksilver/manage-work/tasks/task-information/handoff-task-date.md).

A Data de Transferência de uma tarefa é visível em listas de tarefas e relatórios.

## Última Dt Atual Financ

A data em que qualquer informação financeira de um projeto foi atualizada. Isso inclui a atualização de campos financeiros na seção Finanças ou na seção Business Case do projeto.

A Última Data de Atualização Financeira está visível em listas e relatórios de projeto.

## Última data de atualização

A data em que o projeto, tarefa ou problema foi atualizado pela última vez. Uma atualização é considerada qualquer alteração que aciona o salvamento de um projeto, tarefa ou problema. Isso inclui alterações de status, condição, linha do tempo, finanças ou qualquer outro campo.

A Data da última atualização está visível nas listas e relatórios de projetos, tarefas e problemas.

## [!UICONTROL Data de Entrada da Hora]

Quando você registra horas para projetos, tarefas e problemas para indicar quanto tempo real (em horas) você gasta trabalhando no projeto, tarefa ou problema, o tempo que você registra torna-se as [!UICONTROL Horas efetivas] do projeto, tarefa ou problema.

A data para a qual você registra a hora é o campo [!UICONTROL Data de Entrada da Hora] na entrada da hora.

A Data de entrada de hora é visível em listas de horas e relatórios.

>[!TIP]
>
>A [!UICONTROL Data de Entrada] de uma hora é diferente da [!UICONTROL Data de Entrada] de outro objeto do Workfront, pois não é a data em que o log de horas foi criado, mas sim a data com a qual você deseja que as horas sejam associadas.
>
>Por exemplo, você pode registrar horas para uma tarefa em 5 de setembro, mas associar as horas com 1º de setembro. A Data de Entrada da hora é 1º de setembro.

Para obter informações sobre como registrar horas no Workfront, consulte [Registrar horas](../../../timesheets/create-and-manage-timesheets/log-time.md).

>[!TIP]
>
>Recomendamos registrar tempo em tarefas e problemas de trabalho, em vez de tarefas ou projetos principais. O tempo registrado nas tarefas de trabalho totaliza as tarefas pai e o projeto como [!UICONTROL Horas Reais] para as tarefas pai e o projeto. O tempo registrado nos problemas é acumulado no projeto como [!UICONTROL Horas efetivas] para o projeto.

## [!UICONTROL Data de Término Planejada]

A [!UICONTROL Data de Conclusão Planejada] ou a data [!UICONTROL De Término] é a data em que há planos para a conclusão de um projeto, tarefa ou problema.

Dependendo da [!UICONTROL Restrição de Tarefa], talvez você não consiga editar a [!UICONTROL Data de Conclusão Planejada] de uma tarefa. Dependendo do [!UICONTROL Modo de Agendamento] do projeto, talvez você não possa editar a [!UICONTROL Data de Conclusão Planejada] de um projeto.

A [!UICONTROL Data de conclusão planejada] é exibida como a data de vencimento em algumas áreas de [!DNL Workfront].

Para obter mais informações, consulte os seguintes artigos:

* [Visão geral da tarefa [!UICONTROL Data de conclusão planejada]](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Definir a [!UICONTROL Data de Término Planejada] do projeto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Visão geral do problema [!UICONTROL Data de conclusão planejada]](../../../manage-work/issues/issue-information/issue-planned-completion-date.md)

![Data de conclusão planejada no cabeçalho](assets/project-header-planned-completion-date-highlighted-nwe-350x34.png)

![Data de conclusão planejada na lista de tarefas](assets/planned-completion-date-in-task-list-highlighted-nwe-350x183.png)


## Alinhamento de Data Planejada

Este é um indicador automático que o Workfront atribui a projetos, tarefas e problemas para mostrar quando um item será concluído em relação à Data de conclusão planejada.

A seguir estão os valores possíveis para o indicador de Alinhamento de Data Planejada:

* Será terminado na data planejada de término
* Será terminado antes da data planejada de término
* Será terminado depois da data planejada de término

O Alinhamento da data planejada está visível em listas e relatórios de projetos, tarefas e problemas.

## [!UICONTROL Data de Início Planejada]

A [!UICONTROL Data de Início Planejada] é a data em que um projeto, tarefa ou problema está planejado para começar.

Dependendo da [!UICONTROL Restrição de Tarefa], talvez você não consiga editar a [!UICONTROL Data de Início Planejada] de uma tarefa. Dependendo do [!UICONTROL Modo de Agendamento] do projeto, talvez você não possa editar a [!UICONTROL Data de Início Planejada] de um projeto.

Para obter mais informações, consulte [Visão geral do projeto [!UICONTROL Data de Início Planejada]](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

![Data de início planejada na tarefa de edição](assets/planned-start-date-on-edit-task-highlighted-nwe.png)

![Data de início dos planos na lista de tarefas](assets/planned-start-date-in-task-list-highlighted-nwe-350x167.png)

## [!UICONTROL Data de Término Projetada]

A [!UICONTROL Data de Conclusão Projetada] é um indicador calculado em tempo real de quando o projeto, tarefa ou problema será concluído. Quando o projeto, tarefa ou problema é marcado como Concluído, a [!UICONTROL Data de Conclusão Projetada] muda para a data da [!UICONTROL Data de Conclusão Efetiva].

Se tudo correr bem e conforme planejado, a [!UICONTROL Data de conclusão projetada] deve corresponder à [!UICONTROL Data de conclusão planejada]. Caso contrário, devido a atrasos nas tarefas predecessoras, a [!UICONTROL Data de Conclusão Projetada] pode se tornar diferente da [!UICONTROL Data de Conclusão Planejada].

Para obter mais informações, consulte [Visão geral da [!UICONTROL Data de conclusão projetada] para projetos, tarefas e problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

![Data de término projetada](assets/projected-completion-date-in-task-details-highlighted-nwe-350x187.png)

## [!UICONTROL Data de Início Projetada]

A [!UICONTROL Data de Início Projetada] é uma data em tempo real em que o projeto, tarefa ou problema começa e leva em consideração todos os atrasos. Esta é uma Data de Início mais precisa para o projeto, tarefa ou problema do que a [!UICONTROL Data de Início Planejada]. A [!UICONTROL Data de Início Planejada] não considera atrasos ou datas passadas.

Quando você planeja um projeto pela primeira vez, a [!UICONTROL Data de Início Planejada] e a [!UICONTROL Data de Início Projetada] das tarefas e do projeto são idênticas. Como podem ocorrer atrasos ou as tarefas podem ser concluídas anteriormente, a [!UICONTROL Data de Início Projetada] pode se tornar diferente da [!UICONTROL Data de Início Planejada].

Para uma tarefa, uma [!UICONTROL Data de Início Projetada] também pode diferir de sua [!UICONTROL Data de Início Planejada] quando um de seus predecessores estiver atrasado no agendamento.

>[!TIP]
>
>Você pode exibir a [!UICONTROL Data de Início Projetada] de um problema somente em uma lista ou relatório.

Para obter mais informações, consulte [Visão geral do projeto [!UICONTROL Data de Início Projetada]](../../../manage-work/projects/planning-a-project/project-projected-start-date.md).

![Data de início projetada](assets/projected-start-date-in-task-details-highlighted-nwe-350x188.png)

<!--## Rejection Date-->

## Data do Slack

Às vezes, as tarefas podem ser iniciadas e concluídas com atraso sem afetar a Data de conclusão do projeto.

A Data do Slack exibe a data exata em que uma tarefa poderia definitivamente afetar a Data de conclusão do projeto.

Para obter informações sobre a Data Slack de uma tarefa, consulte [Visão geral da Data Slack da Tarefa](/help/quicksilver/manage-work/tasks/task-information/task-slack-date.md).

As Datas de Slack de tarefas estão visíveis em listas de tarefas e relatórios.

## Início em

A data planejada de início do projeto. A data de início de um projeto é igual à data de início planejada do projeto.

Este campo está visível em listas de projetos e relatórios.

Para obter informações, consulte a seção [Data de Início Planejada](#planned-start-date) neste artigo.



