---
product-area: projects
navigation-topic: create-tasks
title: Criar Subtarefas
description: No Adobe Workfront, as tarefas podem ter relacionamentos pai-filho. Tarefas secundárias são chamadas de subtarefas. É possível criar subtarefas na lista de tarefas transformando uma tarefa principal em uma subtarefa. Também é possível transformar uma subtarefa em uma tarefa principal.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Criar subtarefas

<!-- Audited: 01/2025 -->

No Adobe Workfront, as tarefas podem ter relacionamentos pai-filho. Tarefas secundárias são chamadas de subtarefas. É possível criar subtarefas na lista de tarefas transformando uma tarefa principal em uma subtarefa. Também é possível transformar uma subtarefa em uma tarefa principal.

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
   <td> <p>Standard</p> 
   <p>Trabalhar ou superior</p> </td> 
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

<!--Old:

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
</table>-->

## Criar subtarefas

É possível criar subtarefas a partir da lista de tarefas ou da seção de subtarefas de tarefas.

### Criar subtarefas da lista de tarefas {#create-subtasks-from-the-task-list}

1. Vá para o projeto em que deseja criar subtarefas.
1. Clique na seção **Tarefas** no painel esquerdo.
1. (Condicional) Se a tarefa que você deseja tornar a tarefa filho ainda não estiver localizada diretamente abaixo da tarefa que você deseja tornar pai, arraste-a e solte-a no local apropriado na lista de tarefas.
1. Selecione a tarefa que você deseja transformar em uma subtarefa e siga um destes procedimentos:

   * Clique no ícone **Recuo** ![](assets/indent-icon-nwe-33x29.png) para tornar a tarefa selecionada uma subtarefa da tarefa diretamente acima dela.
   * Ao usar um teclado QWERTY padrão em inglês, pressione Option + > (Mac) ou Alt + > (Windows) no teclado. Outras linguagens podem usar os comandos Option + , (Mac) ou Alt + , (Windows) para recuar.

     >[!TIP]
     >
     >Os atalhos de teclado não funcionam ao editar tarefas em edição em linha. Nesse caso, use o ícone de Recuo ![](assets/indent-icon-nwe-33x29.png) para criar subtarefas.

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
1. Clique na seção **Subtarefas** no painel esquerdo, se presente.
1. Clique em **Nova tarefa.**

   Siga as etapas no artigo a seguir para continuar criando a subtarefa: [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Clique em **Criar tarefa.**

## Transformar uma subtarefa em uma tarefa principal

1. Vá para o projeto em que deseja tornar uma subtarefa uma tarefa principal.
1. Clique na seção **Tarefas** no painel esquerdo.
1. Selecione a subtarefa que você deseja transformar em uma tarefa principal.
1. Clique no ícone **Diminuir recuo** ![](assets/outdent-icon-nwe-31x29.png) para tornar a subtarefa uma tarefa principal.

   Ou

   Em um teclado QWERTY padrão em inglês, pressione Option + &lt; (Mac) ou Alt + &lt; (Windows). Outras linguagens podem usar os comandos Option + . (Mac) ou Alt + . (Windows) para recuar para a esquerda.

   >[!NOTE]
   >
   >Você pode recuar tarefas para a esquerda somente quando a lista de tarefas é classificada por Número da Tarefa e quando não há agrupamentos aplicados à lista de tarefas.
