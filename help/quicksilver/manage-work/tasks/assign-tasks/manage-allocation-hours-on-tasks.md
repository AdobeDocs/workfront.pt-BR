---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gerenciar horas de alocação de usuários e funções em tarefas
description: Ao atribuir usuários ou funções a uma tarefa, eles são alocados para trabalhar um determinado número de horas para concluir a tarefa. Você pode modificar manualmente a quantidade de horas que cada usuário ou função de trabalho é alocada quando é atribuída a uma tarefa, quando o Tipo de duração da tarefa é Simples.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Gerenciar horas de alocação de usuários e funções em tarefas

Ao atribuir usuários ou funções a uma tarefa, eles são alocados para trabalhar um determinado número de horas para concluir a tarefa. Você pode modificar manualmente a quantidade de horas que cada usuário ou função de trabalho é alocada quando é atribuída a uma tarefa, quando o Tipo de duração da tarefa é Simples.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso às tarefas</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir ou aumentar permissões para a tarefa</p> <p>Editar permissões para atualizar horas de alocação na caixa Editar tarefa</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações para modificar as horas de alocação de uma tarefa

>[!IMPORTANT]
>
>Após modificar manualmente as alocações de cada atribuição em tarefas, as Horas Planejadas das tarefas podem ser atualizadas adequadamente. Para obter mais informações, consulte a seção [Atualizar a tarefa Horas Planejadas ao gerenciar alocações de usuários](../../../manage-work/tasks/task-information/planned-hours.md#update) no artigo [Visão geral das Horas Planejadas](../../../manage-work/tasks/task-information/planned-hours.md).

* O total de horas alocadas para recursos individuais atribuídos à tarefa representa as Horas Planejadas da tarefa.
* Se houver uma atribuição de usuário ou função a uma tarefa, a quantidade de horas alocadas ao usuário ou função corresponderá às Horas Planejadas da tarefa.
* No caso de várias atribuições, cada usuário ou função de trabalho recebe uma quantidade igual de horas para trabalhar na tarefa, por padrão, se o Tipo de duração da tarefa for Simples. Para obter mais informações, consulte os seguintes artigos:

   * [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Visão geral do Tipo de duração: Simples](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Quando a tarefa tem um Tipo de Duração Simples, é possível alterar manualmente a quantidade de horas alocadas para cada usuário ou função de trabalho para indicar que alguns dos destinatários da tarefa podem ter mais tempo para trabalhar em uma tarefa do que outros.
* Não é possível modificar a quantidade de horas alocadas para equipes atribuídas a tarefas.
* Não é possível modificar manualmente a alocação de usuário ou função de trabalho para problemas.
* Você também pode gerenciar alocações diárias, semanais ou mensais de usuários para tarefas ou problemas usando o Balanceador de Carga de Trabalho. Para obter mais informações, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modificar as horas de alocação de usuário ou função para uma tarefa

1. Vá para uma tarefa cujas atribuições deseja alterar as horas de alocação.
1. Clique no botão **Mais** menu ![](assets/qs-more-icon-on-an-object.png) ao lado do nome da tarefa, em seguida, clique em **Editar**, em seguida **Atribuições**.

   Ou

   Clique no botão **Atribuições** no cabeçalho da tarefa e clique em **Avançado**.

1. Certifique-se de que **Tipo de duração** da tarefa **Simples**.
1. Modifique o **Alocações** para cada destinatário da tarefa. Essas são alocações gerais para cada atribuição para essa tarefa, por toda a duração da tarefa. Isso também pode atualizar as Horas Planejadas gerais da tarefa.

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Clique em **Salvar**.
