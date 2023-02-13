---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Criar grupos de tópicos
description: Grupos de tópicos são associados a Filas de solicitação. Eles permitem colocar suas filas de solicitação em várias categorias, dependendo da natureza das solicitações.
author: Alina
feature: Work Management
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Criar grupos de tópicos

Grupos de tópicos são associados a Filas de solicitação. Eles permitem colocar suas filas de solicitação em várias categorias, dependendo da natureza das solicitações.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Licença da Adobe Workfront*</p> </td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront

## Visão geral dos grupos de tópicos

Por exemplo, se você tiver uma Fila de solicitações para solicitações de marketing, poderá ter um Grupo de tópicos de &quot;Campanha do dia das mães&quot;, com um Grupo de tópicos de segundo nível de &quot;Mídia digital&quot; e um Grupo de tópicos de segundo nível adicional de &quot;Mídia impressa&quot;. Em seguida, você pode ter vários Tópicos da fila dentro de cada Grupo de tópicos. Por exemplo, &quot;Banner Ad&quot; e &quot;Blog&quot; podem ser Tópicos da fila para o Grupo de tópicos &quot;Mídia digital&quot;.

Para obter mais informações sobre como criar filas de solicitações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!TIP]
>
>* Você pode criar até 10 níveis de Grupos de tópicos em uma Fila de solicitações.
>* Não há limite para o número de Tópicos da fila que podem ser associados a um grupo de tópicos.
>* Os grupos de tópicos são um objeto relatável.
>


## Criar grupos de tópicos

Recomendamos que você crie Grupos de tópicos antes de criar um Tópico da fila. No entanto, um Grupo de tópicos pode ser criado no construtor de Tópicos da fila. Para obter mais informações sobre como criar tópicos da fila, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Para criar um Grupo de tópicos:

1. Vá para o projeto publicado como uma Fila de solicitação de ajuda.\
   Para obter mais informações sobre como publicar um projeto como uma fila de solicitações de ajuda, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Clique em **Grupos de tópicos** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais**, em seguida **Grupos de tópicos**.
1. Clique em **Novo grupo de tópicos**.

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. Especifique as seguintes informações:

   * **Nome**: O nome é visível para os usuários que enviam solicitações para essa fila de solicitações.
   * **Descrição**: A descrição é exibida quando os usuários selecionam o grupo de tópicos no processo de envio de uma nova solicitação.
   * **Adicionar ao grupo de tópicos**: Você pode adicionar o novo Grupo de Tópicos a um Grupo de Tópicos existente, ou pode adicioná-lo diretamente ao projeto publicado como uma Fila de Solicitações de Ajuda.

1. Clique em **Salvar**.\
   Isso cria um novo Grupo de tópicos na Fila de solicitações. Agora é possível selecionar categorias adicionais no primeiro menu suspenso em uma Fila de solicitações.\
   Para obter mais informações sobre como enviar solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
