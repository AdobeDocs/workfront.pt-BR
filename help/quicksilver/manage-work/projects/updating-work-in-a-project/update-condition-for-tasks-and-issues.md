---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar condição para tarefas e problemas
description: A Condição de uma tarefa ou problema é um sinalizador colocado sobre ele para indicar como está indo. Isso é diferente do Status do item de trabalho, que indica o estágio atual do desenvolvimento do item.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 18dfb67626982d73ad33871b8afce4a3f0d4cdb3
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Atualizar condição para tarefas e problemas

A Condição de uma tarefa ou problema é um sinalizador colocado sobre ele para indicar como está indo. Isso é diferente do Status do item de trabalho, que indica o estágio atual do desenvolvimento do item.

Você pode definir a Condição de uma tarefa ou um problema de forma automática ou manual.

O administrador do Adobe Workfront pode criar condições personalizadas para seu ambiente, conforme descrito em [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## Requisitos de acesso {#access-requirements}

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
   <td>

Para as novas licenças:
<ul><li><p>Padrão para tarefas</p></li>
   <li><p>Colaborador ou superior para problemas</p></li></ul>


Para licenças atuais:
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
   <p>Gerenciar permissões em tarefas e problemas para atualizar a Condição</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront. Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Localizar a condição de tarefas e problemas

As condições são exibidas como um sinalizador associado a tarefas ou problemas. Eles também podem ser associados a um número que pode ser exibido em relatórios em vez do rótulo. Para obter mais informações sobre como associar condições a números, consulte [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

É possível localizar a Condição de tarefas e problemas em relatórios e listas ao exibir o campo Condição em uma Exibição ou Agrupamento.

>[!NOTE]
>
>Quando a palavra &quot;condição&quot; é exibida no campo Nome do campo de um relatório de Lançamento, isso indica que a Condição de um item foi atualizada. Quando o campo Condição é rastreado nos relatórios Lançamentos, os Valores de Número Novo e Antigo exibem o número associado à condição em vez de seu nome. Se uma condição não tiver sido originalmente definida para uma tarefa ou um problema e você atualizá-la posteriormente, o lançamento que capturar a atualização exibirá o Valor Velho de Número do campo Condição como -2.147.483.648.

## Atualizar a Condição automaticamente atualizando o status

Quando uma tarefa ou problema for atribuído a você e você clicar em **Trabalhar na tarefa** , Iniciar tarefa ou Iniciar problema, ou atualizar seu status, a Condição da tarefa ou problema muda automaticamente para a Condição padrão associada a **Indo Bem**.

Para obter informações sobre como usar uma Condição personalizada como uma Condição padrão, consulte os artigos  [Definir uma condição personalizada como padrão para tarefas e problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) e [Definir uma condição personalizada como padrão para projetos](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Para obter informações sobre como alterar o status da tarefa, consulte [Atualizar status da tarefa](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Para obter informações sobre como alterar o status do problema, consulte [Atualizar status do problema](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Para obter informações sobre como configurar o botão Trabalhar na tarefa para um botão Iniciar tarefa ou Iniciar problema, consulte [Substitua o botão Trabalhar na tarefa por um botão Iniciar](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Atualizar manualmente a Condição

Você deve ser atribuído a uma tarefa ou a um problema ou ter permissões de gerenciamento para poder definir a Condição nela.

Você pode atualizar manualmente a Condição de uma tarefa ou problema em um relatório ou lista de tarefas ou problemas ao exibir o campo Condição na exibição.

>[!NOTE]
>
>Peça ao administrador do sistema ou do grupo para adicionar o campo Condição ao painel Resumo para facilitar a atualização em várias áreas do Workfront.
>
>Para obter mais informações, consulte os seguintes artigos:
>
>* [Visão geral do resumo](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personalizar Início e Resumo usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

Para atualizar manualmente a Condição de uma tarefa ou um problema:

1. Vá para uma lista de tarefas ou problemas para os quais você tem permissões de gerenciamento. Assegure a **Condição** está visível na visualização da lista.

1. Atualize o **Condição** do problema ou tarefa em linha, clicando duas vezes na condição existente e selecionando um novo valor no menu suspenso.

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >As condições podem ser personalizadas para seu ambiente, portanto, você pode encontrar mais de três opções de Condição em seu ambiente. Os nomes das Condições podem ser diferentes dos listados acima. Para obter informações sobre como personalizar condições no Workfront, consulte [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. Pressione **Enter** no teclado ou clique fora do campo Condição para salvar a nova tarefa ou condição de problema.

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
