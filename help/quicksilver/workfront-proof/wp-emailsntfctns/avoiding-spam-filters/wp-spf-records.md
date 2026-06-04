---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Registros SPF do Workfront Proof
description: O Workfront Proof envia notificações por email para seus revisores a partir de um endereço de email do Workfront Proof, como notification@proofing.yourdomain.com. Para garantir que os servidores de email dos seus destinatários confiem em todas as notificações por email do Workfront Proof, é necessário configurar um registro SPF (Estrutura  [!DNL Sender Policy] ) para seu domínio personalizado conectado à conta  [!DNL Workfront Proof]  (por exemplo, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
TQID: https://experienceleague.adobe.com/LTZzs99Zzsn5dbOlu4wP1coyJAMDnnCZZ1pTTbEjT24
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 181
ht-degree: 4%

---

# Registros SPF do Workfront Proof

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] envia notificações por email aos seus revisores a partir de um endereço de email [!DNL Workfront Proof], como notification@proofing.yourdomain.com. Para garantir que os servidores de email de seus destinatários confiem em todas as notificações de email do [!DNL Workfront Proof], é necessário configurar um registro do [!UICONTROL Sender Policy Framework] (SPF) para seu domínio personalizado conectado à conta do [!DNL Workfront Proof] (por exemplo, **revisores.seudomínio.com**).

Para configurar um registro SPF, será necessário incluir o registro SPF usado para o domínio principal.

1. Adicione uma entrada **[!UICONTROL TXT de DNS]** para seu domínio com o seguinte valor:

   `v=spf1 a:mx.proofhq.com -all`

   O administrador de e-mail ou a equipe de TI podem ajudar você a configurar isso.

   >[!TIP]
   >
   >Você pode usar a ferramenta gratuita em [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) para revisar [!DNL Workfront] registros SPF.
