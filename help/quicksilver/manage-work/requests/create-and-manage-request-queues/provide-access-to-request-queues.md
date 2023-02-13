---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Fornecer acesso às filas de solicitação
description: Ao fornecer acesso a uma fila de solicitações, determine quem na organização pode exibir a fila de solicitações na área Solicitações do Adobe Workfront.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Fornecer acesso às filas de solicitação

Ao fornecer acesso a uma fila de solicitações, determine quem na organização pode exibir a fila de solicitações na área Solicitações do Adobe Workfront.

Você pode fornecer aos usuários diferentes acesso a uma Fila de solicitações, dependendo se eles fazem parte da equipe do projeto, do grupo de projetos ou da empresa do projeto. Você também pode fornecer acesso a todos no sistema para uma fila de solicitações. 

Isso é útil em organizações que convidam participantes externos para o Workfront e desejam limitar o acesso dos usuários a áreas específicas — nesse caso, uma fila de solicitações aberta apenas para os usuários associados à empresa ou grupo do projeto limita a visibilidade para participantes externos. Dar acesso a qualquer pessoa torna a solicitação visível para as partes interessadas internas e externas.

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
   <td role="rowheader">Licença da Adobe Workfront*</td> 
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

## Pré-requisitos

Antes que a fila de solicitações esteja disponível para usuários na área Solicitações , você deve criar um projeto com as seguintes configurações:

* Designe-o como uma fila de solicitações. Para obter mais informações sobre como criar uma Fila de solicitações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Atualize o Status do projeto para Atual.

## Fornecer acesso a uma fila de solicitações

1. Vá para o projeto onde deseja fornecer acesso às filas de solicitação.

   >[!NOTE]
   >
   >Somente os projetos com status Atual são visíveis na área Solicitações .

1. Clique em **Detalhes da fila** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais**, em seguida **Detalhes da fila**.
1. Selecionar **Publicar como fila de solicitações de ajuda** para designar o projeto como uma Fila de solicitações.
1. Selecione dentre as seguintes opções:

   * **Qualquer pessoa**: Qualquer usuário pode exibir e adicionar solicitações à fila de solicitações.
   * **Pessoas com acesso a este projeto**: os usuários que têm permissões de Exibição do projeto podem exibir e adicionar solicitações à fila de solicitações. 
   * **Pessoas na empresa deste projeto**: os usuários associados à Empresa do projeto podem exibir e adicionar solicitações. A Empresa associada ao projeto é listada entre parênteses ao lado desta opção. 
   * **Pessoas no grupo deste projeto**: os usuários associados ao Grupo do projeto podem exibir e adicionar solicitações. O Grupo associado ao projeto é listado entre parênteses ao lado desta opção.

      As filas de grupo são úteis quando vários departamentos compartilham uma conta do Workfront para atingir metas organizacionais exclusivas. Cada departamento pode ter as suas próprias filas que os membros de outros grupos não devem poder ver.

      Para obter informações sobre quem tem permissões em um projeto, consulte [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
      Grupos e empresas podem ser associados ao projeto ao editar o projeto. Para obter mais informações sobre edição de projetos, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Clique em **Salvar**.
