---
product-area: projects
navigation-topic: manage-tasks
title: Excluir tarefas
description: É possível excluir tarefas que podem estar duplicadas ou que foram criadas com erro.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: 7c373707f6e5ec1431e38cc0e103e25cd8cf2309
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# Excluir tarefas

É possível excluir tarefas que podem estar duplicadas ou que foram criadas com erro.

Para tarefas com informações históricas (atualizações, alterações de agendamento, status ou outros campos), recomendamos que você as feche ou marque como Dead (Desativado), em vez de excluí-las. Isso ajuda a manter as informações históricas dos projetos.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalhar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Tarefas e Projetos com acesso a Excluir</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a tarefas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Conceder acesso a tarefas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões para o projeto com a capacidade de adicionar tarefas ou superior</p> <p>Ao criar uma tarefa, você recebe automaticamente permissões Gerenciar para a tarefa</p> <p> Para obter informações sobre permissões de tarefas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Compartilhar uma tarefa </a>. </p> <p>Para obter informações sobre a solicitação de permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Entender o processo de exclusão de tarefas

* [Limitações para excluir tarefas](#limitations-for-deleting-tasks)
* [O impacto da exclusão de tarefas](#the-impact-of-deleting-tasks)

### Limitações para excluir tarefas  {#limitations-for-deleting-tasks}

* Quando um projeto tem um status de Concluído, você pode excluir tarefas somente se o administrador do Workfront ou um administrador de grupo tiver permitido isso na área Preferências do projeto. Para obter informações sobre como configurar as preferências do projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se a tarefa tiver registrado horas, o Workfront ou o administrador de grupo deverá permitir a exclusão dessas tarefas configurando as Preferências de tarefas e problemas na sua instância do Workfront. Isso também se aplica quando você tenta excluir projetos com tarefas com horas registradas.

  <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

  Para obter mais informações sobre como ativar a exclusão de tarefas em que as horas são registradas, consulte a seção &quot;Exclusão&quot; em [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### O impacto da exclusão de tarefas {#the-impact-of-deleting-tasks}

Ao excluir uma tarefa, você afeta outros objetos vinculados à tarefa.

Os seguintes objetos anexados a uma tarefa também são excluídos quando você exclui uma tarefa:

* Documentos

  Não é possível excluir uma tarefa que tenha um documento com check-out anexado a ela. Para obter mais informações sobre como fazer check-out de documentos, consulte [Fazer check-out de documentos](../../../documents/managing-documents/check-out-documents.md).

* Problemas
* Subtarefas
* Notas
* Aprovações

Dependendo de como o administrador do Workfront configura as Preferências de exclusão de projeto, tarefa ou problema na Planilha de horas e preferências de hora da sua instância do Workfront, as horas registradas para as tarefas são tratadas de uma das seguintes maneiras ao excluir uma tarefa:

* Mover para o projeto e não será restaurado na tarefa, se a tarefa for restaurada posteriormente.
* São excluídos e serão restaurados na tarefa, se a tarefa for restaurada posteriormente.

  Isso também se aplica quando você tenta excluir projetos com tarefas com horas registradas.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

  Para obter mais informações sobre como configurar as preferências de exclusão para horas registradas em problemas, consulte [Configurar preferências de horas e planilha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* As despesas da tarefa serão movidas para o projeto.

* Os usuários atribuídos à tarefa ou à aprovação da tarefa permanecem na equipe do projeto.

  Para obter mais informações sobre as equipes de projeto, consulte [Visão geral da equipe do projeto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Excluir tarefas

* [Excluir várias tarefas em um projeto simultaneamente](#delete-multiple-tasks-in-a-project-simultaneously)
* [Excluir uma única tarefa](#delete-a-single-task)

### Excluir várias tarefas em um projeto simultaneamente  {#delete-multiple-tasks-in-a-project-simultaneously}

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Projetos**.
1. Clique no nome do projeto que contém as tarefas que deseja excluir.
1. Clique em **Tarefas** no painel esquerdo.
1. Siga um destes procedimentos:

   1. (Condicional) Quando a variável **Salvamento automático** a opção de alternância está ativada:

      1. Selecione as tarefas que deseja excluir e clique em **Mais**
      1. Clique em **Excluir**, depois **Sim, exclua.** para confirmar a exclusão.

         As tarefas são excluídas.

   1. (Condicional) Clique no link **Modo de plano** e selecione **Salvamento manual** se quiser reverter as alterações feitas na lista de tarefas.

      ![Selecione Salvar manualmente](assets/manual-save-option.png)

      Faça o seguinte:

      1. Selecione as tarefas que deseja excluir.
      1. Clique em **Excluir**.
      1. (Opcional) Clique em **Desfazer** para reverter a alteração e não excluir as tarefas.
      1. Clique em **Refazer** se desejar manter a alteração e excluir a tarefa.
      1. Clique em **Salvar** para excluir as tarefas.

         As tarefas são excluídas somente depois que você salva suas alterações.

### Excluir uma única tarefa {#delete-a-single-task}

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Projetos**.
1. Clique no nome do projeto que contém a tarefa que deseja excluir.
1. Clique em **Tarefas** no painel esquerdo.
1. Clique no nome da tarefa que deseja excluir.
1. Clique em **Mais** ícone ![](assets/qs-more-menu.png)no canto superior direito.

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. Clique em **Excluir tarefa**.
1. Se a exclusão for permitida, clique em **Sim, exclua**.

   O administrador do Workfront ou o administrador de grupo pode não permitir a exclusão de tarefas em que as horas são registradas.

   Para obter mais informações sobre acesso e permissões necessárias para excluir uma tarefa, consulte a seção [Limitações para excluir tarefas](#limitations-for-deleting-tasks) neste artigo.

## Restaurar tarefas excluídas

Um administrador de grupo ou Workfront pode restaurar tarefas em até 30 dias após sua exclusão, conforme descrito em [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
