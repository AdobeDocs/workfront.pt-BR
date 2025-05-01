---
title: Melhorias na emissão de relatórios no terceiro trimestre de 2025
description: Aprimoramentos no projeto do terceiro trimestre de 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b36cfdc4587bc440867a6a84b9460eaeaf4daf88
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Melhorias na emissão de relatórios no terceiro trimestre de 2025

Esta página descreve todas as melhorias de relatórios feitas com a versão do terceiro trimestre de 2025 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção, conforme observado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2025, consulte [Visão geral da versão do terceiro trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Os curingas do usuário não retornam mais resultados com um valor nulo durante a filtragem

>[!NOTE]
>
>* Visualização: 30 de abril de 2025
>* Versão rápida de produção: 15 de maio de 2025
>* Produção para todos os clientes: 17 de julho de 2025

Atualizamos o comportamento do curinga do usuário para excluir valor nulo ao filtrar um relatório. Essa alteração ajuda o filtro a produzir resultados mais precisos, em vez de retornar resultados que não têm um usuário configurado corretamente (um resultado nulo).

Anteriormente, quando um curinga do usuário produzia um valor nulo, um relatório exibia todos os registros que também tinham um valor nulo.

Essa alteração se aplica aos seguintes filtros curingas:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`

