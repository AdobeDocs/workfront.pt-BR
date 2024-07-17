---
product-area: resource-management
navigation-topic: resource-planning
title: Visão geral dos conjuntos de recursos
description: Como gerenciador de recursos, você pode gerenciar seus recursos adicionando usuários ao conjunto de recursos.
author: Alina
feature: Resource Management
exl-id: f3fc65c8-e436-44a4-9e9d-5b4b138a9f21
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Visão geral dos conjuntos de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** The sections about how to add resource pools to users, templates, projects are duplicated from the articles listed in those sections (Creating Users, Editing Projects, Creating a Template, etc). These sections might be eliminated when the Resource Pools are not something new, and just a routine field to edit on these main objects.) </p>
-->

Como gerenciador de recursos, você pode gerenciar seus recursos adicionando usuários ao conjunto de recursos.

O gerenciamento eficiente de recursos não pode ocorrer sem preencher seus Conjuntos de recursos com usuários e anexá-los a projetos. Isso é um pré-requisito para usar a funcionalidade Planejamento de Recursos.

Para obter mais informações sobre os pré-requisitos necessários antes de começar a usar o Planejamento de Recursos, consulte a seção &quot;Pré-requisitos para trabalhar no Planejador de Recursos&quot; na [Visão geral do Planejador de Recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Para obter informações sobre como criar e gerenciar conjuntos de recursos, consulte os seguintes artigos:

* [Criar pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)
* [Associar conjuntos de recursos a projetos e modelos](../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md)
* [Associar pools de recursos a usuários](../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md)
* [Remover usuários do conjunto de recursos](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Access requirements</h2>
<p>(NOTE: moved to the separate articles below) </p>
<p>You must have the following:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Pro and higher</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to&nbsp;Resource Management that includes access to Manage Resource Pools</p> <p>Edit access to Projects, Templates, and Users</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## Visão geral do conjunto de recursos

* Um Conjunto de Recursos é uma coleção de usuários necessários ao mesmo tempo para a conclusão de um projeto.
* Um Conjunto de recursos pode ser compartilhado entre vários projetos, programas ou portfólios quando estiver associado a todos os projetos nos programas e portfólios.
* Você pode criar um Conjunto de recursos e preenchê-lo com usuários existentes após sua criação ou pode criar o Conjunto de recursos e associá-lo a um usuário existente ou a um novo usuário durante a criação ou edição do usuário.
* Depois de preencher os Conjuntos de recursos com usuários, você pode associá-los a projetos e modelos e gerenciar a alocação de usuários para os projetos com mais eficiência.
* Você pode associar quantos Conjuntos de recursos forem necessários a um projeto, modelo ou usuário.

## Critérios para associar usuários a um Conjunto de recursos

Há várias maneiras de estruturar seus Conjuntos de recursos.

Recomendamos as seguintes abordagens:

* Você pode fazer com que todos os usuários do mesmo Conjunto de recursos pertençam à mesma equipe.

  Por exemplo, se você quiser que todos os usuários de uma equipe de marketing estejam disponíveis para um projeto, você pode desejar um Conjunto de recursos de marketing no qual você adicionaria todos os usuários dessa equipe. Em seguida, você pode associar o Conjunto de recursos de marketing aos projetos aos quais os membros dessa equipe estão atribuídos.

* Você pode fazer com que todos os usuários no mesmo Conjunto de recursos cumpram funções semelhantes, especialmente se as funções estiverem em alta demanda e tiverem que ser orçadas separadamente.

  Por exemplo, você pode ter recursos externos que funcionam como Consultores que você deseja disponibilizar para um projeto de vez em quando. Você pode criar um Conjunto de recursos para consultores que você pode anexar aos seus projetos, onde você pode colocar ambos os usuários que são consultores internos ou externos.

* Você também pode criar Conjuntos de Recursos por departamento ou centro de custo.
* Não recomendamos adicionar todos os usuários no sistema a um Conjunto de recursos se você tiver um grande número de usuários ou se gerenciar recursos para um grande número de projetos de cada vez.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Create a Resource Pool</strong></p>
<p>(NOTE: Alina: **^^ Linked to messaging from emails/ AC/ Pendo, possibly. Do not rename or change the anchor. << this comment is old.</p>
<p>***Feb 2022: moved this section to its own article and drafted it here. Consider undrafting the section with a short intro to point to the new article IF there are any complaints.) </p>
<ol>
<li value="1">Log in as a user who has access to edit Resource Pools.<br>For more information, see <a href="#create-a-resource-pool" class="MCXref xref">Create a Resource Pool</a>.</li>
<li value="2">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="3"> Click <strong>Resourcing</strong>. </li>
<li value="4"> Click <strong>Resource Pools</strong> in the left panel. <br><img src="assets/resource-pools-tab-350x198.png" alt="resource_pools_tab.png" style="width: 350;height: 198;"></li>
<li value="5">Click <strong>New Resource Pool</strong>.</li>
<li value="6">Specify the following: <p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><strong>Name</strong></td>
<td>This is the name of the Resource Pool.</td>
</tr>
<tr>
<td role="rowheader"><strong>Description</strong></td>
<td>This is a brief description about this Resource Pool. For example, you can specify for what purpose it should be used.</td>
</tr>
<tr>
<td role="rowheader">(Optional) <strong>Pool Members</strong></td>
<td><p> Add users to the Resource Pool individually.<br>Or <br>To add a large amount of users to the Resource Pool at one time, you can add one of the following entities associated with users. This adds those users to the Resource Pool:
<ul>
<li><strong>Teams</strong>: all members of the team are added to the Resource Pool.</li>
<li><strong>Groups</strong>: all members of the group are added to the Resource Pool.</li>
<li><strong>Roles</strong>: all users associated with that role are added to the Resource Pool.</li>
<li><strong>Companies</strong>: all users in the company are added to the Resource Pool.</li>
</ul><note type="tip">
You can only add active users, teams,
<span>roles,</span> or companies.
</note><note type="note">
If a user becomes a member of a group, team, company or is associated with a job role after the group, team, company or job role have been added to the Resource Pool, the new member is not automatically added to the Resource Pool.
<br>If a user belongs to the team, group, company, and job role you are adding, at the same time, the user is added only once to the Resource Pool.
<br>Users who are deactivated after having been added to the Resource Pool appear dimmed in the list of users and are marked as being deactivated.
</note></p></td>
</tr>
</tbody>
</table></p></li>
<li value="7"> <p>(Optional) Use the <strong>Undo</strong> link to remove the users added through a group, team, company or job role.</p> <note type="note">
There is no limit to how many users you can have in a Resource Pool. However, we recommend not adding too many users to a Resource Pool, as Resource Management could become a challenge otherwise. The list of users only shows the first 2,000 users in the Resource Pool, and they are listed alphabetically.
</note> <p> <img src="assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png" alt="Resource_pools_NEW___UNDO_button_for_teams_groups_etc.png" style="width: 350;height: 113;"> </p> </li>
<li value="8">(Optional) Use the <strong>Search</strong> option to find a user in the Resource Pool.</li>
<li value="9">Click <strong>Create</strong>.</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove users from a Resource Pool</h2>
<p>(NOTE: moved to its own article. Drafted here.) </p>
<p>You can remove users from a Resource Pool when those users are no longer needed in that pool. </p>
<p>To remove a user from a Resource Pool:</p>
<ol>
<li value="1">Log in as a user who has access to edit Resource Pools.<br>For more information, see the section <a href="#create-a-resource-pool" class="MCXref xref">Create a Resource Pool</a> in this article.</li>
<li value="2"> Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="3"> Click <strong>Resourcing</strong>.  </li>
<li value="4"> Click <strong>Resource Pools</strong> in the left panel.  </li>
<li value="5">Select a Resource Pool and click <strong>Edit.</strong>Or<br>Click the name of a Resource Pool. </li>
<li value="6">Start typing the name of a user that you want to remove in the <strong>Search in this Resource Pool</strong> field.<br>Or<br>Start typing the name of a company, job role, team, or group, if you want to remove all the users associated with those entities.<br><img src="assets/search-inside-new-resource-pool-350x314.png" alt="search_inside_NEW_resource_pool.png" style="width: 350;height: 314;"></li>
<li value="7">Click the 'x' icon at the user level to remove a user from the Resource Pool. They are removed from all the lists they appear in.<br>Or<br>To remove all users associated with a job role, group, team, or company, click <strong>Remove</strong> at the job role, group, team level, or company level. This removes all the users associated with that job role, group, team, or company from the Resource Pool. </li>
<li value="8">Click <strong>Save</strong>. </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Associate Resource Pools with users</h2>
<p>You must have administrative rights to editing users in order to edit or create users. <br>For more information about the access needed to edit or create users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p>
<ul>
<li><a href="#associate-resource-pools-with-one-user" class="MCXref xref">Associate Resource Pools with one user</a> </li>
<li><a href="#associate-resource-pools-with-users-in-bulk" class="MCXref xref">Associate Resource Pools with users in bulk</a> </li>
</ul>
<p><strong>Associate Resource Pools with one user</strong></p>
<p>You can associate users with Resource Pools when you are creating your Resource Pools. <br>For more information about creating a Resource Pool, see the section <a href="#create-a-resource-pool" target="_blank" rel="noopener noreferrer" class="MCXref xref">Create a Resource Pool</a> in this article.</p>
<p>If you create Resource Pools without populating them with users, you can later associate them with users as you are editing or creating new users. </p>
<p>The Resource Pools must be created before you can associate them with a user. </p>
<p>To associate Resource Pools with users:</p>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> Click <strong>Users</strong>.  </li>
<li value="3">Check the box next to the name of a user from the list, then click <strong>Edit</strong>.</li>
<li value="4">Click <strong>Resource Planning</strong>.</li>
<li value="5">Start typing the name of a Resource Pool that you want to associate with the user in the <strong>Resource Pools</strong> field, then select it from the list, when it appears.<br>You can associate multiple Resource Pools with one user.<br><img src="assets/add-resource-pool-to-user-350x307.png" alt="add_resource_pool_to_user.png" style="width: 350;height: 307;"><br></li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
<p>For more information about editing users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p>
<p>For more information about creating new users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a>.</p>
<p><strong>Associate Resource Pools with users in bulk</strong></p>
<p>You can edit multiple users in bulk and associate the same Resource Pools with all of them at the same time. </p>
<p>To associate Resource Pools with several users in bulk:</p>
<ol>
<li value="1"> Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> Click <strong>Users</strong>. </li>
<li value="3">Select several users on the list, and click <strong>Edit</strong>.</li>
<li value="4">Click <strong>Resource Planning</strong>.</li>
<li value="5">Start typing the name of a Resource Pool that you want to associate with the users in the <strong>Resource Pools</strong> field, then select it from the list, when it appears.<br>You can associate multiple Resource Pools with multiple users.<br><note type="note">
Only the Resource Pools that are common to all the users selected appear in this field. If the users selected have no shared Resource Pools, this field is empty. If this field is empty, the Resource Pools you specify here will overwrite their individual Resource Pools.
</note> <br><br></li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
<p>For more information about how to edit users in bulk, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Edit user profiles in bulk</a>. </p>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Associate resource pools with projects and templates</h2>
<p>(NOTE: moved to its own article) </p>
<p> After you create Resource Pools, you can associate them with projects or templates so you can later budget your resources on the projects. </p>
<p>You must have the following rights to associate Resource Pools with Projects and Templates: </p>
<ul>
<li>You must have rights to Edit projects in your access level, as well as Manage permissions on the project in order to edit the project and associate it with Resource Pools.</li>
<li>You must have rights to Edit templates in your access level, as well as Manage permissions on the template in order to edit the template and associate it with Resource Pools.</li>
</ul>
<p>We recommend that you create your Resource Pools in advance, associate them with projects, and budget your resources before the project starts. </p>
<ul>
<li><a href="#associate-resource-pools-with-one-project-or-template" class="MCXref xref">Associate Resource Pools with one project or template</a> </li>
<li><a href="#associate-resource-pools-with-several-projects-or-templates-in-bulk" class="MCXref xref">Associate Resource Pools with several projects or templates in bulk</a> </li>
</ul>
<p><strong>Associate Resource Pools with one project or template</strong></p>
<p> You can associate Resource Pools with a template in the same manner you associate Resource Pools with a project. </p>
<p> To associate Resource Pools with a project: </p>
<ol>
<li value="1">Go to a project and click the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png">in the upper-right corner.</li>
<li value="2"> Click <strong>Settings</strong>. </li>
<li value="3">Start typing the name of a Resource Pool in the <strong>Resource Pools</strong> field, then select it from the list when it appears.<br>You can associate multiple Resource Pools with one project or template.<br><img src="assets/resource-pool-to-project-350x254.png" alt="resource_pool_to_project.png" style="width: 350;height: 254;"><br><br></li>
<li value="4">Click <strong>Save Changes</strong>.</li>
</ol>
<p> For more information about how to edit a project and associate it with Resource Pools, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p>
<p> For more information about how to edit a template and associate it with Resource Pools, see <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Edit project templates</a>.</p>
<p><strong>Associate Resource Pools with several projects or templates in bulk</strong></p>
<p> You can edit multiple projects or templates in bulk and associate the same Resource Pools with all of them at the same time. </p>
<p>You can associate Resource Pools with templates in the same manner you associate Resource Pools with projects. </p>
<p>To associate Resource Pools with several projects in bulk:</p>
<ol>
<li value="1">Go to a list of projects.</li>
<li value="2">Select multiple projects, then click <strong>Edit</strong>.</li>
<li value="3">Click <strong>Settings</strong>.</li>
<li value="4"> <p>Start typing the name of a Resource Pool in the <strong>Resource Pools</strong> field, then select it from the list when it appears.<br>You can associate multiple Resource Pools with the projects or templates. </p> <note type="note">
When you edit projects or templates in bulk, only the Resource Pools that are common to all the projects or templates selected appear in this field. If the projects selected have no shared Resource Pools, this field will be empty. The Resource Pools you specify here will overwrite the individual Resource Pools of the projects or templates.
</note> </li>
<li value="5">Click <strong>Save Changes</strong>. <br>When your Resource Pools are associated with your projects or your templates, you can budget user allocations for your projects inside the Resource Planner. <br>For more information about the Resource Planner, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</li>
</ol>
<p> For more information about how to edit projects in bulk, see the "Edit projects in bulk" section in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p>
<p> For more information about how to edit templates in bulk, see the "Edit templates in bulk" section in <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Edit project templates</a>.</p>
</div>
-->
