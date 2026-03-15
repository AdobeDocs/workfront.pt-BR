---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Comparação entre campos personalizados calculados e colunas calculadas
description: Para agregar vários campos no Adobe Workfront e exibir esse valor agregado em um novo campo, você pode criar um campo personalizado calculado em um formulário personalizado ou em uma coluna calculada em uma exibição.
author: Courtney
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 15%

---

# Comparação entre campos personalizados calculados e colunas calculadas

Para agregar vários campos no Adobe Workfront e exibir esse valor agregado em um novo campo, você pode criar o seguinte:

* Um campo personalizado calculado em um formulário personalizado\
  Para obter mais informações sobre como adicionar um campo personalizado calculado a um formulário personalizado, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Uma coluna calculada em uma exibição\
  Para obter mais informações sobre o uso de cálculos em uma exibição, consulte a seção [Usar Modo de Texto em exibições](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views) no artigo [Visão geral dos usos comuns do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Embora você use o modo de texto para criar campos calculados e colunas calculadas, a sintaxe para criá-los é diferente. Consulte os artigos listados acima para saber como criar campos calculados e colunas calculadas. Para obter informações sobre a sintaxe diferente usada em expressões de dados calculados, como campos e colunas personalizados calculados, consulte a seção [Sintaxe de campos personalizados calculados versus colunas personalizadas calculadas](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) neste artigo.

Você pode usar os mesmos cálculos em ambos os campos calculados, bem como em uma coluna calculada. No entanto, dependendo da finalidade desses cálculos, talvez você queira considerar construir um em vez do outro.

## Sintaxe dos campos personalizados calculados vs. colunas personalizadas calculadas

Embora as funções usadas sejam as mesmas, a sintaxe para criar uma expressão em um campo personalizado calculado pode ser diferente do que é para criar uma coluna personalizada calculada.

Por exemplo:

* Em um campo personalizado, em um formulário personalizado para tarefas, você usaria o seguinte para gerar o nome do projeto principal da tarefa à qual o formulário personalizado está anexado:

  `{project}.{name}`

* Em uma coluna personalizada em um relatório, você usaria o seguinte para adicionar uma coluna personalizada “Nome do projeto” em um relatório de tarefas:

  `valuefield=project:name`

  Ou

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >A mesma sintaxe se aplica a todos os elementos de relatório de modo de texto nos quais as expressões calculadas são usadas: exibições, filtros, agrupamentos e prompts.

As diferenças entre as duas sintaxes são:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Campo personalizado calculado</strong></td>
   <td><strong>Elemento de relatório personalizado calculado</strong></td> 
  </tr> 
  <tr> 
   <td> <p>Use o nome dos campos conforme eles aparecem na interface do Workfront.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Exemplo de nome de campo usado em um campo personalizado calculado: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Use o nome dos objetos ou campos conforme eles aparecem no banco de dados do Workfront. Os nomes de objetos e campos são escritos em minúsculas ou em caixa alta, se forem nomes compostos. </p> <p>Para obter um inventário de todos os objetos e campos do Workfront à medida que aparecem no banco de dados, consulte o <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Exemplo de nome de campo usado em um elemento de relatório personalizado calculado: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Colocar nomes de campo entre parênteses ou chaves</td> 
   <td> <p>Não coloque os nomes de campo entre parênteses ou entre parênteses ao usá-los em uma linha <code>valuefield </code>.</p> <p>Coloque os nomes de campo entre chaves ao usá-los em uma linha <code>valueexpression</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Separe os campos por pontos</td> 
   <td> <p>Separe os campos por dois pontos ao usá-los em uma linha <code>valuefield</code>.</p> <p>Separe os campos por pontos ao usá-los em uma linha <code>valueexpression</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações sobre a sintaxe que você deve usar em uma coluna personalizada calculada, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Quando usar campos personalizados calculados

* Quando você deseja agrupar os resultados agregados em um relatório ou mostrar essas informações em um gráfico
* Quando quiser agregar os dados além da agregação calculada no campo
* Quando você não está preocupado com a pontualidade dos dados, pois eles não são atualizados e podem mudar com o tempo

## Ações que acionam a atualização de um campo personalizado calculado

* Na página principal de um objeto, clicando no ícone Mais ![ícone Mais](assets/more-icon.png) e clicando em **Recalcular Expressões**

* Edição de vários objetos em massa quando **Recalcular Expressões Personalizadas** está habilitado.
* Editar vários objetos em massa ao clicar em **Recalcular Expressões** no menu Mais em uma lista de objetos.
* Editar um formulário personalizado quando **Atualizar cálculos anteriores** estiver habilitado para o campo personalizado calculado.

Para obter mais informações, consulte [Editar informações em campos de formulário personalizados](/help/quicksilver/workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Quando usar colunas calculadas em uma exibição

* Quando você deseja que dados em tempo real estejam disponíveis em um relatório.

  As exibições calculadas são sempre novas porque o cálculo é feito quando o relatório é executado ou a exibição é aplicada.

* Quando você não tem planos de agrupar por resultados agregados nem usar essas informações em um gráfico.
* Quando você não planeja agregar os dados além da agregação calculada na coluna (os dados podem ser agregados apenas uma vez).
* Quando quiser que o cálculo inclua uma referência à data atual usando os curingas $$TODAY ou $$NOW.

  >[!TIP]
  >
  >Não use essa referência em campos personalizados calculados porque eles só são recalculados quando o objeto anexado é editado. Esses tipos de cálculos ficam desatualizados.

## Exemplos de campos personalizados e colunas calculados

Para exemplos de campos personalizados calculados, consulte [Dados personalizados calculados em relatórios](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Para exemplos de colunas personalizadas calculadas em exibições, consulte os seguintes artigos:

* [Visão geral dos usos comuns do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Exemplos de exibição personalizada, filtros e agrupamento: índice do artigo](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
