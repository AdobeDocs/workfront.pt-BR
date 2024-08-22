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
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Email não autenticado não aceito devido à política DMARC do domínio

## Problema

[Teste] Recebi o seguinte email de devolução:

550-5.7.1 E-mail não autenticado de &quot;customer domain.com&quot; não é aceito devido a\
550-5.7.1 política DMARC do domínio. Entre em contato com o administrador de &quot;customer domain.com&quot;\
550-5.7.1 se este for um email legítimo. Visite\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) para saber mais sobre DMARC\
550 5.7.1.

## Solução

O DMARC está configurado no sistema de email da sua empresa e não faz parte de [!DNL Adobe Workfront]. Se você receber esse email, precisará entrar em contato com o administrador de email.

O administrador de email deve configurar seu sistema de email para permitir/confiar em emails de noreply@workfront.com ou, de preferência, em todos os emails de workfront.com.

Para obter mais informações sobre o DMARC, consulte [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
