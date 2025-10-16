---
product-area: projects
navigation-topic: manage-projects
title: Alterar o status de um projeto
description: Você pode atualizar manualmente o status de um projeto para qualquer outro status, se necessário. Você pode atualizar manualmente o status de um projeto para um status que equivale a Concluído somente quando o Modo de conclusão do projeto estiver definido como Manual.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# Alterar o status de um projeto

<!--Audited: 02/2024-->

Você pode atualizar manualmente o status de um projeto para qualquer outro status, se necessário.

Você pode atualizar manualmente o status de um projeto para um status que equivale a Concluído somente quando o Modo de conclusão do projeto estiver definido como Manual.

Caso contrário, o Adobe Workfront marcará automaticamente o projeto como Concluído quando todas as tarefas e problemas do projeto forem concluídas e aprovadas.

Para obter mais informações sobre o Modo de conclusão do projeto, consulte [Editar projetos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

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
</table>-->

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
