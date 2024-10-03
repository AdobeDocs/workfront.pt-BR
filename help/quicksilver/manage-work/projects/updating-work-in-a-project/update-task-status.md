---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar Status da Tarefa
description: Você pode atualizar o status de uma tarefa para informar a outras pessoas sobre onde a tarefa está (e o projeto geral) e como está progredindo.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 1%

---

# Atualizar status da tarefa

<!--Audited: 10/2024-->

Você pode atualizar o status de uma tarefa para informar a outras pessoas sobre onde a tarefa está (e o projeto geral) e como está progredindo.

Os status padrão são Novo, Em andamento e Concluído. O administrador do Adobe Workfront pode adicionar status personalizados para sua organização. Para obter mais informações, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Você pode atualizar manualmente os status das tarefas ou permitir que o Workfront os atualize automaticamente quando determinadas ações ocorrerem.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para atualizar tarefas manualmente:

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
   <td> <p>Novo: Padrão</p> 
   Ou
   <p>Atual: trabalho ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para a tarefa</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre a atualização do Status das tarefas

* Quando você marca uma tarefa como Concluída, o percentual concluído da tarefa é atualizado para 100%.
* Existem os seguintes cenários para tarefas pai:
   * Você não pode atualizar o Status de uma tarefa pai para Concluído quando o Modo de Conclusão em Resumo do projeto estiver definido como Automático e as subtarefas não estiverem concluídas.
   * Você pode atualizar o Status de uma tarefa-pai para Concluído quando o Modo de Conclusão em Resumo do projeto estiver definido como Manual e as subtarefas estiverem concluídas ou incompletas.

  Para obter mais informações, consulte [Editar projetos](../manage-projects/edit-projects.md).

## Atualizar manualmente o status da tarefa

Você pode atualizar o status da tarefa nas seguintes áreas do Workfront:

* O cabeçalho da tarefa na página da tarefa.
* A caixa Editar tarefa, ao editar uma tarefa.
* A seção Detalhes da Tarefa na página da tarefa.
* Em uma lista de tarefas ou relatório, quando o campo Status estiver visível na exibição.
* No painel Resumo da tarefa.

Para atualizar manualmente o status da tarefa no cabeçalho da tarefa:

1. Vá para uma tarefa para a qual deseja atualizar o status.
1. Clique no campo **Status** no cabeçalho da tarefa e selecione um novo status.
1. Para fornecer uma indicação visual da conclusão da tarefa, arraste ou clique duas vezes na bolha em **Percentual concluído** no cabeçalho da tarefa

   Ou

   Clique dentro da bolha no cabeçalho da tarefa para inserir uma porcentagem.

   ![](assets/percent-complete-status-widgets-task-header.png)

1. (Opcional) Siga qualquer um destes procedimentos para fornecer informações adicionais sobre a atualização:

   * Para adicionar uma observação sobre a atualização, vá para a seção **Atualizações**, clique em **Novo comentário** e digite uma observação.

     ![](assets/add-update-to-task.png)

   * Para notificar determinados usuários sobre a atualização, digite seus nomes no campo **Marcar pessoas ou equipes**, que aparece quando você digita um comentário. Para obter mais informações, consulte [Marcar outros em atualizações](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Para atualizar a Data de confirmação da tarefa, clique em **Detalhes da tarefa** e edite o campo **Data de confirmação**. Para obter informações, consulte [Editar tarefas](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).


   >[!IMPORTANT]
   >
   >  Somente os atribuídos da tarefa podem atualizar a Data de confirmação.

<!--old functionality in old commenting: 

1. Go to a task that you are assigned to for which you want to update the status.
1. Click the **Status** field in the task header and select a new status. 
1. (Optional) Do any of the following to provide additional information about the update, then click **Update** or, if the task has the **Complete** status, click **Done:**

   * To add a note about the update, go to the **Updates** area and click **Start a new update**, then type your note.  

   * To notify certain users about the update, type their names in the **Notify** box that appears when you type a note about the update. For more information, see [Tag others on updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md). 
   * To update the condition of the task, click **Select Condition** to the right of the **Notify** box (these appear when you type a note about the update), then select the condition that best reflects the current condition of the task.
   
   * To update the Commit Date of the task, expand the **Commit Date** drop-down calendar, and select a new Commit Date. 
   * To provide a visual indication of task completion, drag the bubble under Percent Complete or double-click it to enter a percent value.   
     ![](assets/drag-the-progress-bar-350x155.png)-->

## Atualizar automaticamente o status da tarefa

O Workfront atualiza automaticamente o status existente de uma tarefa para um status diferente quando as ações listadas na tabela abaixo ocorrem.

>[!NOTE]
>
>Os status na tabela a seguir são os status padrão do sistema. O administrador do Workfront ou um administrador de grupo pode renomear os status na sua instância do Workfront. Para obter informações sobre como criar e gerenciar status no Workfront, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Ação</b></td> 
   <td><b>Status Original</b></td> 
   <td><b>Novo Status</b></td> 
  </tr> 
  <tr> 
   <td>Atualizar o percentual concluído da tarefa para 100%</td> 
   <td>Novo ou em andamento</td> 
   <td>Completo</td> 
  </tr> 
  <tr> 
   <td>Atualizar o percentual concluído da tarefa de 100% para um número mais baixo</td> 
   <td>Completo</td> 
   <td>Em andamento</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Clique no botão Iniciar Tarefa para aceitar trabalhar em uma tarefa atribuída a você</span> </td> 
   <td><span>Novo</span> </td> 
   <td> <p>Qualquer status associado ao botão Iniciar Tarefa nas configurações da Equipe Doméstica.</p> <p>Para obter informações sobre como substituir o botão Trabalhar na tarefa pelo botão Iniciar tarefa, consulte <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Substituir o botão Trabalhar na tarefa por um botão Iniciar</a></span>.</p> <p>Dica: <span>Clicar</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">no botão Desfazer</span>depois de clicar em Iniciar Tarefa, reverte o status para Novo. </p> </td> 
  </tr> 
 </tbody> 
</table>
