---
product-area: projects
navigation-topic: plan-a-project
title: Atualizar Proprietários e Patrocinadores do Projeto
description: Ao criar um projeto no Adobe Workfront, você é automaticamente definido como o Proprietário do projeto. Você pode atualizar este campo com outro usuário. Você também pode atualizar o campo Patrocinador do projeto de um projeto.
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YqTw5b0p4p605v7O0wVx99A7gLvJYF8xEPtthwW0CWc
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
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 433
ht-degree: 9%

---

# Atualizar proprietários e patrocinadores do projeto

<!--Audited: 07/2024-->

Ao criar um projeto no Adobe Workfront, você é automaticamente definido como o Proprietário do projeto. Você pode atualizar este campo com outro usuário. Você também pode atualizar o campo Patrocinador do projeto de um projeto.

Para obter informações sobre proprietários e patrocinadores de projetos, consulte [Visão geral dos proprietários e patrocinadores de projetos](../../../manage-work/projects/planning-a-project/project-owners-and-sponsors.md).

>[!TIP]
>
>É possível identificar um proprietário e um patrocinador de um modelo. Ao criar um projeto a partir desse modelo, o Proprietário do modelo se torna o Proprietário do projeto e o Patrocinador do modelo se torna o Patrocinador do projeto.
>
>Se o modelo não tiver um Proprietário, o usuário que cria o projeto a partir do modelo se torna o Proprietário do projeto.
>
>Para obter informações sobre como editar modelos, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Padrão</p> 
   <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Editar permissões para um projeto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit permissions to a project</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Atualizar o Proprietário de um projeto

Quando você adiciona um usuário como Proprietário de um projeto, o Workfront automaticamente oferece permissões para visualizar o projeto.

1. Vá para o projeto que deseja atualizar.
1. Clique em **Detalhes do projeto** no painel esquerdo.
1. Clique no ícone **Editar** ![Ícone Editar](assets/qs-edit-icon.png) no canto superior direito da área Detalhes do Projeto e clique em **Visão Geral**.

1. Especifique o nome de um usuário para o campo **Proprietário do Projeto**.

   Somente usuários ativos podem ser especificados como Proprietários do Projeto.

1. Clique em **Salvar alterações**.

   O Proprietário do projeto é atualizado no cabeçalho do projeto e na área Detalhes do projeto.

   ![O proprietário dos participantes do projeto destacou](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

## Atualizar o Patrocinador do Projeto de um Projeto

Ao adicionar um usuário como Patrocinador do projeto, o Workfront automaticamente fornece a ele permissões para exibir o projeto.

>[!TIP]
>
>Se o usuário adicionado como Patrocinador do projeto for um Administrador do sistema, ele não será adicionado à lista Compartilhamento do projeto.

1. Vá para o Projeto que deseja atualizar.
1. Clique em **Detalhes do projeto** no painel esquerdo.
1. Clique no ícone **Editar** ![Ícone Editar](assets/qs-edit-icon.png) no canto superior direito da área Detalhes do Projeto e clique em **Visão Geral**.

1. Especifique o nome de um usuário para o campo **Patrocinador do Projeto**.

   Somente usuários ativos podem ser especificados como Patrocinadores do Projeto.

1. Clique em **Salvar alterações**.

   O Patrocinador do projeto atualiza na área Detalhes do projeto.

   ![Destaque do patrocinador do projeto](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
