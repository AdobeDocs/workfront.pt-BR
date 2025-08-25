---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migração do conector herdado ou aprimorado para o Workfront para integração com o Adobe Experience Manager as a Cloud Service
description: As informações nesta página explicam as práticas recomendadas para mudar dos conectores aprimorados ou herdados do Workfront for Experience Cloud para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: f381b37e6d4537e6f83e55ed4a2f4ff7f868dd54
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Migração do conector herdado ou aprimorado para o Workfront para integração com o Adobe Experience Manager as a Cloud Service

As informações nesta página explicam as práticas recomendadas para mudar dos conectores aprimorados ou herdados do Workfront for Experience Cloud para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Essas informações não se aplicam aos clientes que usam ambientes Adobe Experience Manager Assets no local ou Managed Services.

## Mover sua instância do Workfront para a Admin Console

>[!IMPORTANT]
>
>Como todas as organizações da Workfront foram migradas para o Adobe Admin Console, esta seção será removida em breve.

<!--DELETE THIS SECTION MARCH 2026-->

<!--
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
