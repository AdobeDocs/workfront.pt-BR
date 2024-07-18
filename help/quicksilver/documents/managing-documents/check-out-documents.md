---
product-area: documents
navigation-topic: manage-documents
title: Fazer check-out de documentos
description: Você pode fazer check-out de um documento para impedir que outros usuários o excluam ou façam upload de uma nova versão dele. Somente um usuário pode fazer check-out de um documento por vez. Você pode fazer check-out de qualquer documento carregado no Adobe Workfront, bem como de documentos vinculados a provedores de documentos de terceiros (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint ou qualquer outro provedor personalizado).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: 9aa6822c9c1ecade776d4c71b113c1afd997f40c
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Fazer check-out de documentos

Você pode fazer check-out de um documento para impedir que outros usuários o excluam ou façam upload de uma nova versão dele. Somente um usuário pode fazer check-out de um documento por vez. Você pode fazer check-out de qualquer documento carregado no Adobe Workfront, bem como de documentos vinculados a provedores de documentos de terceiros (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint ou qualquer outro provedor personalizado). 

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar acesso ao documento</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

+++

## Ações permitidas em documentos com check-out

Os usuários com acesso de gerenciamento ao documento podem fazer o seguinte:

* Editar o documento (nome do documento, descrição, dados personalizados)
* Mover o documento
* Compartilhar o documento
* Visualizar o documento
* Baixar o documento

  >[!TIP]
  >
  > Embora um usuário possa baixar um documento quando seu check-out for feito por outro usuário, recomendamos que os usuários aguardem até que o check-in do documento seja feito novamente antes de baixá-lo. Quando é feito o check-out de um documento, isso geralmente indica que o trabalho ainda está sendo feito no documento. Aguardar o check-in de um documento para baixá-lo garante que o usuário tenha a versão mais recente.

* Aprove um documento ou aplique uma aprovação ao documento.
* Revisar o documento no visualizador de provas

  Para obter mais informações sobre revisões, consulte [Revisão](../../review-and-approve-work/proofing/proofing.md)

## Fazer check-out de um documento

Se você tiver permissões de gerenciamento para um documento, poderá fazer check-out dele para proibir determinadas ações no documento. 

1. Vá para a área onde o documento está armazenado e selecione o documento. 

   Para obter informações sobre como adicionar documentos, consulte [Adicionar documentos ao Adobe Workfront a partir do seu sistema de arquivos](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Clique no ícone ![](assets/check-out-25x23.png) do **Check-out**.

1. Um ícone de bloqueio ![](assets/lock-icon-locked-qs.png) é exibido à direita do nome do documento. O documento permanece com check-out após fazer logoff do Workfront.
1. Somente o usuário que fez check-out do documento ou o administrador do Workfront pode fazer check-in do documento.

## Gerenciar documentos obtidos

Considere o seguinte sobre documentos com check-out:

* Antes de excluir um objeto no qual um documento com check-out está armazenado, você deve primeiro fazer o check-in do documento. 
* Se o administrador do Workfront excluir um usuário que fez o check-out de um documento que não era seu, o Workfront fará o check-in do documento automaticamente.
* Se o administrador do Workfront excluir um usuário que fez check-out de um documento de sua propriedade e o documento for carregado em um objeto, o documento permanecerá com check-out. Somente um administrador do Workfront pode fazer check-in novamente.
* Se o administrador do Workfront excluir um usuário que fez check-out de um documento de sua propriedade e o documento for carregado somente na área Documentos (não em um objeto), o documento será excluído com o usuário.

  Para obter informações sobre como excluir usuários, consulte [Excluir usuários](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Se o administrador do Workfront desativar um usuário, todos os documentos dos quais ele fez check-out permanecerão com check-out. Somente um administrador do Workfront pode fazer o check-in deles novamente. 

## Incluir um documento

Você deve fazer check-in de um documento novamente antes de carregar uma nova versão ou excluí-la. 

Para fazer check-in de um documento:

1. Vá para a área onde o documento está armazenado e selecione o documento. 

   Um ícone de bloqueio ![](assets/lock-icon-locked-qs.png) é exibido à direita do nome do documento.

1. Clique no ícone ![](assets/check-in-25x22.png) do **Check-in**.
