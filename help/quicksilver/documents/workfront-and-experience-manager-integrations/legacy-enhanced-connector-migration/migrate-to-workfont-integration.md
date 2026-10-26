---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migração do conector herdado ou aprimorado para o Workfront para integração com o Adobe Experience Manager as a Cloud Service
description: As informações nesta página explicam as práticas recomendadas para mudar dos conectores aprimorados ou herdados do Workfront para Experience Cloud para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
TQID: 'https://experienceleague.adobe.com/0pAHfS7cDqv1tV4TBdx9WqvJA1-zySGsPHVXI8EG7Hc'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: e7123179a59cd7ed9c76f4718b3b8019854cbfe1
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%
---
# Migração do conector herdado ou aprimorado para o Workfront para integração com o Adobe Experience Manager as a Cloud Service

As informações nesta página explicam as práticas recomendadas para mudar dos conectores aprimorados ou herdados do Workfront para Experience Cloud para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Essas informações não se aplicam aos clientes que usam ambientes Adobe Experience Manager Assets no local ou Managed Services.

<!--

## Move your Workfront instance to the Admin Console

Customers that intend to use the new native integration between Workfront and Adobe Experience Manager Assets as a Cloud Service must ensure their Workfront environment is tied to an Adobe Admin Console. For existing Workfront environments, this will likely require a migration of the environment to a connected Adobe Admin Console. For more details regarding this migration and the associated checklist, see [Prepare to onboard your organization to the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md). 

 Adobe must help carry out this migration. To request help, do one of the following:

* If you have Workfront Hub access, submit your request to the [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* If you do not have Workfront Hub access, you can submit your request to the [Workfront to Adobe Admin Console Early Migration Request Queue](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

-->

## Configurar seu novo Workfront para integração do as a Cloud Service com o Adobe Experience Manager Assets

Depois que o ambiente do Workfront for migrado para uma Adobe Admin Console, os administradores do Workfront poderão configurar a nova integração nativa. Para obter ajuda sobre configuração, consulte [Configurar a integração do Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Mover ativos existentes para sua integração do as a Cloud Service com o Workfront for Adobe Experience Manager Assets

Após configurar seu ambiente, é possível mover ativos e pastas vinculados existentes para o Adobe Experience Manager. Essa é uma etapa opcional, mas garantirá que as pastas e os ativos vinculados anteriormente por meio do conector herdado ou aprimorado ainda estejam acessíveis assim que esses conectores forem desinstalados.

Para obter mais informações sobre como mover seus ativos, consulte [Migrar pastas e documentos vinculados](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validar todos os casos de uso críticos que devem ser usados

Será importante validar todos os casos de uso críticos que devem ser usados por meio da integração nativa antes de desinstalar o conector herdado ou aprimorado.

## Desinstale o conector herdado ou aprimorado

Por último, é necessário desinstalar o conector herdado ou aprimorado. A integração nativa não deve ser executada em paralelo com nenhum dos conectores.

Para desinstalar, consulte

* Instruções de desinstalação do conector herdado: [Desinstale o Workfront com o conector herdado do Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Instruções de desinstalação do conector aprimorado: [Desinstale o Workfront com o conector aprimorado do Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
