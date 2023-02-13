---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gerenciar porcentagem de alocação de usuário ou função em tarefas
description: A porcentagem de alocação representa a quantidade de tempo em que um recurso atribuído está planejado para trabalhar em uma tarefa em um dia. É a porcentagem de um dia de trabalho (de acordo com o agendamento do usuário ou do projeto) em que um recurso é alocado durante toda a tarefa.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---

# Gerenciar porcentagem de alocação de usuário ou função em tarefas

A porcentagem de alocação representa a quantidade de tempo em que um recurso atribuído está planejado para trabalhar em uma tarefa em um dia. É a porcentagem de um dia de trabalho (de acordo com o agendamento do usuário ou do projeto) em que um recurso é alocado durante toda a tarefa.

>[!NOTE]
>
>Ao atribuir usuários ao trabalho, sua disponibilidade de acordo com suas programações afeta as Datas Planejadas e Projetadas das tarefas e problemas. Para obter informações sobre programações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

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
   <td> <p>Contribuir ou aumentar permissões para a tarefa</p> <p>Edite permissões para atualizar a porcentagem de alocação na caixa Editar tarefa</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações sobre a modificação de alocações de porcentagem para tarefas

* Por padrão, os usuários recebem uma porcentagem igual de tempo para tarefas às quais estão atribuídos.
* Você pode modificar manualmente a porcentagem de alocação para usuários e funções de job atribuídas a tarefas somente quando o Tipo de Duração da tarefa for Trabalho Calculado ou Orientado a Esforço.

   Para obter mais informações, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Não é possível modificar a alocação de porcentagem para equipes atribuídas a tarefas.
* Não é possível modificar a alocação de porcentagem para usuários e funções de tarefas atribuídas a problemas.

## Modificar a alocação de porcentagem de usuário ou função para uma tarefa

1. Vá para uma tarefa cujos recursos você está alterando a alocação de porcentagem.
1. Clique no botão **Mais** menu ![](assets/qs-more-icon-on-an-object.png) ao lado do nome da tarefa, em seguida, clique em **Editar**.

   Ou

   Clique no botão **Atribuições** no cabeçalho da tarefa e clique em **Avançado**.

1. Certifique-se de que **Tipo de duração** da tarefa é um dos seguintes:

   * Trabalho Calculado
   * Controlado pelo empenho

   >[!TIP]
   >
   >* Para o Tipo de Duração da Atribuição Calculada, o Workfront usa a seguinte fórmula para calcular a porcentagem de alocação de cada destinatário: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Para o Tipo de duração simples, você pode estimar as horas atribuídas a cada recurso, não a porcentagem de alocação.


1. Clique em **Atribuições** e modifique o **Alocações** para cada destinatário da tarefa.

   Você só pode modificar a porcentagem de alocação para atribuições de usuário e função de cargo.

   Não é possível modificar a porcentagem de alocação de uma equipe atribuída a uma tarefa.

   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. Clique em **Salvar**.
