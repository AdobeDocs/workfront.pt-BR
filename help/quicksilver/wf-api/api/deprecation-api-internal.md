---
content-type: api
navigation-topic: api-navigation-topic
title: Substituição de API-Interno
description: Substituição de API-Interno
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Substituição de API-Interno

API-Interno é uma versão da API do Adobe Workfront que não é compatível devido ao seu design e finalidade. Embora contenha as atualizações mais recentes da API do Workfront, ela está sujeita a alterações sem aviso prévio e, portanto, deve ser usada com cuidado em integrações de produção. A Workfront recomenda que todas as integrações API-Internas sejam atualizadas para uma API com versão.

Para saber mais sobre as versões compatíveis da API do Workfront, consulte [Controle de versão da API e programação de suporte](../../wf-api/api/api-version-support-schedule.md).

**Uso de API-Unsupported**

Se suas integrações exigirem uma funcionalidade que não esteja disponível em uma API com versão, a Workfront recomenda usar API-Unsupported. Semelhante a API-Internal, API-Unsupported não é compatível. API-Incompatível também inclui as alterações mais recentes na API do Workfront e está sujeito a alterações sem aviso prévio. A Workfront incentiva você a usar a API - Não compatível em seu ambiente de teste, onde você pode explorar novas funcionalidades e garantir que a API não tenha erros.

**Determinar a versão da API que você está usando**

Você pode determinar a versão da API que suas integrações usam usando REST para construir um URI que envia uma chamada por HTTPS para o Workfront e retorna uma resposta JSON.

O exemplo a seguir mostra um URI que chama API-Internal:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

O exemplo a seguir mostra um URI que chama API-Unsupported:

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

O exemplo a seguir mostra um URI que chama a Versão 15.0 da API:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
