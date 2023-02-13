---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrar do conector herdado ou aprimorado para o Workfront para integração com o Adobe Experience Manager as a Cloud Service
description: As informações nesta página explicam as práticas recomendadas para migrar da Workfront para conectores herdados ou aprimorados do Experience Cloud para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Migrar do conector herdado ou aprimorado para o Workfront para integração com o Adobe Experience Manager as a Cloud Service

As informações nesta página explicam as práticas recomendadas para migrar da Workfront para conectores herdados ou aprimorados do Experience Cloud para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Essas informações não se aplicam aos clientes que usam os ambientes Adobe Experience Manager Assets no local ou Managed Services.

## Mova a instância do Workfront para o Admin Console

Os clientes que pretendem usar a nova integração nativa entre o Workfront e o Adobe Experience Manager Assets as a Cloud Service devem garantir que seu ambiente Workfront esteja vinculado a uma Adobe Admin Console. Para ambientes Workfront existentes, isso provavelmente exigirá uma migração do ambiente para um Adobe Admin Console conectado. Para obter mais detalhes sobre essa migração e a lista de verificação associada, consulte [Preparar-se para integrar sua organização à Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

O Adobe deve ajudar a realizar essa migração. Para solicitar ajuda, siga um destes procedimentos:

* Caso tenha acesso ao Workfront Hub, envie sua solicitação para a [Migração do Workfront para o Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* Caso não tenha acesso ao Workfront Hub, envie sua solicitação para o [Fila de solicitações de migração antecipada do Workfront para o Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Configurar a nova Workfront para integração as a Cloud Service do Adobe Experience Manager Assets

Depois que o ambiente do Workfront for migrado para um Adobe Admin Console, os administradores do Workfront poderão configurar a nova integração nativa. Para obter ajuda sobre configuração, consulte [Configurar a integração as a Cloud Service do Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Mover ativos existentes para a Workfront para a integração as a Cloud Service de ativos da Adobe Experience Manager

Após configurar seu ambiente, você pode mover ativos e pastas vinculados existentes para a Adobe Experience Manager. Esta é uma etapa opcional, mas garantirá que as pastas e os ativos vinculados anteriormente por meio do conector herdado ou aprimorado ainda estejam acessíveis após a desinstalação desses conectores.

Para obter mais informações sobre como mover seus ativos, consulte [Migrar pastas e documentos vinculados](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validar todos os casos de uso críticos destinados a serem usados

É importante validar todos os casos de uso críticos destinados a serem usados por meio da integração nativa antes de desinstalar o conector herdado ou aprimorado.

## Desinstale o conector herdado ou aprimorado

Por último, é necessário desinstalar o conector herdado ou aprimorado. A integração nativa não deve ser executada em paralelo com qualquer um dos conectores.

Para desinstalar, consulte

* Instruções de desinstalação do conector herdado: [Desinstale o Workfront com o conector herdado do Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Instruções de desinstalação do conector aprimorado: [Desinstale o Workfront com o conector aprimorado Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
