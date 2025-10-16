---
product-area: projects
navigation-topic: manage-tasks
title: Associar Etapas a Tarefas
description: Você pode associar marcos a tarefas para indicar quando atinge etapas importantes na vida útil do projeto. Você deve associar um caminho de etapas a um projeto antes de associar etapas a tarefas no projeto.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 1%

---

# Associar marcos a tarefas

<!--Audited: 01/2024-->

Você pode associar marcos a tarefas para indicar quando atinge etapas importantes na vida útil do projeto.

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
   <p>Trabalhar ou superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para a tarefa</p></td> 
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
   <td> <p>New license: Standard</p> 
   <p>Current license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Pré-requisitos

Antes de associar uma etapa a uma tarefa, é necessário que haja o seguinte:

* O administrador do Workfront deve criar um caminho de etapas, conforme descrito em [Criar um caminho de etapas](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Você deve associar um Caminho de Etapas a um projeto.

  Para obter informações, consulte [Editar projetos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* Para associar um caminho de etapas a um projeto, o projeto deve estar no status Planejamento ou Atual.

  >[!TIP]
  >
  >Para obter a melhor visão geral do progresso dos marcos em seus projetos usando a visualização Marco, você deve criar tarefas pai e associá-las a cada fase principal do seu projeto. Em seguida, associe essas tarefas pai a cada um dos marcos do caminho de marcos.

## Associar uma etapa a uma tarefa

Depois que um caminho de marcos é associado a um projeto, as tarefas podem ser atribuídas a um marco.

1. Vá para uma tarefa e clique no ícone **Mais** ![](assets/more-icon.png) à direita do nome da tarefa e **Editar**.

   Tarefas e Etapas têm uma relação 1:1. Não é possível anexar o mesmo marco a várias tarefas. Cada tarefa pode ser vinculada a um único marco ou cada marco pode ser mapeado para uma tarefa.

1. Clique em **Configurações** e selecione uma etapa no campo **Etapa** da tarefa.
1. Clique em **Salvar**.
1. (Opcional) Em uma lista de tarefas, adicione a coluna **Ícones de Status** para identificar quais tarefas têm marcos. O indicador de diamante de etapas é exibido na coluna Ícones de status.

   Para obter informações, consulte [Criar ou editar exibições no Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

   ![](assets/amwt3.png)

1. (Opcional) Vá para uma lista de projetos, selecione a visualização **Marco** para identificar o progresso de suas tarefas de marco.

   ![](assets/milestone-view-project-list.png)
