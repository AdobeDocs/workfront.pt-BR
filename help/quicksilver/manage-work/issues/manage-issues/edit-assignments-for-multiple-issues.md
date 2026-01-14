---
product-area: projects
navigation-topic: manage-issues
title: Modificar atribuições de usuário para vários problemas em uma lista
description: Modificar atribuições de usuário para vários problemas em uma lista
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 8f7249e08268a8cb784d4c0ecc8c534542fa80cf
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 4%

---

# Modificar atribuições de usuário para vários problemas em uma lista

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Você pode modificar simultaneamente as atribuições de usuários para várias questões. Para obter informações sobre como editar problemas ou atribuí-los um de cada vez, consulte também os seguintes artigos:

* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Atribuir problemas](../../../manage-work/issues/manage-issues/assign-issues.md)

Para obter informações gerais sobre atribuição de problemas, consulte [Visão geral da modificação de atribuições de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Você deve ter pelo menos permissões do Contribute para que um problema possa fazer atribuições a ele.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td> <p>Colaborador ou superior</p>
   <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Acesso de visualização ou superior aos Projetos e Tarefas para atribuir um problema</p> </td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do problema</p> <p>Ao atribuir vários problemas, contribua com permissões ou mais altas para o projeto ou tarefa em que o problema está localizado.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Modificar atribuições para vários problemas

1. Vá para a lista de problemas que contém os problemas cujas atribuições você deseja modificar.
1. (Opcional) Crie um filtro para exibir somente problemas atribuídos ao destinatário que você deseja modificar.

   Por exemplo, você pode criar um filtro para exibir somente problemas com uma função específica como destinatário.  Em seguida, você pode substituir a função por um usuário específico. Faça o seguinte:

   1. Clique na lista suspensa **Filtros** e em **Novo filtro**.

   1. No primeiro campo, comece digitando **Funções de atribuição** e escolha **Funções de atribuição: Nome** na lista.
   1. Selecione **É qualquer um de** no menu suspenso do modificador, em seguida, comece a digitar o nome de uma função e selecione-o quando ele for exibido na lista. Você pode digitar várias funções.

      >[!TIP]
      >
      >Não use **Atribuído a** porque este campo se refere apenas ao Proprietário do problema e não a todos os atribuídos.

      A lista de problemas filtra automaticamente os critérios de filtro.
   1. (Opcional) Clique em **Salvar como novo** e depois em **Salvar**.

1. Selecione os problemas para os quais deseja modificar atribuições e clique no **ícone Editar** ![ícone Editar](assets/qs-edit-icon.png).

   O **Editar problemas** é exibido. O número de itens selecionados é exibido no canto superior esquerdo da página.

1. Clique em **Atribuições** no painel esquerdo e clique no ícone **x** ao lado do destinatário que você deseja remover.

   >[!TIP]
   >
   >Somente os atribuídos atribuídos a todas as questões selecionadas são exibidos na área **Atribuições**.

   ![Área de atribuições em problemas de edição em massa](assets/assignments-area-on-bulk-edit-issues.png)

1. Comece digitando o nome de um usuário, função ou equipe para adicionar atribuídos a todas as questões selecionadas.

   >[!TIP]
   >
   >Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos.
   >
   >Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
   >
   >* Reatribuir o item de trabalho aos recursos ativos.
   >* Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.

   Os atribuídos adicionados são adicionados aos existentes. Elas não substituem as existentes para cada problema selecionado.

1. (Opcional) Clique em **Atribuir a mim** para atribuir todos os problemas a você mesmo.
1. Clique em **Salvar**.


   <!--Old functionality for assignments for issues - before November 2025:
   1. (Conditional) In the Production environment, do the following: 
   1. Go to the **Assignments** section, then select **Assignee**.
      ![Assignments area](assets/classic-assignmens-area-on-edit-box-350x119.png)
   1. Do one of the following:
      1. To add a new assignee:
         1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected issues.
         >[!TIP]
         >
         >You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
         >
         >If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
         >
         >* Reassign the work item to active resources.
         >* Associate the users in a deactivated team with an active team and reassign the work item to the active team.
          Information that is common across all issues selected displays. For example, if the same user is assigned to all issues, that user displays in the **Assignee**  column. If information is not common across the issues selected, no information displays.
      1. To remove individual assignees:
         1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.
            Or
            If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the issues that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.
         1. Click  **Remove Assignee** again to add another assignee to remove.
      1. To remove all existing assignees:
         1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.
            This removes not only common assignees (assignees that are displayed in the edit  dialog box), but also all assignees on all the selected issues.
         1. (Optional) Modify any of the following options for the assignees you selected to associate with the issues:
          * **Issue Owner:**  Select the radio button to indicate which assignee is designated as the Issues Owner. If left unselected, Adobe Workfront designates the first assignee as the Issue Owner. This is not available for team assignments. 
            * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Workfront automatically selects the Primary Role of the user.
      1. Click **Save Changes**.-->




