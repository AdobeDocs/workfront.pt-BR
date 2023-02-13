---
product-area: projects
navigation-topic: manage-issues
title: Excluir problemas
description: Você pode excluir problemas ou solicitações no Adobe Workfront se tiver o acesso e as permissões corretas para isso.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# Excluir problemas

Você pode excluir problemas ou solicitações no Adobe Workfront se tiver o acesso e as permissões corretas para isso.

>[!TIP]
>
>&quot;Problemas&quot; e &quot;solicitações&quot; são usadas alternadamente no Workfront. Você pode registrar problemas em projetos e tarefas para indicar trabalhos imprevistos que precisam ser abordados. Também é possível enviar solicitações registradas como problemas em um projeto designado como Fila de solicitações.

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
   <td> <p>Solicitação ou superior</p> <p>Revise a licença ou superior para excluir problemas na seção Problemas de um projeto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuração de nível de acesso*</td> 
   <td> <p>Editar acesso a problemas</p> <p>Visualizar ou aumentar o acesso a Projetos e Tarefas</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a problemas no Nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso a problemas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no problema</p> <p>Contribuir ou obter permissões mais altas no projeto ou na tarefa</p> <p> Para obter informações sobre a concessão de permissões para problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a></p> <p>Para obter informações sobre a solicitação de permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações para exclusão de problemas

* O administrador do Workfront ou um administrador de grupo deve habilitar a exclusão de problemas em um projeto que tenha o status Concluído na área Preferências do projeto . Para obter informações sobre como configurar preferências de projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se o problema tiver horas registradas, o administrador do Workfront ou um administrador de grupo deve permitir a exclusão desses problemas configurando as Preferências de tarefa e ocorrência na sua instância do Workfront. Isso também se aplica quando você tenta excluir projetos que têm problemas com horas registradas neles.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   Para obter mais informações sobre como ativar a exclusão de problemas em que as horas são registradas, consulte a seção &quot;Exclusão&quot; em [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## O impacto da exclusão de problemas

Ao excluir um problema, você afeta outros objetos vinculados ao problema.

Os seguintes objetos anexados a um problema também são excluídos quando você exclui um problema:

* Documentos

   Não é possível excluir um problema que tenha um documento com check-out anexado a ele. Para obter mais informações sobre como fazer check-out de documentos, consulte [Verificar documentos](../../../documents/managing-documents/check-out-documents.md).

* Notas
* Aprovações

Dependendo de como seu Workfront ou administrador de grupo configura as Preferências de Exclusão de Projeto, Tarefa ou Edição no **Folha de Horas e Preferências de Hora** da sua instância do Workfront, as horas registradas para os problemas são tratadas de uma das seguintes maneiras ao excluir um problema:

* Mova para o projeto e não será restaurado no problema, se o problema for restaurado posteriormente.
* Ser excluído e será restaurado no problema, se o problema for restaurado posteriormente.

   Isso também se aplica quando você tenta excluir projetos que têm tarefas com horas conectadas.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   Para obter mais informações sobre como configurar as preferências de exclusão para horas registradas em problemas, consulte [Configurar preferências de hora e folha de ponto](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Os usuários atribuídos à emissão ou à aprovação de emissão permanecem na equipe do projeto.\
   Para obter mais informações sobre equipes de projeto, consulte [Visão geral da equipe do projeto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Excluir problemas

* [Excluir vários problemas em um projeto simultaneamente](#delete-multiple-issues-in-a-project-simultaneously)
* [Excluir um único problema](#delete-a-single-issue)

### Excluir vários problemas em um projeto simultaneamente  {#delete-multiple-issues-in-a-project-simultaneously}

1. Vá para o **Menu principal**.
1. Clique em **Projetos**.
1. Clique no nome do projeto que contém os problemas que deseja excluir.
1. Clique em **Problemas** no painel esquerdo.
1. Selecione um problema e clique no botão **Excluir** ícone ![](assets/delete.png) na parte superior da lista.

1. Se a exclusão for permitida, clique em **Sim, excluir**.\
   O administrador do Workfront pode não permitir a exclusão de problemas em que as horas são registradas.\
   Para obter mais informações sobre o acesso e as permissões necessárias para excluir um problema, consulte [Excluir problemas](#access-and-permissions-needed).

### Excluir um único problema {#delete-a-single-issue}

1. Clique no botão **Principal** menu.
1. Clique em **Projetos**.
1. Clique no nome do projeto que contém o problema que deseja excluir.
1. Clique em **Problemas** no painel esquerdo.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Clique no nome do problema que deseja excluir.
1. Clique no botão **Mais** menu.

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Clique em **Excluir**.
1. Se a exclusão for permitida, clique em **Sim, excluir**.

   O administrador do Workfront pode não permitir a exclusão de problemas em que as horas são registradas.\
   Para obter mais informações sobre o acesso e as permissões necessárias para excluir um problema, consulte [Excluir problemas](#access-and-permissions-needed).

## Restaurar problemas excluídos

Um administrador de grupo ou Workfront pode restaurar problemas dentro de 30 dias após serem excluídos. Para obter mais informações sobre como restaurar itens no Workfront, consulte [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
