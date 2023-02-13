---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Registros SPF de prova do Workfront
description: A Workfront Proof envia notificações por email para seus revisores a partir de um endereço de email da Workfront Proof, como notification@proofing.yourdomain.com. Para garantir que os servidores de email dos recipients confiem em todas as notificações por email da Workfront Proof, é necessário configurar um [!DNL Sender Policy] Registro de estrutura (SPF) para seu domínio personalizado conectado ao [!DNL Workfront Proof] conta (por exemplo, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Registros SPF de prova do Workfront

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] envia notificações por email para seus revisores a partir de um [!DNL Workfront Proof] endereço de email, como notification@proofing.yourdomain.com. Para garantir que os servidores de email dos recipients confiem em todos [!DNL Workfront Proof] notificações por email, é necessário configurar um [!UICONTROL Estrutura de Política do Remetente] (SPF) registro do seu domínio personalizado conectado à [!DNL Workfront Proof] conta (por exemplo, **proofing.yourdomain.com**).

Para configurar um registro SPF, você precisará incluir o registro SPF usado para nosso domínio primário.

1. Adicione um **[!UICONTROL TXT DNS]** para seu domínio com o seguinte valor:

   `v=spf1 a:mx.proofhq.com -all`

   O administrador de email ou a equipe de TI podem ajudar você a configurar isso.

   >[!TIP]
   >
   >Você pode usar a ferramenta gratuita em [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) para analisar [!DNL Workfront] registros SPF.
