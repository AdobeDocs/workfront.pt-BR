---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Criar Regras de Encaminhamento
description: As Regras de Encaminhamento controlam o que o Adobe Workfront faz com os problemas quando eles são enviados para uma Fila de solicitações.
author: Becky
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 1%

---

# Criar Regras de Encaminhamento

<!-- Audited: 12/2023 -->

As regras de roteamento controlam o que o Adobe Workfront faz com os problemas quando são enviadas para uma fila de solicitações. Para obter mais informações sobre como criar Filas de Solicitações, consulte [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

As regras de roteamento enviam problemas para usuários específicos ou funções de trabalho mais bem equipadas para resolver o problema ou a solicitação enviada. As regras de roteamento geralmente são associadas a tópicos de fila, que são usados para controlar qual regra de roteamento será aplicada à ocorrência ou solicitação.

Depois de criado, não é possível mover regras de roteamento de um projeto para outro.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Pacotes Adobe Workfront</p></td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Plano</p> </td> 
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

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma Regra de Encaminhamento

1. Vá para o projeto no qual deseja adicionar regras de roteamento para suas solicitações.
1. Clique em **Regras de roteamento** no painel esquerdo.
1. Clique em **Nova Regra de Roteamento** para adicionar a nova regra. A caixa **Nova Regra de Roteamento** é aberta.

   ![Caixa Nova Regra de Roteamento](assets/new-routing-rule-box.png)
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

1. Clique em **Salvar**.

   Esse processo define apenas a Regra de Encaminhamento. Para garantir que o problema seja roteado quando for enviado à fila de solicitações, você deve selecionar a regra de roteamento na guia **Detalhes da fila** em **Rota padrão**.

   Para obter informações sobre como adicionar uma Rota Padrão a uma fila de solicitações, consulte [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Se quiser associar várias regras de roteamento à fila de solicitações, você deverá criar vários tópicos de fila e associar cada um a uma regra de roteamento separada. Para obter mais informações sobre como criar um tópico de fila, consulte [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
