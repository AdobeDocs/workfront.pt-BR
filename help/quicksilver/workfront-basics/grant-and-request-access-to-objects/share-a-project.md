---
title: Compartilhar um projeto no Adobe Workfront
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: O administrador do Adobe Workfront pode conceder acesso para visualizar ou editar projetos ao atribuir seu nível de acesso. Para obter mais informações, consulte Conceder acesso a projetos.
author: Alina
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 3%

---

# Compartilhar um projeto no Adobe Workfront

O administrador do Adobe Workfront pode conceder acesso para visualizar ou editar projetos ao atribuir seu nível de acesso. Para obter mais informações, consulte [Conceder acesso aos projetos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Além do nível de acesso que os usuários recebem, você também pode conceder permissões para Exibir, Contribuir ou Gerenciar projetos específicos que você tem acesso para compartilhar.

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item.

## Considerações sobre o compartilhamento de projetos

Além das considerações abaixo, consulte também [Visão geral do compartilhamento de permissões em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Por padrão, o criador de um projeto tem permissões para gerenciar o projeto e também é designado como o Proprietário do projeto. Se o projeto for atribuído a outro proprietário, esse usuário também terá permissões para gerenciar o projeto. Quando o criador (ou proprietário) do projeto compartilha o projeto com outros usuários, eles concedem certas permissões a esses usuários para controlar o que podem fazer enquanto trabalham no projeto.

   No entanto, se o proprietário de um projeto não tiver uma licença do Planejador, ele não terá acesso total para gerenciar o projeto. Somente um usuário com uma licença do Plano pode ter permissões para gerenciar um projeto. Para obter mais informações, consulte [Como os níveis de acesso e as permissões funcionam em conjunto](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

* Você pode compartilhar projetos individualmente ou pode compartilhá-los vários de cada vez. O compartilhamento de projetos é idêntico ao compartilhamento de outros objetos. Para obter mais informações sobre como compartilhar itens no Workfront, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Você pode conceder as seguintes permissões a um projeto: 

   * Exibir
   * Gerenciar
   * Contribuir

      ![](assets/view-on-projects-190x207.png) ![](assets/contribute-on-projects-159x243.png) ![](assets/manage-on-projects-178x230.png)

* Quando você compartilha um projeto, todas as tarefas, problemas e documentos herdam as mesmas permissões, a menos que especificado de outra forma.

   Para obter informações sobre como gerenciar o acesso a tarefas e problemas no projeto com base nas permissões de um usuário para o projeto, consulte o [](../../manage-work/projects/manage-projects/edit-projects.md#access) no artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

   O administrador do Workfront pode especificar se os documentos devem herdar permissões de objetos mais altos no nível de acesso do usuário. Para obter mais informações sobre como restringir permissões herdadas em documentos, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Você pode remover permissões herdadas de um projeto para que os objetos filhos não os herdem. Para obter mais informações sobre como remover permissões herdadas de objetos, consulte  [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Maneiras de compartilhar um projeto {#ways-to-share-a-project}

Você pode compartilhar um projeto das seguintes maneiras:

* Manualmente, seguindo um destes procedimentos:

   * Adicionar usuários à equipe do projeto. Ao adicionar usuários à equipe do projeto, eles obtêm automaticamente permissões de Exibição para o projeto.\
      Para obter mais informações sobre como adicionar usuários a uma equipe de projeto, consulte a seção &quot;Adicionar usuários a uma equipe de projeto&quot; em [Visão geral da equipe do projeto](../../manage-work/projects/planning-a-project/project-team-overview.md).
   * Compartilhamento individual ou em massa dos projetos ao usar a variável **Compartilhamento** opção.

      O compartilhamento de um projeto é semelhante ao compartilhamento de todos os outros objetos no Adobe Workfront.

      Para obter informações sobre o compartilhamento de objetos no Workfront, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Automaticamente, executando um dos seguintes procedimentos:

   * Coloque um projeto em um **Portfolio** ou **Programa** isso já está compartilhado com outros. Os usuários recebem as mesmas permissões do projeto que têm para o portfólio ou programa.\
      Para obter informações sobre como adicionar um projeto a um **Portfolio**, consulte [Adicionar projetos a um portfólio](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).\
      Para obter informações sobre como adicionar um projeto a um **Programa**, consulte [Adicionar um projeto a um programa](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

      Para obter informações sobre como visualizar permissões herdadas em um objeto, consulte [Exibir permissões herdadas em objetos](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

   * Adicione entidades ao Compartilhamento de projeto em um modelo usado para criar o projeto. Para obter informações sobre o compartilhamento de projetos a partir de modelos, consulte [Compartilhar um modelo](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).
   * Defina o modelo de acesso do projeto.

      Para definir o modelo de acesso do projeto, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

      >[!TIP]
      >
      >Ao anexar ou salvar um modelo, você pode limpar as regras de Compartilhamento de projeto do modelo.

   * Edite um projeto e defina a variável **Quando alguém recebe acesso a esse projeto** configuração. Para obter mais informações, consulte [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p> <p> <img src="assets/screen-shot-2014-01-22-at-10.13.10-am-350x284.png" style="width: 350;height: 284;"> </p> </li>
</ol>
</div>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)&nbsp;</li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## Limitações para diferentes tipos de licença

* Os usuários com uma licença do Worker não têm permissões para gerenciar projetos. Para Trabalhadores, a maior permissão de compartilhamento é o Contribute.
* Os usuários com uma licença de Solicitação podem exibir informações do projeto, mas têm acesso limitado ao projeto.
* Uma exceção à alteração do status de um projeto ocorre quando um usuário com permissões de Exibição ou Contributo também é incluído em um processo de aprovação. Eles podem aprovar o projeto, o que altera o status do projeto, mas o status é o status predefinido para aprovação ou rejeição.
* Para poder copiar um projeto, um usuário também deve ter acesso para criar projetos em seu Nível de acesso.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing&nbsp;the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/edit-projnwe-350x155.png" style="width: 350;height: 155;"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see&nbsp;<a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can&nbsp;delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.&nbsp;
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## Opções de permissão do projeto

A tabela a seguir lista as permissões que os usuários podem conceder ao compartilhar um projeto. Para obter mais informações sobre o acesso que os usuários têm com base em sua licença, consulte [Conceder acesso aos projetos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Ações</strong> </p> </th> 
   <th> <p><strong>Gerenciar</strong> </p> </th> 
   <th> <p><strong>Contribuir</strong> </p> </th> 
   <th> <p><strong>Exibir</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Adicionar formulário personalizado</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Atualizar campos personalizados</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Adicionar Um Processo De Aprovação</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aprovar um projeto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aprovar horas</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓ </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Criar Um Projeto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Adicionar documento(s)</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Adicionar problemas</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Adicionar tarefa(s)</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Copiar Projeto</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Excluir Projeto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modificar Datas Planejadas</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Compartilhar projeto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Compartilhe com todo o sistema</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exibir Projeto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Atualizações/comentários</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Alterar status</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Registre as horas</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Editar Atribuições</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gerenciar linha de base</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gerenciar riscos*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gerencie Finanças*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Adicionar/ Editar Despesas*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exibir finanças*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Vincular Modelo</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Salvar como modelo</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Adicionar/ Editar Caso Comercial</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Editar detalhes do projeto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Editar Pessoal</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exportar para o MS Project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Recalcular Finanças/Linha do Tempo*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Definir propriedades da fila</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Editar projeto em massa em uma lista</p> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Usuários sem acesso a dados financeiros não podem gerenciar riscos e finanças de projetos, mesmo que tenham acesso ao Edit para projetos. Para obter informações sobre o acesso a dados financeiros, consulte [Conceder acesso aos dados financeiros](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
