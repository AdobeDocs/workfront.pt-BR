---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Criar Regras de Encaminhamento
description: As Regras de Encaminhamento controlam o que o Adobe Workfront faz com os problemas quando eles são enviados para uma Fila de solicitações. Para obter mais informações sobre como criar Filas de solicitações, consulte Criar uma fila de solicitações.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---

# Criar Regras de Encaminhamento

<!-- Audited: 12/2023 -->

As regras de roteamento controlam o que o Adobe Workfront faz com os problemas quando são enviadas para uma fila de solicitações. Para obter mais informações sobre como criar Filas de Solicitações, consulte [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

As regras de roteamento enviam problemas para usuários específicos ou funções de trabalho mais bem equipadas para resolver o problema ou a solicitação enviada. As regras de roteamento geralmente são associadas a tópicos de fila, que são usados para controlar qual regra de roteamento será aplicada à ocorrência ou solicitação.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
    <p>Novo: Padrão</p>
    <p>ou</p>
    <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td>
   <td> <p>Editar acesso a projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Gerenciar permissões do projeto</p> </td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma Regra de Encaminhamento

1. Vá para o projeto no qual deseja adicionar as regras de roteamento para suas solicitações.
1. Clique em **Regras de roteamento** no painel esquerdo. Talvez seja necessário clicar em **Mostrar Mais** e depois em **Regras de Roteamento**.
1. Clique em **Nova Regra de Roteamento** para adicionar a nova regra.
1. Especifique as seguintes informações para a Regra de Encaminhamento:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nome</strong> </td> 
      <td>O nome da regra de roteamento. Você poderá ver a regra de roteamento se tiver acesso para ver essas informações no projeto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrição</strong> </td> 
      <td>Adicione uma descrição para a regra de roteamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Atribuído padrão*</strong> </td> 
      <td>Adicione um usuário ativo ou uma função de trabalho ativa à qual os novos problemas devem ser atribuídos. Você só pode ter um destinatário padrão nesse campo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Equipe padrão*</strong> </td> 
      <td>Adicione uma equipe ativa à qual o novo problema deve ser atribuído. Você só pode ter uma equipe padrão neste campo.

   <p><b>Nota</b></p>

   Depois que o problema for enviado, você poderá editar suas atribuições e atribuir outros usuários, funções ou equipes. Para obter informações, consulte <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Atribuir problemas</a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Rotear para Projeto</strong> </td> 
      <td>Este é o projeto no qual o problema é adicionado.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*Se um usuário, função de trabalho ou equipe for desativado depois de ser associado a uma regra de roteamento, as solicitações continuarão a ser encaminhadas para eles. Periodicamente, você deve fazer um inventário de todas as regras de roteamento e substituir atribuições desativadas por ativas.

   Ao rotear um problema para um projeto, os usuários com permissões sobre o problema recebem as permissões definidas nesse projeto. Para obter informações sobre como configurar permissões em projetos, consulte [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![Caixa Nova Regra de Roteamento](assets/new-routing-rule-box.png)

1. Clique em **Salvar**.

   Esse processo define apenas a Regra de Encaminhamento. Para garantir que o problema seja roteado quando for enviado à fila de solicitações, você deve selecionar a regra de roteamento na guia **Detalhes da fila** em **Rota padrão**.

   Para obter informações sobre como adicionar uma Rota Padrão a uma fila de solicitações, consulte [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Se quiser associar várias regras de roteamento à fila de solicitações, você deverá criar vários tópicos de fila e associar cada um a uma regra de roteamento separada. Para obter mais informações sobre como criar um tópico de fila, consulte [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
