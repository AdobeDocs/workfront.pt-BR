---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migração do conector herdado ou aprimorado para o Workfront para integração com o Adobe Experience Manager as a Cloud Service
description: As informações nesta página explicam as práticas recomendadas para mudar dos conectores aprimorados ou herdados do Workfront for Experience Cloud para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Migração do conector herdado ou aprimorado para o Workfront para integração com o Adobe Experience Manager as a Cloud Service

As informações nesta página explicam as práticas recomendadas para mudar dos conectores aprimorados ou herdados do Workfront for Experience Cloud para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Essas informações não se aplicam aos clientes que usam ambientes Adobe Experience Manager Assets no local ou Managed Services.

## Mover sua instância do Workfront para a Admin Console

Os clientes que pretendem usar a nova integração nativa entre o Workfront e o Adobe Experience Manager Assets as a Cloud Service devem garantir que seu ambiente do Workfront esteja vinculado a uma Adobe Admin Console. Para ambientes Workfront existentes, isso provavelmente exigirá uma migração do ambiente para um Adobe Admin Console conectado. Para obter mais detalhes sobre esta migração e a lista de verificação associada, consulte [Preparar para integrar sua organização à Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

A Adobe deve ajudar a realizar essa migração. Para solicitar ajuda, siga um destes procedimentos:

* Se você tiver acesso ao Workfront Hub, envie sua solicitação para a [Migração do Workfront para o Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* Se você não tiver acesso ao Hub do Workfront, poderá enviar sua solicitação para a [Fila de solicitações de migração antecipada do Workfront Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

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
