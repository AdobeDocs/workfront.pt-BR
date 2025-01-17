---
product-area: reporting
navigation-topic: text-mode-reporting
title: Visão geral do modo de texto
description: Você pode criar um relatório ou uma lista no Adobe Workfront usando a interface padrão ou de modo de texto ao criar os elementos que compõem o relatório ou a lista.
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Visão geral do modo de texto

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

Você pode criar um relatório ou uma lista no Adobe Workfront usando a interface padrão ou de modo de texto ao criar os elementos que compõem o relatório ou a lista.

A interface padrão permite referenciar campos e seus atributos que estão prontamente disponíveis na interface do Workfront.

Usando o modo texto, você pode fazer referência a campos e atributos que podem não estar disponíveis no modo padrão, mas estão disponíveis no banco de dados do Workfront.

Para obter mais informações sobre como criar relatórios usando o modo de texto, incluindo classes, vídeos e tutoriais, consulte a seção Saiba mais no site do Adobe Experience League.

## Considerações antes de usar o modo de texto

>[!TIP]
>
>Também é possível expandir os recursos de campos personalizados calculados usando uma versão do modo de texto para campos personalizados. A sintaxe e as regras para criar um campo personalizado calculado são diferentes daquelas usadas em relatórios e listas. Para obter informações sobre como adicionar um campo personalizado calculado, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Antes de começar a usar o modo de texto em seus relatórios, recomendamos que você faça nossas aulas sobre relatórios avançados para obter uma compreensão mais profunda da linguagem do modo de texto.
* Recomendamos que você use o modo padrão para garantir que os relatórios criados permaneçam intactos quando o software da Workfront for atualizado. Embora o modo de texto permita a criação de exibições, filtros e agrupamentos mais complexos, sua manutenção também é mais complicada e não é garantida quando o software do Workfront é atualizado.
* Recomendamos que você sempre tente criar todos os elementos de relatórios na interface padrão e alternar para o construtor de modo de texto somente para alguns ajustes.

  >[!TIP]
  >
  >Usar o construtor padrão fornece blocos de construção e padrões de código importantes que você pode usar ao modificar o código no modo de texto.

* Há um conjunto de regras e uma sintaxe exclusiva que você deve usar para criar relatórios e listas no modo de texto com êxito. Familiarize-se com a sintaxe do Workfront para o modo de texto antes de começar.

  Para obter informações sobre a sintaxe e as regras de uso do modo de texto, consulte [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

* Depois de personalizar um elemento de relatório no modo de texto, talvez você não consiga voltar para o modo padrão (em uma exibição) ou o código do elemento criado pode ser excluído (em filtros e agrupamentos). Isso ocorre porque nem todos os campos compatíveis com o modo de texto são compatíveis com o modo padrão.

## Interface do modo padrão

A interface do Modo Padrão exibe campos para mapear os elementos do aplicativo que você deseja exibir em um relatório ou uma lista. A interface do modo padrão é um conjunto de menus suspensos a partir dos quais você pode selecionar os campos que deseja exibir em seus relatórios ou listas.

Para obter mais informações sobre a interface de modo padrão e aprender a criar um relatório ou uma lista, consulte:

* [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
* [Elementos de relatórios: filtros, visualizações e agrupamentos](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## Interface do modo de texto

O modo de texto permite que você crie exibições, filtros, agrupamentos e prompts mais complexos, permitindo que você use campos que não estão disponíveis na interface do modo padrão. No modo de texto Workfront, há uma coleção de instruções codificadas que indicam quais objetos você deseja exibir em um relatório ou uma lista.

Para obter uma lista completa de todos os campos reportáveis, consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Nem todos os campos disponíveis por meio da API estão disponíveis por meio da interface do modo de texto. Se você usar o campo correto no código do modo de texto e não exibir os resultados esperados, o campo poderá ser reportado somente por meio da API.

## Acessar elementos de relatórios e editar modo de texto {#access-reporting-elements-and-edit-text-mode}

O acesso à interface do modo de texto é semelhante para exibições, agrupamentos e filtros ao acessá-los de um relatório ou lista.

Para obter informações sobre como usar o modo de texto em exibições, filtros e agrupamentos, consulte:

* [Editar uma exibição usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [Editar um filtro usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [Editar um agrupamento usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

Solicitações personalizadas só podem ser editadas no modo texto. Você pode acessar prompts somente a partir de um relatório.

Para obter informações sobre como acessar a interface de modo de texto para prompts personalizados, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Motivos comuns para usar o modo de texto {#common-reasons-to-use-text-mode}

Além de criar prompts personalizados que só podem ser configurados usando o modo de texto, recomendamos que você use o Report Builder para criar seus modos de exibição, filtros e agrupamentos. No entanto, há algumas instâncias em que você pode usar o modo de texto para aprimorar seus relatórios e listas.

Para obter mais informações sobre usos comuns do modo de texto, consulte [Visão geral dos usos comuns do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
