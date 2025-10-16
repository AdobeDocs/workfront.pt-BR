---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Fornecer acesso às filas de solicitações
description: Ao fornecer acesso a uma fila de solicitações, você determina quem na organização pode exibir a fila de solicitações na área Solicitações do Adobe Workfront.
author: Becky
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 1%

---

# Fornecer acesso a filas de solicitações

<!-- Audited: 6/2025 -->

Ao fornecer acesso a uma fila de solicitações, você determina quem na organização pode exibir a fila de solicitações na área Solicitações do Adobe Workfront.

Você pode fornecer a diferentes usuários acesso a uma Fila de solicitações, dependendo se eles fazem parte da equipe do projeto, do grupo do projeto ou da empresa do projeto. Você também pode fornecer acesso à fila de solicitações a todos no sistema.

Isso é útil em organizações que convidam participantes externos para o Workfront e desejam limitar o acesso dos usuários a áreas específicas. Nesse caso, uma fila de solicitações aberta apenas para os usuários associados à empresa ou grupo do projeto limita a visibilidade a participantes externos. Dar acesso a qualquer pessoa torna a solicitação visível para os participantes internos e externos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Standard </p>
   <p>Plano </p> </td> 
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

## Pré-requisitos

Antes da fila de solicitações estar disponível para usuários na área Solicitações, você deve criar um projeto com as seguintes configurações:

* Designe-a como uma fila de solicitações. Para obter mais informações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Atualize o status do projeto para Atual.

## Fornecer acesso a uma Fila de solicitações

1. Vá para o projeto em que deseja fornecer acesso às filas de solicitações.

   >[!NOTE]
   >
   >Somente projetos com o status Atual ficam visíveis na área Solicitações.

1. Clique em **Detalhes da fila** no painel esquerdo.
1. Selecione **Publicar como Fila de Solicitação de Ajuda** para designar o projeto como uma Fila de Solicitação.
1. Selecione entre as seguintes opções exibidas:

   * **Qualquer um**: qualquer usuário pode visualizar e adicionar solicitações à fila de solicitações.
   * **Pessoas com acesso de exibição a este projeto**: os usuários com permissões de exibição para o projeto podem exibir e adicionar solicitações à fila de solicitações.
   * **Pessoas da empresa deste projeto**: os usuários associados à Empresa do projeto podem exibir e adicionar solicitações. A Empresa associada ao projeto está listada entre parênteses ao lado dessa opção.
   * **Pessoas neste grupo de projeto**: os usuários associados ao Grupo do projeto podem exibir e adicionar solicitações. O Grupo associado ao projeto é listado entre parênteses ao lado dessa opção.

     As filas de grupo são úteis quando vários departamentos compartilham uma conta do Workfront para atingir metas organizacionais exclusivas. Cada departamento pode ter suas próprias filas que os membros de outros grupos não deveriam ver.

     Para obter informações sobre quem tem permissões em um projeto, consulte [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

     Grupos e empresas podem ser associados ao projeto ao editar o projeto. Para obter mais informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Clique em **Salvar**.
