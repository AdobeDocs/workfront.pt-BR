---
title: Excluir projetos
product-area: projects
navigation-topic: manage-projects
description: Você pode excluir um projeto se ele e seus dados não forem mais necessários. Como alternativa à exclusão de um projeto, recomendamos editar o projeto e alterar o status para Concluído ou Inativo. Isso remove todas as tarefas atuais relacionadas ao projeto da lista de tarefas de um usuário, mas salva todos os dados associados ao projeto.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
recommendations: noDisplay, noCatalog
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 1%

---

# Excluir projetos

<!--Audited: 01/2024-->

Você pode excluir um projeto se ele e seus dados não forem mais necessários.

Como alternativa à exclusão de um projeto, recomendamos editar o projeto e alterar o status para Concluído ou Inativo. Isso remove todas as tarefas atuais relacionadas ao projeto da lista de tarefas de um usuário, mas salva todos os dados associados ao projeto.

Você pode excluir um projeto em uma lista de projetos ou no nível do projeto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>plano do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td> <p>Licença da Adobe Workfront*</p> </td> 
   <td> <p>Licença atual: plano </p> 
   Ou
   <p>Nova licença: Standard </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configuração do nível de acesso</td> 
   <td> <p>Editar acesso aos Projetos com capacidade para Criar e Excluir projetos</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto </p> </td> 
   <td> <p>Editar acesso a Projetos, Tarefas, Problemas com capacidade de Excluir projetos, tarefas e problemas</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront. Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Entender o processo de exclusão de projetos

* [Limitações para excluir projetos](#limitations-for-deleting-projects)
* [O impacto da exclusão de projetos](#the-impact-of-deleting-projects)

### Limitações para excluir projetos  {#limitations-for-deleting-projects}

* Os itens excluídos são movidos para a Lixeira por 30 dias e podem ser recuperados somente pelo administrador do Workfront.

  Para obter mais informações sobre como restaurar objetos, consulte o artigo [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Se o projeto tiver tarefas ou problemas com horas reportadas, o administrador do Workfront ou do grupo deverá permitir a exclusão dessas tarefas configurando as Preferências de tarefas e problemas na sua instância do Workfront para que você possa excluir o projeto que contém as tarefas.

  Para obter mais informações sobre como habilitar a exclusão de tarefas, problemas ou projetos com horas registradas, consulte a seção &quot;Exclusão&quot; em [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### O impacto da exclusão de projetos {#the-impact-of-deleting-projects}

* Ao excluir um projeto, você afeta outros objetos vinculados ao projeto.

  Os seguintes objetos anexados a um projeto também são excluídos quando você exclui um projeto:

   * Documentos

     Não é possível excluir um projeto que tenha um documento anexado cujo check-out tenha sido feito. Para obter mais informações sobre o check-out de documentos, consulte [Check-out de documentos](../../../documents/managing-documents/check-out-documents.md).

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

* Dependendo de como o administrador do Workfront configura as Preferências de exclusão de projeto, tarefa ou problema na Planilha de horas e preferências de horas da sua instância do Workfront, as horas registradas para as tarefas, problemas ou o projeto são tratadas de uma das seguintes maneiras ao excluir o projeto:

   * As horas permanecem na folha de horas como tempo geral.
   * As horas são excluídas e serão restauradas se o projeto for restaurado.

  Para obter mais informações sobre como configurar as preferências de exclusão para horas registradas em problemas, consulte [Configurar preferências de horas e planilha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Se o projeto excluído estiver vinculado a uma iniciativa no Planejador de cenários do Workfront:

   * A iniciativa permanece no plano, mas o link para o projeto foi removido.
   * Se o projeto excluído estiver vinculado à única iniciativa publicada de um plano, a indicação de que o plano foi publicado também será removida.
   * Se você recuperar um projeto excluído, o projeto será recuperado, mas o link para a iniciativa não será restaurado e a área do Planejador de cenários não será mais exibida em Detalhes do projeto.

     O Planejador de cenários requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../../scenario-planner/scenario-planner-overview.md).

     Para obter informações sobre projetos vinculados a iniciativas no Planejador de cenários, consulte [Atualizar ou criar projetos publicando iniciativas no Planejador de cenários](../../../scenario-planner/publish-scenarios-update-projects.md).

* Se o projeto também for uma atividade para uma meta no Workfront Goals:

   * O projeto é excluído da meta. O progresso indicado na meta pelo projeto também é removido.

   * Se você recuperar o projeto excluído, o projeto também será restaurado como a atividade da meta.

     Isso requer uma licença adicional. Para obter informações sobre as Metas do Workfront, consulte [Visão geral das Metas do Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Para obter informações sobre como associar projetos a metas, consulte [Adicionar projetos a metas nas Metas da Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Excluir um projeto em uma lista

É possível excluir projetos de uma lista de projetos.

1. Ir para uma lista de projetos ou um relatório de projeto.
1. Selecione o(s) projeto(s) que deseja excluir e clique no ícone **Excluir** ![](assets/delete-icon.png) na parte superior da lista.

1. Clique em **Sim, Excluir** para confirmar a exclusão.

   Os projetos são excluídos e armazenados na Lixeira por 30 dias. O administrador do Workfront pode restaurar projetos excluídos da Lixeira durante esse período.

## Excluir um projeto no nível do projeto

1. Vá para o projeto que deseja excluir.
1. Clique no ícone **Mais** ![](assets/qs-more-menu.png) à direita do nome do projeto e clique em **Excluir projeto**.

   ![](assets/more-icon-expanded-delete-project-highlighted.png)

1. Clique em **Sim, exclua**.

   O projeto é excluído e armazenado na Lixeira por 30 dias. O administrador do Workfront pode restaurá-lo da Lixeira durante esse período.

## Restauração de projetos excluídos

Um administrador de sistema ou de grupo pode restaurar projetos no prazo de 30 dias após sua exclusão, conforme descrito no artigo [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
