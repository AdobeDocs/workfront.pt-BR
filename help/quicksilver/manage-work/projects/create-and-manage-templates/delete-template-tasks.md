---
product-area: templates
keywords: tarefa,padrões,automatizar,criação
navigation-topic: templates-navigation-topic
title: Excluir um Modelo de Tarefa
description: É possível excluir um modelo de tarefa se ele não for mais necessário. Tarefas de modelo excluídas não podem ser recuperadas. Tarefas de projeto criadas a partir da tarefa de modelo não são excluídas ou modificadas.
author: Alina
feature: Work Management
exl-id: dd733e9f-8045-4b65-828b-fe6aa40d973f
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/G4OdOAGqiLA0PNUADG9ONsN9Dc2euNHQQGCYXK6ohvA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 285
ht-degree: 12%

---

# Excluir uma tarefa de modelo

É possível excluir um modelo de tarefa se ele não for mais necessário. Tarefas de projeto criadas a partir da tarefa de modelo não são excluídas ou modificadas.

>[!NOTE]
>
>Tarefas de modelo excluídas e suas informações adicionais (atribuições, documentos, aprovações) não podem ser recuperadas. Você pode recuperar um modelo que também recupera todas as tarefas no modelo. Se você excluir as tarefas de modelo (e não o modelo), nunca poderá recuperá-las.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td> <p>Padrão</p>
   <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Editar acesso a modelos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p> </td> 
   <td> <p>Gerenciar permissões de um modelo.</p> <p>Não é possível compartilhar uma tarefa de modelo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Standard </p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level</p></td> 
   <td> <p>Edit access to Templates</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p> </td> 
   <td> <p>Manage permissions for a template.</p> <p>You cannot share a template task.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Excluir uma tarefa de modelo

É possível excluir uma ou várias tarefas de modelo em massa.

{{step1-to-templates}}

1. Clique no nome de um template para abri-lo.
1. Clique em **Tarefas de modelo** no painel esquerdo.
1. Siga um destes procedimentos:
   * Clique no nome de uma tarefa de modelo na lista para abrir a tarefa de modelo > clique no menu **Mais** ![Mais menu](assets/more-icon.png) > **Excluir Tarefa de Modelo**.
   * Selecione uma ou várias tarefas de modelo na lista > **Excluir** ícone ![Excluir ícone](assets/delete.png).

   A caixa **Excluir Tarefa de Modelo** é aberta.
1. Clique em **Sim, exclua-o** para confirmar.

   As tarefas de modelo são excluídas e não podem ser recuperadas.

>[!TIP]
>
>Você pode clicar nas seções Predecessores ou Subtarefas no painel esquerdo de uma tarefa de modelo para excluir um predecessor ou uma subtarefa.
>
>Repita as etapas acima para excluir tarefas de modelo predecessoras ou subtarefas.
