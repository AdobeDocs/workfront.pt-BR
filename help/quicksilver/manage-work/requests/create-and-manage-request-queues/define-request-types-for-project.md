---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definir tipos de solicitação para um projeto
description: Você pode organizar o tipo de problemas ou solicitações que estão registradas no Adobe Workfront por Tipos de solicitação.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# Definir tipos de solicitação para um projeto

Você pode organizar o tipo de problemas ou solicitações que estão registradas no Adobe Workfront por Tipos de solicitação.

Essa organização é útil para relatar motivos e ajudar os usuários a entender que tipo de trabalho inesperado pode ocorrer durante a vida útil de um projeto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plano Adobe Workfront</a>*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Licença Adobe Workfront</a>*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar, você deve

* Ter ou criar um projeto

   Para obter informações sobre como criar projetos, consulte [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

## Considerações sobre os tipos de solicitação

* Você pode especificar o tipo de problemas ou solicitações que podem ser registradas em um projeto ao configurar a variável **Detalhes da fila** área do projeto.
* Você não precisa habilitar o projeto para ser uma fila de solicitações para poder definir Tipos de solicitação para um projeto. Qualquer problema registrado em um projeto pode ser rotulado com um Tipo de solicitação diferente.
* Se você adicionar Tópicos da fila ao seu projeto, defina Tipos de solicitação em cada tópico da fila para exibi-lo ao adicionar um novo problema ou solicitação. Para obter mais informações, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definir o problema ou os tipos de solicitação para um projeto

1. Clique em **Projetos** no Menu principal. ![](assets/main-menu-icon.png)

1. Clique no nome do projeto para abri-lo.
1. No painel esquerdo, clique em **Detalhes da fila**.
1. No **Propriedades da fila** selecione a **Tipos de solicitação** você deseja para o projeto.

   >[!NOTE]
   >
   >Você deve ter pelo menos um tipo de solicitação selecionado. Você pode selecionar vários tipos de solicitação.

   Selecione entre os seguintes tipos:

   * Registro de Defeito
   * Pedido de alteração
   * Problema
   * Solicitar

   >[!TIP]
   >
   >O administrador do Workfront pode ter renomeado algumas dessas opções. Para obter mais informações, consulte [Configurar tipos de solicitação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Clique em **Salvar**.

   Os tipos de solicitação especificados estarão disponíveis para seleção ao inserir um novo problema em uma tarefa ou projeto, ou ao enviar uma nova solicitação ao projeto, se o projeto estiver habilitado como uma fila de solicitações.
