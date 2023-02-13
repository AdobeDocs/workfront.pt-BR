---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar status da tarefa
description: Você pode atualizar o status de uma tarefa para informar outros sobre onde a tarefa está (e o projeto geral) e como está progredindo.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 1%

---

# Atualizar status da tarefa

Você pode atualizar o status de uma tarefa para informar outros sobre onde a tarefa está (e o projeto geral) e como está progredindo.

Os status padrão são Novo, Em andamento e Concluído. O administrador da Adobe Workfront pode adicionar status personalizados para sua organização. Para obter mais informações, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Você pode atualizar manualmente os status da tarefa ou permitir que o Workfront os atualize automaticamente quando determinadas ações ocorrerem.

## Requisitos de acesso

<!--drafted for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para atualizar manualmente as tarefas:

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
   <td> <p>Editar acesso às tarefas</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para a tarefa</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Atualizar manualmente o status da tarefa

Ao atualizar um status de tarefa, você também pode digitar uma explicação sobre o novo status e alterar outras informações da tarefa, como a data de vencimento.

1. Vá para uma tarefa para a qual você está atribuído para a qual deseja atualizar o status.
1. Clique no botão **Status** no cabeçalho da tarefa e selecione um novo status.
1. (Opcional) Siga qualquer um dos procedimentos a seguir para fornecer informações adicionais sobre a atualização, em seguida, clique em **Atualizar** ou, se a tarefa tiver o **Concluído** status, clique em **Feito em:**

   * Para adicionar uma observação sobre a atualização, acesse o **Atualizações** e clique em **Iniciar uma nova atualização** e digite a nota.

   * Para notificar determinados usuários sobre a atualização, digite os nomes deles na **Notificar** que é exibida quando você digita uma nota sobre a atualização. Para obter mais informações, consulte [Marcar outras pessoas em atualizações](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Para atualizar a condição da tarefa, clique em **Selecionar condição** à direita do **Notificar** (aparecem quando você digita uma nota sobre a atualização), em seguida, selecione a condição que reflete melhor a condição atual da tarefa.

   * Para atualizar a Data de confirmação da tarefa, expanda a **Data de confirmação** calendário suspenso e selecione uma nova Data de confirmação.
   * Para fornecer uma indicação visual da conclusão da tarefa, arraste a bolha abaixo de Porcentagem concluída ou clique duas vezes nela para inserir um valor percentual.\
      ![](assets/drag-the-progress-bar-350x155.png)

## Atualizar automaticamente o status da tarefa

O Workfront atualiza automaticamente o status existente de uma tarefa para um status diferente quando as ações listadas na tabela abaixo ocorrem.

>[!NOTE]
>
>Os status na tabela a seguir são status padrão do sistema. O administrador do Workfront ou um administrador de grupo pode renomear os status na instância do Workfront. Para obter informações sobre como criar e gerenciar status no Workfront, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Ação</td> 
   <td>Status original</td> 
   <td>Novo status</td> 
  </tr> 
  <tr> 
   <td>Atualizar o percentual de conclusão da tarefa para 100%</td> 
   <td>Novo ou Em Andamento</td> 
   <td>Completo</td> 
  </tr> 
  <tr> 
   <td>Atualizar o percentual de conclusão da tarefa de 100% para um número menor</td> 
   <td>Completo</td> 
   <td>Em andamento</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Clique no botão Iniciar tarefa para aceitar o trabalho em uma tarefa atribuída a você</span> </td> 
   <td><span>Novo(a)</span> </td> 
   <td> <p>Qualquer status associado ao botão Iniciar Tarefa nas configurações da Equipe Inicial.</p> <p>Para obter informações sobre a substituição do botão Trabalhar nele por um botão Iniciar Tarefa, consulte <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Substitua o botão Trabalho nele por um botão Iniciar</a></span>.</p> <p>Dica: <span>Clicar</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">o botão Desfazer</span>depois de clicar em Iniciar tarefa, o status é revertido para Novo. </p> </td> 
  </tr> 
 </tbody> 
</table>
