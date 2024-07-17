---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definir Tipos de Solicitação para um projeto
description: Você pode organizar os tipos de problemas ou solicitações que estão conectados no Adobe Workfront por Tipos de solicitação.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 2%

---

# Definir Tipos de Solicitação para um projeto

Você pode organizar os tipos de problemas ou solicitações que estão conectados no Adobe Workfront por Tipos de solicitação.

Essa organização é útil para relatar motivos e ajudar os usuários a entender que tipo de trabalho inesperado pode ocorrer durante a vida útil de um projeto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plano do Adobe Workfront</a>*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Visão geral das licenças</a>*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Pré-requisitos

Antes de começar, você deve fazer o seguinte:

* Ter ou criar um projeto

  Para obter informações sobre como criar projetos, consulte [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

## Considerações sobre tipos de solicitação

* Você pode especificar o tipo de problemas ou solicitações que podem ser registradas em um projeto ao configurar a área **Detalhes da fila** para o projeto.
* Você não precisa ativar o projeto para ser uma fila de solicitações para poder definir Tipos de solicitação para um projeto. Quaisquer problemas registrados para um projeto podem ser rotulados com um Tipo de solicitação diferente.
* Se você adicionar Tópicos de fila ao seu projeto, deverá definir Tipos de solicitação em cada tópico de fila para exibi-los ao adicionar um novo problema ou solicitação. Para obter mais informações, consulte [Criar tópicos da fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definir os tipos de problema ou solicitação para um projeto

1. Clique em **Projetos** no menu principal. ![](assets/main-menu-icon.png)

1. Clique no nome do projeto para abri-lo.
1. No painel esquerdo, clique em **Detalhes da fila**.
1. Na seção **Propriedades da fila**, selecione os **Tipos de solicitação** desejados para o projeto.

   >[!NOTE]
   >
   >Você deve ter pelo menos um tipo de solicitação selecionado. Você pode selecionar vários tipos de solicitação.

   Selecione entre os seguintes tipos:

   * Relatório de erro
   * Pedido de alteração
   * Problema
   * Solicitar

   >[!TIP]
   >
   >O administrador do Workfront pode ter renomeado algumas dessas opções. Para obter informações, consulte [Configurar tipos de solicitação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Clique em **Salvar**.

   Os tipos de solicitação especificados estarão disponíveis para seleção quando você informar um novo problema em uma tarefa ou um projeto, ou quando submeter uma nova solicitação ao projeto, se o projeto estiver ativado como uma fila de solicitações.
