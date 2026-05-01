---
product-area: documents
navigation-topic: manage-documents
title: Verificar limites de armazenamento de documentos
description: Como administrador do Adobe Workfront, você visualiza a cota e o uso do armazenamento de documentos na página Informações do cliente. A forma como o armazenamento é exibido depende de sua organização usar o armazenamento Workfront herdado ou o armazenamento corporativo Adobe.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: e25be455e16beee813e612b983bca1302f129e6f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 8%

---

# Verificar limites de armazenamento de documentos

{{highlighted-preview}}

Embora não haja restrições quanto aos tipos e tamanhos de arquivos individuais que os usuários podem fazer upload para sua instância do Workfront, seu plano da Workfront inclui uma cota de armazenamento total. Como administrador do Workfront, você monitora o uso e a cota na área Configuração da página Informações do cliente.

A forma como o armazenamento é exibido depende de sua organização usar o armazenamento Workfront herdado ou o armazenamento corporativo Adobe:

* Se você usa o armazenamento herdado do Workfront, consulte [Armazenamento herdado do Workfront](#legacy-workfront-storage) neste artigo.
* Se você usa o Adobe enterprise storage, consulte [Adobe enterprise storage](#adobe-enterprise-storage) neste artigo.

  Para obter mais informações sobre o armazenamento corporativo, consulte [visão geral sobre o armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">plano do Workfront</td> 
   <td> <p>Qualquer pacote do Workfront para gerenciar documentos usando o armazenamento herdado</p>
      <p>Qualquer pacote de fluxo de trabalho para gerenciar documentos usando o armazenamento corporativo da Adobe</p> </td> 
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

## armazenamento corporativo Adobe

Se sua organização usa o armazenamento corporativo da Adobe, as informações do cliente mostram uma visão geral do armazenamento que divide o uso em diferentes seções para armazenamento Workfront herdado, armazenamento corporativo Adobe e Frame.io. O Workfront também aplica um limite flexível para uploads quando o uso excede a cota, para que os usuários ainda possam carregar documentos.

### Visualizar o uso do armazenamento nas informações do cliente

Para verificar o armazenamento de documentos corporativos do Adobe:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Sistema** > **Informações do cliente**.
1. Vá para a seção **Visão geral do armazenamento**.
1. Visualize o uso do armazenamento corporativo da Adobe.
   <!--Both Workfront and Frame.io usage are broken down separately, but roll up to the total usage for Adobe enterprise storage.-->

![uso do armazenamento corporativo da Adobe nas Informações do cliente](assets/storage-usage.png)

Os números de uso são atualizados regularmente para que você veja uma contagem atualizada.

### Notificações por email para administradores

Quando o uso ultrapassa 75%, 85% ou 100% da cota de armazenamento, a Workfront envia uma notificação por e-mail para os administradores do sistema.

</div>