---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrar do conector herdado para o conector aprimorado
description: O processo a seguir descreve as práticas recomendadas para sair do conector herdado do Adobe Experience Manager para o conector aprimorado para integração do Adobe Workfront com o AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Migrar do conector herdado para o conector aprimorado

O processo a seguir descreve as práticas recomendadas para sair do conector herdado do Adobe Experience Manager para o conector aprimorado para integração do Adobe Workfront com o AEM Assets.

>[!IMPORTANT]
>
>Esta documentação se aplica somente aos clientes que usam ambientes Adobe Experience Manager Assets no local ou Managed Services.


Para clientes no Adobe Experience Manager Assets as a Cloud Service, o caminho de migração do conector herdado será para a nova integração nativa dentro do Workfront. Para saber mais sobre esse processo de migração, consulte [Migrar do conector herdado ou aprimorado para o Workfront para integração com o Adobe Experience Manager as a Cloud Service](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Implementar o conector aprimorado

>[!IMPORTANT]
>
>É necessário um parceiro certificado ou serviços de consultoria do Adobe para a implementação do conector aprimorado.
>
> Para parceiros que desejam certificar no conector aprimorado, consulte o seguinte artigo: [Workfront para Experience Manager Enhanced connector Expert Series](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

Para implementar o conector aprimorado, consulte [Configurar o Workfront para conector avançado Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## Mover ativos existentes

Após configurar seu ambiente, você pode mover ativos e pastas vinculados existentes para a Adobe Experience Manager. Essa é uma etapa opcional, mas garantirá que as pastas e os ativos vinculados anteriormente por meio do conector herdado ainda estejam acessíveis após a desinstalação do conector herdado.

Para obter mais informações sobre como mover seus ativos, consulte [Migrar pastas e documentos vinculados](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validar todos os casos de uso críticos destinados a serem usados

É importante validar todos os casos de uso críticos destinados a serem usados por meio do conector aprimorado antes de desinstalar o conector herdado.

## Desinstale o conector herdado

Por último, você precisa desinstalar o conector herdado. O conector herdado não deve funcionar em paralelo com o conector aprimorado.

Para desinstalar, consulte [Desinstale o Workfront com o conector herdado do Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
