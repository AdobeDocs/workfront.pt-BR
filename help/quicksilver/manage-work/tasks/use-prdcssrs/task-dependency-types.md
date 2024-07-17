---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Visão geral dos tipos de dependência de tarefa
description: Os Tipos de Dependências referem-se aos relacionamentos de predecessores entre tarefas. Eles definem quando a tarefa dependente pode iniciar ou terminar com base no início ou término de seu antecessor.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Visão geral dos tipos de dependência de tarefa

<!-- Audited: 12/2023 -->

Os Tipos de Dependências referem-se aos relacionamentos de predecessores entre tarefas. Eles definem quando a tarefa dependente pode iniciar ou terminar com base no início ou término de seu antecessor.

>[!IMPORTANT]
>
>O Adobe Workfront não restringe o início ou a conclusão das tarefas dependentes com base nos tipos de dependência, a menos que os relacionamentos predecessores sejam impostos. Para obter informações sobre como impor predecessores, consulte [Impor predecessores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Você deve especificar o Tipo de dependência de um relacionamento de predecessor ao estabelecer esse relacionamento entre suas tarefas.

Para obter mais informações sobre predecessores, consulte [Visão geral dos predecessores da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

A seguir estão os Tipos de Dependência da Workfront:

* **Término-Início (fs)**: a tarefa predecessora deve ser concluída antes que a tarefa dependente possa ser iniciada. Este é o tipo de dependência padrão, usado quando nenhum outro tipo de dependência é especificado.
* **Término-Término (ff)**: a tarefa predecessora deve terminar antes que a tarefa dependente possa terminar.
* **Início-Início (ss)**: a tarefa predecessora deve ser iniciada antes que a tarefa dependente possa ser iniciada. Não é possível iniciar a tarefa dependente, a menos que o predecessor tenha pelo menos iniciado.
* **Início-Término (sf)**: a tarefa predecessora deve iniciar antes que a tarefa dependente possa terminar. Você pode iniciar a tarefa dependente antes que a predecessora seja iniciada, mas não pode concluí-la até que a predecessora seja iniciada.
* **Início Agendado (sd)**: agenda uma tarefa como Término-Início, mas o tipo de imposição real é Término-Término. Quando você usa isso, a tarefa dependente é agendada para iniciar depois que a tarefa predecessora é concluída. No entanto, a imposição a torna a tarefa dependente pode iniciar a qualquer momento, mas não pode terminar até que a tarefa predecessora seja concluída.

>[!NOTE]
>
>As abreviações dos Tipos de Dependência são usadas em listas de tarefas para definir relações de predecessoras. Para obter mais informações, consulte [Exemplos de valores predecessores em uma lista de tarefas](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) em [Visão geral dos predecessores da tarefa](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

