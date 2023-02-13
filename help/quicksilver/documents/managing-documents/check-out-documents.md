---
product-area: documents
navigation-topic: manage-documents
title: Verificar documentos
description: Você pode fazer check-out de um documento para impedir que outros usuários o excluam ou façam upload de uma nova versão dele. Somente um usuário pode fazer check-out de um documento de cada vez. Você pode fazer check-out de qualquer documento carregado no Adobe Workfront, bem como de documentos vinculados a provedores de documentos de terceiros (Caixa, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint ou qualquer outro provedor personalizado).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Verificar documentos

Você pode fazer check-out de um documento para impedir que outros usuários o excluam ou façam upload de uma nova versão dele. Somente um usuário pode fazer check-out de um documento de cada vez. Você pode fazer check-out de qualquer documento carregado no Adobe Workfront, bem como de documentos vinculados a provedores de documentos de terceiros (Caixa, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint ou qualquer outro provedor personalizado). 

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar acesso ao documento</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Ações permitidas em documentos com check-out

Os usuários com acesso de gerenciamento ao documento podem fazer o seguinte:

* Editar o documento (nome do documento, descrição, dados personalizados)
* Mover o documento
* Compartilhar o documento
* Visualizar o documento
* Baixe o documento

   >[!TIP]
   >
   > Embora um usuário possa baixar um documento quando ele for tirado por outro usuário, recomendamos que os usuários aguardem até que o documento tenha sido devolvido para download antes de baixá-lo. Quando um documento é passado por check-out, isso geralmente indica que o trabalho ainda está sendo feito no documento. Aguardar até que o check-in de um documento seja feito para baixá-lo garante que o usuário tenha a versão mais recente.

* Aprove um documento ou aplique uma aprovação ao documento.
* Revisar o documento no visualizador de prova

   Para obter mais informações sobre revisão, consulte [Tofing](../../review-and-approve-work/proofing/proofing.md)

## Verificar um documento

Se você tiver permissões de gerenciamento para um documento, poderá fazer check-out dele para proibir determinadas ações no documento. 

1. Vá para a área onde seu documento está armazenado e selecione o documento. 

   Para obter informações sobre como adicionar documentos, consulte [Adicionar documentos ao Adobe Workfront a partir do seu sistema de arquivos](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Clique no botão **Check-out** ícone ![](assets/check-out-25x23.png).

1. Um ícone de cadeado ![](assets/lock-icon-locked-qs.png) é exibido à direita do nome do documento. O documento fica com check-out depois que você sai do Workfront.
1. Somente o usuário que fez check-out do documento ou o administrador do Workfront pode fazer check-in do documento.

## Gerenciar documentos com check-out

Considere o seguinte sobre documentos com check-out:

* Antes de excluir um objeto em que um documento com check-out é armazenado, primeiro verifique o documento de volta. 
* Se o administrador do Workfront excluir um usuário que fez check-out de um documento que não era de sua propriedade, a Workfront verificará automaticamente o documento.
* Se o administrador do Workfront excluir um usuário que fez check-out de um documento que possui e o documento for carregado em um objeto, o documento permanecerá com check-out. Somente um administrador do Workfront pode fazer check-in.
* Se o administrador do Workfront excluir um usuário que fez check-out de um documento que possui e o documento for carregado somente na área Documentos (não em um objeto), o documento será excluído com o usuário.

   Para obter informações sobre como excluir usuários, consulte [Excluir usuários](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Se o administrador do Workfront desativar um usuário, os documentos com check-out permanecerão com check-out. Somente um administrador do Workfront pode fazer o check-in. 

## Verificar um documento em

Você deve verificar um documento novamente antes de fazer upload de uma nova versão ou excluí-la. 

Para fazer check-in de um documento:

1. Vá para a área onde o documento está armazenado e selecione o documento. 

   Um ícone de cadeado ![](assets/lock-icon-locked-qs.png) é exibido à direita do nome do documento.

1. Clique no botão **Fazer check-in** ícone ![](assets/check-in-25x22.png).
