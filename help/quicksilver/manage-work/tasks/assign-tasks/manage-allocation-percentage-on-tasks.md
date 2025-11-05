---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gerenciar porcentagem de alocação de usuários ou funções em tarefas
description: A porcentagem de alocação representa a quantidade de tempo que um recurso atribuído deve trabalhar em uma tarefa em um dia. É a porcentagem de um dia útil (de acordo com o agendamento do usuário ou projeto) em que um recurso é alocado durante toda a duração da tarefa.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 1%

---

# Gerenciar porcentagem de alocação de usuários ou funções em tarefas

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

A porcentagem de alocação representa a quantidade de tempo que um recurso atribuído deve trabalhar em uma tarefa em um dia. É a porcentagem de um dia útil (de acordo com o agendamento do usuário ou projeto) em que um recurso é alocado durante toda a duração da tarefa.

>[!NOTE]
>
>Ao atribuir usuários para trabalhar, sua disponibilidade de acordo com seus agendamentos afeta as Datas Planejadas e Projetadas de tarefas e problemas. Para obter informações sobre agendamentos, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Trabalhar ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Editar acesso a tarefas</td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td>
   <td><p>Contribuir com ou mais permissões para a tarefa</p>
   <p>Editar permissões para atualizar a porcentagem de alocação na caixa Editar tarefa</p></td>
  </tr>
 </tbody>
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Change this sentence in the table when unshimmming assignments on Edit task:
<p>Edit permissions to update allocation percentage in the Edit Task box</p>
To this:
<p>Edit permissions to update allocation percentage in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.
-->

## Considerações sobre a modificação de alocações de percentual para tarefas

* Os usuários recebem uma porcentagem igual de tempo das tarefas às quais estão atribuídos, por padrão.
* Você pode modificar manualmente a porcentagem de alocação para usuários e funções de cargo atribuídos a tarefas somente quando o Tipo de Duração da tarefa for Trabalho Calculado ou Orientado pelo Esforço.

  Para obter informações, consulte [Visão geral da duração e do tipo de duração da tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Não é possível modificar a alocação percentual das equipes atribuídas a tarefas.
* Não é possível modificar a alocação de porcentagem para usuários e funções de trabalho atribuídos a problemas.

## Modificar a alocação percentual de usuário ou função para uma tarefa

1. Vá para uma tarefa cujos recursos você está alterando a alocação percentual.
1. Clique no menu **Mais** ![](assets/qs-more-icon-on-an-object.png) ao lado do nome da tarefa e clique em **Editar**.

   Ou

   Clique na área **Atribuições** no cabeçalho da tarefa e clique em **Avançadas**.

1. Verifique se o **Tipo de Duração** da tarefa é um dos seguintes:

   * Trabalho Calculado
   * Controlado pelo empenho

   >[!TIP]
   >
   >* Para o Tipo de Duração da Atribuição Calculada, o Workfront usa a seguinte fórmula para calcular a porcentagem de alocação de cada destinatário: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Para o Tipo de Duração Simples, é possível estimar as horas atribuídas a cada recurso, não a porcentagem de alocação.

1. Clique em **Atribuições** e modifique as **Alocações** para cada destinatário de tarefa.

   Você só pode modificar a porcentagem de alocação para atribuições de usuário e funções de trabalho.

   Não é possível modificar a porcentagem de alocação de uma equipe atribuída a uma tarefa.

   ![Modificar porcentagem de alocação](assets/advanced-assignments-allocation-percentage.png)

1. Clique em **Salvar**.
