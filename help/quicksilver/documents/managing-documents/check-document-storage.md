---
product-area: documents
navigation-topic: manage-documents
title: Verificar limites de armazenamento de documentos
description: Como administrador do Adobe Workfront, você visualiza a cota e o uso do armazenamento de documentos na página Informações do cliente. A forma como o armazenamento é exibido depende de sua organização usar o armazenamento herdado do Workfront ou o armazenamento em nuvem do Adobe.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 7%

---

# Verificar limites de armazenamento de documentos

{{highlighted-preview}}

Embora não haja restrições quanto aos tipos e tamanhos de arquivos individuais que os usuários podem fazer upload para sua instância do Workfront, seu plano da Workfront inclui uma cota de armazenamento total. Como administrador do Workfront, você monitora o uso e a cota na área Configuração da página Informações do cliente.

A forma como o armazenamento é exibido depende de sua organização usar o armazenamento herdado do Workfront ou o armazenamento em nuvem do Adobe:

* Se você usa o armazenamento herdado do Workfront, consulte [Armazenamento herdado do Workfront](#legacy-workfront-storage) neste artigo.
* Se você usa o Adobe Cloud Storage, consulte [Adobe Cloud Storage](#adobe-cloud-storage) neste artigo.

  Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">plano do Workfront</td> 
   <td> <p>Qualquer pacote do Workfront para gerenciar documentos usando o armazenamento herdado</p>
      <p>Qualquer pacote de fluxo de trabalho para gerenciar documentos usando o armazenamento em nuvem do Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Armazenamento herdado do Workfront

Se sua organização usa o armazenamento Workfront herdado, a página Informações do cliente mostra uma única cota de armazenamento para documentos carregados diretamente na Workfront.

Para verificar o armazenamento de documentos herdados do Workfront:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Sistema** > **Informações do cliente**.
1. Na seção **Informações Básicas**, encontre **Cota de Armazenamento**. Aqui, você pode visualizar o armazenamento que está usando no momento, bem como o volume total de armazenamento que seu plano Workfront inclui.

A cota de armazenamento é atualizada diariamente para mostrar a contagem mais atualizada.

>[!NOTE]
>
>Esse limite não se aplica a documentos vinculados ao Workfront por qualquer outro provedor de serviços de terceiros (SharePoint, Google Drive, Webdam, Box, Dropbox ou qualquer outro provedor de gerenciamento de ativos de documentos).

<div class="preview">

## armazenamento em nuvem Adobe


Se sua organização usa o Adobe Cloud Storage, sua cota de armazenamento é relatada como uma alocação em pool única que combina armazenamento provisionado por meio de sua licença da Workfront e qualquer armazenamento provisionado por meio de um complemento Frame.io Enterprise. Não há limite rígido de uso do armazenamento; os usuários podem continuar carregando documentos mesmo quando o uso excede sua cota.

### Visualizar o uso do armazenamento nas informações do cliente

Para verificar documentos no armazenamento em nuvem do Adobe:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Sistema** > **Informações do cliente**.
1. Vá para a seção **Visão geral do armazenamento**.
1. Revise seu uso. A Visão geral de armazenamento mostra a cota de armazenamento em pool e divide o uso em:

   * Os projetos herdados do Workfront e os projetos de armazenamento na nuvem do Adobe são exibidos na barra azul.
   * Os projetos autônomos do quadro são exibidos na barra verde. Esses projetos são separados do Workfront e só estarão disponíveis se você tiver uma licença Frame.io Enterprise.


![uso do Adobe Cloud Storage nas Informações do cliente](assets/storage-usage.png)

Os números de uso são atualizados regularmente para que você veja uma contagem atualizada.

### Notificações por email para administradores

Quando o uso ultrapassa 75%, 90% ou 100% da cota de armazenamento, a Workfront envia uma notificação por e-mail para os administradores do sistema.

</div>