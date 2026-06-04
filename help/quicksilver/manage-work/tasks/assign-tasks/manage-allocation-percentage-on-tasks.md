---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gerenciar porcentagem de alocação de usuários ou funções em tarefas
description: A porcentagem de alocação representa a quantidade de tempo que um recurso atribuído deve trabalhar em uma tarefa em um dia. É a porcentagem de um dia útil (de acordo com o agendamento do usuário ou projeto) em que um recurso é alocado durante toda a duração da tarefa.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/tpBEkOgTsJSJ-dk-gKZ6uLyCk4j4vP4nMIQ5-ciHMAI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 444
ht-degree: 11%

---

# Gerenciar porcentagem de alocação de usuários ou funções em tarefas

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->


A porcentagem de alocação representa a quantidade de tempo que um recurso atribuído deve trabalhar em uma tarefa em um dia. É a porcentagem de um dia útil (de acordo com o agendamento do usuário ou projeto) em que um recurso é alocado durante toda a duração da tarefa.

Você pode modificar a porcentagem de alocação quando faz atribuições avançadas em uma tarefa.

>[!NOTE]
>
>Ao atribuir usuários para trabalhar, sua disponibilidade de acordo com seus agendamentos afeta as Datas Planejadas e Projetadas de tarefas e problemas. Para obter informações sobre agendamentos, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <td> <p>Padrão</p>
   <p>Trabalho ou maior</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Editar acesso a tarefas</td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td>
   <td><p>Contribuir com ou mais permissões para a tarefa</p>
   <p>Edite permissões para atualizar a porcentagem de alocação na caixa Editar tarefa.</p>
   <!--
   Not true anymore: 
   <p><b>NOTE</b></p>
   <p> You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a>.</p>
   -->
   </td>
  </tr>
 </tbody>
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   Você pode ver uma dessas telas, dependendo do Workfront ou do pacote de fluxo de trabalho da sua organização.

   ![Modificar porcentagem de alocação](assets/advanced-assignments-allocation-percentage.png)

   ![Modificar porcentagem de alocação](assets/new-aa-allocation-by-percentage.png)

1. Clique em **Salvar**.
