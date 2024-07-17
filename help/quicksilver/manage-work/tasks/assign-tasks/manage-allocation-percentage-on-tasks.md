---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gerenciar porcentagem de alocação de usuários ou funções em tarefas
description: A porcentagem de alocação representa a quantidade de tempo que um recurso atribuído deve trabalhar em uma tarefa em um dia. É a porcentagem de um dia útil (de acordo com o agendamento do usuário ou projeto) em que um recurso é alocado durante toda a duração da tarefa.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 1%

---

# Gerenciar porcentagem de alocação de usuários ou funções em tarefas

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização para todos os clientes ou no ambiente de Produção para clientes que habilitaram versões rápidas.</span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obter informações sobre a versão atual, consulte a [Visão geral da versão do Terceiro Trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

A porcentagem de alocação representa a quantidade de tempo que um recurso atribuído deve trabalhar em uma tarefa em um dia. É a porcentagem de um dia útil (de acordo com o agendamento do usuário ou projeto) em que um recurso é alocado durante toda a duração da tarefa.

>[!NOTE]
>
>Ao atribuir usuários para trabalhar, sua disponibilidade de acordo com seus agendamentos afeta as Datas Planejadas e Projetadas de tarefas e problemas. Para obter informações sobre agendamentos, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

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
   <td> <p>Contribute ou permissões mais altas para a tarefa</p> <p>Editar permissões para atualizar a porcentagem de alocação na caixa Editar tarefa</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

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

   Imagem de amostra no ambiente de produção:
   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

   <span class="preview">Imagem de exemplo no ambiente de Visualização:</span>
   ![Modificar porcentagem de alocação](assets/advanced-assignments-allocation-percentage.png)

1. Clique em **Salvar**.
