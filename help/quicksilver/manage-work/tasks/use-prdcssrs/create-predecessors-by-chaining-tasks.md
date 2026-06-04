---
product-area: projects
navigation-topic: use-predecessors
title: Criar Relacionamentos Predecessores por Encadeamento de Tarefas
description: Você pode criar relações de predecessoras de várias maneiras no Adobe Workfront. Um método é encadear tarefas.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/iHJkCABzPdAjLYSlUTtXyBvQzU7eney-daOuvhXLbPQ
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
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 288
ht-degree: 11%

---

# Criar relações de predecessores por encadeamento de tarefas

Você pode criar relações de predecessoras de várias maneiras no Adobe Workfront. Um método é encadear tarefas.

Para obter informações sobre tarefas predecessoras, consulte [Visão geral das predecessoras da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Ao encadear tarefas, você pode permitir que o sistema crie os relacionamentos de predecessora automaticamente em tarefas selecionadas, em vez de criar manualmente um relacionamento em cada tarefa. Ainda é possível usar diferentes tipos de relações de predecessoras entre tarefas.

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
   <td><p>Padrão</p> 
   <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e o projeto</p></td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Encadear tarefas para criar relacionamentos predecessores

1. Vá para o projeto que contém as tarefas que você deseja encadear.
1. Clique em **Tarefas** no painel esquerdo.
1. (Condicional) Selecione **Salvar automaticamente** no canto superior direito da lista de tarefas e selecione as tarefas que deseja encadear.

   ![Ícone de salvamento automático em realçado](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >Não é possível encadear tarefas em uma lista de tarefas quando você salva manualmente as alterações em tarefas ou usa o modo de Planejamento de linha do tempo para salvar tarefas.

1. Clique com o botão direito do mouse nas tarefas selecionadas e clique em **Cadeia**.
1. Selecione um dos seguintes tipos de dependência:

   * **Término-Início**
   * **Término-Término**
   * **Início-Início**
   * **Início-Término**

   Para obter mais informações sobre tipos de dependência predecessora, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Opcional) Clique em **Desencadear** se algumas das tarefas tiverem sido encadeadas anteriormente.

   >[!CAUTION]
   >
   >Somente predecessores sequenciais são removidos usando a opção unchain ao editar tarefas em massa.

   Suas tarefas selecionadas agora estão vinculadas por relacionamentos de predecessores.
