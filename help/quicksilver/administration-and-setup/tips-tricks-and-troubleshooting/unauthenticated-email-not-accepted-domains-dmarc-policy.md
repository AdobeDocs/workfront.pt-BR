---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Email não autenticado não aceito devido à política DMARC do domínio
description: Se um email enviado do sistema  [!DNL Workfront]  não for aceito devido à política DMARC do domínio, o administrador de email poderá corrigir o problema configurando seu sistema de email para permitir todos os emails de workfront.com.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
TQID: https://experienceleague.adobe.com/f44Wkid-gwfXgHKmSKa6oevhN5jA6720JTlOcH8kJKY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 177
ht-degree: 1%

---

# Email não autenticado não aceito devido à política DMARC do domínio

## Problema

[Teste] Recebi o seguinte email de devolução:

550-5.7.1 E-mail não autenticado de &quot;customer domain.com&quot; não é aceito devido a\
550-5.7.1 política do DMARC do domínio. Entre em contato com o administrador de &quot;customer domain.com&quot;\
550-5.7.1 se este for um email legítimo. Visite\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) para saber mais sobre o DMARC\
550 5.7.1.

## Solução

O DMARC está configurado no sistema de email da sua empresa e não faz parte do [!DNL Adobe Workfront]. Se você receber esse email, precisará entrar em contato com o administrador de email.

O administrador de email deve configurar seu sistema de email para permitir/confiar em emails de noreply@workfront.com ou, de preferência, em todos os emails de workfront.com.

Para obter mais informações sobre o DMARC, consulte [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
