---
title: Melhorias na geração de relatórios no primeiro trimestre de 2026
description: Melhorias na geração de relatórios no primeiro trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 00483638948941c933e5f8bc8cb3edaf8e43fea1
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Melhorias na geração de relatórios no primeiro trimestre de 2026

Esta página descreve os aprimoramentos de relatórios feitos com a versão do primeiro trimestre de 2026 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção, conforme observado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do Primeiro trimestre de 2026, consulte [Visão geral da versão do Primeiro trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Duplicação de um relatório em um Painel da tela

>[!NOTE]
>
>Versão de pré-visualização: 23 de outubro de 2025
>Produção para todos os clientes: 23 de outubro de 2025
>[!BADGE Fora do cronograma]{type=Neutral}

Agora é possível duplicar um relatório de KPI, tabela ou gráfico em um Painel da tela após sua criação. Após a duplicação, é possível editar o relatório conforme necessário antes de salvar.

## Remoção de opções de campo de filtros de relatório

>[!NOTE]
>
>Visualização: 6 de novembro de 2025
>Versão rápida de produção: 13 de novembro de 2025
>Produção para todos: 15 de janeiro de 2026

Removemos as seguintes opções de campo que estavam disponíveis anteriormente ao aplicar um filtro a um relatório:

* IDs de outros grupos
* Outras IDs de funções
* Outras IDs de equipes

Eles foram removidos devido a problemas associados aos operadores Not Equal e Is Blank. Se você tiver um filtro existente que use um desses campos, ele continuará a funcionar conforme esperado. Como alternativa, você pode continuar usando esses campos no modo de texto <code></code>, mas é recomendável evitar o uso dos operadores Diferente ou Está em branco ao fazer isso.

As seguintes opções de campo estão disponíveis como alternativas:

* Outros grupos: ID
* Outras Funções: ID
* Outras equipes: ID

## Melhoria na exibição da contagem de agrupamento nos Painéis do Canvas

>[!NOTE]
>
>Visualização: 6 de novembro de 2025
>Versão rápida de produção: 13 de novembro de 2025
>Produção para todos: 15 de janeiro de 2026

Quando um relatório de tabela tem várias páginas de resultados e a tabela está configurada com agrupamentos, a tabela agora exibe o valor do registro da página atual e a contagem geral do registro de todas as páginas. Por exemplo, se o seu relatório de tabela tem 7 agrupamentos e a primeira página mostra 3, a tabela exibirá 3 de 7.


## Novas medidas de proteção para melhorar os tempos de carregamento nos Painéis do Canvas

>[!NOTE]
>
>Visualização: 6 de novembro de 2025
>Versão rápida de produção: 13 de novembro de 2025
>Produção para todos: 15 de janeiro de 2026

Para evitar atrasos de tempo de carregamento e melhorar o desempenho geral nos Painéis do Canvas, aplicamos limites em quantos componentes do painel podem ser adicionados a um painel:

* Relatórios por painel: limite de 25
* Agrupamentos em visualizações de tabela: limite de 5
* Distância do objeto base do relatório: limite de 10
* Colunas em uma exibição de tabela: limite de 25
* Prompts de filtro no nível do painel: limite de 10