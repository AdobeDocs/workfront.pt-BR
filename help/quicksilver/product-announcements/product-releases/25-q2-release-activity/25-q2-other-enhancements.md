---
title: Outras melhorias durante o período da versão do segundo trimestre de 2025
description: Other enhancements during the Second Quarter 2025 release time frame
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 23%

---

# Outras melhorias durante o período da versão do segundo trimestre de 2025

This page describes enhancements made with the Second Quarter 2025 release to the Preview environment. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste ponto do ciclo de lançamento do segundo trimestre de 2025, consulte [Visão geral da versão do segundo trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md).

## Upgrade to the new event subscription version with version upgrade endpoints

>[!NOTE]
>
>Produção para todos os clientes: sexta-feira, 6 de março de 2025

Workfront now has versions of event subscriptions. The new version is not a change to the Workfront API, but rather a change to the event subscription functionality.

A capacidade de atualizar ou fazer downgrade de assinaturas de evento garante que, quando alterações forem feitas na estrutura dos eventos, as assinaturas existentes não sejam interrompidas, permitindo testar e atualizar para a nova versão sem uma lacuna na assinatura do evento.

For more information on the differences between the two versions, see the article [Event subscription versioning](/help/quicksilver/wf-api/general/event-subs-versioning.md).

For information on the endpoints used to upgrade or downgrade an event subscription between versions, see the section [Event subscription versioning](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) in the article Event subscription API.

## Represent Adobe Admin Console user changes as &quot;System&quot; in the Workfront update feed

>[!NOTE]
>
>Preview release: January 23, 2025; Production for fast release: With the 25.2 release (February 13, 2025); Production for quarterly release: With the 25.4 release (April 2025)

Now, when the administrator of the Adobe Admin Console makes a change to the user information of a Workfront user, Workfront records this change in the System activity tab of the user&#39;s Updates area as belonging to the &quot;System&quot;. This refers to the Adobe Admin Console administrator.

Prior to this update, user changes made by the administrator of the Admin Console were recorded as made by the main Workfront system administrator.

For information about managing users in the Adobe Admin Console, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)
