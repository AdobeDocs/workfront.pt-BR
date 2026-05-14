---
title: Melhorias na emissão de relatórios no terceiro trimestre de 2026
description: Melhorias na emissão de relatórios no terceiro trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 9a86968cf8fff2c7c930aa6c8408ab8566905cb8
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 6%

---

# Melhorias na emissão de relatórios no terceiro trimestre de 2026

Esta página descreve as melhorias de relatórios feitas com a versão do terceiro trimestre de 2026 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2026, consulte [Visão geral da versão do terceiro trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Melhoria na precisão dos dados nos relatórios do painel do Canvas

>[!NOTE]
>
>Visualização: 14 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026
>
>Painéis do Canvas atualmente está na versão beta.

Os painéis da tela agora estruturam consultas de relatório para evitar linhas duplicadas quando filtros ou campos cruzam registros relacionados, de modo que contagens, somas e outras agregações retornem valores precisos.

Anteriormente, um join entre registros relacionados poderia repetir registros pai uma vez para cada registro relacionado. Por exemplo, em um relatório de projeto filtrado para tarefas atribuídas a um usuário específico, cada projeto era repetido uma vez para cada tarefa correspondente. Um KPI que somasse o orçamento do projeto poderia mostrar US$ 6.000 em vez dos US$ 1.250 corretos.

Não há alterações na interface do painel da Tela de Pintura. Os relatórios existentes retornam automaticamente dados precisos após esta versão.
