---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral da data de transferência da tarefa
description: A Data de Transferência é a data em que uma tarefa se torna disponível para trabalho. Normalmente, isso significa que suas predecessoras foram resolvidas e o destinatário da tarefa pode começar a trabalhar nela.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 709b36f4471e5576e45ed918783216a1f7f4abac
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 3%

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
* **Quando a tarefa tiver um predecessor completo**: A Data de Transferência é a mesma que a Data de Conclusão Efetiva da tarefa predecessora. Se o predecessor tiver um atraso, o Workfront calculará a Data de Transferência da tarefa sucessora usando a seguinte fórmula:

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  Para obter informações sobre o tempo de atraso, consulte [Visão Geral dos Tipos de Defasagem](../use-prdcssrs/lag-types.md).

  Se a tarefa sucessora tiver mais de um predecessor, a Data de Transferência será calculada com base na Data de Conclusão Efetiva mais recente dos predecessores. Por exemplo, se as Datas de conclusão real dos dois predecessores forem 8 de novembro de 2022 e 20 de novembro de 2022, a Data de transferência do sucessor será 20 de novembro de 2022.

  >[!NOTE]
  >
  >   Calcular a Data de Transferência de uma tarefa sucessora com base na Data de Conclusão Efetiva ou em uma tarefa predecessora é a mesma independentemente de a predecessora ser imposta ou não. Para obter mais informações sobre predecessores impostos, consulte [Forçar predecessores](../use-prdcssrs/enforced-predecessors.md).


* **Quando a tarefa não tiver predecessor e**:

   * **A data de início planejada está no passado**: a data de transferência é igual à data de início planejada do projeto.
   * **A Data de Início Planejada está no futuro (qualquer data posterior à data atual)**: A Data de Transferência é a mesma que a Data de Início Planejada da tarefa.

>[!NOTE]
>
>Quando a tarefa tem uma predecessora entre projetos, a data de transferência da sucessora é recalculada somente quando uma das situações a seguir ocorrer:
>
>* Você recalcula manualmente a linha do tempo do projeto do sucessor. Você deve ter permissões de Gerenciamento para que o projeto recalcule a linha do tempo.
>* A linha do tempo do projeto do sucessor é recalculada automaticamente à noite.
>
>Para obter informações sobre como recalcular a linha do tempo do projeto, consulte [Recalcular linhas do tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Quando a tarefa tem uma restrição forçada para as Datas Planejadas**: A Data de Transferência varia dependendo do tipo de restrição e se a tarefa tem ou não uma Data Inicial Real.\
  Veja a seguir restrições forçadas sobre tarefas:

   * Precisa Iniciar Em
   * Precisa Terminar Em
   * Não Iniciar Antes De
   * Não Iniciar Depois De
   * Data fixa

  Existem os seguintes cenários:

   * Quando a tarefa tem uma restrição de Deve Iniciar em ou Não Iniciar Antes de, a Data de Transferência é a Data de Restrição, a menos que haja uma Data de Início Real na tarefa. Se houver uma Data de Início Efetivo na tarefa, a Data de Transferência será a Data de Conclusão Efetiva do antecessor.
   * Quando a tarefa tiver uma restrição de Precisa Ser Concluída em ou Iniciar Não Depois de, a Data de Transferência sempre será a Data de Conclusão Efetiva do antecessor, independentemente de haver ou não uma Data de Início Efetiva na tarefa.
   * Quando a tarefa tem uma restrição de Datas Fixas, a Data de Transferência é a Data Inicial Planejada da tarefa, independentemente de ter ou não um predecessor e independentemente de o predecessor estar concluído ou não.

## Localize a data de transferência

Você pode exibir a Data de Transferência de uma tarefa em um relatório de tarefa ou na exibição de uma lista de tarefas.\
Para obter mais informações sobre criação de relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
