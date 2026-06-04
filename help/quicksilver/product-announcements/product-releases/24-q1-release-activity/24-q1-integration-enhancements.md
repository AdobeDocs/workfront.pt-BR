---
title: Aprimoramentos na integração do primeiro trimestre de 2024
description: Aprimoramentos na integração do primeiro trimestre de 2024
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
TQID: https://experienceleague.adobe.com/ZPt9H-R2eSNNha-gjfwkgnUOQqvU5tzAQPE5fMA-9uA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 385
ht-degree: 0%

---

# Aprimoramentos na integração do primeiro trimestre de 2024

Esta página descreve todas as melhorias de integração feitas com a versão do Primeiro trimestre de 2024 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção com a versão do primeiro trimestre de 2024.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do Primeiro trimestre de 2024, consulte [Visão geral da versão do Primeiro trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## O mapeamento de metadados no Experience Manager Assets Essentials agora usa `xcm:keywords` em vez de `dc:subject`

Atualizamos a integração do Experience Manager Assets Essentials para corresponder à experiência na integração do Experience Manager Assets as a Cloud Service. Agora, ao mapear vários campos de texto de linha única para um único campo no Experience Manager Assets, ambos os serviços usam o campo `xcm:keywords`.

Anteriormente, esses campos seriam mapeados para o campo `dc:subject` no Experience Manager Assets Essentials. A funcionalidade do Experience Manager Assets as a Cloud Service permanece inalterada.

Qualquer metadado do Experience Manager Assets Essentials atualmente mapeado para `dc:subject` deve ser remapeado para `xcm:keywords`.

Para obter informações sobre como mapear metadados para o Experience Manager Assets Essentials, consulte [AEM Keyword](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## Campos de digitação antecipada agora disponíveis na Integração do Adobe Experience Manager

Para facilitar a vinculação de campos entre o Workfront e o Adobe Experience Manager, adicionamos suporte para campos de digitação antecipada no mapeamento de metadados. Agora é possível mapear campos de digitação antecipada para campos correspondentes no Adobe Experience Manager.

Se um usuário selecionar um valor diferente para um campo no Workfront, essa alteração será refletida imediatamente no Adobe Experience Manager. Além disso, se uma opção de valor de campo for alterada (como uma equipe mudando seu nome para um novo nome), essa alteração também será refletida no Adobe Experience Manager.

Para obter informações e instruções sobre o mapeamento de metadados na integração do Adobe Experience Manager, consulte [Configurar metadados](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Publicar ativos automaticamente no Adobe Experience Manager

Adicionamos outro fluxo de trabalho à integração do Adobe Experience Manager. Agora, você pode definir que seus ativos sejam publicados automaticamente quando enviados para a Adobe Experience Manager. A integração pode ser configurada para publicar no serviço de publicação do Adobe Experience Manager ou em um portal de marcas da Adobe Experience Manager.

O fluxo de trabalho de Publicação automática pode ser ativado e configurado na integração com o Adobe Experience Manager. Quando ativado, o fluxo de trabalho pode ser editado no nível do modelo ou do projeto.

Para obter mais informações, consulte [Publicar ativos](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) em [Usar fluxos de trabalho na integração com o Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
