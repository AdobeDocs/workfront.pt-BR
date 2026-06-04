---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicatas retornadas durante uma pesquisa paginada grande
description: Duplicatas retornadas durante uma pesquisa paginada grande
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
TQID: https://experienceleague.adobe.com/1FXTHSro-rlUVHaajM1monR2Y-sxVHN6KIviogoXqRc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 111
ht-degree: 19%

---

# Duplicatas retornadas durante uma pesquisa paginada grande

## Problema

Ao executar uma grande pesquisa paginada na API para um objeto, o cliente recebe entradas duplicadas e registros ausentes.

## Solução

Quando a ordem não é definida formalmente, dependemos da ordem das linhas retornadas pelo banco de dados do Oracle, que não garante uma ordem determinística. Por exemplo, duas chamadas consecutivas com a mesma query podem retornar linhas em uma ordem diferente. Da mesma forma, ao fazer a paginação, as linhas podem ser atribuídas aleatoriamente a &quot;páginas&quot; diferentes, gerando duplicatas. A solução mais simples pode ser adicionar classificação por ID:

```
&ID_Sort=asc
```

