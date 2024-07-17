---
product-area: documents
navigation-topic: manage-documents
title: Gerenciar versões do documento
description: É possível gerenciar várias versões de um documento no Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Gerenciar versões do documento

É possível gerenciar várias versões de um documento no Workfront.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar acesso a documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar acesso ao documento</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Pré-requisitos

* Este artigo supõe que o documento tenha várias versões.

  Se você precisar de informações sobre como carregar novas versões de um documento no Workfront, consulte [Carregar uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md).

## Exibir uma lista de todas as versões de um documento

1. No Resumo, role até a exibição da seção **Todas as versões**. Aqui é possível exibir todas as versões do documento.

## Exibir e gerenciar detalhes de uma versão anterior do documento

1. Próximo à parte superior da página Detalhes do documento, clique no menu suspenso próximo ao nome e, em seguida, clique no nome da versão que deseja exibir e gerenciar.

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Além de visualizar os Detalhes da versão, você pode fazer alterações na versão, como nome, metadados e configurações de prova (se for uma prova de documento).

## Baixar uma única versão do documento

1. No Resumo, em **Versões**, clique no menu Mais ![](assets/more-icon.png) à direita da versão e clique em **Baixar** na lista suspensa exibida.

   ![](assets/more-versions-350x143.png)

## Baixar todas as versões de um documento

1. Clique em **Detalhes do documento** e selecione **Todas as versões** no painel esquerdo.

1. Clique em **Baixar tudo** na parte superior da lista.

## Excluir uma versão do documento

Se você fizer upload de uma versão de um documento por engano ou se uma versão não for mais necessária, exclua a versão e mantenha o documento original.

>[!IMPORTANT]
>
>Não é possível recuperar uma versão do documento que você exclui individualmente.

Lembre-se do seguinte ao considerar a exclusão de uma versão do documento:

* Somente uma versão pode ser excluída de cada vez. Se uma versão for excluída, esta ação aparecerá em **Atualizações** no documento.
* Se você fizer upload de uma nova versão após excluir uma versão, a nova versão receberá o próximo número sequencial. Por exemplo, se houver três versões de um documento e você excluir a versão 3, o próximo documento carregado será a versão 4.
* Atualizações do sistema e comentários feitos em uma versão são retidos no Workfront após a exclusão da versão.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Para excluir uma versão do documento:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.Localize o documento necessário.
1. Na área **Versão** do Resumo, clique na versão e em **Excluir** na lista suspensa exibida. A opção **Excluir** só estará visível se houver pelo menos duas versões.

   Se o documento estiver vinculado a uma origem externa, esse link será excluído e o documento não estará mais acessível por meio do Workfront.

   ![](assets/more-versions-350x143.png)
