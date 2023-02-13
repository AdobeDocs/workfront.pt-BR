---
content-type: api
navigation-topic: api-navigation-topic
title: Substituição de API - Interno
description: Substituição de API - Interno
author: John
feature: Workfront API
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Substituição de API - Interno

API-Internal é uma versão da API do Adobe Workfront que não é suportada devido ao seu design e propósito. Embora contenha as atualizações mais recentes para a API do Workfront, ela está sujeita a alterações sem aviso prévio e, portanto, deve ser usada com cuidado nas integrações de produção. A Workfront recomenda atualizar todas as integrações internas da API para uma API com versão.

Para saber mais sobre as versões compatíveis da API do Workfront, consulte [Controle de versão da API e cronograma de suporte](../../wf-api/api/api-version-support-schedule.md).

**Uso de APIs sem suporte**

Se as integrações exigirem uma funcionalidade que não esteja disponível em uma API com versão, a Workfront recomenda usar API-Unsupported. Semelhante a API-Interno, não há suporte para API-Unsupported. A API-Não compatível também inclui as alterações mais recentes na API do Workfront e está sujeita a alterações sem aviso prévio. A Workfront incentiva você a usar API-Não suportado em seu ambiente de teste, onde é possível explorar novas funcionalidades e garantir que a API não tenha bugs.

**Determinar a versão da API que você está usando**

Você pode determinar a versão da API que suas integrações usam usando REST para criar um URI que envia uma chamada por HTTPS para o Workfront e retorna uma resposta JSON.

O exemplo a seguir mostra um URI que chama API-Interno:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

O exemplo a seguir mostra o URI que chama API-Unsupported:

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

O exemplo a seguir mostra um URI que chama a Versão 7.0 da API:

```
https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c70…
```
