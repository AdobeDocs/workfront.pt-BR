---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aplicar status ao trabalho associado a um grupo
description: Se um projeto estiver associado a um grupo, você poderá aplicar ambos os status do sistema, bem como um status personalizado associado a esse grupo ao projeto, tarefa ou problemas nesse projeto.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# Aplicar status ao trabalho associado a um grupo

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Se um projeto estiver associado a um grupo, você poderá aplicar ambos os status do sistema, bem como um status personalizado associado a esse grupo ao projeto, ou tarefas e problemas nesse projeto. Para obter informações sobre status de grupo no Adobe Workfront, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

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

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Atualizar grupo de projetos e status

Quando você atualiza o Grupo de um projeto, as opções disponíveis para o Status de tarefas, problemas ou a alteração do projeto são alteradas para corresponder ao grupo.

1. Vá para um projeto ou crie um novo projeto, conforme descrito em [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).
1. Clique no botão **Mais** ícone ![](assets/more-icon.png), depois clique em **Editar**.

1. No **Editar projeto** caixa exibida, perto da parte inferior da **Visão geral** selecione o grupo na seção **Grupo** menu suspenso.

1. No **Status** selecione o status personalizado no menu suspenso.

   >[!NOTE]
   >
   >Se você selecionar um grupo diferente na variável **Grupo** no menu suspenso, os status personalizados na **Status** alteração de menu automaticamente para correlacionar com o novo grupo.
   >
   >
   >![](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)   >

1. Selecione o status do projeto. Os status personalizados criados e aplicados a esse grupo são exibidos na lista.
