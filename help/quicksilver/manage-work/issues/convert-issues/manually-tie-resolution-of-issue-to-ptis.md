---
product-area: projects
navigation-topic: convert-issues
title: Vincular manualmente a resolução de um problema a outros problemas, tarefas ou projetos
description: Você pode vincular manualmente a resolução de um problema à resolução de um projeto, tarefa ou problema sem converter o problema. O problema se torna um dos Objetos Resolvíveis do projeto, tarefa ou problema selecionado. Quando você faz isso, uma alteração no status do projeto, tarefa ou problema aciona uma alteração no status do problema original.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/S3V5QxHwFzd8kOrPlU7wjmEt8IalZvpfgIv9iSgBYK4
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
source-wordcount: 518
ht-degree: 12%

---

# Vincular manualmente a resolução de um problema a outros problemas, tarefas ou projetos

<!--Audited: 08/2025-->

Você pode vincular manualmente a resolução de um problema à resolução de um projeto, tarefa ou problema sem converter o problema. O problema se torna um dos Objetos Resolvíveis do projeto, tarefa ou problema selecionado. Quando você faz isso, uma alteração no status do projeto, tarefa ou problema aciona uma alteração no status do problema original.

>[!TIP]
>
>Ao vincular a resolução de uma ocorrência à resolução de outro objeto, não é mais possível editar manualmente o status da ocorrência original.

Para obter mais informações sobre resolução e objetos resolvíveis, consulte [Visão Geral de Objetos Resolvíveis e Resolvíveis](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

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
   <td><p>Colaborador ou posterior</p> 
   <p>Solicitação ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a problemas, tarefas e projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões para o problema que você vincula a outro problema, tarefa ou projeto</p> <p>Visualize ou aumente as permissões para o problema, tarefa ou projeto que você adiciona ao problema existente</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue you link to another issue, task, or project</p> <p>View or higher permissions to the issue, task, or project you add to the existing issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Pré-requisitos

Antes de começar, você deve:

* Ter um problema cuja resolução você deseja vincular à resolução de outro problema, tarefa ou projeto

* Ter um problema, tarefa ou projeto adicional

## Vincular a resolução de um problema à resolução de outro problema, tarefa ou projeto

1. Navegue até uma ocorrência cuja resolução você deseja vincular à resolução de outra ocorrência ou à resolução de uma tarefa ou projeto.
1. Clique em **Detalhes do problema** no painel esquerdo e expanda a área **Visão geral**.

   ![Ícone de detalhes do problema](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Clique no campo **Resolvido por** e selecione um dos seguintes tipos de objetos de resolução:

   * **Projeto**
   * **Tarefa**
   * **Problema**

   Dependendo do objeto selecionado, os seguintes campos serão exibidos:

   * **Resolvendo Projeto**
   * **Resolvendo tarefa**
   * **Resolvendo problema**

1. Comece digitando o nome de um projeto, tarefa ou problema específico no campo **Resolvendo Projeto**, **Tarefa** ou **Problema**, e clique nele quando ele aparecer na lista.

   >[!NOTE]
   >
   >Não é possível vincular a resolução de um problema à tarefa ou ao projeto em que o problema está localizado. A tarefa ou o projeto do problema não são exibidos nos campos Resolving Task (Tarefa de resolução) ou Resolving Task (Tarefa de resolução).


1. Clique em **Salvar alterações**.

   O problema original torna-se o Objeto resolvível do projeto, tarefa ou problema selecionado nas etapas 4 e 5. Isso significa que o problema original é concluído quando o objeto de resolução (o projeto, a tarefa ou o problema ao qual você o vinculou) é concluído.

   >[!NOTE]
   >
   >Um projeto, tarefa ou problema pode ter vários problemas como Objetos resolvíveis.
