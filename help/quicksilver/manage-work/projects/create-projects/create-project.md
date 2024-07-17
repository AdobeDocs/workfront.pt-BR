---
product-area: projects
navigation-topic: create-projects
title: Criar um Projeto
description: Um projeto é uma grande unidade de trabalho no Adobe Workfront. Você pode criar projetos do zero, usar um modelo ou converter problemas ou tarefas em projetos.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: 49bd393af77a67aa1e3a443c4189569178e99ada
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 1%

---

# Criar um Projeto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is linked from the UI from the Projects global nav section in classic. Do not change/ remove)</p>
-->

<!-- Audited: 12/2023 -->

Os projetos representam uma grande quantidade de trabalho que precisa ser feito no Adobe Workfront.

## Requisitos de acesso

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td> <p>Novo: Padrão</p>
        <p>ou</p>
        <p>Atual: Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Ao criar um projeto, você recebe automaticamente permissões de gerenciamento para o projeto.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação da Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Maneiras de criar projetos

Você pode criar um projeto no Workfront usando um dos seguintes métodos:

* Crie um projeto do zero sem usar um modelo. Este artigo descreve como criar um projeto do zero.

* Copie um projeto existente.\
  Para obter mais informações sobre como copiar um projeto, consulte [Copiar um projeto](../../../manage-work/projects/manage-projects/copy-project.md).

* Use um modelo.\
  Para obter mais informações sobre como usar um modelo para criar um novo projeto, consulte [Criar um projeto usando um modelo](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Importe um projeto do Microsoft Project.\
  Para obter mais informações sobre como importar um projeto do MS Project, consulte [Importar um projeto do Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importe um projeto usando o kick-starts.

  Como administrador do Workfront, você pode importar projetos usando um início.

  Para obter informações sobre como importar dados usando o kick-starts no Workfront, consulte [Importar dados para o Adobe Workfront usando um modelo de Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  Para obter informações sobre como importar projetos usando o kick-starts, consulte [Cenário de Kick-Starts: preparação de importação de projetos e tarefas simples](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Publish uma iniciativa de um cenário no Planejador de cenários do Adobe Workfront. O Planejador de cenários requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../../scenario-planner/scenario-planner-overview.md). Para obter informações sobre como criar projetos a partir de iniciativas de publicação, consulte [Atualizar ou criar projetos publicando iniciativas no Planejador de Cenários](../../../scenario-planner/publish-scenarios-update-projects.md).

## Pré-requisitos

Antes de começar, verifique se:

* O administrador de sistema ou de grupo ativou a preferência &quot;Permitir que os usuários criem projetos sem usar um modelo&quot; na área Configuração.

  Para obter mais informações, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Configurações padrão do novo projeto

Ao criar um projeto, o Workfront aplica um conjunto de configurações padrão a ele. Por exemplo, o Status, o Grupo e o Modo de agendamento são predefinidos quando você cria um projeto.

Considere o seguinte:

* Como administrador do Workfront ou administrador de grupo, você pode definir as configurações padrão para um novo projeto ao configurar as Preferências do projeto para toda a instância do Workfront ou para um grupo.
* O Workfront aplica as configurações do grupo, se houver, antes de aplicar as definidas pelo administrador do Workfront.
* O status padrão de um novo projeto corresponde ao status definido pelo administrador do Workfront na área principal Preferências do projeto ou por um administrador de grupo (ou administrador do Workfront) na área Preferências do projeto de um grupo.

  >[!NOTE]
  >
  >Recomendamos que o status padrão de um novo projeto seja Planejamento. Conforme você faz alterações no novo projeto, isso garante que as notificações não sejam enviadas aos usuários atribuídos ao projeto.
  >
  >Para obter mais informações sobre como configurar o status padrão e outras configurações padrão para um novo projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* Existem os seguintes cenários para como o Workfront define o Grupo e o Status de um novo projeto:

   * Se você criar um projeto do zero, o Grupo do projeto será seu Grupo inicial.

     O Status do projeto é o status padrão nas Preferências do projeto do seu Grupo inicial, se houver, ou da sua instância do Workfront. Você pode alterar o status padrão ao criar o projeto para qualquer status disponível para o Grupo do projeto.

   * Se você criar um projeto usando um modelo, as configurações do modelo terão prioridade sobre as configurações estabelecidas pelo Workfront ou pelo administrador de grupo.

     O Grupo do novo projeto é o Grupo do modelo. Se o modelo não estiver associado a um Grupo, o Grupo do projeto será o Grupo inicial do usuário que cria o projeto.

     O status padrão de um novo projeto criado a partir de um modelo corresponde ao status definido pelo administrador do Workfront na área principal Preferências do projeto ou por um administrador de grupo (ou administrador do Workfront) na área Preferências do projeto do grupo. Você pode alterar o status padrão ao criar um projeto a partir de um modelo, para qualquer um dos status do Grupo do projeto que é o Grupo do modelo ou o Grupo inicial do usuário que cria o projeto.

   * Se você criar um projeto convertendo um problema, o grupo de um novo projeto será o Grupo do projeto existente do problema. Se o usuário que converte o problema não tiver acesso ao projeto do problema ou se o projeto do problema não tiver um Grupo, o Grupo do novo projeto é o Grupo inicial do usuário que converte o problema.

     Os novos status do projeto correspondem aos status do grupo associado ao projeto, que é o Grupo do projeto original ou o Grupo inicial do usuário que está convertendo a ocorrência.

     Se estiver usando um modelo ao criar o projeto convertendo o problema, consulte o segundo cenário acima para entender qual Grupo e qual Status o Workfront aplica ao novo projeto.

## Criar um projeto do zero

>[!NOTE]
>
>Se você estiver criando um projeto usando um modelo, recomendamos que também veja o artigo [Criar um projeto usando um modelo](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).


1. Siga um destes procedimentos:

   * Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo. Clique em **Projetos** e expanda **Novo projeto**.
   * Vá para um portfólio e expanda **Novo projeto**.
   * Vá para um programa e expanda **Novo Projeto**.
   * Se você for um administrador de grupo, também poderá criar um projeto na seção Projetos de um grupo gerenciado. Para obter mais informações, consulte [Criar e modificar projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![Menu Novo Projeto](assets/new-project-dropdown-nwe-350x358.png)

1. Clique em **Novo projeto** no menu para criar um projeto do zero.
1. Digite um nome para o projeto. Pressione Enter para salvar o nome.

   ![Insira um nome para o projeto](assets/rename-untitled-project.png)

   O cabeçalho da página do projeto exibe uma visão geral rápida da integridade atual e do progresso de um projeto. As informações no cabeçalho do projeto são alteradas à medida que as informações do projeto são atualizadas.

1. Clique em **Começar a adicionar tarefas**.

   Ou

   Clique em **Nova tarefa** para adicionar tarefas ao projeto e atribuir recursos a elas.

   Para obter mais informações sobre como adicionar tarefas a um projeto, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Edite os detalhes do projeto clicando no menu **Mais** e em **Editar** ![](assets/qs-edit-icon.png) ao lado do nome do projeto.

   A caixa de diálogo **Editar Projeto** é aberta.

   Para obter mais informações sobre como editar um projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Opcional) Após definir as configurações do projeto e adicionar as tarefas, você pode alterar o status do projeto para **Atual**.

   Isso indica que o projeto agora está pronto para ser iniciado e os usuários atribuídos às tarefas agora podem começar a trabalhar nelas.

   Para obter mais informações sobre status de projeto, consulte [Acessar a lista de status de projeto do sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
