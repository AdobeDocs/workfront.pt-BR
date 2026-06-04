---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aplicar status a trabalhos associados a um grupo
description: Se um projeto estiver associado a um grupo, você poderá aplicar tanto status de nível de sistema quanto um status personalizado associado a esse grupo ao projeto, tarefa ou problemas nesse projeto.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/D6IbseeEu-prRZcdJNLvHvW-wSaclUAreufre9Fkyjo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 14%

---

# Aplicar status a trabalhos associados a grupos

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Se um projeto estiver associado a um grupo, você poderá aplicar tanto status de nível de sistema quanto um status personalizado associado a esse grupo ao projeto, ou tarefas e problemas nesse projeto. Para obter informações sobre status de grupo no Adobe Workfront, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

>[!TIP]
>
>Você pode associar somente projetos a grupos. Problemas e tarefas herdam o grupo do projeto ao qual pertencem.

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
   <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do projeto</p> </td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Atualizar Grupo e Status do Projeto

Quando você atualiza o Grupo de um projeto, as opções disponíveis para o Status de tarefas, problemas ou para o projeto são alteradas para corresponder ao grupo.

1. Vá para um projeto ou crie um novo projeto, conforme descrito em [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).
1. Clique no ícone **Mais** ícone ![Mais ícone](assets/more-icon.png) e em **Editar**.

1. Na caixa **Editar Projeto** que é exibida, próxima à parte inferior da seção **Visão Geral**, selecione o grupo no menu suspenso **Grupo**.

1. No menu suspenso **Status**, selecione o status personalizado.

   >[!NOTE]
   >
   >Se você selecionar um grupo diferente no menu suspenso **Grupo**, os status personalizados no menu **Status** serão alterados automaticamente para se correlacionarem com o novo grupo.
   >
   >
   >![Lista suspensa de status expandida com status personalizados para o projeto](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)
   >

1. Selecione o status do projeto. Os status personalizados criados e aplicados a esse grupo são exibidos na lista.
