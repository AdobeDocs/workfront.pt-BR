---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar condição para tarefas e problemas
description: A Condição de uma tarefa ou problema é um sinalizador colocado sobre ele para indicar como está indo. Isso é diferente do Status do item de trabalho, que indica o estágio atual do desenvolvimento do item.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---

# Atualizar condição para tarefas e problemas

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

A Condição de uma tarefa ou problema é um sinalizador colocado sobre ele para indicar como está indo. Isso é diferente do Status do item de trabalho, que indica o estágio atual do desenvolvimento do item.

Você pode definir a Condição de uma tarefa ou um problema de forma automática ou manual.

Os valores de Condição aos quais nos referimos neste artigo estão disponíveis no Workfront por padrão. O administrador do Adobe Workfront pode criar condições personalizadas para o seu ambiente, conforme descrito em [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Requisitos de acesso {#access-requirements}

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td> 
   Novo:
   <ul><li><p>Padrão para tarefas</p></li>
   <li><p>Colaborador ou superior para problemas</p></li></ul>
   Atual:
   <ul><li><p>Trabalhar ou mais para tarefas</p></li>
   <li><p>Solicitação ou superior para problemas</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir ou aumentar o acesso aos projetos</p> <p>Editar acesso a tarefas e problemas </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exiba permissões ou mais altas em tarefas e problemas para exibir sua Condição</p>
   <p>Permissões do Contribute em tarefas e problemas para atualizar a Condição</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você deve ser atribuído a uma tarefa ou a um problema para poder atualizar manualmente sua Condição.

## Localizar a condição de tarefas e problemas

As condições são exibidas como um sinalizador associado a tarefas ou problemas. Eles também podem ser associados a um número que pode ser exibido em relatórios em vez do rótulo. Para obter mais informações sobre como associar condições a números, consulte [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

É possível localizar a Condição de tarefas e problemas nas seguintes áreas do Workfront:

* A página Detalhes, depois que um administrador de Workfront ou grupo a adiciona ao modelo de layout. Para obter informações, consulte [Personalizar o modo de exibição de Detalhes usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

* O cabeçalho de uma tarefa ou problema, depois que um administrador de Workfront ou grupo o adiciona ao seu modelo de layout. Para obter informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

* O painel Resumo, depois que um administrador de Workfront ou grupo o adiciona ao modelo de layout. Para obter informações, consulte [Personalizar Início e Resumo usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

* Relatórios e listas quando você exibe o campo Condição em uma Exibição ou Agrupamento.

  >[!NOTE]
  >
  >Quando a palavra &quot;condição&quot; é exibida no campo Nome do campo de um relatório de Lançamento, isso indica que a Condição de um item foi atualizada. Quando o campo Condição é rastreado nos relatórios Lançamentos, os Valores de Número Novo e Antigo exibem o número associado à condição em vez de seu nome. Se uma condição não tiver sido originalmente definida para uma tarefa ou um problema e você atualizá-la posteriormente, o lançamento que capturar a atualização exibirá o Valor Velho de Número do campo Condição como -2.147.483.648.

## Atualizar a Condição automaticamente atualizando o status

Quando uma tarefa ou problema é atribuído a você e você clica em **Trabalhar nisto**, Iniciar tarefa ou Iniciar problema, ou atualizar seu status, a Condição da tarefa ou problema muda automaticamente para a Condição padrão associada a **Indo bem**.

Para obter informações sobre como usar uma Condição personalizada como uma Condição padrão, consulte os artigos [Definir uma condição personalizada como padrão para tarefas e problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) e [Definir uma condição personalizada como padrão para projetos](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Para obter informações sobre como alterar o status da tarefa, consulte [Atualizar status da tarefa](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Para obter informações sobre como alterar o status do problema, consulte [Atualizar status do problema](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Para obter informações sobre como configurar o botão Trabalhar na tarefa como um botão Iniciar tarefa ou Iniciar problema, consulte [Substituir o botão Trabalhar na tarefa por um botão Iniciar](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Atualizar manualmente a Condição

Você deve ser atribuído a uma tarefa ou a um problema ou ter permissões de gerenciamento para poder definir a Condição nela.

Você pode atualizar manualmente a Condição de uma tarefa ou problema em um relatório ou lista de tarefas ou problemas ao exibir o campo Condição na exibição.

>[!NOTE]
>
>Você pode pedir ao administrador do sistema ou do grupo para adicionar o campo Condição ao painel Resumo ou às páginas de detalhes ou cabeçalho de tarefas ou problemas.
>
>Para obter mais informações, consulte os seguintes artigos:
>
>* [Resumo geral](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personalizar Página Inicial e Resumo usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

Você pode atualizar manualmente a Condição de tarefas e problemas em várias áreas do Workfront. As seções a seguir descrevem como você pode atualizar manualmente a Condição de tarefas e problemas.

### Atualizar a Condição de uma tarefa ou problema no cabeçalho da tarefa ou problema

1. (Condicional) Se o administrador do Workfront ou do grupo tiver adicionado o campo Condição ao cabeçalho da tarefa ou do problema do modelo de layout, clique no campo **Condição** no cabeçalho e selecione uma das seguintes opções:
   * Indo Bem
   * Algumas Dificuldades
   * Com Problemas

   ![](assets/condition-in-task-header.png)
1. Clique em Enter para salvar a Condição.

### Atualizar a Condição de uma tarefa ou problema na seção Detalhes da tarefa ou problema

1. (Condicional) Se o administrador do Workfront ou do grupo tiver adicionado o campo Condição à seção Detalhes de uma tarefa ou problema no modelo de layout, clique em **Detalhes** no painel esquerdo e, em seguida, clique em **Condição da tarefa** ou **Condição do problema** e selecione uma das seguintes opções:
   * Indo Bem
   * Algumas Dificuldades
   * Com Problemas
1. Clique em **Salvar alterações**. A condição da tarefa ou problema é atualizada.

### Atualizar a Condição de uma tarefa ou problema em um relatório ou lista

1. Vá para uma lista de tarefas ou problemas para os quais você tem permissões de gerenciamento. Verifique se o campo **Condição** está visível no modo de exibição da lista.

1. Atualize a **Condição** do problema ou tarefa em linha, clicando duas vezes na condição existente e selecionando um novo valor no menu suspenso.

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >As condições podem ser personalizadas para seu ambiente, portanto, você pode encontrar mais de três opções de Condição em seu ambiente. Os nomes das Condições podem ser diferentes dos listados acima. Para obter informações sobre como personalizar Condições no Workfront, consulte [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. Pressione **Enter** no teclado ou clique fora do campo Condição para salvar a nova tarefa ou condição de problema.

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


