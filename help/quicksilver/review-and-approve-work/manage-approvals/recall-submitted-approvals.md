---
product-area: projects
navigation-topic: approvals
title: Recuperar aprovações enviadas
description: Você pode rechamar qualquer um dos seguintes objetos enviados para aprovação.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
exl-id: 33df75f0-47d0-4848-8d9a-203f40d8831c
TQID: https://experienceleague.adobe.com/ItAwwM5EdjZeV5LRwfkSnEYB6GCfpuLzOCfANanm-hE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1202
ht-degree: 4%

---

# Recuperar aprovações enviadas

Você pode rechamar qualquer um dos seguintes objetos enviados para aprovação:

* Projetos
* Tarefas
* Problemas
* Planilhas de horas
* Documentos
* Solicitações de Acesso

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
   <td>
   <p>Contribute ou superior</p>
   <p>Solicitação ou posterior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso superior ou igual a projetos, tarefas, problemas, planilhas de horas, documentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso de visualização ou superior ao objeto associado à aprovação </p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Projetos

Quando você recupera uma aprovação de projeto, o projeto retorna ao status em que estava antes do início do processo de aprovação.

Se você cancelar uma aprovação associada ao status inicial do projeto, o processo de aprovação será ignorado e o projeto permanecerá no status inicial.

>[!NOTE]
>
>Você pode associar o primeiro status de um projeto ou tarefa a um processo de aprovação usando um modelo. Para obter mais informações sobre como adicionar aprovações a um modelo, consulte [Editar modelos de projeto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Para cancelar uma aprovação de projeto enviada:

1. Clique no ícone **Página inicial** ![Ícone da página inicial](assets/home-icon-30x29.png), no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   >
   >O administrador do Workfront pode fazer as seguintes alterações no ícone Início do ambiente:
   >
   >* Substitua-a por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone será diferente do mostrado neste artigo.
   >* Substituir a página vinculada a ela por uma página diferente. Nesse caso, clique no **Ícone do** ![Menu Principal](assets/main-menu-icon.png) no canto superior direito da página e clique em **Página Inicial**.

1. Na área **Lista de Trabalho**, navegue até o agrupamento **Aprovações que enviei**.

1. Clique em uma aprovação de **Projeto** na Lista de Trabalho.

   Isso abre o projeto à direita da Lista de trabalho.

   ![Aprovação pendente de projeto](assets/project-pending-approval-phome-nwe-350x106.png)

1. Clique em **Cancelar** no canto superior direito do painel direito.

## Tarefas

Quando você cancela a aprovação de uma tarefa, ela retorna ao status em que estava antes do início do processo de aprovação.

Se você cancelar uma aprovação associada ao status inicial da tarefa, o processo de aprovação será ignorado e a tarefa permanecerá no status inicial.

>[!NOTE]
>
>Você pode associar o primeiro status de um projeto ou tarefa a um processo de aprovação usando um modelo. Para obter mais informações sobre como adicionar aprovações a um modelo, consulte [Editar modelos de projeto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Para cancelar uma aprovação de tarefa enviada:

1. Clique no ícone **Página inicial** ![Ícone da página inicial](assets/home-icon-30x29.png), no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   >
   >O administrador do Workfront pode fazer as seguintes alterações no ícone Início do ambiente:
   >
   >* Substitua-a por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone será diferente do mostrado neste artigo.
   >* Substituir a página vinculada a ela por uma página diferente. Nesse caso, clique no **Ícone do** ![Menu Principal](assets/main-menu-icon.png) no canto superior direito da página e clique em **Página Inicial**.

1. Na área **Lista de Trabalho**, navegue até o agrupamento **Aprovações que enviei**.

1. Clique em uma aprovação de **Tarefa** na Lista de trabalho.

   Isso abre a tarefa à direita da Lista de trabalho.

   ![Aprovação pendente de tarefa](assets/task-pending-approval-home-nwe-350x97.png)

1. Clique em **Cancelar** no canto superior direito do painel direito.

## Problemas

Quando você cancela uma aprovação de problema, o problema retorna ao status em que estava antes do início do processo de aprovação.

Se você cancelar uma aprovação associada ao status inicial da ocorrência, o processo de aprovação será ignorado e a ocorrência permanecerá no status inicial.

>[!NOTE]
>
>Você pode associar o primeiro status de um problema a um processo de aprovação usando um modelo. Para obter mais informações sobre como criar uma fila de solicitações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Clique no ícone **Página inicial** ![Ícone da página inicial](assets/home-icon-30x29.png), no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   >
   >O administrador do Workfront pode fazer as seguintes alterações no ícone Início do ambiente:
   >
   >* Substitua-a por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone será diferente do mostrado neste artigo.
   >* Substituir a página vinculada a ela por uma página diferente. Nesse caso, clique no **Ícone do** ![Menu Principal](assets/main-menu-icon.png) no canto superior direito da página e clique em **Página Inicial**.

1. Na área **Lista de Trabalho**, navegue até o agrupamento **Aprovações que enviei**.

1. Clique em uma aprovação de **Problema** na Lista de Trabalho.

   Isso abre a ocorrência à direita da Lista de trabalho.

   ![Problema pendente de aprovação](assets/issue-pending-approval-home-nwe-350x103.png)

1. Clique em **Cancelar** no canto superior direito do painel direito.

## Planilhas de horas

Quando você cancela a aprovação de uma folha de horas, ela retorna ao status em que estava antes de ser enviada para aprovação.

1. Clique no ícone **Página inicial** ![Ícone da página inicial](assets/home-icon-30x29.png), no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   >
   >O administrador do Workfront pode fazer as seguintes alterações no ícone Início do ambiente:
   >
   >* Substitua-a por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone será diferente do mostrado neste artigo.
   >* Substituir a página vinculada a ela por uma página diferente. Nesse caso, clique no **Ícone do** ![Menu Principal](assets/main-menu-icon.png) no canto superior direito da página e clique em **Página Inicial**.

1. Na área **Lista de Trabalho**, navegue até o agrupamento **Aprovações que enviei**.

1. Clique em uma aprovação de **Planilha de horas** na Lista de Trabalho.

   Isso abre a folha de horas à direita da Lista de trabalho.

   ![Planilha de horas com aprovação pendente](assets/timesheet-pending-approval-home-nwe-350x157.png)

1. Clique em **Cancelar** no canto superior direito do painel direito.

## Documentos

Para cancelar uma aprovação de documento, você deve remover manualmente um ou todos os usuários da aprovação.

1. Clique no ícone **Página inicial** ![Ícone da página inicial](assets/home-icon-30x29.png), no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   >
   >O administrador do Workfront pode fazer as seguintes alterações no ícone Início do ambiente:
   >
   >* Substitua-a por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone será diferente do mostrado neste artigo.
   >* Substituir a página vinculada a ela por uma página diferente. Nesse caso, clique no **Ícone do** ![Menu Principal](assets/main-menu-icon.png) no canto superior direito da página e clique em **Página Inicial**.

1. Na área **Lista de Trabalho**, navegue até o agrupamento **Aprovações que enviei**.

1. Clique em uma aprovação de **Documento** na Lista de Trabalho.

   Isso abre o documento à direita da Lista de trabalho.

   ![Document.png](assets/document-350x232.png)

1. Clique em **Gerenciar aprovações** no canto superior direito do painel direito. Isso abre a caixa Gerenciar aprovações.
1. Clique no ícone **Remover** incorporado com o nome de um usuário dentro da caixa Gerenciar aprovações. Remova todos os usuários para cancelar completamente a aprovação do documento.

   ![Remover_Usuário.png](assets/remove-user-350x41.png)

## Solicitações de Acesso

1. Clique no ícone **Página inicial** ![Ícone da página inicial](assets/home-icon-30x29.png), no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   >
   >O administrador do Workfront pode fazer as seguintes alterações no ícone Início do ambiente:
   >
   >* Substitua-a por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone será diferente do mostrado neste artigo.
   >* Substituir a página vinculada a ela por uma página diferente. Nesse caso, clique no **Ícone do** ![Menu Principal](assets/main-menu-icon.png) no canto superior direito da página e clique em **Página Inicial**.

1. Na área **Lista de Trabalho**, navegue até o agrupamento **Aprovações que enviei**.

1. Clique em uma aprovação de **Solicitação de acesso** na Lista de trabalho.

   Isso abre a solicitação de acesso à direita da Lista de trabalho.

   ![Solicitação de acesso com aprovação pendente](assets/access-request-pending-approval-nwe-350x104.png)

1. Clique em **Cancelar** no canto superior direito do painel direito.
