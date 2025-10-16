---
title: Compartilhar um projeto
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: O administrador do Adobe Workfront pode conceder acesso para visualizar ou editar projetos ao atribuir seu nível de acesso. Para obter mais informações, consulte Conceder acesso aos projetos.
author: Courtney
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '1574'
ht-degree: 5%

---

# Compartilhar um projeto

<!-- Audited: 1/2024 -->

O administrador do Adobe Workfront pode conceder acesso para visualizar ou editar projetos ao atribuir seu nível de acesso. Para obter mais informações, consulte [Conceder acesso aos projetos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Juntamente com o nível de acesso concedido aos usuários, você também pode conceder a eles permissões para Exibir, Contribute ou Gerenciar projetos específicos que você tenha acesso para compartilhar.

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Trabalhar ou superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir o acesso ou superior aos objetos que você deseja compartilhar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superiores aos objetos que você deseja compartilhar</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre o compartilhamento de projetos

Além das considerações abaixo, consulte também [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Por padrão, o criador de um projeto tem permissões para gerenciar o projeto e também é designado como o Proprietário do projeto. Se o projeto for atribuído a outro proprietário, esse usuário também terá permissões para gerenciar o projeto. Quando o criador (ou proprietário) do projeto compartilha o projeto com outros usuários, ele concede determinadas permissões a esses usuários para controlar o que eles podem fazer enquanto trabalham no projeto.

  No entanto, se o proprietário de um projeto não tiver uma licença Plan ou Standard, ele não terá acesso total para gerenciar o projeto. Somente um usuário com uma licença do Plan ou Standard pode ter permissões para gerenciar um projeto. Para obter mais informações, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

* Você pode compartilhar projetos individualmente ou vários deles de cada vez. O compartilhamento de projetos é idêntico ao compartilhamento de outros objetos. Para obter mais informações sobre como compartilhar itens no Workfront, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Você pode conceder as seguintes permissões a um projeto:

   * Exibir
   * Gerenciar
   * Contribuir

* Quando você compartilha um projeto, todas as tarefas, problemas e documentos herdam as mesmas permissões, a menos que especificado de outra forma.

  Para obter informações sobre como gerenciar o acesso a tarefas e problemas no projeto com base nas permissões de um usuário para o projeto, consulte a seção [&#128279;](../../manage-work/projects/manage-projects/edit-projects.md#access) no artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

  O administrador do Workfront pode especificar se os documentos devem herdar permissões de objetos superiores no nível de acesso do usuário. Para obter mais informações sobre como restringir permissões herdadas em documentos, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Você pode remover permissões herdadas de um projeto para que os objetos filhos não as herdem. Para obter mais informações sobre como remover permissões herdadas de objetos, consulte [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Limitações para diferentes tipos de licença

* Os usuários com uma licença de Trabalhador não têm permissões para gerenciar projetos. Para os funcionários, a maior permissão de compartilhamento é o Contribute.
* Os usuários com uma Solicitação de licença podem visualizar informações do projeto, mas têm acesso limitado ao projeto.
* Uma exceção à alteração do status de um projeto ocorre quando um usuário com permissões de Exibição ou Contribute também é incluído em um processo de aprovação. Eles podem aprovar o projeto, o que altera o status do projeto, mas o status é o status predefinido para aprovação ou rejeição.
* Para poder copiar um projeto, um usuário também deve ter acesso para criar projetos em seu Nível de acesso.

## Maneiras de compartilhar um projeto {#ways-to-share-a-project}

Você pode compartilhar um projeto das seguintes maneiras:

* Manualmente, seguindo um destes procedimentos:

   * Adicionar usuários à equipe do projeto. Quando você adiciona usuários à equipe do projeto, eles obtêm automaticamente permissões de Visualização para o projeto.\
     Para obter mais informações sobre como adicionar usuários a uma equipe de projeto, consulte a seção Adicionando usuários a uma equipe de projeto na [Visão geral da Equipe de Projeto](../../manage-work/projects/planning-a-project/project-team-overview.md).
   * Compartilhamento individual ou em massa de projetos ao usar a opção **Compartilhamento**.

* Automaticamente, seguindo um destes procedimentos:

   * Coloque um projeto em um **Portfolio** ou **Programa** que já esteja compartilhado com outras pessoas. Os usuários obtêm as mesmas permissões para o projeto que têm para o portfólio ou programa.\
     Para obter informações sobre como adicionar um projeto a um **Portfolio**, consulte [Adicionar projetos a um portfólio](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).\
     Para obter informações sobre como adicionar um projeto a um **Programa**, consulte [Adicionar um projeto a um programa](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).
Para obter informações sobre a exibição de permissões herdadas em um objeto, consulte [Exibir permissões herdadas em objetos](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

   * Adicione entidades ao Compartilhamento de projeto em um modelo usado para criar o projeto. Para obter informações sobre como compartilhar projetos a partir de modelos, consulte [Compartilhar um modelo](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).
   * Defina o modelo de acesso ao projeto.

     >[!TIP]
     >
     >Ao anexar ou salvar um modelo, você pode apagar as regras de Compartilhamento do projeto de modelo.

   * Editar um projeto e definir a configuração **Quando alguém tiver acesso a este projeto**. Para obter mais informações, consulte [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p>  </li>
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

## Compartilhar um projeto

{{step1-to-projects}}

1. Na página **Projetos**, selecione o projeto que deseja compartilhar na lista. A página do projeto é aberta.

1. À direita do nome do projeto, clique em **Compartilhar**. A caixa de diálogo **Compartilhar [Nome do Projeto]** será aberta.

   ![Botão Compartilhar projeto](assets/share-project.png)

1. No campo **Conceder acesso ao projeto**, comece digitando o nome do usuário, equipe, função, grupo ou empresa com a qual deseja compartilhar o projeto e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar um projeto com usuários, equipes, funções ou empresas ativos.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso do projeto:

   * **Somente pessoas convidadas podem acessá-lo:** Somente usuários convidados para o projeto podem acessá-lo (Padrão).
   * **Todos no sistema podem exibir**: todos os usuários do sistema podem exibir o projeto sem um convite.

1. (Opcional) Para aplicar automaticamente as configurações de acesso do projeto que você selecionou a todos os novos projetos, clique no ícone **Engrenagem** ![Selecione o ícone de engrenagem](assets/gear-icon.png) e marque a caixa de seleção integrada com **Definir como meu modelo de acesso ao projeto**.

   >[!NOTE]
   >
   >O modelo de acesso ao projeto substitui os padrões de compartilhamento concedidos a você pelo administrador do Workfront em seu Nível de acesso.\
   >Para obter mais informações sobre como especificar padrões de compartilhamento para projetos no Nível de Acesso, consulte [Conceder acesso aos projetos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->


1. Clique no menu suspenso à direita do nome do usuário e selecione o nível de permissão para este projeto:


   * **Exibir**: o usuário pode revisar e compartilhar o projeto.
   * **Contribute**: o usuário pode fazer atualizações, registrar informações, fazer pequenas edições e compartilhar o projeto (também inclui todas as permissões de exibição).
   * **Gerenciar**: o usuário tem acesso total ao projeto sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição e Contribute).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas no projeto.

   ![Opções avançadas de permissão configuradas](assets/advanced-permission-options.png)

1. (Opcional) Para compartilhar rapidamente o projeto usando um link, clique em **Copiar link** e encaminhe-o para o destinatário.

1. Clique em **Salvar**.

## Compartilhar projetos em massa

{{step1-to-projects}}

1. Na página **Projetos**, selecione a caixa à esquerda de cada projeto que você deseja compartilhar e clique no ícone **Compartilhar** ![Ícone Compartilhar](assets/share-icon.png) na parte superior da página. O modal de compartilhamento é aberto.

   ![Projetos de compartilhamento em massa](assets/bulk-share-icon.png)

1. No campo **Conceder acesso ao projeto para**, comece digitando o nome do usuário, equipe, função, grupo ou empresa com a qual deseja compartilhar os projetos e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar projetos com usuários, equipes, funções ou empresas ativos.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso dos projetos:

   * **Somente pessoas convidadas podem acessá-las:** Somente usuários convidados para os projetos podem acessá-las (Padrão).
   * **Todos no sistema podem exibir**: todos os usuários do sistema podem exibir os projetos sem um convite.


1. Clique no menu suspenso à direita do nome do usuário e selecione o nível de permissão para os projetos:

   * **Exibir**: o usuário pode revisar e compartilhar os projetos.
   * **Contribute**: o usuário pode fazer atualizações, registrar informações, fazer pequenas edições e compartilhar os projetos (também inclui todas as permissões de exibição).
   * **Gerenciar**: o usuário tem acesso total aos projetos sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição e Contribute).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas nos projetos.

   ![Opções avançadas de permissão configuradas](assets/advanced-permission-options.png)

1. Clique em **Salvar**.


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing&nbsp;the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
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

A tabela a seguir lista as permissões que os usuários podem conceder ao compartilhar um projeto. Para obter mais informações sobre o acesso que os usuários obtêm com base em suas licenças, consulte [Conceder acesso aos projetos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Ações</strong> </p> </th> 
   <th> <p><strong>Gerenciar</strong> </p> </th> 
   <th> <p><strong>Contribute</strong> </p> </th> 
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
   <td> <p>Adicionar problema(s)</p> </td> 
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
   <td> <p>Gerenciar Linha de Base</p> </td> 
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
   <td> <p>Gerenciar finanças*</p> </td> 
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
   <td> <p>Adicionar/Editar Business Case</p> </td> 
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
   <td> <p>Editar Equipe</p> </td> 
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
   <td> <p>Recalcular Finanças/Linha de Tempo*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Definir Propriedades da Fila</p> </td> 
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

&#42;Os usuários sem acesso a dados financeiros não podem gerenciar riscos e finanças para projetos, mesmo que tenham acesso para Editar aos projetos. Para obter informações sobre acesso a dados financeiros, consulte [Conceder acesso a dados financeiros](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
