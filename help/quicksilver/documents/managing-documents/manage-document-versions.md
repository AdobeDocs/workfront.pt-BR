---
product-area: documents
navigation-topic: manage-documents
title: Gerenciar versões do documento
description: É possível gerenciar várias versões de um documento no Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: a9dbfe21337be9cd9929f4e982e4979265ca14e1
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 0%

---

# Gerenciar versões do documento

<!-- Audited: 5/2025 -->

É possível gerenciar várias versões de um documento no Workfront.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront</td> 
   <td> 
   <p>Novo: Colaborador ou superior<p>
   <p>Ou</p>
   <p>Atual: solicitação ou superior </p>


</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualizar acesso a documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar acesso ao documento</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

* Este artigo supõe que o documento tenha várias versões.

  Se você precisar de informações sobre como carregar novas versões de um documento no Workfront, consulte [Carregar uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md).

## Exibir uma lista de todas as versões de um documento

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.

1. No canto superior direito da página, clique no ícone **Abrir resumo** ![Abrir resumo](assets/qs-summary-in-new-toolbar-small.png). O painel lateral **Resumo do documento** é aberto.

1. Role para baixo até a seção **Versões** para exibir todas as versões do documento.

## Exibir e gerenciar detalhes de uma versão anterior do documento

{{step1-to-documents}}

1. Passe o mouse sobre o documento e clique em **Detalhes do documento**.

1. Próximo à parte superior da página **Detalhes do documento**, clique no menu suspenso próximo ao nome e, em seguida, clique no nome da versão que deseja exibir e gerenciar.

   ![Menu suspenso Versão na página Detalhes do Documento](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Além de visualizar os detalhes da versão, você pode fazer alterações na versão, como nome, metadados e configurações de prova (se for uma prova de documento).

## Baixar uma única versão do documento

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.

1. No canto superior direito da página, clique no ícone **Abrir resumo** ![Abrir resumo](assets/qs-summary-in-new-toolbar-small.png). O painel lateral **Resumo do documento** é aberto.

1. Na seção **Versões**, clique no menu **Mais** ![Mais menu](assets/more-icon.png) à direita da versão e clique em **Download** na lista suspensa exibida.

   ![Baixar um único documento](assets/more-versions-350x143.png)

## Baixar todas as versões de um documento

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.

1. No canto superior direito da página, clique no ícone **Abrir resumo** ![Abrir resumo](assets/qs-summary-in-new-toolbar-small.png). O painel lateral **Resumo do documento** é aberto.

1. Role para baixo até a seção **Versões** e clique em **Baixar tudo**.

## Excluir uma versão do documento

Se você fizer upload de uma versão de um documento por engano ou se uma versão não for mais necessária, exclua a versão e mantenha o documento original.

>[!IMPORTANT]
>
>Não é possível recuperar uma versão do documento que você exclui individualmente.

Lembre-se do seguinte ao considerar a exclusão de uma versão do documento:

* Somente uma versão pode ser excluída de cada vez. Se uma versão for excluída, essa ação aparecerá na seção Atualizações no documento.
* Se você fizer upload de uma nova versão após excluir uma versão, a nova versão receberá o próximo número sequencial. Por exemplo, se houver três versões de um documento e você excluir a versão 3, o próximo documento carregado será a versão 4.
* Atualizações do sistema e comentários feitos em uma versão são retidos no Workfront após a exclusão da versão.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Para excluir uma versão do documento:

{{step1-to-documents}}

1. Na página **Documentos**, selecione o documento na lista.

1. No canto superior direito da página, clique no ícone **Abrir resumo** ![Abrir resumo](assets/qs-summary-in-new-toolbar-small.png). O painel lateral **Resumo do documento** é aberto.

1. Role para baixo até a seção **Versões** para exibir todas as versões do documento.
1. Na seção **Versões**, clique no menu **Mais** ![Mais menu](assets/more-icon.png) à direita da versão e clique em **Excluir** na lista suspensa exibida.

   >[!NOTE]
   >
   >* A opção **Excluir** só estará visível se houver pelo menos duas versões.
   >* Se o documento estiver vinculado a uma origem externa, esse link será excluído e o documento não estará mais acessível por meio do Workfront.

   ![Excluir a versão do documento](assets/more-versions-350x143.png)
