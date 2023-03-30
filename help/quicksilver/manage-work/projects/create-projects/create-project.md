---
product-area: projects
navigation-topic: create-projects
title: Criar um Projeto
description: Um projeto é uma grande unidade de trabalho no Adobe Workfront. Você pode criar projetos do zero, usar um modelo ou converter problemas ou tarefas em projetos.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: 590fd9e5b9ad6cce9c66b708959033ee780b1f10
workflow-type: tm+mt
source-wordcount: '1206'
ht-degree: 1%

---

# Criar um Projeto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is linked from the UI from the Projects global nav section in classic. Do not change/ remove)</p>
-->

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

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a projetos, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Conceder acesso aos projetos</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Ao criar um projeto, você recebe automaticamente as permissões Gerenciar do projeto </p> <p> Para obter informações sobre permissões de projeto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Compartilhar um projeto no Adobe Workfront</a>.</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Maneiras de criar projetos

Você pode criar um projeto no Workfront usando um dos seguintes métodos:

* Crie um projeto do zero sem usar um modelo. Este artigo descreve como criar um projeto do zero.

* Copie um projeto existente.\
   Para obter mais informações sobre cópia do projeto, consulte [Copiar um projeto](../../../manage-work/projects/manage-projects/copy-project.md).

* Use um modelo.\
   Para obter mais informações sobre como usar um modelo para criar um novo projeto, consulte [Criar um projeto usando um modelo](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Importe um projeto do Microsoft Project.\
   Para obter mais informações sobre como importar um projeto do MS Project, consulte [Importar um projeto do Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importe um projeto usando o início.

   Como administrador do Workfront, você pode importar projetos usando um início.

   Para obter informações sobre como importar dados usando início no Workfront, consulte [Importar dados para o Adobe Workfront usando um modelo de Início rápido](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md) .

   Para obter informações sobre como importar projetos usando início, consulte [Cenário de início: preparação simples de importação de projeto e tarefa](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md) .

* Publique uma iniciativa de um cenário no Adobe Workfront Scenario Planner. O Planejador de Cenário requer uma licença adicional. Para obter informações sobre o Planejador de Cenário do Workfront, consulte [A visão geral do Planejador de cenário](../../../scenario-planner/scenario-planner-overview.md). Para obter informações sobre como criar projetos a partir da publicação de iniciativas, consulte  [Atualize ou crie projetos publicando iniciativas no Planejador de Cenários](../../../scenario-planner/publish-scenarios-update-projects.md).

## Pré-requisitos

Antes de começar, você deve garantir que

* Seu administrador de sistema ou grupo ativou a preferência &quot;Permitir que usuários criem projetos sem usar um modelo&quot; na área Configuração.

   Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Configurações padrão do novo projeto

Ao criar um projeto, o Workfront aplica um conjunto de configurações padrão a ele. Por exemplo, o Status, o Grupo ou o Modo de agendamento são predefinidos quando você cria um projeto.

Considere o seguinte:

* Como administrador do Workfront ou administrador de grupo, você pode definir as configurações padrão de um novo projeto ao definir Preferências do projeto.
* A Workfront aplica as configurações do grupo, se houver, antes de aplicar as configurações definidas pelo administrador do Workfront.
* Se você criar um projeto usando um modelo, as configurações do modelo terão prioridade sobre as configurações estabelecidas pelo administrador do grupo ou da Workfront.

   >[!NOTE]
   >
   >Recomendamos que o status padrão de um novo projeto seja Planejamento. À medida que você faz alterações no novo projeto, isso garante que as notificações não sejam acionadas para os usuários atribuídos ao projeto.
   >
   >Para obter mais informações sobre como configurar o status padrão e outras configurações padrão para um novo projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* O Workfront define o Grupo e o Status do novo projeto da seguinte maneira:

   * O status padrão de um novo projeto criado a partir de um modelo corresponde ao status definido pelo administrador do Workfront na área principal Preferências do projeto ou por um administrador de grupo (ou administrador do Workfront) na área Preferências do projeto de um grupo.

   * O Grupo do novo projeto é o Grupo do modelo. Se o modelo não estiver associado a um Grupo, o Grupo do projeto será o Grupo Doméstico do usuário que cria o projeto.

   * Os status disponíveis para um novo projeto correspondem aos status do Grupo do projeto, que é o Grupo do modelo, ou o Grupo inicial do usuário que cria o projeto.

   * O grupo de um novo projeto criado pela conversão de um problema em um projeto é o Grupo do projeto existente do problema. Se o usuário que está convertendo o problema não tiver acesso ao projeto do problema, o Grupo do novo projeto será o Grupo Doméstico do usuário que está convertendo o problema. Os status do novo projeto correspondem aos status do grupo associado ao projeto, que é o Grupo do projeto original ou o Grupo inicial do usuário que está convertendo o problema.

## Criar um projeto do zero

1. Siga um destes procedimentos:

   * Clique no botão **Menu principal** ![](assets/main-menu-icon.png), clique em **Projetos**, em seguida expanda **Novo projeto**.
   * Vá para um portfólio e expanda **Novo projeto**.

      >[!TIP]
      >
      >Ao criar um projeto usando um modelo de um portfólio, o campo Portfolio do novo projeto é atualizado para exibir o portfólio do qual você escolheu criar o projeto. Isso substitui o campo Portfolio no template, se ele for especificado.

   * Vá para um programa e expanda **Novo projeto**.

      >[!TIP]
      >
      >Ao criar um projeto usando um modelo de um programa, o campo Programa dos novos projetos é atualizado para exibir o Programa do qual você escolheu criar o projeto. O campo Portfolio do template é atualizado para exibir o portfólio do programa escolhido para criar o projeto. Isso substitui os campos Programa e Portfolio no modelo, se forem especificados.

   * Se você for um administrador de grupo, também poderá criar um projeto na seção Projetos de um grupo que você gerencia. Para obter mais informações, consulte [Criar e modificar projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

      >[!TIP]
      >
      >Quando você cria um projeto usando um modelo de um grupo, o grupo a partir do qual você cria o projeto é exibido no campo Grupo do novo projeto somente quando o campo Grupo do modelo não é especificado. Se o campo Grupo de modelo for especificado, o campo Grupo do novo projeto será o do modelo.
   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Clique em **Novo projeto** se quiser criar um projeto do zero.
1. Insira um nome para o projeto. Pressione Enter para salvar o nome.

   ![](assets/untitled-project-rename-new-project-nwe-350x127.png)

   O cabeçalho da página do projeto exibe uma visão geral rápida da integridade e do progresso atuais de um projeto. As informações no cabeçalho do projeto são alteradas à medida que as informações do projeto são atualizadas.

1. Clique em **Comece a adicionar** **Tarefas**.

   Ou

   Clique em **Nova tarefa** para adicionar tarefas ao projeto e atribuir recursos a elas.\
   Para obter mais informações sobre como adicionar tarefas a um projeto, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Edite os detalhes do projeto clicando no botão **Menu Mais** e depois **Editar** ![](assets/qs-edit-icon.png) ao lado do nome do projeto.

   O **Editar projeto** será aberta.

   Para obter mais informações sobre como editar um projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Opcional) Após definir as configurações do projeto e adicionar as tarefas, você pode alterar o status do projeto para **Atual**.

   Isso indica que o projeto agora está pronto para iniciar e que os usuários atribuídos às tarefas agora podem começar a trabalhar nelas.

   Para obter mais informações sobre os status do projeto, consulte [Acessar a lista de status de projeto do sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
