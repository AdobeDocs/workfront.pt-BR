---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migração do conector herdado para o conector aprimorado
description: O processo a seguir descreve as práticas recomendadas para mudar do conector herdado do Adobe Experience Manager para o conector aprimorado para integrar o Adobe Workfront com o AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Migração do conector herdado para o conector aprimorado

O processo a seguir descreve as práticas recomendadas para mudar do conector herdado do Adobe Experience Manager para o conector aprimorado para integrar o Adobe Workfront com o AEM Assets.

>[!IMPORTANT]
>
>Esta documentação se aplica somente a clientes que usam ambientes Adobe Experience Manager Assets no local ou Managed Services.


Para clientes no Adobe Experience Manager Assets as a Cloud Service, o caminho de migração do conector herdado será para a nova integração nativa dentro do Workfront. Para saber mais sobre este processo de migração, consulte [Migrar do conector herdado ou aprimorado para o Workfront para integração com o Adobe Experience Manager as a Cloud Service](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Implementar o conector aprimorado

>[!IMPORTANT]
>
>Um parceiro certificado ou os serviços da Adobe Consulting são necessários para a implementação do conector aprimorado.
>
> Para parceiros que desejam se certificar no conector aprimorado, consulte o seguinte artigo: [Série de especialistas sobre conectores aprimorados do Workfront for Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

Para implementar o conector aprimorado, consulte [Configurar Workfront para conector aprimorado Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## Mover ativos existentes

Após configurar seu ambiente, é possível mover ativos e pastas vinculados existentes para o Adobe Experience Manager. Essa é uma etapa opcional, mas garantirá que as pastas e os ativos vinculados anteriormente por meio do conector herdado ainda estejam acessíveis assim que o conector herdado for desinstalado.

Para obter mais informações sobre como mover seus ativos, consulte [Migrar pastas e documentos vinculados](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validar todos os casos de uso críticos que devem ser usados

É importante validar todos os casos de uso críticos que devem ser usados por meio do conector aprimorado antes de desinstalar o conector herdado.

## Desinstale o conector herdado

Por último, é necessário desinstalar o conector herdado. O conector herdado não deve ser executado em paralelo com o conector aprimorado.

Para desinstalar, consulte [Desinstalar o Workfront com conector herdado do Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
