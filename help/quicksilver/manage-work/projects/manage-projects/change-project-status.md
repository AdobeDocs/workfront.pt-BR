---
product-area: projects
navigation-topic: manage-projects
title: Alterar o status de um projeto
description: Você pode atualizar manualmente o status de um projeto para qualquer outro status, se necessário. Você pode atualizar manualmente o status de um projeto para um status que equivale a Concluído somente quando o Modo de conclusão do projeto estiver definido como Manual.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/PRLph0Euqn69SUFkRMT1N7BmJinnao-xfzMWWEE407Q
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 358
ht-degree: 9%

---

# Alterar o status de um projeto

<!--Audited: 02/2024-->

Você pode atualizar manualmente o status de um projeto para qualquer outro status, se necessário.

Você pode atualizar manualmente o status de um projeto para um status que equivale a Concluído somente quando o Modo de conclusão do projeto estiver definido como Manual.

Caso contrário, o Adobe Workfront marcará automaticamente o projeto como Concluído quando todas as tarefas e problemas do projeto forem concluídas e aprovadas.

Para obter mais informações sobre o Modo de conclusão do projeto, consulte [Editar projetos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

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
   <p>Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no projeto</p> </td> 
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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Considerações sobre a atualização para status específicos

* **Ao atualizar um projeto para Concluído:** Verifique se todas as tarefas e problemas foram concluídos no projeto. Você não pode selecionar o status Concluído para um projeto, ou qualquer outro status que seja igual a Concluído quando houver tarefas ou problemas que não foram concluídos no projeto. Isso inclui a aprovação de qualquer tarefa ou problema que esteja com o status Concluído Pendente de Aprovação.
* **Ao atualizar um projeto de Concluído para Atual:** Se todas as tarefas e problemas do projeto forem concluídos, verifique se o Modo de Conclusão do projeto está definido como Manual. Se o Modo de conclusão do projeto for Automático, o status do projeto permanecerá como Concluído.

## Alterar status do projeto

1. Vá para o projeto cujo status você deseja atualizar.
1. No cabeçalho do projeto, clique no nome do status no campo **Status** e selecione um novo status.

   ![Alterar status do projeto](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   Ou

   Clique no menu **Mais** ![Mais menu](assets/qs-more-menu.png) ao lado do nome do projeto e clique em **Editar**, selecione um novo status no campo **Status** e clique em **Salvar**.

   O status do projeto é atualizado para o status selecionado.
