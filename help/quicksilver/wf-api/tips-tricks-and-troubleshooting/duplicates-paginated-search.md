---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicatas retornadas durante uma pesquisa paginada grande
description: Duplicatas retornadas durante uma pesquisa paginada grande
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# Duplicatas retornadas durante uma pesquisa paginada grande

## Problema

Ao executar uma grande pesquisa paginada na API para um objeto, o cliente recebe entradas duplicadas e registros ausentes.

## Solução

Quando a ordem não é formalmente definida, dependemos da ordem das linhas retornadas pelo banco de dados do Oracle, que não garante uma ordem determinística. Por exemplo, duas chamadas consecutivas com a mesma query podem retornar linhas em uma ordem diferente. Da mesma forma, ao fazer a paginação, as linhas podem ser atribuídas aleatoriamente a &quot;páginas&quot; diferentes, gerando duplicatas. A solução mais simples pode ser adicionar classificação por ID:

```
&ID_Sort=asc
```

