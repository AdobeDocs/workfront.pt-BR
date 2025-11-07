---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gerenciar porcentagem de alocação de usuários ou funções em tarefas
description: A porcentagem de alocação representa a quantidade de tempo que um recurso atribuído deve trabalhar em uma tarefa em um dia. É a porcentagem de um dia útil (de acordo com o agendamento do usuário ou projeto) em que um recurso é alocado durante toda a duração da tarefa.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 1%

---

# Gerenciar porcentagem de alocação de usuários ou funções em tarefas

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<div class="preview">

As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Os mesmos recursos também estarão disponíveis no ambiente de Produção para todos os clientes, a partir de uma semana da versão de Pré-visualização.

Para obter mais informações, consulte [Modernização da interface](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>


A porcentagem de alocação representa a quantidade de tempo que um recurso atribuído deve trabalhar em uma tarefa em um dia. É a porcentagem de um dia útil (de acordo com o agendamento do usuário ou projeto) em que um recurso é alocado durante toda a duração da tarefa.

Você pode modificar a porcentagem de alocação quando faz atribuições avançadas em uma tarefa.

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
   <p>Edite permissões para atualizar a porcentagem de alocação na caixa Editar tarefa quando <span class="preview"> editar tarefas usando a experiência antiga. Não é mais possível gerenciar a porcentagem de alocação na caixa Editar tarefa ao editar tarefas na nova experiência.</span></p> <p>Para obter informações, consulte <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Editar tarefas</a>.</p></td>
  </tr>
 </tbody>
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

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
1. Clique na área **Atribuições** no cabeçalho da tarefa e clique em **Avançadas**.

1. Verifique se o **Tipo de Duração** da tarefa é um dos seguintes:

   * Trabalho Calculado
   * Controlado pelo empenho

   >[!TIP]
   >
   >* Para o Tipo de Duração da Atribuição Calculada, o Workfront usa a seguinte fórmula para calcular a porcentagem de alocação de cada destinatário: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Para o Tipo de Duração Simples, é possível estimar as horas atribuídas a cada recurso, não a porcentagem de alocação.

1. Modifique o campo **Alocações** para cada destinatário da tarefa.

   Você só pode modificar a porcentagem de alocação para atribuições de usuário e funções de trabalho.

   Não é possível modificar a porcentagem de alocação de uma equipe atribuída a uma tarefa.

   ![Modificar porcentagem de alocação](assets/advanced-assignments-allocation-percentage.png)

1. Clique em **Salvar**.
