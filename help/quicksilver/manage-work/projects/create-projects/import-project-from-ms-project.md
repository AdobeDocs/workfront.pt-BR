---
product-area: projects
navigation-topic: create-projects
title: Importar um projeto do Microsoft Project
description: Você pode importar projetos do Microsoft Project para o Adobe Workfront e gerenciar todos os seus projetos em um único aplicativo. Toda vez que você importa um projeto do Microsoft Project, um novo projeto é criado no Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/drxvgi-xQLjEt5JOL6-MxLdkmVcXxkcXMN14nwmNZvs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 604
ht-degree: 9%

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

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

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
   <td> <p>Padrão</p> 
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

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
old permissions model: 

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

1. Faça login no Workfront.
1. Siga um destes procedimentos:

   * Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e, em seguida, clique em **Projetos** e expanda **Novo Projeto**.
   * Vá para um portfólio e expanda **Novo projeto**.
   * Vá para um programa e expanda **Novo Projeto**.
   * Se você for um administrador de grupo, poderá criar um projeto na seção **Projetos** de um grupo que gerencia. Para obter mais informações, consulte [Criar e modificar projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Clique em **Importar projeto MS**.

   ![Lista suspensa de novos projetos](assets/import-ms-project-option.png)

   A caixa **Importar Arquivo MS** é aberta.

1. Clique em **Selecionar arquivo** e procure o arquivo .xml em seu computador que você exportou do Microsoft Project.
1. Importar o arquivo selecionado. O Workfront inicia o processo de importação e cria um novo projeto com base no arquivo exportado do Microsoft Project.

   >[!NOTE]
   >
   >O Workfront tem uma limitação de tempo de 15 minutos para uploads de arquivos. Se o upload do arquivo demorar mais que isso, recomendamos dividir o projeto em projetos menores e importá-los separadamente. Depois de importadas para o Workfront, mova as tarefas de um projeto para outro para combiná-las em um projeto. Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

   Após a conclusão do processo de importação, você é direcionado para a nova página do projeto que exibe uma confirmação de que a importação foi concluída com êxito.

   >[!CAUTION]
   >
   >Se sua instância do Workfront tiver acesso ao armazenamento em nuvem do Workfront e do Adobe para documentos, importar um projeto do MS Project criará um projeto de armazenamento herdado do Workfront, mesmo quando o administrador do Workfront tiver tornado o armazenamento em nuvem do Adobe o padrão para o seu sistema.
   >
   >Para obter mais informações, consulte [Visão geral do gerenciamento de documentos para projetos e objetos relacionados](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).


1. (Opcional) Continue editando o projeto no Workfront. Para obter informações sobre como editar projetos, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).


   >[!NOTE]
   >
   >O status de um novo projeto criado a partir de um modelo corresponde ao status definido pelo administrador do Workfront na área **Preferências do projeto** ou por um administrador de grupo na área **Preferências do projeto do grupo**. Para obter informações sobre como configurar preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
