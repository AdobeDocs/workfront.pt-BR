---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gerenciar horas de alocação de usuários e funções em tarefas
description: Ao atribuir usuários ou funções a uma tarefa, eles são alocados para trabalhar um determinado número de horas para concluir a tarefa. Você pode modificar manualmente a quantidade de horas que cada usuário ou função de trabalho é alocada quando é atribuída a uma tarefa, quando o Tipo de Duração da tarefa é Simples.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Gerenciar horas de alocação de usuários e funções em tarefas

<span class="preview">As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes ou no ambiente Produção para clientes que ativaram versões rápidas.</span>

<span class="preview">Para obter informações sobre lançamentos rápidos, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obter informações sobre a versão atual, consulte [Visão geral da versão do terceiro trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Ao atribuir usuários ou funções a uma tarefa, eles são alocados para trabalhar um determinado número de horas para concluir a tarefa. Você pode modificar manualmente a quantidade de horas que cada usuário ou função de trabalho é alocada quando é atribuída a uma tarefa, quando o Tipo de Duração da tarefa é Simples.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalhar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com ou mais permissões para a tarefa</p> <p>Editar permissões para atualizar horas de alocação na caixa Editar tarefa</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Considerações para modificar as horas de alocação de uma tarefa

>[!IMPORTANT]
>
>Depois de modificar manualmente as alocações para cada atribuição nas tarefas, as Horas Planejadas das tarefas podem ser atualizadas de acordo. Para obter mais informações, consulte a seção [Atualizar Trabalho de Horas Planejadas da tarefa ao gerenciar alocações de usuários](../../../manage-work/tasks/task-information/planned-hours.md#update) no artigo [Visão geral das Horas planejadas](../../../manage-work/tasks/task-information/planned-hours.md).

* O total de horas alocadas a recursos individuais atribuídos à tarefa representa as Horas Planejadas da tarefa.
* Se houver uma atribuição de usuário ou função para uma tarefa, a quantidade de horas alocadas para o usuário ou função corresponderá às Horas planejadas da tarefa.
* No caso de várias atribuições, cada usuário ou função de trabalho recebe uma quantidade igual de horas para trabalhar na tarefa, por padrão, se o Tipo de duração da tarefa for Simples. Para obter mais informações, consulte os seguintes artigos:

   * [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Visão geral do tipo de duração: simples](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Quando a tarefa tem um Tipo de Duração Simples, você pode alterar manualmente a quantidade de horas alocadas para cada usuário ou função de trabalho para indicar que alguns dos atribuídos da tarefa podem ter mais tempo para trabalhar em uma tarefa do que outros.
* Não é possível modificar a quantidade de horas alocadas para as equipes atribuídas a tarefas.
* Não é possível modificar manualmente a alocação de usuários ou funções de trabalho para ocorrências.
* Você também pode gerenciar alocações diárias, semanais ou mensais de usuários para tarefas ou problemas usando o Balanceador de carga de trabalho. Para obter mais informações, consulte [Gerenciar alocações de usuário no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modificar as horas de alocação de usuário ou função para uma tarefa

1. Vá para uma tarefa cujas atribuições você deseja alterar as horas de alocação.
1. Clique em **Mais** menu ![](assets/qs-more-icon-on-an-object.png) ao lado do nome da tarefa e clique em **Editar**, depois **Atribuições**.

   Ou

   Clique em **Atribuições** no cabeçalho da tarefa e clique em **Avançado**.

1. Certifique-se de que o **Tipo de Duração** da tarefa é **Simples**.
1. Modifique o **Alocações** para cada destinatário de tarefa. São alocações gerais para cada atribuição a esta tarefa, para toda a duração da tarefa. Isso também pode atualizar o total de Horas planejadas da tarefa.

   Imagem de amostra no ambiente de produção:
   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

   <span class="preview">Imagem de exemplo no ambiente de Pré-visualização:</span>
   ![Modificar alocações](assets/advanced-assignments-duration-type-allocations.png)

1. Clique em **Salvar**.
