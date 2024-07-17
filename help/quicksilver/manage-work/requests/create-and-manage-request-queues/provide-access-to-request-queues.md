---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Fornecer acesso a filas de solicitações
description: Ao fornecer acesso a uma fila de solicitações, você determina quem na organização pode exibir a fila de solicitações na área Solicitações do Adobe Workfront.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Fornecer acesso a filas de solicitações

Ao fornecer acesso a uma fila de solicitações, você determina quem na organização pode exibir a fila de solicitações na área Solicitações do Adobe Workfront.

Você pode fornecer a diferentes usuários acesso a uma Fila de solicitações, dependendo se eles fazem parte da equipe do projeto, do grupo do projeto ou da empresa do projeto. Você também pode fornecer acesso a todos no sistema a uma fila de solicitações. 

Isso é útil em organizações que convidam participantes externos para o Workfront e desejam limitar o acesso dos usuários a áreas específicas — nesse caso, uma fila de solicitações aberta apenas para os usuários associados à empresa ou grupo do projeto limita a visibilidade a participantes externos. Dar acesso a qualquer pessoa torna a solicitação visível para os participantes internos e externos.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront

## Pré-requisitos

Antes da fila de solicitações estar disponível para usuários na área Solicitações, você deve criar um projeto com as seguintes configurações:

* Designe-a como uma fila de solicitações. Para obter mais informações sobre como criar uma Fila de solicitações, consulte [Criar uma Fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Atualize o status do projeto para Atual.

## Fornecer acesso a uma Fila de solicitações

1. Vá para o projeto em que deseja fornecer acesso às filas de solicitações.

   >[!NOTE]
   >
   >Somente projetos com o status Atual ficam visíveis na área Solicitações.

1. Clique em **Detalhes da fila** no painel esquerdo. Talvez seja necessário clicar em **Mostrar Mais** e em **Detalhes da Fila**.
1. Selecione **Publish como Fila de solicitação de ajuda** para designar o projeto como uma Fila de solicitação.
1. Selecione entre as seguintes opções:

   * **Qualquer um**: qualquer usuário pode visualizar e adicionar solicitações à fila de solicitações.
   * **Pessoas com acesso de exibição a este projeto**: os usuários com permissões de exibição para o projeto podem exibir e adicionar solicitações à fila de solicitações. 
   * **Pessoas da empresa deste projeto**: os usuários associados à Empresa do projeto podem exibir e adicionar solicitações. A Empresa associada ao projeto está listada entre parênteses ao lado dessa opção. 
   * **Pessoas neste grupo de projeto**:Os usuários associados ao Grupo do projeto podem exibir e adicionar solicitações. O Grupo associado ao projeto é listado entre parênteses ao lado dessa opção.

     As filas de grupo são úteis quando vários departamentos compartilham uma conta do Workfront para atingir metas organizacionais exclusivas. Cada departamento pode ter suas próprias filas que os membros de outros grupos não podem ver.

     Para obter informações sobre quem tem permissões em um projeto, consulte [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
     Grupos e empresas podem ser associados ao projeto ao editar o projeto. Para obter mais informações sobre a edição de projetos, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Clique em **Salvar**.
