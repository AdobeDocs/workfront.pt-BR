---
product-area: projects;templates
navigation-topic: create-projects
title: Criar um projeto usando um modelo
description: Você pode usar modelos como uma estrutura para criar projetos no Adobe Workfront. Se você tiver projetos que se repetem com frequência, usar modelos para a linha do tempo geral do novo projeto evita que você tenha que criar os mesmos projetos repetidamente.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: 9447310f0d4cf4504ee6d690116fb62f718fe23d
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 0%

---

# Criar um projeto usando um modelo

<!-- Audited: 01/2024 -->

Você pode usar modelos como uma estrutura para criar projetos no Adobe Workfront. Se você tiver projetos que se repetem com frequência, usar modelos para a linha do tempo geral do novo projeto evita que você tenha que criar os mesmos projetos repetidamente.

Os modelos fornecem uma maneira de capturar processos, informações e configurações repetíveis associados aos seus projetos. As informações associadas a um modelo são transferidas para o projeto. Isso inclui tarefas, atribuições, durações, documentos, detalhes financeiros, riscos e formulários personalizados.

>[!TIP]
>
>O Workfront define o Grupo e o Status do novo projeto da seguinte maneira:
>
>* O status padrão de um novo projeto criado a partir de um modelo corresponde ao status definido pelo administrador do Workfront na área principal Preferências do projeto, ou por um administrador de grupo (ou administrador do Workfront) na área Preferências do projeto de um grupo. Para obter informações sobre como configurar as preferências do projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Configurar as preferências do projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* O Grupo do novo projeto é o Grupo do modelo. Se o modelo não estiver associado a um Grupo, o Grupo do projeto será o Grupo inicial do usuário que cria o projeto.
>
>* Os status disponíveis para um novo projeto correspondem aos status do Grupo do projeto, que é o Grupo do modelo ou o Grupo inicial do usuário que cria o projeto.

Você tem as seguintes opções para criar um projeto a partir de um modelo:

* Crie um projeto com base em um modelo na área Projetos
* Criar um projeto a partir de um modelo no nível do modelo
* Anexar um modelo a um projeto existente

  Para obter informações, consulte [Anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Crie um projeto com base em um modelo na área Grupos

## Requisitos de acesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Workfront</td> 
   <td> <p>Novo: Padrão</p>
        <p>ou</p>
        <p>Atual: Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos e modelos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para um modelo</p> <p>Ao criar um projeto, você recebe automaticamente permissões de gerenciamento para o projeto.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Crie um projeto com base em um modelo na área Projetos

Você pode criar um projeto na área Projetos do menu principal ou na área Projetos de um portfólio ou programa.

1. Siga um destes procedimentos:

   * Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo. Clique em **Projetos**, em seguida, expandir **Novo projeto**.
   * Acesse um portfólio e expanda **Novo projeto**.

     >[!TIP]
     >
     >Ao criar um projeto usando um modelo de um portfólio, o campo Portfolio do novo projeto é atualizado para exibir o portfólio escolhido para criar o projeto. Isso substitui o campo Portfolio no modelo, se for especificado.

   * Ir para um programa e expandir **Novo projeto**.

     >[!TIP]
     >
     >Ao criar um projeto usando um modelo de um programa, o campo Programa dos novos projetos é atualizado para exibir o Programa escolhido para criar o projeto. O campo Portfolio das atualizações de modelo para exibir o portfólio do programa escolhido para criar o projeto. Isso substitui os campos Program e Portfolio no modelo, se forem especificados.

   * Se você for um administrador de grupo, também poderá criar um projeto na seção Projetos de um grupo gerenciado. Para obter mais informações, consulte [Criar e modificar os projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >Ao criar um projeto usando um modelo de um grupo, o grupo do qual você cria o projeto é exibido no campo Grupo do novo projeto somente quando o campo Grupo do modelo não é especificado. Se o campo Grupo do modelo for especificado, o campo Grupo do novo projeto será o do modelo.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![Novas opções de projeto](assets/new-project-dropdown.png)

1. Clique no nome de um modelo na **Modelos favoritos** lista.

   ![Selecionar um modelo favorito](assets/new-project-from-template-dropdown-with-template-favorites.png)

   Ou

   Faça o seguinte:

   1. Selecionar **Novo projeto do modelo**.
   1. No **Procurar Modelos** digite o nome de um template e clique nele quando ele for exibido na lista.
   1. Revise os detalhes do modelo à direita.

      Os detalhes do template incluem o seguinte:

      * Duração do modelo
      * Proprietário do modelo
      * O número de tarefas de nível superior, que inclui os nomes das três principais tarefas
      * O número de todas as tarefas no modelo
      * Os nomes dos formulários personalizados do modelo

   1. (Opcional) Passe o mouse sobre o nome de um modelo no painel esquerdo e clique no **Favoritos** **ícone** ![](assets/favorites-icon-small.png) para marcá-la como favorita para uso futuro.

      Ou

      Expanda a **Modelos favoritos** e selecione um template na lista suspensa.

      >[!TIP]
      >
      >É possível marcar até 40 itens do Workfront como favoritos. Isso inclui modelos e outros itens.

   1. Clique em **Usar modelo** quando você seleciona um template.

      ![Detalhes do modelo](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >Se você tiver a visualização Marco aplicada à lista de projetos, clique no nome de um modelo na **Novo na seção Modelo**.
      >
      >
      >![Exibição de marco da criação de um projeto a partir de um modelo](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   A variável **Novo projeto** é aberta.

   ![Caixa Novo projeto](assets/new-project-from-template-box.png)

1. Se um campo já estiver preenchido no modelo, ele será preenchido previamente na variável **Novo projeto** caixa. É possível editar os valores pré-preenchidos para melhor corresponder ao seu projeto. Para obter mais informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Clique em **Criar projeto**.

   Todos os detalhes definidos no modelo são associados automaticamente ao projeto recém-criado se você não os alterou na etapa anterior.

## Crie um projeto a partir de um modelo na área Modelos

Em vez de começar na área Projetos, você pode criar um projeto a partir de um modelo começando pelo modelo.

{{step1-to-templates}}

1. Clique no nome de um modelo que deseja usar.
1. Clique em **Mais** menu ![](assets/more-icon.png)e, em seguida, clique em **Criar projeto**.

   ![Criar projeto a partir de modelo](assets/project-sharing-on-template.png)

   A variável **Novo projeto** é aberta.

1. Insira um nome para o projeto, revise cada seção e faça as alterações necessárias.

   ![Caixa Novo projeto](assets/new-project-from-template-box.png)

   Se um campo já estiver preenchido no modelo, ele será preenchido previamente na variável **Novo projeto** caixa. É possível editar os valores pré-preenchidos para melhor corresponder ao seu projeto. Para obter mais informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Clique em **Criar projeto**.

   Todos os detalhes definidos no modelo são associados automaticamente ao projeto recém-criado se você não os alterou na etapa anterior.
