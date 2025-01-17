---
product-area: reporting
navigation-topic: text-mode-reporting
title: Visão geral de usos comuns do modo de texto
description: Visão geral de usos comuns do modo de texto
author: Nolan
feature: Reports and Dashboards
exl-id: 81512837-1ec4-4dbc-ace4-bdf08fe667ce
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Visão geral de usos comuns do modo de texto

<!-- Audited: 1/2025 -->

<!--(NOTE: Alina: ***This is linked to Understanding Text Mode (article), and the TOC article for examples of various reporting elements)</p>-->

Você pode expandir seus recursos de relatórios usando o modo de texto em relatórios e elementos de relatório. Também é possível usar uma versão do modo de texto para criar campos personalizados calculados mais complexos. Para obter mais informações sobre o modo de texto, consulte [Visão geral do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Este artigo descreve apenas alguns exemplos comuns de onde você provavelmente precisaria usar o modo de texto para expandir os recursos de relatórios ou campos personalizados calculados no Adobe Workfront. Para obter uma lista mais abrangente de exemplos, consulte:

* [Exemplos personalizados de exibição, filtro e agrupamento: índice do artigo](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
* [Dados personalizados calculados em relatórios](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)

Para obter mais informações sobre como criar relatórios usando o modo de texto, incluindo classes, vídeos e tutoriais, consulte a seção Saiba mais no site do Adobe Experience League.

## Instâncias em que você pode usar o modo de texto em listas e relatórios

Recomendamos que você use o construtor de relatórios e listas para criar suas visualizações, filtros e agrupamentos. No entanto, há algumas instâncias em que você pode usar o modo de texto para aprimorar seus relatórios e listas.

Você pode usar o modo de texto quando quiser fazer o seguinte no Workfront:

* Crie campos personalizados calculados personalizados em um formulário personalizado.\
  Para obter mais informações sobre campos personalizados calculados, consulte a seção [Usar modo de texto em campos personalizados calculados](#use-text-mode-in-calculated-custom-fields) neste artigo.
* Aprimore filtros, visualizações e agrupamentos além do que é possível no Report Builder. Para obter informações sobre como usar o modo de texto para filtros, visualizações e agrupamentos, consulte as seguintes seções neste artigo:

   * [Usar Modo de Texto em modos de exibição](#use-text-mode-in-views)
   * [Usar Modo de Texto em filtros](#use-text-mode-in-filters)
   * [Usar o modo de texto em agrupamentos](#use-text-mode-in-groupings)

* Criar prompts personalizados. Você só pode criar prompts personalizados usando o Modo de texto.

  Para obter informações sobre como criar prompts personalizados, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Usar o modo de texto em campos personalizados calculados {#use-text-mode-in-calculated-custom-fields}

Você pode usar o modo texto para adicionar um campo personalizado calculado a um Formulário personalizado.

Para obter mais informações sobre como adicionar um campo personalizado calculado a um Formulário personalizado, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Para obter mais informações sobre como criar um campo personalizado calculado no modo de texto, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Por exemplo, é possível adicionar um campo personalizado calculado que mostre um carimbo de data e hora do momento em que um item foi marcado como Em andamento. Você pode usar esse cálculo para outros status.

Para obter informações, consulte [Exemplo de campo personalizado calculado: exibir um carimbo de data/hora de status em um Formulário personalizado](../../../reports-and-dashboards/reports/calc-cstm-data-reports/example-status-timestamp-in-calculated-field.md).

## Usar modo de texto em visualizações {#use-text-mode-in-views}

Você pode usar o modo de texto em exibições para expandir os campos e objetos que podem ser exibidos na exibição.

Para obter exemplos dos motivos mais comuns para usar o modo de texto em uma exibição, consulte os seguintes artigos:

* [Exibir: objetos de exibição que não estão incluídos na interface padrão](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-objects-not-in-standard-interface.md)
* [Exibir: exibir o resultado de um cálculo entre dois campos em uma coluna](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculation-between-two-fields.md)
* [Exibir: edite permanentemente a largura de uma coluna](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)
* [Exibir: mesclar informações de várias colunas em uma coluna compartilhada](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)
* [Exibir: remover link para um objeto em uma coluna](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-remove-link-to-object.md)
* [Referenciar coleções em um relatório](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)
* [Exibir: ocultar o conteúdo de uma coluna](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-hide-column-content.md)
* [Exibir: exibir uma imagem em vez de uma cadeia de caracteres em uma coluna](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-image-in-view.md)
* [Exibir: exibe recuos de tarefas em uma lista de tarefas](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-task-identations.md)
* [Exibir: calcular diferenças de data e hora](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculate-time-and-date-differences.md)

## Usar o modo de texto em filtros {#use-text-mode-in-filters}

Você pode usar o modo de texto ao criar filtros para expandir os campos e objetos que você pode filtrar.

Para obter exemplos dos motivos mais comuns para usar o modo de texto em um filtro, consulte os seguintes artigos:

* [Filtro: crie várias regras de filtro que fazem referência ao mesmo campo (&quot;AND&quot; instruções)](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-refrence-the-same-field-multiple-times.md)
* [Filtro: exibir somente itens em um status de aprovação](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-for-items-in-approval-status.md)
* [Filtro: exibir itens por status de mesmo nome quando os status forem associados a grupos diferentes](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-same-name-statuses-from-different-groups.md)
* [Filtro: elimine itens em uma lista comparando dois campos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-items-by-comparing-two-fields.md)
* A seção [Exemplos de filtros de modo de texto que abrangem vários níveis na hierarquia de objeto](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#examples) no artigo [Criar filtros complexos de Modo de Texto usando instruções EXISTS](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)
* A seção [Criar filtros de modo de texto complexo para objetos ausentes](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#missing-object-filters) do artigo [Criar filtros de Modo de Texto complexos usando instruções EXISTS](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)

## Usar o modo de texto em agrupamentos {#use-text-mode-in-groupings}

Você pode usar o modo texto ao criar agrupamentos para expandir os campos e objetos pelos quais você pode agrupar em listas e relatórios.

Para obter exemplos dos motivos mais comuns para usar o modo de texto em um agrupamento, consulte os seguintes artigos:

* [Agrupamento: organize os resultados da lista por um valor calculado comum a todos os objetos no agrupamento](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-by-calculated-common-values.md)
* [Agrupamento: adicionar um quarto agrupamento a uma lista](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-add-fourth-grouping.md)
* [Agrupamento: editar o nome para exibição em um agrupamento](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-rename-grouping.md)
* [Agrupamento: indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-collapsed-or-expanded-results.md)
