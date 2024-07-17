---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral da data de transferência da tarefa
description: A Data de Transferência é a data em que uma tarefa se torna disponível para trabalho. Normalmente, isso significa que suas predecessoras foram resolvidas e o destinatário da tarefa pode começar a trabalhar nela.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 2%

---

# Visão geral da data de transferência da tarefa

A Data de Transferência é a data em que uma tarefa se torna disponível para trabalho. Normalmente, isso significa que suas predecessoras foram resolvidas e o destinatário da tarefa pode começar a trabalhar nela.

>[!TIP]
>
>Não existem datas de transferência para problemas e projetos.

## Como a Adobe Workfront calcula a data de transferência

>[!NOTE]
>
>A Data de Transferência é calculada somente se o status do projeto for igual aos seguintes status:
>
>* Em Espera
>* Em Andamento
>* Completo
>* Parado
>

O Workfront usa as seguintes regras para calcular a Data de Transferência de uma tarefa:

* **Quando a tarefa tem um predecessor incompleto**: a Data de Transferência da tarefa é nula.
* **Quando a tarefa tiver uma predecessora concluída**: a Data de Transferência é igual à Data de Conclusão Efetiva da tarefa predecessora. Se o predecessor tiver um atraso, o Workfront calculará a Data de Transferência da tarefa sucessora usando a seguinte fórmula:

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  Para obter informações sobre o tempo de atraso, consulte [Visão Geral dos Tipos de Atraso](../use-prdcssrs/lag-types.md).

  Se a tarefa sucessora tiver mais de um predecessor, a Data de Transferência será calculada com base na Data de Conclusão Efetiva mais recente dos predecessores. Por exemplo, se as Datas de conclusão real dos dois predecessores forem 8 de novembro de 2022 e 20 de novembro de 2022, a Data de transferência do sucessor será 20 de novembro de 2022.

  >[!NOTE]
  >
  >   Calcular a Data de Transferência de uma tarefa sucessora com base na Data de Conclusão Efetiva ou em uma tarefa predecessora é a mesma independentemente de a predecessora ser imposta ou não. Para obter mais informações sobre predecessores impostos, consulte [Impor predecessores](../use-prdcssrs/enforced-predecessors.md).


* **Quando a tarefa não tem predecessor e**:

   * **A Data de Início Planejada está no passado**: a Data de Transferência é a mesma que a Data de Início Planejada do projeto se a tarefa não tiver nenhuma restrição forçada definida. Para os casos em que as tarefas têm restrições forçadas, consulte a seção &quot;Quando a tarefa tem uma restrição forçada para as Datas Planejadas&quot; abaixo.
   * **A Data de Início Planejada está no futuro (qualquer data posterior à data atual)**: a Data de Transferência é a mesma que a Data de Início Planejada da tarefa se a tarefa não tiver nenhuma restrição forçada definida. Para os casos em que as tarefas têm restrições forçadas, consulte a seção &quot;Quando a tarefa tem uma restrição forçada para as Datas Planejadas&quot; abaixo.

>[!NOTE]
>
>Quando a tarefa tem uma predecessora entre projetos, a data de transferência da sucessora é recalculada somente quando uma das situações a seguir ocorrer:
>
>* Você recalcula manualmente a linha do tempo do projeto do sucessor. Você deve ter permissões de Gerenciamento para que o projeto recalcule a linha do tempo.
>* A linha do tempo do projeto do sucessor é recalculada automaticamente à noite.
>
>Para obter informações sobre como recalcular a linha de tempo do projeto, consulte [Recalcular linhas de tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Quando a tarefa tem uma restrição forçada para as Datas Planejadas**: a Data de Transferência varia dependendo do tipo de restrição e se a tarefa tem ou não uma Data de Início Efetiva.\
  Veja a seguir restrições forçadas sobre tarefas:

   * Precisa Iniciar Em
   * Precisa Terminar Em
   * Não Iniciar Antes De
   * Não Iniciar Depois De
   * Data fixa

  Existem os seguintes cenários:

   * **Quando a tarefa tiver uma restrição de Deve Iniciar em ou Não Iniciar Antes de**: Se a data de restrição da tarefa estiver no passado e não houver uma Data de Início Efetivo na tarefa (a tarefa ainda não começou), a Data de Transferência será a data mais próxima possível na qual a tarefa poderá ser iniciada. Se a tarefa tiver sido iniciada, a Data de Transferência será igual à data de início do projeto.
   * **Quando a tarefa tiver uma restrição de Deve Terminar em ou Iniciar Não Posterior a**: Se a data de restrição da tarefa estiver no futuro e não houver uma Data de Início Efetiva na tarefa (a tarefa ainda não começou), a Data de Transferência será a Data de Início Planejada da tarefa. Se houver uma Data de Início Real na tarefa, a Data de Transferência será a data de início do projeto.
   * **Quando a tarefa tem uma restrição de Datas Fixas**: a Data de Transferência é a Data Inicial Planejada da tarefa, independentemente de ter ou não uma predecessora e de a predecessora estar concluída ou não.

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## Localize a data de transferência

Você pode exibir a Data de Transferência de uma tarefa em um relatório de tarefa ou na exibição de uma lista de tarefas.\
Para obter mais informações sobre a criação de um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
