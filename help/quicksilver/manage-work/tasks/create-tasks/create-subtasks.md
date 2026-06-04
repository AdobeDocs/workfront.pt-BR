---
product-area: projects
navigation-topic: create-tasks
title: Criar Subtarefas
description: No Adobe Workfront, as tarefas podem ter relacionamentos pai-filho. Tarefas secundárias são chamadas de subtarefas. É possível criar subtarefas na lista de tarefas transformando uma tarefa principal em uma subtarefa. Também é possível transformar uma subtarefa em uma tarefa principal.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/FTIJQXYSmMiUcYnmU7wVnYJKBZxae8XhLcNlH-vxvZQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 580
ht-degree: 5%

---

# Criar subtarefas

<!-- Audited: 01/2025 -->

No Adobe Workfront, as tarefas podem ter relacionamentos pai-filho. Tarefas secundárias são chamadas de subtarefas. Você pode criar subtarefas na lista de tarefas tornando uma tarefa principal uma subtarefa de outra tarefa. Também é possível transformar uma subtarefa em uma tarefa principal.

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
   <p>Trabalho ou maior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões para o projeto com a capacidade de adicionar tarefas ou superior</p> 
   <p>Ao criar uma tarefa, você recebe automaticamente permissões Gerenciar para a tarefa</p> 
    </td> 
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
   <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project and the parent task with ability to Add Tasks or higher</p> <p>You automatically receive Manage permissions to the task after you create it.</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Criar subtarefas

É possível criar subtarefas a partir da lista de tarefas ou da seção de subtarefas de tarefas.

>[!TIP]
>
>A criação de subtarefas para um projeto é semelhante à criação de subtarefas de modelo para tarefas de modelo em um modelo.


### Criar subtarefas da lista de tarefas {#create-subtasks-from-the-task-list}

1. Vá para o projeto em que deseja criar subtarefas.
1. Clique na seção **Tarefas** no painel esquerdo.
1. (Condicional) Se a tarefa que você deseja tornar a tarefa filho ainda não estiver localizada diretamente abaixo da tarefa que você deseja tornar pai, arraste-a e solte-a no local apropriado na lista de tarefas.
1. Selecione a tarefa que você deseja transformar em uma subtarefa e siga um destes procedimentos:

   * Clique no ícone **Recuo** ![ícone de Recuo](assets/indent-icon-nwe-33x29.png) para transformar a tarefa selecionada em uma subtarefa da tarefa diretamente acima dela.
   * Ao usar um teclado QWERTY padrão em inglês, pressione Option + > (Mac) ou Alt + > (Windows) no teclado. Outras linguagens podem usar os comandos Option + , (Mac) ou Alt + , (Windows) para recuar.

     >[!TIP]
     >
     >Os atalhos de teclado não funcionam ao editar tarefas em edição em linha. Nesse caso, use o ícone Recuar ![ícone Recuar](assets/indent-icon-nwe-33x29.png) para criar subtarefas.

   * Arraste e solte a tarefa sobre a tarefa que deseja designar como a tarefa pai.

     >[!NOTE]
     >
     >Você pode recuar tarefas somente quando a lista de tarefas é classificada por Número da Tarefa e quando não há agrupamentos aplicados à lista de tarefas.

### Criar subtarefas a partir da seção Subtarefas de tarefa {#create-subtasks-from-the-task-subtasks-section}

>[!NOTE]
>
>O administrador do Workfront ou de grupo pode remover a seção Subtarefas do seu ambiente usando um modelo de layout.

1. Vá para o projeto em que deseja criar subtarefas.
1. Clique na seção **Tarefas** no painel esquerdo.
1. Clique no nome da tarefa em que deseja criar uma subtarefa.
1. Clique na seção **Subtarefas** no painel esquerdo, se disponível.
1. Clique em **Nova tarefa.**

   Para obter informações sobre como criar tarefas, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Clique em **Criar tarefa.**

   A nova tarefa é criada como uma subtarefa para a tarefa que você selecionou na etapa 3. <!--ensure this is accurate-->

## Transformar uma subtarefa em uma tarefa principal

1. Vá para o projeto em que deseja tornar uma subtarefa uma tarefa principal.
1. Clique na seção **Tarefas** no painel esquerdo.
1. Selecione a subtarefa que você deseja transformar em uma tarefa principal.
1. Clique no ícone **Diminuir recuo** ![Ícone Diminuir recuo](assets/outdent-icon-nwe-31x29.png) para tornar a subtarefa uma tarefa principal.

   Ou

   Em um teclado QWERTY padrão em inglês, pressione Option + &lt; (Mac) ou Alt + &lt; (Windows). Outras linguagens podem usar os comandos Option + . (Mac) ou Alt + . (Windows) para recuar para a esquerda.

   >[!NOTE]
   >
   >Você pode recuar tarefas para a esquerda somente quando a lista de tarefas é classificada por Número da Tarefa e quando não há agrupamentos aplicados à lista de tarefas.
