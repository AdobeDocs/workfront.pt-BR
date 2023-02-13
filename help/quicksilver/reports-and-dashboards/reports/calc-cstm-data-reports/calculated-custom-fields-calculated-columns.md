---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Campos personalizados calculados vs. colunas calculadas
description: Para agregar vários campos no Adobe Workfront e exibir esse valor agregado em um novo campo, você pode fazer o seguinte - EDITAR ME.
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Campos personalizados calculados vs. colunas calculadas

Para agregar vários campos no Adobe Workfront e exibir esse valor agregado em um novo campo, é possível fazer o seguinte:

* Um campo personalizado calculado em um formulário personalizado\
   Para obter mais informações sobre como adicionar um campo personalizado calculado a um Formulário personalizado, consulte a seção [Adicionar um campo calculado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#creating-calculated-custom-fields) no artigo [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Uma coluna calculada em uma Exibição\
   Para obter mais informações sobre como usar cálculos em uma Exibição, consulte a seção [Usar o modo de texto em exibições](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#using-text-mode-in-views) no artigo [Visão geral dos usos comuns do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Embora o modo de texto seja usado para criar campos calculados e colunas calculadas, a sintaxe para a criação é diferente. Consulte os artigos listados acima para saber como criar campos calculados e colunas calculadas. Para obter informações sobre a diferente sintaxe usada em expressões de dados calculadas, como campos e colunas personalizados calculados, consulte a seção [Sintaxe de campos personalizados calculados vs. colunas personalizadas calculadas](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns-syntax) neste artigo.

Você pode usar os mesmos cálculos em ambos os campos calculados, bem como em uma coluna calculada. No entanto, dependendo da finalidade desses cálculos, talvez você queira considerar a criação de uma em vez da outra.

## Sintaxe de campos personalizados calculados vs. colunas personalizadas calculadas

Embora as funções usadas sejam as mesmas, a sintaxe para a criação de uma expressão em um campo personalizado calculado pode ser diferente da criação de uma coluna personalizada calculada.

Por exemplo:

* Em um campo personalizado, em um formulário personalizado para tarefas, você usaria o seguinte para gerar o nome do projeto pai da tarefa em que o formulário personalizado está anexado:

   ```
   {project}.{name}
   ```

* Em uma coluna personalizada de um relatório, você usaria o seguinte para adicionar uma coluna personalizada Nome do projeto em um relatório de tarefa:

   ```
   valuefield=project:name
   ```

   Ou

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >A mesma sintaxe se aplica a todos os elementos de relatório do modo de texto, onde as expressões calculadas são usadas: exibições, filtros, agrupamentos, prompts.

As diferenças entre as duas sintaxes são:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campo personalizado calculado</td> 
   <td>Elemento de relatório personalizado calculado</td> 
  </tr> 
  <tr> 
   <td> <p>Use o nome dos campos conforme eles aparecem na interface do Workfront.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Exemplo de nome de campo usado em um campo personalizado calculado: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Use o nome dos objetos ou campos conforme eles aparecem no banco de dados do Workfront. Os nomes de objetos e campos são digitados em letras minúsculas ou minúsculas, se forem nomes compostos. </p> <p>Para obter um inventário de todos os objetos e campos do Workfront conforme aparecem no banco de dados, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Exemplo de nome de campo usado em um elemento de relatório personalizado calculado: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Incluir nomes de campos entre parênteses ou chaves</td> 
   <td> <p>Não coloque nomes de campos entre parênteses ou entre parênteses ao usá-los em um <code>valuefield </code>linha.</p> <p>Inclua nomes de campos entre colchetes ao usá-los em um <code>valueexpression</code> linha.</p> </td> 
  </tr> 
  <tr> 
   <td>Separar os campos por períodos</td> 
   <td> <p>Separe os campos por dois pontos ao usá-los em um <code>valuefield </code>line</p> <p>Separe os campos por períodos ao usá-los em um <code>valueexpression </code>linha. </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações sobre a sintaxe que deve ser usada em uma coluna personalizada calculada, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Quando usar campos personalizados calculados

* Quando quiser agrupar os resultados agregados em um relatório ou exibir essas informações em um gráfico
* Quando quiser agregar os dados além da agregação que é calculada no campo
* Quando não estiver preocupado com a atualidade dos dados, os dados não são atualizados e podem mudar com o tempo

## Ações que acionam a atualização de um campo personalizado calculado

* Na página principal de um objeto, ao clicar no ícone Mais ![](assets/more-icon.png), depois clicando em **Recalcular expressões**

* Edição em massa de vários objetos ao **Recalcular expressões personalizadas** está ativado
* Editar um formulário personalizado ao **Atualizar cálculos anteriores** está ativado para o campo personalizado calculado

## Quando usar Colunas calculadas em uma Exibição

* Quando quiser que dados em tempo real estejam disponíveis em um relatório.

   As exibições calculadas sempre são novas, pois o cálculo é feito quando o relatório é executado ou a exibição é aplicada.

* Quando você não tem planos de agrupar por resultados agregados ou usar essas informações em um gráfico.
* Quando você não planeja agregar os dados além da agregação que é calculada na coluna (os dados podem ser agregados apenas uma vez).
* Quando quiser que o cálculo inclua uma referência à data atual usando os curingas $$TODAY ou $$NOW .

   >[!TIP]
   >
   >Não use essa referência em campos personalizados calculados porque eles só recalcular quando o objeto anexado for editado. Esses tipos de cálculos ficam desatualizados.

## Exemplos de campos e colunas personalizadas calculadas

Para obter exemplos de campos personalizados calculados, consulte [Dados personalizados calculados nos relatórios](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Para obter exemplos de colunas personalizadas calculadas em exibições, consulte os seguintes artigos:

* [Visão geral dos usos comuns do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Exibição personalizada, filtro e amostras de agrupamento](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
