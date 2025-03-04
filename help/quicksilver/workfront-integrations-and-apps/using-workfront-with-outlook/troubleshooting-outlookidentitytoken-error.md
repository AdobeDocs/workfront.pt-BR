---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Solução de problemas: erro do outlookIdentityToken ao usar o Workfront para Outlook'
description: Se você receber um erro do outlookIdentityToken ao usar o Workfront para Outlook, será necessário habilitar os tokens herdados do Microsoft 365 para sua organização.
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 571ed00f44322d73183323c4d4154284cd028301
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Solução de problemas: erro do outlookIdentityToken ao usar o Workfront para Outlook

Ao usar o Workfront para Outlook, você pode ver o seguinte erro:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Para resolver esse erro, você deve ativar os tokens herdados do Microsoft 365 para para sua organização. Como isso deve ser feito no Microsoft 365, a Workfront não pode habilitar esses tokens para sua organização.

Para obter instruções sobre como habilitar tokens herdados do Microsoft 365, consulte [Ativar ou desativar tokens herdados do Exchange Online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) na documentação do Microsoft.

Para obter mais informações sobre tokens herdados, consulte [Posso ativar novamente os tokens herdados do Exchange Online?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) na documentação do Microsoft.
