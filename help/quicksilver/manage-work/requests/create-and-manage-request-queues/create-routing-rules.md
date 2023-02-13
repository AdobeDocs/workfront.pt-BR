---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Criar regras de roteamento
description: As Regras de Roteamento controlam o que o Adobe Workfront faz com problemas quando são submetidos a uma Fila de Solicitações. Para obter mais informações sobre como criar Filas de solicitações, consulte Criar uma fila de solicitações.
author: Alina
feature: Work Management
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 2%

---

# Criar regras de roteamento

As regras de roteamento controlam o que o Adobe Workfront faz com problemas quando são enviados para uma fila de solicitações. Para obter mais informações sobre como criar Filas de Solicitação, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

As regras de roteamento enviam problemas para usuários específicos ou funções de trabalho mais bem equipadas para resolver o problema ou a solicitação enviada. As regras de roteamento geralmente são associadas a tópicos da fila, que são usados para controlar qual regra de roteamento será aplicada à emissão ou solicitação.

## Requisitos de acesso

<!--drafted - replace the table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront

## Criar uma regra de roteamento

1. Vá para o projeto ao qual deseja adicionar as regras de roteamento para suas solicitações.
1. Clique em **Regras de roteamento** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais**, em seguida **Regras de roteamento**.
1. Clique em **Novas Regras de Roteamento** para adicionar a nova regra.
1. Especifique as seguintes informações para a Regra de Roteamento:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nome</strong> </td> 
      <td> <p>O nome da regra de roteamento. Você pode ver a regra de roteamento se tiver acesso para ver essas informações no projeto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrição</strong> </td> 
      <td>Adicione uma descrição para a regra de roteamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Atribuidor padrão*</strong> </td> 
      <td>Adicione um usuário ativo ou uma função de trabalho ativa para a qual os novos problemas devem ser atribuídos. Você só pode ter um destinatário padrão neste campo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Equipe padrão*</strong> </td> 
      <td>Adicione uma equipe ativa à qual o novo problema deve ser atribuído. Você só pode ter uma equipe padrão neste campo.

   <p><b>Nota</b></p>

   Depois que o problema for enviado, você poderá editar suas atribuições e atribuir outros usuários, funções ou equipes. Para obter mais informações, consulte  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Atribuir problemas </a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Roteamento para o Projeto</strong> </td> 
      <td>Este é o projeto ao qual o problema é adicionado.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*Se um usuário, uma função de trabalho ou uma equipe forem desativados depois de serem associados a uma regra de roteamento, as solicitações continuarão a ser roteadas para elas. Você deve fazer periodicamente um inventário de todas as regras de roteamento e substituir atribuições desativadas por atribuições ativas.

   Quando você direciona um problema para um projeto, os usuários com permissões sobre o problema recebem as permissões definidas nesse projeto. Para obter informações sobre como definir permissões em projetos, consulte [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![](assets/new-routing-rule-box-nwe-350x419.png)

1. Clique em **Salvar**.

   Esse processo só define a Regra de Roteamento. Para garantir que o problema seja roteado quando for enviado para a fila de solicitações, você deve selecionar a regra de roteamento no **Detalhes da fila** guia em **Rota padrão**.

   Para obter informações sobre como adicionar uma Rota Padrão a uma fila de solicitações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Se quiser associar várias regras de roteamento à fila de solicitações, crie vários tópicos de fila e associe cada um a uma regra de roteamento separada. Para obter mais informações sobre como criar um tópico de fila, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
