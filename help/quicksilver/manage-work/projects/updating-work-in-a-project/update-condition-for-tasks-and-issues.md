---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar condição para tarefas e problemas
description: A Condição de uma tarefa ou problema é um sinalizador colocado nela para indicar como está indo. É diferente do Status do item de trabalho, que indica o estágio atual de desenvolvimento do item.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# Atualizar condição para tarefas e problemas

A Condição de uma tarefa ou problema é um sinalizador colocado nela para indicar como está indo. É diferente do Status do item de trabalho, que indica o estágio atual de desenvolvimento do item.

Você pode definir a Condição de uma tarefa ou um problema automática ou manualmente.

O administrador do Adobe Workfront pode criar Condições personalizadas para o seu ambiente, conforme descrito em [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## Requisitos de acesso {#access-requirements}

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
   <td> 
   
   For the current licenses:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>


   For legacy licenses:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Trabalhar ou superior para tarefas</p>
   <p>Solicitação ou superior para problemas</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso aos projetos</p> <p>Editar acesso a tarefas e problemas </p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar permissões ou permissões superiores em tarefas e problemas para visualizar sua condição</p>
   <p>Gerenciar permissões em tarefas e problemas para atualizar a condição</p>
    <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Localizar a condição de tarefas e problemas

As condições são exibidas como um sinalizador associado a tarefas ou problemas. Eles também podem ser associados a um número que pode ser exibido em relatórios em vez do rótulo. Para obter mais informações sobre como associar condições a números, consulte [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Você pode localizar a Condição de tarefas e problemas nas seguintes áreas:

* Área Atualizações de tarefa e emissão, dentro de uma atualização, quando você é atribuído à tarefa ou ocorrência.
* Relatórios e listas quando você exibe o campo Condição em uma Exibição ou Agrupamento.

>[!NOTE]
>
>Quando a palavra &quot;condição&quot; é exibida no campo Nome do campo de um relatório de Entrada de diário, isso indica que a Condição de um item foi atualizada. Quando o campo Condição é rastreado nos relatórios de Entradas de Diário, os Novos e Antigos Valores de Número exibem o número associado à condição em vez de seu nome. Se uma condição originalmente não estiver definida para uma tarefa ou um problema e você depois a atualizar, o lançamento que captura a atualização exibirá o Valor antigo do campo Condição como -2,147,483,648.

## Atualizar automaticamente a condição atualizando o status

Quando uma tarefa ou problema é atribuído e você clica em **Trabalhe Com Ele** , Iniciar Tarefa ou Iniciar Problema, ou atualizar seu status, a Condição da tarefa ou ocorrência muda automaticamente para a Condição padrão associada a **Suavizando sem problemas**.

Para obter informações sobre como usar uma condição personalizada como uma condição padrão, consulte os artigos  [Definir uma condição personalizada como padrão para tarefas e problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) e [Definir uma condição personalizada como padrão para projetos](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Para obter informações sobre como alterar o status da tarefa, consulte [Atualizar status da tarefa](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Para obter informações sobre como alterar o status do problema, consulte [Atualizar status do problema](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Para obter informações sobre como configurar o botão Trabalhar nele para um botão Iniciar Tarefa ou Iniciar Problema, consulte [Substitua o botão Trabalho nele por um botão Iniciar](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Atualizar manualmente a condição

Você deve ser atribuído a uma tarefa ou ao problema ou ter permissões de Gerenciar para poder definir a Condição nela.

A atualização da Condição de uma tarefa ou problema difere dependendo se você está atribuído a ela ou não:

* Você pode atualizar a Condição na guia Atualizações ou em uma lista de tarefas ou problemas se você estiver atribuído a elas.
* Você pode atualizar a condição somente em uma lista de tarefas ou problemas se não estiver atribuído a elas, mas tiver permissões de gerenciamento para elas. Nesse caso, não é possível atualizar a Condição na guia Update da tarefa ou problema.

Para definir manualmente a Condição de uma tarefa ou um problema:

1. Vá para uma tarefa ou problema atribuído a você para o qual deseja definir a Condição.

   Ou

   Acesse uma lista de tarefas ou problemas aos quais você tem permissões de gerenciamento, mas que não estão atribuídos a você.

1. Altere a Condição do problema ou tarefa da seguinte maneira:

   * Se você estiver atribuído à tarefa ou problema e tiver permissões de gerenciamento para ela, no **Atualizações** clique em **Iniciar uma nova atualização**, selecione o **Condição** que reflete melhor como a tarefa está indo, digite seu motivo para alterar a Condição no **Iniciar uma nova atualização** área (opcional) e clique em **Atualizar**.

      ![](assets/change-condition-update-comment-350x141.png)

      >[!NOTE]
      >
      >As condições podem ser personalizadas para o seu ambiente, portanto, você pode encontrar mais de três opções para Condição no seu ambiente. Os nomes das Condições podem ser diferentes dos acima enumerados. Para obter informações sobre como personalizar Condições no Workfront, consulte [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

      Para obter informações sobre a funcionalidade adicional que está disponível ao atualizar um item de trabalho, consulte [Atualizar trabalho](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
