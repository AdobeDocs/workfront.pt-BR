---
product-area: projects
navigation-topic: manage-tasks
title: Excluir Tarefas
description: É possível excluir tarefas que podem estar duplicadas ou que foram criadas com erro.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: 0c0ffbeefb0eed8d1ca2a6e68ed19b40080726df
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 5%

---

# Excluir tarefas

É possível excluir tarefas que podem estar duplicadas ou que foram criadas com erro.

Para tarefas com informações históricas (atualizações, alterações de agendamento, status ou outros campos), recomendamos que você as feche ou marque como Dead (Desativado), em vez de excluí-las. Isso ajuda a manter as informações históricas dos projetos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Padrão</p> 
   <p>Trabalho ou maior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Tarefas e Projetos com acesso a Excluir</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões para o projeto com a capacidade de adicionar tarefas ou superior</p> <p>Ao criar uma tarefa, você recebe automaticamente permissões Gerenciar para a tarefa</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects with access to&nbsp;Delete</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Entender o processo de exclusão de tarefas

* [Limitações para excluir tarefas](#limitations-for-deleting-tasks)
* [O impacto da exclusão de tarefas](#the-impact-of-deleting-tasks)

### Limitações para excluir tarefas  {#limitations-for-deleting-tasks}

* Quando um projeto tem um status de Concluído, você pode excluir tarefas somente se o administrador do Workfront ou um administrador de grupo tiver permitido isso na área Preferências do projeto. Para obter informações sobre como configurar preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se a tarefa tiver registrado horas, o Workfront ou o administrador de grupo deverá permitir a exclusão dessas tarefas configurando as Preferências de tarefas e problemas na sua instância do Workfront. Isso também se aplica quando você tenta excluir projetos com tarefas com horas registradas.

  <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

  Para obter mais informações sobre como habilitar a exclusão de tarefas em que as horas são registradas, consulte a seção &quot;Exclusão&quot; em [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### O impacto da exclusão de tarefas {#the-impact-of-deleting-tasks}

Ao excluir uma tarefa, você afeta outros objetos vinculados à tarefa.

Considere o seguinte:

* Os seguintes objetos anexados a uma tarefa também são excluídos quando você exclui uma tarefa:

   * Documentos

  Não é possível excluir uma tarefa que tenha um documento com check-out anexado a ela. Para obter mais informações sobre o check-out de documentos, consulte [Check-out de documentos](../../../documents/managing-documents/check-out-documents.md).

   * Problemas
   * Subtarefas
   * Notas
   * Aprovações

* Dependendo de como o administrador do Workfront configura as Preferências de exclusão de projeto, tarefa ou problema na Planilha de horas e preferências de hora da sua instância do Workfront, as horas registradas para as tarefas são tratadas de uma das seguintes maneiras ao excluir uma tarefa:

   * Mover para o projeto e não será restaurado na tarefa, se a tarefa for restaurada posteriormente.
   * São excluídos e serão restaurados na tarefa, se a tarefa for restaurada posteriormente.

  Isso também se aplica quando você tenta excluir projetos com tarefas com horas registradas.

  Para obter mais informações sobre como configurar as preferências de exclusão para horas registradas em problemas, consulte [Configurar preferências de horas e planilha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
   * As despesas da tarefa serão movidas para o projeto.

   * Os usuários atribuídos à tarefa ou à aprovação da tarefa permanecem na equipe do projeto.

  Para obter mais informações sobre as equipes de projeto, consulte [Visão geral da Equipe de Projeto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

* Quando você exclui uma tarefa filho e move seu pai para outro projeto e, em seguida, restaura a tarefa filho excluída, a tarefa é adicionada de volta ao projeto original como uma tarefa principal.

<!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

## Excluir tarefas

* [Excluir várias tarefas em um projeto simultaneamente](#delete-multiple-tasks-in-a-project-simultaneously)
* [Excluir uma única tarefa](#delete-a-single-task)

### Excluir várias tarefas em um projeto simultaneamente  {#delete-multiple-tasks-in-a-project-simultaneously}

1. Clique no ícone **do** Menu principal![](assets/main-menu-icon.png), no canto superior direito do Adobe Workfront.

1. Clique em **Projetos**.
1. Clique no nome do projeto que contém as tarefas que deseja excluir.
1. Clique em **Tarefas** no painel esquerdo.
1. Siga um destes procedimentos:

   1. (Condicional) Quando a opção **Salvar automaticamente** está habilitada:

      1. Selecione as tarefas que deseja excluir e clique em **Mais**
      1. Clique em **Excluir** e depois em **Excluir** para confirmar a exclusão.

         As tarefas são excluídas.

   1. (Condicional) Clique no ícone **Modo de Plano** e selecione **Salvar manualmente** se desejar reverter as alterações feitas na lista de tarefas.

      ![Selecionar Salvamento Manual](assets/manual-save-option.png)

      Faça o seguinte:

      1. Selecione as tarefas que deseja excluir.
      1. Clique em **Excluir**.
      1. (Opcional) Clique em **Desfazer** para reverter sua alteração e não excluir as tarefas.
      1. Clique em **Refazer** se desejar manter a alteração e excluir a tarefa.
      1. Clique em **Salvar** para excluir as tarefas.

         As tarefas são excluídas somente depois que você salva suas alterações.

### Excluir uma única tarefa {#delete-a-single-task}

1. Clique no ícone **do** Menu principal![](assets/main-menu-icon.png), no canto superior direito do Adobe Workfront.

1. Clique em **Projetos**.
1. Clique no nome do projeto que contém a tarefa que deseja excluir.
1. Clique em **Tarefas** no painel esquerdo.
1. Clique no nome da tarefa que deseja excluir.
1. Clique no ícone **Mais** ![](assets/qs-more-menu.png)no canto superior direito.

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. Clique em **Excluir tarefa**.
1. Se a exclusão for permitida, clique em **Excluir**.

   O administrador do Workfront ou o administrador de grupo pode não permitir a exclusão de tarefas em que as horas são registradas.

   Para obter mais informações sobre o acesso e as permissões necessárias para excluir uma tarefa, consulte a seção [Limitações para excluir tarefas](#limitations-for-deleting-tasks) neste artigo.

## Restaurar tarefas excluídas

Um administrador de Workfront ou de grupo pode restaurar tarefas em até 30 dias após sua exclusão, conforme descrito em [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
