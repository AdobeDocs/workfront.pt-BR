---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral da Data de Entrega da Tarefa
description: A Data de Destino é a data em que uma tarefa fica disponível para trabalho. Isso normalmente significa que seus antecessores foram resolvidos e o responsável pela tarefa pode começar a trabalhar nela.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 161084a3b459d4a9598fa780132d420bf0890c71
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Visão geral da Data de Entrega da Tarefa

A Data de Destino é a data em que uma tarefa fica disponível para trabalho. Isso normalmente significa que seus antecessores foram resolvidos e o responsável pela tarefa pode começar a trabalhar nela.

>[!TIP]
>
>Datas de handoff não existem para problemas e projetos.

## Como o Adobe Workfront calcula a data de desistência

>[!NOTE]
>
>A Data de Apresentação é calculada somente se o status do projeto for igual aos seguintes status:
>
>* Em Espera
>* Em Andamento
>* Completo
>* Parado
>


O Workfront usa as seguintes regras para calcular a Data de handoff de uma tarefa:

* **Quando a tarefa tiver um antecessor incompleto**: A Data de Apresentação da tarefa é nula.
* **Quando a tarefa tiver um antecessor completo**: A Data de Apresentação é igual à Data de Conclusão Real da tarefa antecessora. Se o antecessor tiver um atraso, o Workfront calculará a Data de handoff da tarefa sucessora usando a seguinte fórmula:

   `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

   Para obter informações sobre o tempo de atraso, consulte [Visão geral dos tipos de atraso](../use-prdcssrs/lag-types.md).

   Se a tarefa sucessora tiver mais de um antecessor, a Data de Apresentação será calculada com base na Data de Conclusão Real mais recente dos antecessores. Por exemplo, se as Datas de conclusão reais dos dois antecessores forem 8 de novembro de 2022 e 20 de novembro de 2022, a Data de transferência do sucessor será 20 de novembro de 2022.

   >[!NOTE]
   >
   >   O cálculo da Data de Envio de uma tarefa sucessora com base na Data de Conclusão Real ou em uma tarefa antecessora é o mesmo se o antecessor é empregado ou não. Para obter mais informações sobre predecessores forçados, consulte [Impor predecessores](../use-prdcssrs/enforced-predecessors.md).


* **Quando a tarefa não tiver antecessor e**:

   * **A Data de início planejada está no passado**: A Data de Apresentação é igual à Data Inicial Planejada do projeto.
   * **A Data Inicial Planejada está no futuro (qualquer data após a data atual)**: A Data de Apresentação é igual à Data Inicial Planejada do projeto.

>[!NOTE]
>
>Quando a tarefa tem um antecessor entre projetos, a data de handoff do sucessor recalcula apenas quando uma das seguintes situações ocorrer:
>
>* Você recalcula manualmente a linha do tempo do projeto do sucessor. Você deve ter permissões de Gerenciar para o projeto para recalcular a linha do tempo.
>* A linha do tempo do projeto do sucessor é automaticamente recalculada à noite.
>
>Para obter informações sobre como recalcular a linha do tempo do projeto, consulte [Recalcular linhas do tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Quando a tarefa tem uma restrição forçada para as Datas Planejadas**: A Data de transferência varia dependendo do tipo de restrição e se a tarefa tem ou não uma Data de início real.\
   Os itens a seguir são restrições forçadas em tarefas:

   * Precisa Iniciar Em
   * Precisa Terminar Em
   * Não Iniciar Antes De
   * Não Iniciar Depois De
   * Data fixa

   Os seguintes cenários existem:

   * Quando a tarefa tem uma restrição de Deve Iniciar em ou Iniciar Não Antes de, a Data de Aprovação é a Data da Restrição, a menos que haja uma Data de Início Real na tarefa. Se houver uma Data de Início Real na tarefa, a Data de Entrega será a Data de Conclusão Real do antecessor.
   * Quando a tarefa tem uma restrição de Deve Concluir Em ou Iniciar Não Mais Tarde, a Data de Apresentação é sempre a Data de Conclusão Real do antecessor, independentemente de haver ou não uma Data de Início Real na tarefa.
   * Quando a tarefa tem uma restrição de Datas Fixas, a Data de Apresentação é a Data Inicial Planejada da tarefa, independentemente de ter ou não um antecessor e independentemente de o antecessor ser concluído ou não.


## Localize a data de transferência

Você pode exibir a Data de handoff de uma tarefa em um relatório de tarefa ou na exibição de uma lista de tarefas.\
Para obter mais informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
