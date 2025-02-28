---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aplicar status a trabalhos associados a grupos
description: Se um projeto estiver associado a um grupo, você poderá aplicar tanto status de nível de sistema quanto um status personalizado associado a esse grupo ao projeto, tarefa ou problemas nesse projeto.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

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

<!--drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
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

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

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
   >![](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)   >
   >

1. Selecione o status do projeto. Os status personalizados criados e aplicados a esse grupo são exibidos na lista.
