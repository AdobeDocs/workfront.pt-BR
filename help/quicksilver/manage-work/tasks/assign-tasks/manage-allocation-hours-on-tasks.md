---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gerenciar horas de alocação de usuários e funções em tarefas
description: Ao atribuir usuários ou funções a uma tarefa, eles são alocados para trabalhar um determinado número de horas para concluir a tarefa. Você pode modificar manualmente a quantidade de horas que cada usuário ou função de trabalho é alocada quando é atribuída a uma tarefa, quando o Tipo de Duração da tarefa é Simples.
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 259fd0e3fdaa07bfdb0301d60bf0d9b1090b4ef7
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Gerenciar horas de alocação de usuários e funções em tarefas

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Novo: Padrão </p>
   <p>Atual: trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribute ou permissões mais altas para a tarefa</p> <p>Editar permissões para atualizar horas de alocação na caixa Editar tarefa</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações para modificar as horas de alocação de uma tarefa

>[!IMPORTANT]
>
>Depois de modificar manualmente as alocações para cada atribuição nas tarefas, as Horas Planejadas das tarefas podem ser atualizadas de acordo. Para obter mais informações, consulte a seção [Atualizar horas planejadas da tarefa ao gerenciar alocações de usuário](../../../manage-work/tasks/task-information/planned-hours.md#update) no artigo [visão geral das horas planejadas](../../../manage-work/tasks/task-information/planned-hours.md).

* O total de horas alocadas a recursos individuais atribuídos à tarefa representa as Horas Planejadas da tarefa.
* Se houver uma atribuição de usuário ou função para uma tarefa, a quantidade de horas alocadas para o usuário ou função corresponderá às Horas planejadas da tarefa.
* No caso de várias atribuições, cada usuário ou função de trabalho recebe uma quantidade igual de horas para trabalhar na tarefa, por padrão, se o Tipo de duração da tarefa for Simples. Para obter mais informações, consulte os seguintes artigos:

   * [Visão Geral da Duração e do Tipo de Duração da Tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Visão geral do tipo de duração: simples](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Quando a tarefa tem um Tipo de Duração Simples, você pode alterar manualmente a quantidade de horas alocadas para cada usuário ou função de trabalho para indicar que alguns dos atribuídos da tarefa podem ter mais tempo para trabalhar em uma tarefa do que outros.
* Não é possível modificar a quantidade de horas alocadas para as equipes atribuídas a tarefas.
* Não é possível modificar manualmente a alocação de usuários ou funções de trabalho para ocorrências.
* Você também pode gerenciar alocações diárias, semanais ou mensais de usuários para tarefas ou problemas usando o Balanceador de carga de trabalho. Para obter mais informações, consulte [Gerenciar alocações de usuário no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modificar as horas de alocação de usuário ou função para uma tarefa

1. Vá para uma tarefa cujas atribuições você deseja alterar as horas de alocação.
1. Clique no menu **Mais** ![](assets/qs-more-icon-on-an-object.png) ao lado do nome da tarefa e clique em **Editar** e depois em **Atribuições**.

   Ou

   Clique na área **Atribuições** no cabeçalho da tarefa e clique em **Avançadas**.

1. Verifique se o **Tipo de Duração** da tarefa é **Simples**.
1. Modifique as **Alocações** para cada destinatário de tarefa. São alocações gerais para cada atribuição a esta tarefa, para toda a duração da tarefa. Isso também pode atualizar o total de Horas planejadas da tarefa.

   ![Modificar alocações](assets/advanced-assignments-duration-type-allocations.png)

1. Clique em **Salvar**.
