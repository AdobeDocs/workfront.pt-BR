---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Criar Regras de Encaminhamento
description: As Regras de Encaminhamento controlam o que o Adobe Workfront faz com os problemas quando eles são enviados para uma Fila de solicitações. Para obter mais informações sobre como criar Filas de solicitações, consulte Criar uma fila de solicitações.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: c5053b78dd80fe9017ba96e193e59fbd9b17e7c8
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 2%

---

# Criar Regras de Encaminhamento

As regras de roteamento controlam o que o Adobe Workfront faz com os problemas quando são enviadas para uma fila de solicitações. Para obter mais informações sobre como criar Filas de solicitações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

As regras de roteamento enviam problemas para usuários específicos ou funções de trabalho mais bem equipadas para resolver o problema ou a solicitação enviada. As regras de roteamento geralmente são associadas a tópicos de fila, que são usados para controlar qual regra de roteamento será aplicada à ocorrência ou solicitação.

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
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront

## Criar uma Regra de Encaminhamento

1. Vá para o projeto ao qual deseja adicionar as regras de roteamento para suas solicitações.
1. Clique em **Regras de Encaminhamento** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais**, depois **Regras de Encaminhamento**.
1. Clique em **Novas Regras de Encaminhamento** para adicionar a nova regra.
1. Especifique as seguintes informações para a Regra de Encaminhamento:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nome</strong> </td> 
      <td> <p>O nome da regra de roteamento. Você poderá ver a regra de roteamento se tiver acesso para ver essas informações no projeto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrição</strong> </td> 
      <td>Adicione uma descrição para a regra de roteamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Atribuidor padrão*</strong> </td> 
      <td>Adicione um usuário ativo ou uma função de trabalho ativa à qual os novos problemas devem ser atribuídos. Você só pode ter um destinatário padrão nesse campo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Equipe padrão*</strong> </td> 
      <td>Adicione uma equipe ativa à qual o novo problema deve ser atribuído. Você só pode ter uma equipe padrão neste campo.

   <p><b>Nota</b></p>

   Depois que o problema for enviado, você poderá editar suas atribuições e atribuir outros usuários, funções ou equipes. Para obter informações, consulte  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Atribuir problemas </a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Roteamento para o Projeto</strong> </td> 
      <td>Este é o projeto no qual o problema é adicionado.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*Se um usuário, função de trabalho ou equipe for desativado depois de ser associado a uma regra de roteamento, as solicitações continuarão a ser encaminhadas para eles. Periodicamente, você deve fazer um inventário de todas as regras de roteamento e substituir atribuições desativadas por ativas.

   Ao rotear um problema para um projeto, os usuários com permissões sobre o problema recebem as permissões definidas nesse projeto. Para obter informações sobre como configurar permissões em projetos, consulte [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![](assets/new-routing-rule-box-nwe-350x419.png)

1. Clique em **Salvar**.

   Esse processo define apenas a Regra de Encaminhamento. Para garantir que a ocorrência seja roteada quando for enviada para a fila de solicitações, você deverá selecionar a regra de roteamento no **Detalhes da fila** em **Rota Padrão**.

   Para obter informações sobre como adicionar uma Rota padrão a uma fila de solicitações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Se quiser associar várias regras de roteamento à fila de solicitações, você deverá criar vários tópicos de fila e associar cada um a uma regra de roteamento separada. Para obter mais informações sobre como criar um tópico de fila, consulte [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
