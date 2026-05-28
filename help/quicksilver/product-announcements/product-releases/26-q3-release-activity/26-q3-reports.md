---
title: Melhorias na emissão de relatórios no terceiro trimestre de 2026
description: Melhorias na emissão de relatórios no terceiro trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a177e2887c2b8b281b19cda45ce59c6f8149cefb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 4%

---

# Melhorias na emissão de relatórios no terceiro trimestre de 2026

Esta página descreve as melhorias de relatórios feitas com a versão do terceiro trimestre de 2026 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2026, consulte [Visão geral da versão do terceiro trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Campos de dados de moeda personalizados em relatórios do Painel de controle da tela

>[!NOTE]
>
>Visualização: 28 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026

Os relatórios do Painel do Canvas agora oferecem suporte a campos de dados de moeda personalizados como colunas, filtros, agrupamentos e agregações, inclusive quando várias taxas de câmbio são configuradas na Configuração do sistema. Quando um campo de dados de moeda personalizado é exibido como uma coluna ou agregação, os valores são convertidos na moeda selecionada na opção de taxa de câmbio do painel, a menos que o campo esteja bloqueado no nível do relatório.

Os relatórios que anteriormente falhavam com uma mensagem &quot;campo restrito&quot; após uma segunda moeda de taxa de câmbio foram adicionados agora são renderizados. Os campos de moeda de planejamento permanecem restritos quando várias taxas de câmbio são definidas.

Para obter mais informações, consulte [Usar campos de moeda em Painéis da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md).

## Melhoria na precisão dos dados nos relatórios do painel do Canvas

>[!NOTE]
>
>Visualização: 14 de maio de 2026>Versão rápida de produção: 11 de junho de 2026>Produção para todos: 16 de julho de 2026
>
>Painéis do Canvas atualmente está na versão beta.

Os painéis da tela agora estruturam consultas de relatório para evitar linhas duplicadas quando filtros ou campos cruzam registros relacionados, de modo que contagens, somas e outras agregações retornem valores precisos.

Anteriormente, um join entre registros relacionados poderia repetir registros pai uma vez para cada registro relacionado. Por exemplo, em um relatório de projeto filtrado para tarefas atribuídas a um usuário específico, cada projeto era repetido uma vez para cada tarefa correspondente. Um KPI que somasse o orçamento do projeto poderia mostrar US$ 6.000 em vez dos US$ 1.250 corretos.

Não há alterações na interface do painel da Tela de Pintura. Os relatórios existentes retornam automaticamente dados precisos após esta versão.
