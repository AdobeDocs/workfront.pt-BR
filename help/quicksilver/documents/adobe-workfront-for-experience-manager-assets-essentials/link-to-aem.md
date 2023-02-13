---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Vincular ativos e pastas da Experience Manager Assets ou Assets Essentials
description: Você pode vincular um ativo ou uma pasta do Experience Manager Assets ou Assets Essentials a qualquer objeto do Adobe Workfront que seja compatível com documentos. Os ativos enviados do Assets Essentials não contam para o armazenamento geral de documentos no Workfront. Os documentos carregados e enviados do Workfront para o Assets Essentials não contam no armazenamento geral.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Vincular ativos e pastas da Experience Manager Assets ou Assets Essentials

Você pode vincular um ativo ou uma pasta do Experience Manager Assets ou Assets Essentials a qualquer objeto do Adobe Workfront que seja compatível com documentos. Os ativos enviados do Assets Essentials não contam para o armazenamento geral de documentos no Workfront. Os documentos carregados e enviados do Workfront para o Assets Essentials não contam no armazenamento geral.

Os campos de metadados são mapeados pela primeira vez ao enviar um ativo do Workfront para a Experience Manager Assets ou Assets Essentials. Se o administrador do Workfront ativou a sincronização de metadados de objetos, os campos permanecerão atualizados se forem alterados em qualquer um dos aplicativos.

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
   <td role="rowheader">Produto</td> 
   <td>Você deve ter o Experience Manager as a Cloud Service ou Assets Essentials e deve ser adicionado ao produto como um usuário no Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Permissões de Experience Manager</td> 
    <td>Você deve ter acesso de gravação à pasta.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ou superior</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar,

* O administrador do Workfront deve configurar uma integração com o Experience Manager. Para obter mais informações, consulte [Configurar a integração as a Cloud Service do Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Vincular um ativo da Experience Manager Assets ou Assets Essentials

Você pode vincular um ativo do Experience Manager Assets ou Assets Essentials ao Workfront. Depois que o ativo é vinculado, é possível

* [Prova de um ativo vinculado para Experience Manager Assets ou Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Fazer upload de uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md)

1. Vá para o **Documentos** no Workfront, onde deseja adicionar o documento.
1. Selecionar **Adicionar novo** e selecione a integração do Experience Manager configurada pelo administrador.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, de modo que pode não mencionar especificamente o Assets ou o Assets Essentials.

1. Selecione os ativos desejados.

   ![](assets/select-an-asset.png)

1. Clique em **Selecionar**.

## Vincular uma pasta do Experience Manager Assets ou Assets Essentials

As permissões para exibir ativos individuais dentro de uma pasta dependem das permissões do Experience Manager Assets ou Assets Essentials.

1. Vá para o **Documentos** no Workfront, onde deseja colocar a pasta.
1. Selecionar **Adicionar novo** e selecione a integração do Experience Manager configurada pelo administrador.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, de modo que talvez não mencione especificamente os Ativos ou o Assets Essentials.

1. Selecione as pastas desejadas.

   ![](assets/select-a-folder.png)

1. Clique em **Selecionar**.

## Vincular uma nova versão do Experience Manager Assets ou Assets Essentials

Você pode extrair um novo ativo do Assets Essentials e adicioná-lo a um ativo existente como uma nova versão. Se o documento já estiver vinculado e uma nova versão for adicionada ao Assets Essentials, a nova versão será exibida automaticamente no Workfront.

Para vincular uma nova versão do Assets Essentials:

1. Vá para o **Documentos** no Workfront, onde deseja adicionar o documento.
1. Selecione o ativo que deseja substituir por uma nova versão. Não é possível criar uma nova versão de um ativo em uma pasta vinculada.
1. Selecionar **Adicionar novo** > **Versão** e selecione a integração do Experience Manager configurada pelo administrador.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, de modo que talvez não mencione especificamente os Ativos ou o Assets Essentials.

1. Selecione o ativo que deseja.

   ![](assets/select-an-asset.png)

1. Clique em **Selecionar**.

>[!TIP]
>
>É possível exibir todas as versões de um ativo em **Detalhes do documento** > **Versões**.
