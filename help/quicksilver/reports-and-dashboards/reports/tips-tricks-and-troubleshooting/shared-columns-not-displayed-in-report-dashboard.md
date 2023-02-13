---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Dados de colunas compartilhadas não são exibidos nos relatórios do painel
description: Os dados de colunas compartilhadas não são exibidos quando o relatório é colocado em um layout de painel de várias colunas, mas em um layout de única coluna. Quebras de linha também são substituídas.
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Dados de colunas compartilhadas não são exibidos nos relatórios do painel

## Problema

Os dados de colunas compartilhadas não são exibidos quando o relatório é colocado em um layout de painel de várias colunas, mas em um layout de única coluna. Quebras de linha também são substituídas.

## Causa

Apenas colunas marcadas como

```
shortview=true
```

são incluídos na exibição de painel do relatório quando o layout do painel tem a divisão esquerda/direita ou a divisão esquerda/média/direita configurada.

## Solução

Acesse a exibição usada no relatório e abra o modo de texto. (Para obter mais informações, consulte [Editar uma exibição usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Rotule todas as colunas no relatório, incluindo as colunas usadas em uma coluna compartilhada/unida, com

```
shortview=true
```

. As colunas de relatório serão exibidas corretamente no painel.
