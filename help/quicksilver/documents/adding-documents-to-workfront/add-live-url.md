---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Adicionar um link da Web como um documento
description: Você pode adicionar um site ao Adobe Workfront como um link da Web e solicitar aprovação para ele.
author: Courtney
feature: Digital Content and Documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 05f148f2c28555e37fb415f606e314a5df564047
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 8%
---
# Adicionar um link da Web como um documento

Você pode adicionar um site ao Adobe Workfront como um link da Web na nova área Documentos. Depois de adicioná-lo, você pode solicitar aprovação na página da Web ao vivo da mesma maneira que solicita aprovação em um arquivo carregado.

Se sua organização usar o armazenamento em nuvem do Adobe, você verá a nova área Documentos ao acessar documentos no Workfront. Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

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
   <p>Solicitação ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Armazenamento herdado do Workfront: editar acesso a documentos</p> 
   <p>Armazenamento em nuvem do Adobe: o acesso para Editar documentos está habilitado por padrão e não pode ser alterado</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar um link da Web como um documento

Você pode fazer upload de uma página da Web html para o Workfront como um link da Web. Depois de adicioná-lo, você pode solicitar aprovação na página da Web ao vivo da mesma maneira que solicita aprovação em um arquivo carregado. Para obter mais informações sobre como o Frame.io processa links da Web, consulte [HTML Review for Frame.io](https://support.frame.io/hc/en-us/articles/360041187574-Frame-io-Web-Links).


>[!IMPORTANT]
>
>* Os URLs são suportados se o site permitir incorporações de iFrame.
>* URLs da Web privados são suportados, mas determinados fluxos de autenticação podem não funcionar, dependendo da configuração do servidor.
>* No momento, não há suporte para URLs do Youtube e do Figma.<br>
>Para obter mais informações, consulte [HTML Review for Frame.io](https://help.frame.io/en/articles/12893213-html-review-for-frame-io).


Para adicionar um link da Web:

1. Vá para o projeto, tarefa ou problema ao qual deseja adicionar o site e selecione **Documentos** no painel esquerdo.
1. Clique em **Novo** e selecione **Link da Web**.
1. Digite um nome no campo **Nome do documento** e digite o endereço do site no campo **URL**.
1. Clique em **Adicionar**.
   ![Adicionar um link da Web como um documento](assets/web-url.png)

Para solicitar aprovação no link da Web, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

## Limitações conhecidas

* Há um problema temporário com documentos de link da Web criados no Frame.io. Se você criar um link da Web no Frame.io e, em seguida, criar uma aprovação nele no Workfront, o documento não será aberto no Frame.io. Os links da Web criados no Workfront não são afetados. Até que isso seja resolvido, crie documentos de link da Web no Workfront antes de iniciar uma aprovação.
* No momento, não é possível criar novas versões de documentos de links da Web no Frame.io. Se precisar criar uma nova versão de um documento de link da Web, crie a nova versão no Workfront.