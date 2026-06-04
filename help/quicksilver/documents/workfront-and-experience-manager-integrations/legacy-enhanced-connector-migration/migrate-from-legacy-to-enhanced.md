---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migração do conector legado para o conector aprimorado
description: O processo a seguir descreve as práticas recomendadas para mudar do conector herdado do Adobe Experience Manager para o conector aprimorado para integrar o Adobe Workfront com o AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
TQID: https://experienceleague.adobe.com/px8ysyDqpwzajmCfRPJLclKOUSuIFacl99Uf6sRCKFQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 356
ht-degree: 5%

---

# Migração do conector legado para o conector aprimorado

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
> Para parceiros que desejam se certificar no conector aprimorado, consulte o seguinte artigo: [Série de especialistas em conectores aprimorados do Workfront for Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview).

Para implementar o conector aprimorado, consulte [Configurar conector aprimorado do Workfront para Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/integrations/workfront-connector-configure).


## Mover ativos existentes

Após configurar seu ambiente, é possível mover ativos e pastas vinculados existentes para o Adobe Experience Manager. Essa é uma etapa opcional, mas garantirá que as pastas e os ativos vinculados anteriormente por meio do conector herdado ainda estejam acessíveis assim que o conector herdado for desinstalado.

Para obter mais informações sobre como mover seus ativos, consulte [Migrar pastas e documentos vinculados](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validar todos os casos de uso críticos que devem ser usados

É importante validar todos os casos de uso críticos que devem ser usados por meio do conector aprimorado antes de desinstalar o conector herdado.

## Desinstale o conector herdado

Por último, é necessário desinstalar o conector herdado. O conector herdado não deve ser executado em paralelo com o conector aprimorado.

Para desinstalar, consulte [Desinstalar o Workfront com conector herdado do Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
