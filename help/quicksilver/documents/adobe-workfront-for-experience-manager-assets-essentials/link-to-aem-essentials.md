---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Vincular ativos e pastas do Experience Manager Assets Essentials
description: Você pode vincular um ativo ou pasta do Experience Manager Assets Essentials a qualquer objeto do Adobe Workfront compatível com documentos. O Assets enviado do Assets Essentials não conta para o armazenamento geral de documentos no Workfront. Os documentos carregados e enviados do Workfront para o Assets Essentials contam para o armazenamento geral.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: a9dfc5c7838668bd3007c157a4e1a53ab4bd86f5
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 12%

---

# Vincular ativos e pastas do Experience Manager Assets Essentials

Você pode vincular um ativo ou pasta do Experience Manager Assets Essentials a qualquer objeto do Adobe Workfront compatível com documentos.

Para vincular ativos e pastas do Experience Manager Assets usando o Supervisor de Conteúdo, consulte [Vincular ativos e pastas ao Supervisor de Conteúdo habilitado pelo Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou posterior</p> 
   <p>Solicitação ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produtos adicionais</td> 
   <td>Você deve ter o Experience Manager as a Cloud Service ou o Assets Essentials e deve ser adicionado ao produto como usuário na Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Permissões do Experience Manager</td> 
    <td>Você deve ter acesso de gravação à pasta.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar:

* O administrador do Workfront deve configurar uma integração do Experience Manager. Para obter mais informações, consulte [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Vincular um ativo do Experience Manager Assets Essentials

1. Vá para a área **Documentos** no Workfront onde deseja adicionar o documento.
1. Selecione **Adicionar novo** e depois selecione a integração do Experience Manager que o administrador configurou.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, talvez ele não mencione especificamente o Experience Manager Assets Essentials.

1. Selecione os ativos desejados.

   ![Selecione um ativo](assets/select-an-asset.png)

1. Clique em **Selecionar**.

## Vincular uma nova versão do Experience Manager Assets Essentials

Você pode obter um novo ativo do Experience Manager Assets Essentials e adicioná-lo a um ativo existente como uma nova versão. Se o documento já estiver vinculado e uma nova versão for adicionada no Experience Manager Assets Essentials, a nova versão será exibida automaticamente no Workfront.

Para vincular uma nova versão:

1. Vá para a área **Documentos** no Workfront onde deseja adicionar o documento.
1. Selecione o ativo que deseja substituir por uma nova versão. Não é possível criar uma nova versão de um ativo em uma pasta vinculada.
1. Selecione **Adicionar novo** > **Versão** e selecione a integração do Experience Manager que seu administrador configurou.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, pode ser que ele não mencione especificamente o Experience Manager Assets Essentials.

1. Selecione o ativo que deseja vincular.

1. Clique em **Selecionar**.

## Vincular uma pasta do Experience Manager Assets Essentials

As permissões para visualizar ativos individuais dentro de uma pasta dependem das permissões do Experience Manager Assets Essentials.

1. Vá para a área **Documentos** no Workfront onde deseja colocar a pasta.
1. Selecione **Adicionar novo** e depois selecione a integração do Experience Manager que o administrador configurou.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, pode ser que ele não mencione especificamente o Experience Manager Assets Essentials.

1. Selecione as pastas desejadas.

   ![Selecionar uma pasta](assets/select-a-folder.png)

1. Clique em **Selecionar**.

## Considerações

* A funcionalidade Supervisor de conteúdo não está disponível para o Assets Essentials. Para vincular ativos e pastas usando o Supervisor de Conteúdo, consulte [Vincular ativos e pastas ao Supervisor de Conteúdo habilitado pelo Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

* O Assets enviado do Assets Essentials não conta para o armazenamento geral de documentos no Workfront. Os documentos carregados e enviados do Workfront para o Assets Essentials contam para o armazenamento geral.

* Os campos de metadados são mapeados pela primeira vez quando você envia um ativo do Workfront para o Experience Manager Assets Essentials. Se o administrador do Workfront tiver ativado a sincronização de metadados de objeto, os campos permanecerão atualizados se forem alterados em qualquer um dos aplicativos.
