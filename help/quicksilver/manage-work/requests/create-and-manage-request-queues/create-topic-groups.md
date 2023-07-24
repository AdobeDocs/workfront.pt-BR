---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Criar Grupos de Tópicos
description: Grupos de Tópicos estão associados a Filas de solicitações. Eles permitem criar camadas das Filas de solicitações em várias categorias, dependendo da natureza das solicitações.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: c5053b78dd80fe9017ba96e193e59fbd9b17e7c8
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Criar Grupos de Tópicos

Grupos de Tópicos estão associados a Filas de solicitações. Eles permitem criar camadas das Filas de solicitações em várias categorias, dependendo da natureza das solicitações.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Licença da Adobe Workfront*</p> </td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront

## Visão Geral de Grupos de Tópicos

Por exemplo, se você tiver uma Fila de solicitações para solicitações de marketing, poderá ter um Grupo de tópicos &quot;Campanha do dia das mães&quot;, com um Grupo de tópicos de segundo nível de &quot;Mídia digital&quot; e um Grupo de tópicos de segundo nível adicional de &quot;Mídia impressa&quot;. Em seguida, você pode ter vários Tópicos de fila dentro de cada Grupo de tópicos. Por exemplo, &quot;Anúncio de banner&quot; e &quot;Blog&quot; podem ser tópicos da fila do grupo de tópicos &quot;Mídia digital&quot;.

Para obter mais informações sobre como criar Filas de solicitações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!TIP]
>
>* Você pode criar até 10 camadas de Grupos de tópicos em uma Fila de solicitações.
>* Não há limite para o número de Tópicos da Fila que podem ser associados a um grupo de tópicos.
>* Grupos de tópicos são um objeto reportável.
>

## Criar Grupos de Tópicos

Recomendamos que você crie Grupos de Tópicos antes de criar um Tópico da Fila. No entanto, um Grupo de tópicos pode ser criado no Construtor de tópicos da fila. Para obter mais informações sobre a criação de Tópicos de Fila, consulte [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Para criar um Grupo de Tópicos:

1. Vá para o projeto publicado como uma Fila de solicitação de ajuda.\
   Para obter mais informações sobre como publicar um projeto como uma Fila de solicitação de ajuda, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Clique em **Grupos de Tópicos** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais**, depois **Grupos de Tópicos**.
1. Clique em **Novo grupo de tópicos**.

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. Especifique as seguintes informações:

   * **Nome**: O nome é visível para usuários que enviam solicitações para essa fila de solicitações.
   * **Descrição**: A descrição é exibida quando os usuários selecionam o grupo de tópicos no processo de enviar uma nova solicitação.
   * **Adicionar ao Grupo de Tópicos**: Você pode adicionar o novo Grupo de Tópicos a um Grupo de Tópicos existente, ou pode adicioná-lo diretamente ao projeto publicado como uma Fila de solicitação de ajuda.

1. Clique em **Salvar**.\
   Isso cria um novo Grupo de Tópicos na sua Fila de solicitações. Agora é possível selecionar categorias adicionais no primeiro menu suspenso em uma Fila de solicitações.\
   Para obter mais informações sobre o envio de solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
