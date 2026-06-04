---
content-type: overview
product-area: projects
keywords: recorrente,recorrente,recorrente
navigation-topic: manage-tasks
title: Visão geral de tarefas recorrentes
description: Visão geral de tarefas recorrentes
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
TQID: https://experienceleague.adobe.com/O5PP-k5GFVPeJoKRHiJbOv1r-05X7sAnmAR4wBLmijk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 679
ht-degree: 4%

---

# Visão geral de tarefas recorrentes

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

Você pode criar tarefas recorrentes para atividades que você precisa repetir como parte de um único projeto.

Este artigo descreve informações e considerações sobre como criar e editar tarefas recorrentes.

Para obter informações sobre como criar tarefas recorrentes no Adobe Workfront, consulte [Criar tarefas recorrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Visão geral e considerações sobre tarefas recorrentes

Você pode optar por criar tarefas recorrentes para indicar trabalho repetível durante a vida útil de um projeto.

Por exemplo, durante um projeto de TI, é provável que seja necessário fazer backup do software em intervalos regulares. A criação de uma tarefa recorrente para essa atividade reduz o tempo necessário para configurar várias tarefas individuais.

Considere o seguinte ao criar tarefas recorrentes no Workfront:

* Não é possível adicionar tarefas recorrentes a um modelo.
* Não é possível adicionar uma frequência de recorrência a uma tarefa existente.
* As tarefas recorrentes aparecem como subtarefas ou filhos para a ocorrência principal que aparece como a tarefa pai.
* Não é possível anexar uma aprovação a uma tarefa pai recorrente.
* O Workfront transfere a maioria dos campos que você atualiza para a recorrência pai ao criá-la para as tarefas filho. Os seguintes campos não são transferidos para tarefas filhas quando são criados:

   * A Restrição de Tarefa das tarefas filhas altera automaticamente para:

      * Deve iniciar em para projetos planejados a partir da data de início.
      * Deve ser concluída em para projetos planejados a partir da data de conclusão.

   * Os documentos anexados ao pai não são transferidos aos filhos.

* As seguintes alterações ocorrem na tarefa pai depois que você indica que a tarefa é recorrente:

   * O campo Duração é renomeado para Duração por Ocorrência para a tarefa pai. Ela permanece como Duração para as tarefas secundárias.
   * O status é desabilitado na tarefa pai e é automaticamente definido como Novo nos filhos. A tarefa pai é concluída automaticamente e o status é atualizado para Concluído quando todos os filhos forem concluídos.
   * Os únicos Tipos de duração disponíveis para tarefas recorrentes são:

      * Simples
      * Controlado pelo empenho
* A Duração e as Horas planejadas indicadas para uma nova tarefa recorrente são a Duração e as Horas planejadas de cada ocorrência. A Duração da tarefa pai é o tempo entre a Data de Início Planejada da tarefa mais antiga e a Data de Conclusão Planejada da tarefa mais recente. As Horas Planejadas da tarefa pai é o total de todas as Horas Planejadas de todas as ocorrências.

## Considerações para edição de tarefas recorrentes

Algumas alterações feitas em uma tarefa pai recorrente podem não ser atualizadas em todas as ocorrências existentes. As tarefas filho que mostrarem progresso ou tiverem sido atualizadas individualmente não serão atualizadas quando você atualizar o pai. A Workfront considera que uma tarefa mostra o progresso nas seguintes situações:

* O status é atualizado e a tarefa não é mais Nova
* A Porcentagem Concluída da tarefa é maior que zero
* A tarefa tem relações de predecessoras

A tabela a seguir ilustra se as alterações feitas nas atualizações do acionador principal nas páginas secundárias que não foram editadas individualmente ou mostram progresso:

| Campos atualizados na tarefa pai | Transferência de atualizações para filhos não editados ou filhos sem progresso registrado |
|---|---|
| Frequência de recorrência* | ✔ |
| Atribuições | ✔ |
| Nome | ✔ |
| Descrição | ✔ |
| Prioridade | ✔ |
| Duração | ✔ |
| Horas planejadas | ✔ |
| Tipo de Custo | ✔ |
| Tipo de Receita | ✔ |
| Nivelamento de recurso | ✔ |
| Atraso de Nivelamento | ✔ |
| Restrição de Tarefa | Não atualiza os filhos |
| Anexar ou remover o Forms personalizado | Não atualiza os filhos |
| Tipo de Duração | Não atualiza os filhos |
| Informações do formulário personalizado | Não atualiza os filhos |

{style="table-layout:auto"}

&#42; Os cenários a seguir existem quando você atualiza a Frequência de Recorrência de uma tarefa pai:

* Se você alterar a Frequência de Recorrência em uma tarefa pai existente, as subtarefas existentes serão excluídas e substituídas por novas subtarefas que seguem a nova frequência de recorrência se elas não mostrarem nenhum progresso e se você não as tiver atualizado manualmente.
* Se você alterar a Frequência de Recorrência em uma tarefa pai existente, as subtarefas que mostram progresso não serão excluídas. Essas tarefas são consideradas separadas da recorrência neste ponto.

&#42;&#42; Atribuições feitas na tarefa pai são aplicadas a todas as subtarefas na recorrência. Quaisquer alterações feitas na atribuição da tarefa-pai substituem quaisquer atribuições individuais na subtarefa. Se a tarefa mostrar andamento, a atribuição não será alterada.


