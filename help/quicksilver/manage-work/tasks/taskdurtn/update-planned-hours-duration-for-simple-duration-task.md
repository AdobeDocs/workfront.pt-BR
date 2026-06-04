---
product-area: projects
navigation-topic: task-duration
title: Atualizar as horas planejadas e a duração de uma tarefa com um tipo de duração simples
description: Por padrão, o Adobe Workfront calcula a Duração de uma tarefa com um Tipo de duração simples com base na quantidade de Horas planejadas. No entanto, você também pode editar manualmente a quantidade de Horas planejadas e a duração de uma tarefa de Duração simples em determinadas áreas do Workfront.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/SLemiOnFj-dOnWtXjH6gNzHZdVaXfp47qB0xzVJkRck
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 450
ht-degree: 14%

---

# Atualizar as horas planejadas e a duração de uma tarefa com um tipo de duração simples

Por padrão, o Adobe Workfront calcula a Duração de uma tarefa com um Tipo de duração simples com base na quantidade de Horas planejadas. No entanto, você também pode editar manualmente a quantidade de Horas planejadas e a duração de uma tarefa de Duração simples em determinadas áreas do Workfront.

Você pode editar as Horas planejadas e a Duração de uma tarefa com um Tipo de duração simples em linha ou no nível da tarefa na área Atribuições.

Para obter mais informações sobre como editar informações em linha, consulte [Itens de edição em linha em uma lista no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

Este artigo descreve como você pode atualizar as Horas planejadas e a Duração de uma tarefa com um Tipo de Duração simples no nível da tarefa, na área Atribuições.

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
   <td><p>Padrão ou superior</p> 
   <p>Trabalho ou maior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de visualização ou superior aos Projetos</p> <p>Editar acesso a tarefas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar acesso à tarefa </p></td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Atualizar as horas planejadas e a duração de uma tarefa com um tipo de duração simples

>[!IMPORTANT]
>
>Depois de atualizar manualmente a Duração em uma tarefa de Duração simples, o Workfront para de calculá-la com base nas Horas planejadas.

Para editar as Horas Planejadas e a Duração de uma tarefa com um Tipo de Duração Simples na caixa Atribuições Avançadas:

1. Em uma lista de tarefas, clique no nome da tarefa para a qual deseja alterar o tipo de duração.
1. Siga um destes procedimentos:

   * Clique no ícone **Mais** ícone ![Mais em um objeto](assets/qs-more-icon-on-an-object.png) ao lado do nome da tarefa, clique em **Editar** e depois em **Atribuições**.
   * Clique em **Atribuído a** ou no nome das atribuições na área Atribuições do cabeçalho da tarefa e clique em **Avançado**.

1. Insira um valor total para as **Horas Planejadas** para todas as atribuições, por exemplo, 10 horas. O número total de Horas Planejadas é distribuído igualmente entre todos os recursos atribuídos à tarefa.
1. (Opcional) Ajuste manualmente as Horas Planejadas de cada recurso atribuído à tarefa. O número total de Horas Planejadas para que a tarefa seja atualizada para refletir as novas horas atribuídas individualmente aos seus recursos.
1. Insira um valor para a tarefa **Duração**, por exemplo, 2 Dias.

   ![Múltiplos recursos de duração simples de atribuições avançadas](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Clique em **Salvar**.
