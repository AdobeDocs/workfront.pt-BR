---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicidades devolvidas durante uma pesquisa paginada grande
description: Duplicidades devolvidas durante uma pesquisa paginada grande
author: Becky
feature: Workfront API
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# Duplicidades devolvidas durante uma pesquisa paginada grande

## Problema

Ao realizar uma grande pesquisa paginada na API de um objeto, o cliente está recebendo entradas duplicadas e registros ausentes.

## Solução

Quando a ordem não é formalmente definida, confiamos na ordem das linhas retornadas pelo banco de dados do Oracle, o que não garante qualquer ordem determinística. Por exemplo, duas chamadas consecutivas com a mesma query podem retornar linhas em uma ordem diferente. Da mesma forma, ao fazer paginação, as linhas podem ser atribuídas aleatoriamente a diferentes &quot;páginas&quot;, levando a duplicatas. A solução mais simples pode adicionar a classificação por ID:

```
&ID_Sort=asc
```

