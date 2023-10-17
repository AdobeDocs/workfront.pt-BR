---
title: Excluir projetos
product-area: projects
navigation-topic: manage-projects
description: Você pode excluir um projeto se ele e seus dados não forem mais necessários.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: 5db9a4869e1321bd268e80f786d157fbb41c0656
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 1%

---

# Excluir projetos

Você pode excluir um projeto se ele e seus dados não forem mais necessários.

Como alternativa à exclusão de um projeto, recomendamos editar o projeto e alterar o status para Concluído ou Inativo. Isso remove todas as tarefas atuais relacionadas ao projeto da lista de tarefas de um usuário, mas salva todos os dados associados ao projeto.

## Requisitos de acesso

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Delete</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Edit access to Projects, Tasks, Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos, Tarefas, Problemas com capacidade de Excluir projetos, tarefas e problemas</p> <p><b>Nota</b></p>

<p>Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões para o projeto, tarefas e problemas no projeto com a capacidade de Excluir o projeto, tarefas e problemas. </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.
Você pode excluir um projeto em uma lista de projetos ou no nível do projeto.

## Entender o processo de exclusão de projetos

* [Limitações para excluir projetos](#limitations-for-deleting-projects)
* [O impacto da exclusão de projetos](#the-impact-of-deleting-projects)

### Limitações para excluir projetos  {#limitations-for-deleting-projects}

* Os itens excluídos são movidos para a Lixeira por 30 dias e podem ser recuperados somente pelo administrador do Workfront.

  Para obter mais informações sobre como restaurar objetos, consulte o artigo [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Se o projeto tiver tarefas ou problemas com horas reportadas, o administrador do Workfront ou do grupo deverá permitir a exclusão dessas tarefas configurando as Preferências de tarefas e problemas na sua instância do Workfront para que você possa excluir o projeto que contém as tarefas.

  Para obter mais informações sobre como ativar a exclusão de tarefas, problemas ou projetos em que as horas são registradas, consulte a seção &quot;Exclusão&quot; em [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### O impacto da exclusão de projetos {#the-impact-of-deleting-projects}

* Ao excluir um projeto, você afeta outros objetos vinculados ao projeto.

  Os seguintes objetos anexados a um projeto também são excluídos quando você exclui um projeto:

   * Documentos

     Não é possível excluir um projeto que tenha um documento anexado cujo check-out tenha sido feito. Para obter mais informações sobre como fazer check-out de documentos, consulte [Fazer check-out de documentos](../../../documents/managing-documents/check-out-documents.md).

   * Tarefas
   * Subtarefas
   * Problemas
   * Atualizações
   * Aprovações
   * Despesas
   * Riscos
   * Linhas de base
   * Informações do Business Case
   * Informações de Detalhes da Fila
   * Preços
   * Registro de cobrança

     Não é possível excluir um projeto que tenha Registros de cobrança com status Faturado. Para obter mais informações, consulte [Criar registros de cobrança](../../projects/project-finances/create-billing-records.md).

* Dependendo de como o administrador do Workfront configura as Preferências de exclusão de projeto, tarefa ou problema na Planilha de horas e preferências de hora da sua instância do Workfront, as horas registradas para as tarefas, problemas ou o projeto são tratadas de uma das seguintes maneiras ao excluir o projeto:

   * As horas permanecem na folha de horas como tempo geral.
   * As horas são excluídas e serão restauradas se o projeto for restaurado.

  Para obter mais informações sobre como configurar as preferências de exclusão para horas registradas em problemas, consulte [Configurar preferências de horas e planilha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Se o projeto excluído estiver vinculado a uma iniciativa no Planejador de cenários do Workfront:

   * A iniciativa permanece no plano, mas o link para o projeto foi removido.
   * Se o projeto excluído estiver vinculado à única iniciativa publicada de um plano, a indicação de que o plano foi publicado também será removida.
   * Se você recuperar um projeto excluído, o projeto será recuperado, mas o link para a iniciativa não será restaurado e a área do Planejador de cenários não será mais exibida em Detalhes do projeto.

     O Planejador de cenários está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../../scenario-planner/scenario-planner-overview.md).

     Para obter informações sobre projetos vinculados a iniciativas no Planejador de cenários, consulte [Atualizar ou criar projetos publicando iniciativas no Planejador de cenários](../../../scenario-planner/publish-scenarios-update-projects.md).

* Se o projeto também for uma atividade para uma meta no Workfront Goals:

   * O projeto é excluído da meta. O progresso indicado na meta pelo projeto também é removido.

   * Se você recuperar o projeto excluído, o projeto também será restaurado como a atividade da meta.

     Isso requer uma licença adicional. Para obter informações sobre o Workfront Goals, consulte [Visão geral dos objetivos do Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Para obter informações sobre como associar projetos a metas, consulte [Adicionar projetos às metas no Adobe Workfront Goals](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Excluir um projeto em uma lista

É possível excluir projetos de uma lista de projetos.

1. Ir para uma lista de projetos ou um relatório de projeto.
1. Selecione o(s) projeto(s) que deseja excluir e clique no **Excluir** ícone ![](assets/delete-icon.png) no topo da lista.

1. Clique em **Sim, exclua.** para confirmar a exclusão.

   Os projetos são excluídos e armazenados na Lixeira por 30 dias. O administrador do Workfront pode restaurar projetos excluídos da Lixeira durante esse período.

## Excluir um projeto no nível do projeto

1. Vá para o projeto que deseja excluir.
1. Clique em **Mais** ícone ![](assets/qs-more-menu.png)e, em seguida, clique em **Excluir Projeto**.

   ![](assets/more-icon-expanded-delete-project-highlighted.png)

1. Clique em **Sim, exclua**.

   O projeto é excluído e armazenado na Lixeira por 30 dias. O administrador do Workfront pode restaurá-lo da Lixeira durante esse período.

## Restauração de projetos excluídos

Um administrador de sistema ou de grupo pode restaurar projetos no prazo de 30 dias após sua exclusão, conforme descrito no artigo [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
