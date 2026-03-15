---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Dados de colunas compartilhadas não são exibidos em relatórios de painel
description: Os dados de colunas compartilhadas não são exibidos quando o relatório é colocado em um layout de painel de várias colunas, mas são exibidos em um layout de coluna única. Quebras de linha também são substituídas.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 12%

---

# Dados de colunas compartilhadas não são exibidos em relatórios de painel

## Problema

Os dados de colunas compartilhadas não são exibidos quando o relatório é colocado em um layout de painel de várias colunas, mas são exibidos em um layout de coluna única. Quebras de linha também são substituídas.

## Causa

Somente colunas marcadas como

```
shortview=true
```

são incluídos na visualização de painel do relatório quando o layout do painel tem a divisão esquerda/direita ou a divisão esquerda/meio/direita configurada.

## Solução

Acesse a visualização usada no relatório e abra o modo de texto. (Para obter mais informações, consulte [Editar uma exibição usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Rotule todas as colunas no relatório, incluindo as colunas usadas em uma coluna compartilhada/mesclada, com

```
shortview=true
```

. As colunas do relatório serão exibidas corretamente no painel.
