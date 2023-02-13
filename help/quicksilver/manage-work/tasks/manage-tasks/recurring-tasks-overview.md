---
content-type: overview
product-area: projects
keywords: recorrente,reocorrência,reocorrendo
navigation-topic: manage-tasks
title: Visão geral das tarefas recorrentes
description: Visão geral das tarefas recorrentes
author: Alina
feature: Work Management
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 3%

---

# Visão geral das tarefas recorrentes

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

Você pode criar tarefas recorrentes para atividades que devem ser repetidas como parte de um único projeto.

Este artigo descreve informações e considerações sobre a criação e edição de tarefas recorrentes.

Para obter informações sobre como criar tarefas recorrentes no Adobe Workfront, consulte [Criar tarefas recorrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Visão geral e considerações das Tarefas recorrentes

Você pode optar por criar tarefas recorrentes para indicar trabalhos repetíveis durante a vida de um projeto.

Por exemplo, durante um projeto de TI, é provável que seja necessário fazer backup do software em intervalos regulares. Criar uma tarefa recorrente para essa atividade reduz o tempo necessário para configurar várias tarefas individuais.

Considere o seguinte ao criar tarefas recorrentes no Workfront:

* Não é possível adicionar tarefas recorrentes a um template.
* Não é possível adicionar uma frequência de recorrência a uma tarefa existente.
* As tarefas recorrentes aparecem como subtarefas ou filhos para a ocorrência principal que aparece como a tarefa pai.
* Não é possível anexar uma aprovação a uma tarefa recorrente pai.
* O Workfront transfere a maioria dos campos que você atualiza para a recorrência pai ao criá-la para as tarefas filho. Os seguintes campos não são transferidos para as tarefas filho quando são criados:

   * A Restrição de Tarefa das tarefas filho muda automaticamente para:

      * Deve iniciar em projetos planejados a partir da data inicial.
      * Deve ser concluído para projetos planejados a partir da data de conclusão.
   * Os documentos anexados à empresa-mãe não são transferidos para os filhos.


* As seguintes alterações ocorrem na tarefa pai após indicar que a tarefa é recorrente:

   * O campo Duration é renomeado para Duration per Occurrence para a tarefa pai. Permanece Duração para as tarefas filho.
   * O status é desativado na tarefa pai e é automaticamente definido como Novo nos filhos. A tarefa pai é concluída automaticamente e o status é atualizado para Concluído quando todos os filhos são concluídos.
   * Os únicos Tipos de duração disponíveis para tarefas recorrentes são:

      * Simples
      * Controlado pelo empenho

## Considerações para editar tarefas recorrentes

Algumas alterações feitas em um pai de tarefa recorrente podem não ser atualizadas em todas as recorrentes existentes. As tarefas filho que mostram o progresso ou foram atualizadas individualmente não serão atualizadas quando você atualizar o pai. A Workfront considera que uma tarefa mostra o progresso nas seguintes situações:

* O status é atualizado e a tarefa não é mais Nova
* A porcentagem concluída da tarefa é maior que zero
* A tarefa tem relações predecessoras

A tabela a seguir ilustra se as alterações feitas no acionador principal são atualizadas nos filhos que não foram editados individualmente ou mostram o progresso:

| Campos atualizados na tarefa pai | Atualizações transferidas para filhos ou filhos não editados sem progresso registrado |
|---|---|
| Frequência de recorrência* | ✔ |
| Atribuições&#42;&#42; | ✔ |
| Nome | ✔ |
| Descrição | ✔ |
| Prioridade | ✔ |
| Duração | ✔ |
| Horas planejadas | ✔ |
| Tipo de Custo | ✔ |
| Tipo de receita | ✔ |
| Nivelamento de recurso | ✔ |
| Atraso de Nivelamento | ✔ |
| Restrição de tarefa | Não atualiza os filhos |
| Anexar ou remover o Forms personalizado | Não atualiza os filhos |
| Tipo de duração | Não atualiza os filhos |
| Informações do formulário personalizado | Não atualiza os filhos |

{style=&quot;table-layout:auto&quot;}

&#42; Os seguintes cenários existem quando você atualiza a Frequência de Recorrência de uma tarefa pai:

* Se você alterar a Frequência de Periodicidade em uma tarefa pai existente, as subtarefas existentes serão excluídas e substituídas por novas subtarefas que seguem a nova frequência de recorrência se elas não mostrarem nenhum progresso e se você não as tiver atualizado manualmente.
* Se você alterar a Frequência de Recorrência em uma tarefa pai existente, as subtarefas que mostram o progresso não serão excluídas. Essas tarefas são consideradas separadas da recorrência neste momento.

&#42;&#42; As atribuições feitas na tarefa pai são aplicadas a todas as subtarefas na recorrência. Quaisquer alterações feitas na atribuição na tarefa pai substituem quaisquer atribuições individuais na subtarefa. Se a tarefa mostrar o progresso, a atribuição não será alterada.

 
