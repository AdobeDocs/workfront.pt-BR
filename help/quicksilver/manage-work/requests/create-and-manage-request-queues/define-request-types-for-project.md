---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definir Tipos de Solicitação para um Projeto
description: Você pode organizar os tipos de problemas ou solicitações que estão conectados no Adobe Workfront por Tipos de solicitação.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 2%

---

# Definir Tipos de Solicitação para um projeto

<!-- Audited: 6/2025 -->

Você pode organizar os tipos de problemas ou solicitações que estão conectados no Adobe Workfront por Tipos de solicitação. Isso é útil para relatar motivos e ajudar os usuários a entender que tipo de trabalho inesperado pode ocorrer durante a vida útil de um projeto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
    <p>Novo: Padrão</p>
    <p>Atual: Plano</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um projeto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar, você deve fazer o seguinte:

* Ter ou criar um projeto.

  Para obter informações sobre como criar projetos, consulte [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

## Considerações sobre tipos de solicitação

* Você pode especificar o tipo de problemas ou solicitações que podem ser registradas em um projeto ao configurar a área Detalhes da fila para o projeto.
* Você não precisa ativar o projeto para ser uma fila de solicitações para poder definir Tipos de solicitação para um projeto. Quaisquer problemas registrados para um projeto podem ser rotulados com um Tipo de solicitação diferente.
* Se você adicionar Tópicos de fila ao seu projeto, deverá definir Tipos de solicitação em cada tópico de fila para exibi-los ao adicionar um novo problema ou solicitação. Para obter mais informações, consulte [Criar tópicos da fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definir os tipos de problema ou solicitação para um projeto

{{step1-to-projects}}

1. Na página **Projetos**, selecione um projeto.
1. No painel esquerdo, clique em **Detalhes da fila**.
1. Na seção **Propriedades da fila**, selecione os **Tipos de solicitação** desejados para o projeto:
   * Relatório de erro
   * Pedido de alteração
   * Problema
   * Solicitar

   >[!NOTE]
   >
   >* Você deve ter pelo menos um tipo de solicitação selecionado. É possível selecionar vários tipos.
   >* O administrador do Workfront pode ter renomeado algumas dessas opções. Para obter informações, consulte [Configurar tipos de solicitação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Clique em **Salvar**. Os tipos de solicitação especificados estarão disponíveis para seleção quando você informar um novo problema em uma tarefa ou um projeto, ou quando submeter uma nova solicitação ao projeto (se o projeto estiver ativado como uma fila de solicitações).
