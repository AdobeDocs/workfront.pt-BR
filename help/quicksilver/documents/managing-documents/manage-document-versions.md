---
product-area: documents
navigation-topic: manage-documents
title: Gerenciar versões de documentos
description: É possível gerenciar várias versões de um documento no Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
TQID: https://experienceleague.adobe.com/rCnj3Gx1SB3-UziuppQfifv2hJ6q3OjepNO9FcEEHEk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: c83b252faf7791c51475c5b82ca03cb4ee29bfc0
workflow-type: tm+mt
source-wordcount: 1077
ht-degree: 4%

---

# Gerenciar versões de documentos

<!-- Audited: 5/2025 -->

{{highlighted-preview}}

É possível gerenciar várias versões de um documento no Workfront.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer pacote do Workfront para gerenciar documentos usando o armazenamento herdado do Workfront</p>
<p>Qualquer pacote de fluxo de trabalho para gerenciar documentos usando o armazenamento em nuvem do Adobe</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou posterior</p>
   <p>Solicitação ou posterior </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualizar acesso a documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar acesso ao documento</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

* Este artigo supõe que o documento tenha várias versões.

  Se você precisar de informações sobre como carregar novas versões de um documento no Workfront, consulte [Carregar uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md).

## Gerenciar versões do documento na área de documentos herdados

### Exibir uma lista de todas as versões de um documento

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.

1. No canto superior direito da página, clique no ícone **Abrir resumo** ![Abrir resumo](assets/qs-summary-in-new-toolbar-small.png). O painel lateral **Resumo do documento** é aberto.

1. Role para baixo até a seção **Versões** para exibir todas as versões do documento.

### Exibir e gerenciar detalhes de uma versão anterior do documento

{{step1-to-documents}}

1. Passe o mouse sobre o documento e clique em **Detalhes do documento**.

1. Próximo à parte superior da página **Detalhes do documento**, clique no menu suspenso próximo ao nome e, em seguida, clique no nome da versão que deseja exibir e gerenciar.

   ![Menu suspenso Versão na página Detalhes do Documento](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Além de visualizar os detalhes da versão, você pode fazer alterações na versão, como nome, metadados e configurações de prova (se for uma prova de documento).

### Baixar uma única versão do documento

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.

1. No canto superior direito da página, clique no ícone **Abrir resumo** ![Abrir resumo](assets/qs-summary-in-new-toolbar-small.png). O painel lateral **Resumo do documento** é aberto.

1. Na seção **Versões**, clique no menu **Mais** ![Mais menu](assets/more-icon.png) à direita da versão e clique em **Download** na lista suspensa exibida.

   ![Baixar um único documento](assets/more-versions-350x143.png)

### Baixar todas as versões de um documento

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.

1. No canto superior direito da página, clique no ícone **Abrir resumo** ![Abrir resumo](assets/qs-summary-in-new-toolbar-small.png). O painel lateral **Resumo do documento** é aberto.

1. Role para baixo até a seção **Versões** e clique em **Baixar tudo**.

### Excluir uma versão do documento

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

<div class="preview">

## Gerenciar versões do documento na nova área Documentos em Visualização

Se sua organização usar o armazenamento em nuvem do Adobe, você verá a nova área Documentos ao acessar documentos no Workfront. Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

O Workfront numera cada versão na ordem em que ela é carregada (por exemplo, V1, V2, V3) para corresponder aos números de versão no Frame.io.

### Exibir uma lista de todas as versões de um documento

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.

1. Clique no ícone **Versões** ![Ícone Versões](assets/versions-icon.png) no lado direito da página. O painel Versões é aberto e lista cada versão do documento no Histórico de versões.

   >[!NOTE]
   >
   >Se uma versão tiver um workflow de aprovação, seu status, como &quot;Aprovado&quot; ou &quot;Retirado&quot;, aparecerá ao lado dela. As versões sem um fluxo de trabalho de aprovação não exibem um status.

### Solicitar aprovação em uma versão

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.
1. Clique no ícone **Versões** ![Ícone Versões](assets/versions-icon.png) no lado direito da página.
1. Clique no menu **Mais** ao lado da versão e clique em **Solicitar Aprovação**.
1. Configure o fluxo de trabalho de aprovação. Para obter mais informações, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

   >[!NOTE]
   >
   >Se uma versão anterior já tiver um fluxo de trabalho de aprovação aberto, solicitando aprovação para essa versão, ela será retirada. A versão anterior mantém seu número de versão e seu histórico de aprovação, mas seu status muda para &quot;Retirado&quot;.

### Exibir e gerenciar detalhes de uma versão anterior do documento

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.
1. Clique no ícone **Versões** ![Ícone Versões](assets/versions-icon.png) no lado direito da página.
1. Clique no menu **Mais** ao lado da versão e clique em **Exibir Detalhes**.

### Baixar uma única versão do documento

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.

1. Clique no ícone **Versões** ![Ícone Versões](assets/versions-icon.png) no lado direito da página.

1. Clique no menu **Mais** ao lado da versão e em **Baixar**.

### Baixar todas as versões de um documento

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.

1. Clique no ícone **Versões** ![Ícone Versões](assets/versions-icon.png) no lado direito da página.

1. Clique em **Baixar tudo** na parte superior do painel Versões.

   ![baixar todas as versões de um documento](assets/download-all-versions.png)

### Excluir uma versão do documento

{{step1-to-documents}}

1. Na página **Documentos**, selecione um documento na lista.

1. Clique no ícone **Versões** ![Ícone Versões](assets/versions-icon.png) no lado direito da página.

1. Clique no menu **Mais** ao lado da versão e em **Excluir**.

   >[!NOTE]
   >
   >A exclusão de uma versão não altera os números das outras versões. Por exemplo, se você excluir a V3 de um documento com as versões V1 a V5, as versões restantes manterão seus números originais e não haverá a V3 posteriormente. A próxima versão da qual você fizer upload será a V6.

</div>
