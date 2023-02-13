---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Quando um email autenticado não é aceito devido à política DMARC do domínio
description: Se um email for enviado do [!DNL Workfront] O sistema não é aceito devido à política DMARC do domínio, seu administrador de email pode corrigir o problema configurando seu sistema de email para permitir todos os emails do workfront.com.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# O email não autenticado não é aceito devido à política DMARC do domínio

## Problema

[Teste] Recebi o seguinte email de devolução:

550-5.7.1 O email não autenticado de &quot;customer domain.com&quot; não é aceito devido a\
Política DMARC do domínio 550-5.7.1. Entre em contato com o administrador do &quot;customer domain.com&quot;\
Domínio 550-5.7.1 se for um email legítimo. Visite\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) para saber mais sobre o DMARC\
550 5.7.1.

## Solução

O DMARC é configurado no sistema de email de sua empresa e não faz parte de [!DNL Adobe Workfront]. Se você receber esse email, precisará entrar em contato com o administrador do email.

O administrador de email deve configurar seu sistema de email para permitir/confiar em email de noreply@workfront.com ou, preferencialmente, em todos os emails de workfront.com.

Para obter mais informações sobre o DMARC, consulte [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
