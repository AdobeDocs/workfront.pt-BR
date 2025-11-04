---
product-area: templates
navigation-topic: templates-navigation-topic
title: Excluir modelos de projeto
description: Recomendamos desativar os modelos que não estão mais sendo usados, em vez de excluí-los para que você possa manter as informações de histórico sobre seus projetos ao longo do tempo.
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: 87bf2a4485d3b0c29fcfe8e00dcca57874cdec04
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Excluir modelos de projeto

Recomendamos desativar os modelos que não estão mais sendo usados, em vez de excluí-los para que você possa manter as informações de histórico sobre seus projetos ao longo do tempo. Para obter informações sobre como desativar um modelo, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>Quando você exclui um modelo, os projetos que estão usando esse modelo não são modificados de forma alguma. No entanto, você não pode mais ver o nome do modelo original no campo Modelo no projeto. Além disso, não é mais possível exibir os nomes das tarefas de modelo para as tarefas no projeto em uma exibição de tarefa. O campo Modelo do projeto e o campo Modelo de Tarefa das tarefas permanecem em branco após a exclusão do modelo originalmente associado ao projeto.

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
   <td><p>Standard</p> 
   <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso aos Modelos que incluem acesso a Excluir</p> <td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para o modelo que inclui permissões para excluí-lo</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

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
   <td> <p>Edit access to&nbsp;Templates that includes access to Delete</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the template that includes permissions to Delete it</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Considerações para exclusão de modelos

* As tarefas adicionadas aos projetos quando o modelo foi anexado permanecem nos projetos. No entanto, as informações da tarefa de modelo associadas às tarefas são excluídas.
* O nome do modelo não está mais listado no campo **Modelo** da subguia **Visão geral** do projeto.

* Você pode recuperar um modelo excluído recentemente da Lixeira. Para obter informações sobre como recuperar itens da Lixeira, consulte [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Excluir um modelo

{{step1-to-templates}}

Isso abre uma lista de modelos

1. Selecione o modelo que deseja excluir clicando na caixa de seleção à esquerda do nome do modelo e clique em **Excluir > Sim, Excluir** para confirmar a exclusão.

   Ou

   Clique no nome de um modelo para acessá-lo e no menu **Mais**, ícone ![Mais](assets/more-icon.png) e **Excluir modelo > Sim, excluí-lo**.

   O modelo não está mais disponível para ser associado a um projeto.
