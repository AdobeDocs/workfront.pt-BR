---
product-area: projects
navigation-topic: manage-projects
title: Exportar um projeto para o Microsoft Project
description: Você pode exportar projetos do Adobe Workfront para o Microsoft Project.
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Exportar um projeto para o Microsoft Project

Você pode exportar projetos do Adobe Workfront para o Microsoft Project. 

>[!IMPORTANT]
>
>* Nem todos os campos do Workfront são transferidos no arquivo de projeto do Microsoft.\
>  Para obter mais informações sobre a compatibilidade de campos entre o Workfront e o Microsoft Project, consulte o artigo [Mapear campos do Microsoft Project para projetos do Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).
>* Recomendamos que você limite o número de vezes que transfere projetos de um aplicativo para outro. 
>

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
   <td>  <p>Current license: Light or higher</p>
   Or
   <p>Legacy license: Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso de visualização ou superior aos Projetos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre acesso a projetos, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Conceder acesso a projetos</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Visualizar ou aumentar as permissões do projeto</p> <p>Para obter informações sobre permissões de projeto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Compartilhar um projeto no Adobe Workfront</a>.</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Exportar um projeto do Workfront para o Microsoft Project

Você pode exportar um projeto do Workfront da página do projeto ou de uma lista de projetos ou relatório.

1. Vá para o projeto que deseja exportar e clique no ícone **Mais**, ![Mais menu](assets/qs-more-menu.png) à direita do nome do projeto

   ![Mais lista suspensa](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Ou

   Vá para uma lista de projetos ou relatório, selecione um projeto e clique no ícone Mais ![menu Mais](assets/qs-more-menu.png) na parte superior da lista.

   ![Mais menus expandidos](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Clique em **Exportar projeto MS**.

   O projeto é baixado como um arquivo XML no computador e está pronto para ser importado para o Microsoft Project. 
