---
product-area: projects
navigation-topic: manage-issues
title: Excluir problemas
description: Você pode excluir problemas ou solicitações no Adobe Workfront se tiver o acesso e as permissões corretas para fazer isso.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: aa2bef064df3ff7dd9e4fd896ac7482df3c55e32
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 1%

---

# Excluir problemas

<!--Audited: 05/2025-->

Você pode excluir problemas ou solicitações no Adobe Workfront se tiver o acesso e as permissões corretas para fazer isso.

>[!TIP]
>
>&quot;Problemas&quot; e &quot;solicitações&quot; são usados alternadamente no Workfront. Você pode registrar problemas em projetos e tarefas para indicar trabalho imprevisto que precisa ser resolvido. Você também pode enviar solicitações que são registradas como ocorrências em um projeto designado como uma Fila de solicitações.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td> <p>Novo: Colaborador ou superior</p>
   <p>Atual: solicitação ou superior</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuração do nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Acesso de visualização ou superior a projetos e tarefas</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no problema</p> <p>Permissões do Contribute ou superiores no projeto ou tarefa</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações para exclusão de problemas

* O administrador do Workfront ou um administrador de grupo deve habilitar a exclusão de problemas em um projeto com o status Concluído na área Preferências do projeto.

  Para obter informações sobre como configurar preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se o problema tiver registrado horas, o administrador do Workfront ou um administrador de grupo deverá permitir a exclusão desses problemas configurando as Preferências de tarefas e problemas na sua instância do Workfront. Isso também se aplica quando você tenta excluir projetos que têm problemas com horas registradas neles.

  Para obter mais informações sobre como habilitar a exclusão de problemas em que as horas são registradas, consulte a seção &quot;Exclusão&quot; em [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).


## O impacto da exclusão de problemas

Ao excluir uma ocorrência, você afeta outros objetos vinculados à ocorrência.

Os seguintes objetos anexados a uma ocorrência também são excluídos quando você exclui uma ocorrência:

* Documentos

  Não é possível excluir um problema que tenha um documento com check-out anexado a ele. Para obter mais informações sobre o check-out de documentos, consulte [Check-out de documentos](../../../documents/managing-documents/check-out-documents.md).

* Notas
* Aprovações

Dependendo de como o administrador do Workfront ou do grupo configura as Preferências de exclusão de projeto, tarefa ou problema na **Folha de horas e preferências de hora** da sua instância do Workfront, as horas registradas para os problemas serão tratadas de uma das seguintes maneiras ao excluir um problema:

* Mova para o projeto e não será restaurado no problema, se o problema for restaurado posteriormente.
* Será excluído e será restaurado no problema, se o problema for restaurado posteriormente.

  Isso também se aplica quando você tenta excluir projetos com tarefas com horas registradas.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Para obter mais informações sobre como configurar as preferências de exclusão para horas registradas em problemas, consulte [Configurar preferências de horas e planilha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Os usuários atribuídos ao problema ou à aprovação do problema permanecem na equipe do projeto.\
  Para obter mais informações sobre as equipes de projeto, consulte [Visão geral da Equipe de Projeto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Excluir problemas

### Excluir vários problemas em um projeto simultaneamente  {#delete-multiple-issues-in-a-project-simultaneously}

1. Vá para o **Menu principal**.
1. Clique em **Projetos**.
1. Clique no nome do projeto que contém os problemas que você deseja excluir.
1. Clique em **Problemas** no painel esquerdo.

   Uma lista de problemas associados ao projeto selecionado é exibida à direita.
1. Selecione um ou vários problemas na lista e clique no **ícone Excluir** ![ícone Excluir](assets/delete.png) na parte superior da lista.

1. Se a exclusão for permitida, clique em **Excluir**.

   O administrador do Workfront pode não permitir a exclusão de problemas em que as horas são registradas.\
   Para obter mais informações sobre o acesso e as permissões necessárias para excluir um problema, consulte a seção [Considerações para a exclusão de problemas](#considerations-for-deleting-issues) neste artigo.

### Excluir um único problema {#delete-a-single-issue}

{{step1-to-projects}}

1. Clique no nome do projeto que contém o problema que você deseja excluir.
1. Clique em **Problemas** no painel esquerdo.

   ![Seção de problemas no painel esquerdo](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Clique no nome do problema que deseja excluir.
1. Clique no menu **Mais** à direita do nome do problema.

   ![Menu Emitir Mais](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Clique em **Excluir problema**.
1. Se a exclusão for permitida, clique em **Excluir**.

   O administrador do Workfront pode não permitir a exclusão de problemas em que as horas são registradas.\
   Para obter mais informações sobre o acesso e as permissões necessárias para excluir um problema, consulte a seção [Considerações para a exclusão de problemas](#considerations-for-deleting-issues) neste artigo.

## Restaurar problemas excluídos

Um administrador de grupo ou da Workfront pode restaurar problemas 30 dias após a exclusão.

Para obter mais informações sobre como restaurar itens no Workfront, consulte [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
