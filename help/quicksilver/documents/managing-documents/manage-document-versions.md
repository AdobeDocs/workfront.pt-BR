---
product-area: documents
navigation-topic: manage-documents
title: Gerenciar versões do documento
description: Você pode gerenciar várias versões de um documento no Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# Gerenciar versões do documento

Você pode gerenciar várias versões de um documento no Workfront.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p> Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Exibir acesso a documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ao Documento</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

* Este artigo pressupõe que o documento tenha várias versões.

   Se você precisar de informações sobre o upload de novas versões de um documento para o Workfront, consulte [Fazer upload de uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md).

## Exibir uma lista de todas as versões de um documento

1. No Resumo, role até a exibição da variável **Todas as versões** seção. Aqui você pode exibir todas as versões do documento.

## Exibir e gerenciar detalhes de uma versão anterior do documento

1. Próximo à parte superior da página Detalhes do documento, clique no menu suspenso ao lado do nome e, em seguida, clique no nome da versão que deseja visualizar e gerenciar.

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Juntamente com a exibição dos Detalhes da versão, é possível fazer alterações na versão, como nome, metadados e configurações de prova (se for uma prova de documento).

## Baixar uma versão de documento único

1. No Resumo, em **Versões**, clique no menu Mais ![](assets/more-icon.png) à direita da versão e clique em **Baixar** na lista suspensa que é exibida.

   ![](assets/more-versions-350x143.png)

## Baixar todas as versões de um documento

1. Clique em **Detalhes do documento**, em seguida selecione **Todas as versões** no painel esquerdo.

1. Clique em **Baixar tudo** na parte superior da lista.

## Excluir uma versão do documento

Se você carregar uma versão de um documento por engano ou uma versão não for mais necessária, você poderá excluir a versão e manter o documento original.

>[!IMPORTANT]
>
>Não é possível recuperar uma versão do documento que você exclui individualmente.

Lembre-se do seguinte ao considerar excluir uma versão do documento:

* Somente uma versão pode ser excluída de cada vez. Se uma versão for excluída, essa ação aparecerá no **Atualizações** no documento .
* Se você carregar uma nova versão após excluir uma versão, a nova versão receberá o próximo número sequencial. Por exemplo, se houver 3 versões de um documento e você excluir a versão 3, o próximo documento carregado será a versão 4.
* As atualizações do sistema e os comentários feitos em uma versão são retidos no Workfront depois que a versão é excluída.

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Para excluir uma versão de documento:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.Localize o documento necessário.
1. No **Versão** no Resumo, clique na versão e, em seguida, clique em **Excluir** na lista suspensa que é exibida. O **Excluir** estará visível somente se houver pelo menos duas versões.

   Se o documento estiver vinculado a uma fonte externa, esse link será excluído e o documento não estará mais acessível por meio do Workfront.

   ![](assets/more-versions-350x143.png)
