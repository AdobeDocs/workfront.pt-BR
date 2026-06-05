---
title: Melhorias na emissão de relatórios no terceiro trimestre de 2026
description: Melhorias na emissão de relatórios no terceiro trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b9c63e1ca4b2b301ee104ee84151a2d0148a8cea
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 3%

---

# Melhorias na emissão de relatórios no terceiro trimestre de 2026

Esta página descreve as melhorias de relatórios feitas com a versão do terceiro trimestre de 2026 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2026, consulte [Visão geral da versão do terceiro trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Alterações nas Horas Efetivas em fórmulas personalizadas

>[!NOTE]
>
>Visualização: 1 de junho de 2026>Versão rápida de produção: 1 de junho de 2026>Produção para todos: 1 de junho de 2026

Em 2025, um novo campo Horas efetivas foi adicionado ao banco de dados do Workfront como `actualWorkRequiredDouble`, e o campo Horas efetivas existente (`actualWorkRequired` no banco de dados) foi renomeado para Horas efetivas herdadas. Consulte a [nota de versão](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md) para obter mais informações.

Em junho de 2026, fórmulas personalizadas existentes usando `actualWorkRequired` (Horas efetivas herdadas) foram migradas para usar `actualWorkRequiredDouble` (Horas efetivas) em seu lugar. `actualWorkRequired` não pode mais ser usado em cálculos e fórmulas.

Além disso, é altamente recomendável usar `actualWorkRequiredDouble` em todos os relatórios.

Ao substituir o campo, observe que `actualWorkRequired` armazena valores em minutos, enquanto `actualWorkRequiredDouble` armazena valores em horas com precisão decimal.

Para obter mais informações sobre Horas Reais, consulte [Exibir Horas Reais](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).

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