---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Solução de problemas: erro do outlookIdentityToken ao usar o Workfront para Outlook'
description: Se você receber um erro do outlookIdentityToken ao usar o Workfront para Outlook, será necessário habilitar os tokens herdados do Microsoft 365 para sua organização.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Solução de problemas: erro do outlookIdentityToken ao usar o Workfront para Outlook

>[!IMPORTANT]
>
>[O Microsoft desabilitou o suporte para tokens herdados do Exchange online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que foram usados pelo suplemento do Workfront Outlook para autenticação. Essa alteração pelo Microsoft foi implementada em fases e está concluída a partir de 1 de outubro de 2025.
>
>**Como o Microsoft desabilitou esses tokens, a integração do Workfront para Microsoft Outlook não funciona mais.**

Ao usar o Workfront para Outlook, você pode ver o seguinte erro:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Para resolver esse erro, você deve ativar os tokens herdados do Microsoft 365 para para sua organização. Como isso deve ser feito no Microsoft 365, a Workfront não pode habilitar esses tokens para sua organização.

Para obter instruções sobre como habilitar tokens herdados do Microsoft 365, consulte [Ativar ou desativar tokens herdados do Exchange Online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) na documentação do Microsoft.

Para obter mais informações sobre tokens herdados, consulte [Posso ativar novamente os tokens herdados do Exchange Online?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) na documentação do Microsoft.
