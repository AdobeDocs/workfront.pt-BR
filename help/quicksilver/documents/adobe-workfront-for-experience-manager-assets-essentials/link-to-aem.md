---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Vincular ativos e pastas do Experience Manager Assets ou do Assets Essentials
description: Você pode vincular um ativo ou pasta do Experience Manager Assets ou do Assets Essentials a qualquer objeto do Adobe Workfront compatível com documentos. O Assets enviado do Assets Essentials não conta para o armazenamento geral de documentos no Workfront. Os documentos carregados e enviados do Workfront para o Assets Essentials contam para o armazenamento geral.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Vincular ativos e pastas do Experience Manager Assets ou do Assets Essentials

Você pode vincular um ativo ou pasta do Experience Manager Assets ou do Assets Essentials a qualquer objeto do Adobe Workfront compatível com documentos. O Assets enviado do Assets Essentials não conta para o armazenamento geral de documentos no Workfront. Os documentos carregados e enviados do Workfront para o Assets Essentials contam para o armazenamento geral.

Os campos de metadados são mapeados pela primeira vez quando você envia um ativo do Workfront para o Experience Manager Assets ou o Assets Essentials. Se o administrador do Workfront tiver ativado a sincronização de metadados de objeto, os campos permanecerão atualizados se forem alterados em qualquer um dos aplicativos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td role="rowheader">Produto</td> 
   <td>Você deve ter o Experience Manager as a Cloud Service ou o Assets Essentials e deve ser adicionado ao produto como usuário na Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Permissões do Experience Manager</td> 
    <td>Você deve ter acesso de gravação à pasta.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ou superior</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

+++

## Pré-requisitos

Antes de começar,

* O administrador do Workfront deve configurar uma integração do Experience Manager. Para obter mais informações, consulte [Configurar a integração do Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Vincular um ativo do Experience Manager Assets ou do Assets Essentials

Você pode vincular um ativo do Experience Manager Assets ou do Assets Essentials ao Workfront. Depois que o ativo for vinculado, você poderá

* [Criar uma prova de um ativo vinculado do Experience Manager Assets ou do Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Fazer upload de uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md)

1. Vá para a área **Documentos** no Workfront onde deseja adicionar o documento.
1. Selecione **Adicionar novo** e depois selecione a integração do Experience Manager que o administrador configurou.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, talvez ele não mencione especificamente o Assets ou o Assets Essentials.

1. Selecione os ativos desejados.

   ![Selecione um ativo](assets/select-an-asset.png)

1. Clique em **Selecionar**.

## Vincular uma pasta do Experience Manager Assets ou do Assets Essentials

As permissões para exibir ativos individuais dentro de uma pasta dependem das permissões do Experience Manager Assets ou do Assets Essentials.

1. Vá para a área **Documentos** no Workfront onde deseja colocar a pasta.
1. Selecione **Adicionar novo** e depois selecione a integração do Experience Manager que o administrador configurou.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, pode não mencionar especificamente o Assets ou o Assets Essentials.

1. Selecione as pastas desejadas.

   ![Selecionar uma pasta](assets/select-a-folder.png)

1. Clique em **Selecionar**.

## Vincular uma nova versão do Experience Manager Assets ou do Assets Essentials

Você pode obter um novo ativo do Assets Essentials e adicioná-lo a um ativo existente como uma nova versão. Se o documento já estiver vinculado e uma nova versão for adicionada ao Assets Essentials, a nova versão será exibida automaticamente no Workfront.

Para vincular uma nova versão do Assets Essentials:

1. Vá para a área **Documentos** no Workfront onde deseja adicionar o documento.
1. Selecione o ativo que deseja substituir por uma nova versão. Não é possível criar uma nova versão de um ativo em uma pasta vinculada.
1. Selecione **Adicionar novo** > **Versão** e selecione a integração do Experience Manager que seu administrador configurou.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, pode não mencionar especificamente o Assets ou o Assets Essentials.

1. Selecione o ativo desejado.

   ![Selecione um ativo](assets/select-an-asset.png)

1. Clique em **Selecionar**.

>[!TIP]
>
>Você pode exibir todas as versões de um ativo se acessar **Detalhes do documento** > **Versões**.
