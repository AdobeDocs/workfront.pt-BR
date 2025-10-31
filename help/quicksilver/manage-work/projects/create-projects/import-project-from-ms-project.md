---
product-area: projects
navigation-topic: create-projects
title: Importar um projeto do Microsoft Project
description: Você pode importar projetos do Microsoft Project para o Adobe Workfront e gerenciar todos os seus projetos em um único aplicativo. Toda vez que você importa um projeto do Microsoft Project, um novo projeto é criado no Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 1%

---

# Importar um projeto do Microsoft Project

<!-- Audited: 10/2025 -->

Você pode importar projetos do Microsoft Project para o Adobe Workfront e gerenciar todos os seus projetos em um único aplicativo. Toda vez que você importa um projeto do Microsoft Project, um novo projeto é criado no Workfront.

>[!IMPORTANT]
>
>Nem todos os campos do Projeto do Microsoft são transferidos para o Workfront.
>
>Para obter mais informações sobre a compatibilidade de campos entre o Workfront e o Microsoft Project, consulte [Mapear campos do Microsoft Project para projetos do Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

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
    <p>Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuração do nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> 
   <p>Se você adicionar um projeto a um portfólio ou programa, deverá ter acesso para Editar a Portfólios e Programas.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Ao criar um projeto, você recebe automaticamente permissões de gerenciamento para o projeto</p>
   <p>Se você adicionar um projeto a um portfólio ou programa, deverá ter permissões de Gerenciamento para o portfólio e o programa.</p>
   </td> 
    </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--old permissions model: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Criar um projeto a partir de um MS Project

Você pode criar um projeto na área **Projetos** do **Menu Principal**, ou na área **Projetos** de um portfólio ou programa.

1. Faça logon no Microsoft Project e abra um projeto do qual deseja importar no Workfront.
1. Clique em **Arquivo**, depois em **Salvar como** para salvar o projeto como um arquivo .xml.

1. Faça logon no Workfront.
1. Siga um destes procedimentos:

   * Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo ou no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, se disponível, clique em **Projetos** e expanda **Novo Projeto**.
   * Vá para um portfólio e expanda **Novo projeto**.
   * Vá para um programa e expanda **Novo Projeto**.
   * Se você for um administrador de grupo, poderá criar um projeto na seção **Projetos** de um grupo que gerencia. Para obter mais informações, consulte [Criar e modificar projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Clique em **Importar projeto MS**.

   ![Lista suspensa de novos projetos](assets/import-ms-project-option.png)

   A caixa **Importar Arquivo MS** é aberta.

1. Clique em **Selecionar arquivo** e procure o arquivo .xml em seu computador que você exportou do Microsoft Project.
1. Importar o arquivo selecionado. O Workfront inicia o processo de importação e cria um novo projeto com base no arquivo exportado do Microsoft Project.

   Após a conclusão do processo de importação, você é direcionado para a nova página do projeto que exibe uma confirmação de que a importação foi concluída com êxito.

   >[!NOTE]
   >
   >O Workfront tem uma limitação de tempo de 15 minutos para uploads de arquivos. Se o upload do arquivo demorar mais que isso, recomendamos dividir o projeto em projetos menores e importá-los separadamente. Depois de importadas para o Workfront, mova as tarefas de um projeto para outro para combiná-las em um projeto. Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Opcional) Continue editando o projeto no Workfront. Para obter informações sobre como editar projetos, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).


   >[!NOTE]
   >
   >O status de um novo projeto criado a partir de um modelo corresponde ao status definido pelo administrador do Workfront na área **Preferências do projeto** ou por um administrador de grupo na área **Preferências do projeto do grupo**. Para obter informações sobre como configurar preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
