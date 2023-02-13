---
product-area: reporting
navigation-topic: text-mode-reporting
title: Usar formatação condicional no Modo de texto
description: Usar formatação condicional no Modo de texto
author: Nolan
feature: Reports and Dashboards
exl-id: 48fc8450-35c6-4d59-89d3-0feffe662b25
source-git-commit: 16d59c6e3d790f2804795f5a6fef05c8dca71b30
workflow-type: tm+mt
source-wordcount: '1758'
ht-degree: 2%

---

# Usar formatação condicional no Modo de texto

<!--
(NOTE: Alina: this article might need to be split in its sections. Tony asked that numbers and dates should be in separate articles (??))
-->

O construtor de interface padrão fornece uma grande flexibilidade ao criar elementos de relatório para atender às necessidades em sua organização.

É possível aplicar formatação condicional em uma exibição usando a interface padrão.\
Para obter mais informações sobre como aplicar formatação condicional a uma exibição, consulte [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar o acesso a Relatórios, Painéis, Calendários para editar exibições em um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório para editar exibições em um relatório</p> <p>Gerenciar permissões em uma exibição para editá-la</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Formatação condicional no modo de texto

O modo de texto permite criar exibições, filtros, agrupamentos e prompts mais complexos, permitindo que você use campos que não estão disponíveis na interface padrão.

Para obter uma lista completa de todos os campos relatáveis, consulte  [API Explorer](../../../wf-api/general/api-explorer.md).

Para obter mais informações sobre o uso da sintaxe do modo de texto, consulte [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

Também é possível usar o modo de texto para formatar exibições em relatórios e listas. Usando a formatação condicional, você pode alterar as exibições de seus relatórios alterando o tipo de fonte e o plano de fundo dos resultados no relatório, bem como ícones e sinalizadores. Recomendamos que você sempre crie suas exibições usando a interface padrão primeiro e alterne para a interface do modo de texto somente quando absolutamente necessário.

>[!NOTE]
>
> Não há suporte para o uso do estilo CSS para personalizar a formatação condicional. Em vez disso, você deve usar as opções de formatação pré-projetadas que estão disponíveis no Adobe Workfront.

## Adicionar formatação condicional a Exibições

Para obter mais informações sobre como aplicar formatação condicional a uma exibição na interface padrão do construtor, consulte [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

Para adicionar formatação condicional a uma exibição na interface do modo de texto:

1. Vá para uma lista de objetos.
1. Expanda o menu suspenso de uma exibição à qual deseja adicionar formatação condicional.
1. Clique em **Personalizar exibição**.
1. Clique na coluna na exibição à qual deseja aplicar a formatação condicional.
1. Clique em **Alternar para o modo de texto**.
1. No **Mostrar nesta coluna:** , clique em **Clique para editar texto**.
1. Adicione as amostras de código fornecidas em [Formatar exibições usando o modo de texto](#format-views-using-text-mode) na parte inferior do texto na coluna selecionada.
1. Clique em **Salvar**, depois clique em **Salvar exibição**.

## Formatar exibições usando o modo de texto {#format-views-using-text-mode}

Você pode adicionar os seguintes componentes a uma coluna em uma visualização para formatá-la condicionalmente no modo de texto:

* [Configurações de coluna](#column-settings)
* [Regras de coluna](#column-rules)
* [Formatar condicionalmente uma expressão value](#conditionally-format-a-valueexpression)

### Configurações de coluna {#column-settings}

Familiarize-se com a interface do modo de texto antes de poder adicionar formatação condicional às suas visualizações.

Você pode personalizar os seguintes elementos de uma coluna ao usar a formatação condicional em uma exibição:

* [Cabeçalhos de coluna](#column-headers)
* [Formatar datas](#format-dates)
* [Números de formato](#format-numbers)

#### Cabeçalhos de coluna {#column-headers}

Para alterar o cabeçalho da coluna exibida, adicione o seguinte código à coluna: `displayname= [Name of column]`. Por exemplo, para nomear uma coluna Proprietário do projeto, o código do texto seria semelhante a:

```
displayname=Project Owner
```

#### Formatar datas {#format-dates}

As datas podem ser configuradas para serem exibidas em vários formatos.

Para obter mais informações, consulte [Formatar datas em relatórios de modo de texto](../../../reports-and-dashboards/reports/text-mode/format-dates-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above)</p>
<p>To establish a date format, you must modify the <code>valueformat</code> line of the text mode code in the column.</p>
<pre>valueformat= [new date format]</pre>
<p>For example, if you wanted the Projected Completion Date to be displayed as MM/DD/YY the code would look like:</p>
<pre>valueformat=atDate<br>valuefield=projectedCompletionDate </pre>
<p>If you wanted to show the Planned Completion Date as <em>Mth, DD, Year</em>, the code would look like:</p>
<pre>valueformat=mediumAtdate<br>valuefield=plannedCompletionDate</pre>
<p>You can format dates using the following <code>valueformat</code> text mode values:</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Format</strong> </th>
<th scope="col">Example </th>
<th scope="col"><em><strong>valueformat=</strong></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>atDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY Time</td>
<td>10/11/18 12:00pm</td>
<td><pre>longAtDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>shortAtDate</pre> </td>
</tr>
<tr>
<td>Mth, DD, YR</td>
<td>Oct, 11, 2018</td>
<td><pre>mediumAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR</td>
<td>Mon, Oct, 11, 2018</td>
<td><pre>partialAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR Time</td>
<td>Mon, Oct, 11, 2018 12:00 pm</td>
<td><pre>fullAtDate</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

#### Números de formato {#format-numbers}

Você pode formatar valores numéricos para exibir informações que melhor se adaptem às suas necessidades de relatórios.

Para obter mais informações, consulte [Formatar números, moeda e valores de porcentagem em relatórios de modo de texto](../../../reports-and-dashboards/reports/text-mode/format-numbers-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To modify the format of a numeric value, you must edit the <strong>valueformat</strong> line of your column.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above) </p>
<p>For example, if you wanted to display the Budget column as $1000, the value format line would look like:</p>
<pre>valueformat=currencyStringCurrencyRounded<br>valuefield=budget</pre>
<p>You can format numbers using the following values for the <code>valueformat</code> line of your column:</p>
<table border="2" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Example</strong> </th>
<th scope="col"><em><code>valueformat=</code></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>1234</td>
<td><pre>doubleAsString</pre> or <pre>int</pre></td>
</tr>
<tr>
<td>1,234</td>
<td><pre>doubleAsInt</pre> </td>
</tr>
<tr>
<td>$1,234</td>
<td><pre>currencyStringCurrencyRounded</pre> </td>
</tr>
<tr>
<td>1234.56</td>
<td><pre>doubleAsDouble</pre> </td>
</tr>
<tr>
<td>$1,234.56</td>
<td><pre>currencyStringCurrency</pre> </td>
</tr>
<tr>
<td>12%</td>
<td><pre>doubleAsPercentRounded</pre> </td>
</tr>
<tr>
<td>12.34%</td>
<td><pre>doubleAsPercent</pre> </td>
</tr>
<tr>
<td>(1,234.56)</td>
<td><pre>doubleAsFinancial</pre> </td>
</tr>
<tr>
<td>(1,234)</td>
<td><pre>doubleAsFiancialRounded</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

### Regras de coluna {#column-rules}

As regras de coluna permitem a adição de imagens, cor, formatação e substituições de texto em uma exibição. As regras de coluna podem ser estabelecidas independentemente ou podem conter várias condições para uma coluna.

* [Formatação condicional](#conditional-formatting)
* [Vários formatos condicionais](#multiple-conditional-formats)
* [Aplicar texto](#apply-text)
* [Aplicar formatos de linha](#apply-row-formats)
* [Aplicar imagens](#apply-images)

#### Formatação condicional {#conditional-formatting}

Uma instrução de modo de texto específica deve ser aplicada ao incorporar cor ou formatação de texto.

>[!NOTE]
>
>A formatação condicional pode não ser suportada em colunas unidas.\
>Para obter mais informações sobre como unir colunas ao modo Texto, consulte [Exibir: unir informações de várias colunas em uma coluna compartilhada](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

Insira o seguinte código em qualquer coluna à qual deseja adicionar formatação condicional:

```
styledef.case.0.comparison.leftmethod= [field name]
styledef.case.0.comparison.lefttext= [field name]
styledef.case.0.comparison.righttext= [field value]
styledef.case.0.comparison.operator= [qualifier]
styledef.case.0.comparison.operatortype= [data type]
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

>[!NOTE]
>
>O *styledef.case.0.comparison.icon* A linha é sempre falsa, a menos que funcione com ícones.
>
>O *styledef.case.0.comparison.truetext* é sempre deixada em branco até trabalhar com a substituição do texto.
>
>O *styledef.case.0.comparison.righttext* linha fica em branco quando o qualificador não está em branco.

Por exemplo, se quisermos mostrar o Nome da empresa no texto verde em um relatório de projeto, você pode usar o seguinte código:

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name ;
styledef.case.0.comparison.righttext= 
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
```

>[!NOTE]
>
>* Embora essa instrução pudesse ser aplicada a uma coluna Nome da empresa, ela também poderia ser aplicada a qualquer outra coluna no relatório. O texto verde só seria exibido se o projeto tivesse uma Empresa associada a ele. Lembre-se do `[field name]`, `[value]`e `[qualifier]` unidade, independentemente de o condicionamento ser exibido na coluna.
>* Ao trabalhar com qualificadores, recomendamos usar `cicontains` em vez de `equal`. Por padrão, `equal` procura números de ID. Usar o `cicontains` , você pode acessar itens pelo nome.


![](assets/screen-shot-2013-08-15-at-2.53.51-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-2.54.08-pm-350x185.png)

Se Cor do texto, Alinhamento, Estilo da fonte ou Cor do plano de fundo forem aplicados a um modo de texto, a mesma instrução (mostrada acima) será usada.

As linhas a seguir devem ser modificadas para refletir a formatação correspondente necessária para a coluna:

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

Use as tabelas a seguir para identificar quais linhas precisam ser modificadas e quais valores você deve especificar para definir o estilo de formato da coluna:

| **Cor do texto** | **Linha: textcolor=** |
|---|---|
| Preto | `000000` |
| Azul escuro | `0c6aca` |
| Teal | `1b878c` |
| Verde | `03a219` |
| Roxo | `6408c4` |
| Cinza | `767676` |
| Vermelho | `d30519` |
| Amarelo | `e19503` |

{style=&quot;table-layout:auto&quot;}

| **Alinhamento** | **Linha: align=** |
|---|---|
| Alinhamento à esquerda | `left` |
| Alinhamento à direita | `right` |
| Alinhamento central | `center` |

{style=&quot;table-layout:auto&quot;}

| Fonte | Linha: ***fontstyle=*** |
|---|---|
| Negrito | `bold` |
| Itálico | `italic` |

{style=&quot;table-layout:auto&quot;}

| **Cor de plano de fundo** | **Linha: bgcolor=** |
|---|---|
| Teal | `dcf6f7` |
| Verde | `def6e2` |
| Cinza | `e8e8e8` |
| Azul | `e8f1ff` |
| Roxo | `e9def4` |
| Vermelho | `eac6c9` |
| Amarelo | `feecc8` |
| Branco | `ffffff` |

{style=&quot;table-layout:auto&quot;}

#### Vários formatos condicionais {#multiple-conditional-formats}

É possível aplicar mais de um estilo de formatação a uma instrução. A instrução principal permaneceria inalterada e qualquer expressão de formatação adicional seria adicionada à instrução.

Por exemplo, usando a declaração anterior para incluir Nome da empresa no texto em negrito verde. A instrução seria escrita usando o seguinte código:

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name
styledef.case.0.comparison.righttext=
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
styledef.case.0.comparison.trueproperty.1.name=fontstyle
styledef.case.0.comparison.trueproperty.1.value=bold
```

>[!NOTE]
>
>Ao incluir mais de uma expressão de formatação condicional, é necessário identificar numericamente cada expressão na declaração. Observe que a expressão 0 e a expressão 1 foram identificadas.

![](assets/screen-shot-2013-08-15-at-3.18.45-pm-350x198.png)

#### Aplicar texto {#apply-text}

Se quiser substituir os valores padrão que são preenchidos em uma coluna por um valor de sua escolha, é possível aplicar texto à coluna.

Por exemplo, em um relatório de projeto, defina o valor da coluna Data inicial planejada para não exibir a data inicial planejada do projeto, mas o texto &quot;Não hoje&quot;. Use o seguinte código para a coluna Data inicial planejada:

```
case.0.comparison.leftmethod=plannedStartDate
case.0.comparison.lefttext=plannedStartDate
case.0.comparison.righttext=2013-04-10T10:45:00:000
case.0.comparison.operator=ne
case.0.comparison.operatortype=date
case.0.comparison.icon=false
case.0.comparison.truetext=not today
styledef.case.0.comparison.leftmethod=plannedStartDate
styledef.case.0.comparison.lefttext=plannedStartDate
styledef.case.0.comparison.righttext=2013-04-10T10:45:00:000 
styledef.case.0.comparison.operator=ne
styledef.case.0.comparison.operatortype=date&
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=not today
```

>[!NOTE]
>
>As linhas que começam com `case.0.` use comparações de casos para identificar o uso de texto. As linhas que começam com **styledef.case.0.** são declarações de formatação condicional antigas, onde identificamos o uso do texto por meio da variável `truetext` expressão. Certifique-se de definir `truetext` para um valor, em vez de deixá-lo em branco.

![](assets/screen-shot-2013-08-15-at-3.22.02-pm-350x196.png)

![](assets/screen-shot-2013-08-15-at-3.22.16-pm-350x151.png)

#### Aplicar formatos de linha {#apply-row-formats}

Se quiser aplicar uma condição à linha inteira, use o seguinte código com seu código de coluna:

```
styledef.case.0.comparison.icon=false
```

```
styledef.case.0.comparison.isrowcase=true
```

```
styledef.case.0.comparison.leftmethod= [field name]
```

```
styledef.case.0.comparison.lefttext= [field name]
```

```
styledef.case.0.comparison.operator= [qualifier]
```

```
styledef.case.0.comparison.operatortype= [data type]
```

```
styledef.case.0.comparison.righttext= [field value]
```

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
styledef.case.0.comparison.truetext=
```

```
row.0.styledef.applyallcases=true
```

```
row.0.styledef.case.0.comparison.icon=false
```

```
row.0.styledef.case.0.comparison.isrowcase=true
```

```
row.0.styledef.case.0.comparison.leftmethod= [field name]
```

```
row.0.styledef.case.0.comparison.lefttext= [field name]
```

```
row.0.styledef.case.0.comparison.operator= [qualifier]
```

```
row.0.styledef.case.0.comparison.operatortype= [data type]
```

```
row.0.styledef.case.0.comparison.righttext= [field value]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
row.0.styledef.case.0.comparison.truetext=
```


#### Aplicar imagens {#apply-images}

De maneira semelhante à formatação com texto, as imagens podem ser usadas para exibir informações nos relatórios. O Workfront tem várias imagens incorporadas para transmitir informações visuais em uma configuração de relatório. Para usar imagens na configuração de formatação condicional, a seguinte instrução é necessária:

```
image.case.0.comparison.leftmethod= [field name]
image.case.0.comparison.lefttext= [field name]
image.case.0.comparison.righttext= [field value]
image.case.0.comparison.operator= [qualifier]
image.case.0.comparison.operatortype= [data type]
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=
```

Por exemplo, em um relatório de projeto, é necessário criar uma coluna na qual você mostraria uma face de tela para cada Data de conclusão planejada que não seja igual à data de hoje. Use o seguinte código do modo de texto para adicionar o ícone à coluna:

```
image.case.0.comparison.leftmethod=plannedCompletionDate
image.case.0.comparison.lefttext=plannedCompletionDate
image.case.0.comparison.righttext=2013-04-10T13:00:00:000 
image.case.0.comparison.operator=ne 
image.case.0.comparison.operatortype=date
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif
```

>[!NOTE]
>
>Observe que a declaração usa a variável `icon=true` expressão. Essa declaração também é diferente de outras declarações de formatação condicional, pois não usa a variável `style.def` , mas um formato de imagem exclusivo.

![](assets/screen-shot-2013-08-15-at-3.35.08-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-3.35.22-pm-1-350x167.png)

Para usar as imagens disponíveis, aplique o seguinte código e valores:

| **Ícone** | **Linha: image.case.0.comparison.truetext=** |
|---|---|
| Rosto Congelado ![](assets/face-sad.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif` |
| Rosto Feliz ![](assets/face-happy.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_smile.gif` |
| Sinalizador azul  ![](assets/flag-blue-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_blue.gif` |
| Sinalizador verde  ![](assets/flag-green-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_green.gif` |
| Sinalizador vermelho  ![](assets/flag-red-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_red.gif` |
| Sinalizador Amarelo  ![](assets/flag-yellow-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_yellow.gif` |
| Círculo preto  ![](assets/dot-black.png) | =`/interface/images/v4_redux/icons/casebuilder/light_black.gif` |
| Círculo azul ![](assets/dot-blue.png) | =`/interface/images/v4_redux/icons/casebuilder/light_blue.gif` |
| Círculo Cinza ![](assets/dot-gray.png) | =`/interface/images/v4_redux/icons/casebuilder/light_grey.gif` |
| Círculo Verde ![](assets/dot-green.png) | =`/interface/images/v4_redux/icons/casebuilder/light_green.gif` |
| Círculo Laranja ![](assets/dot-orange.png) | =`/interface/images/v4_redux/icons/casebuilder/light_orange.gif` |
| Círculo rosa ![](assets/dot-pink.png) | =`/interface/images/v4_redux/icons/casebuilder/light_pink.gif` |
| Círculo violeta ![](assets/dot-purple.png) | =`/interface/images/v4_redux/icons/casebuilder/light_purple.gif` |
| Círculo Vermelho ![](assets/dot-red.png) | =`/interface/images/v4_redux/icons/casebuilder/light_red.gif` |
| Círculo Branco ![](assets/dot-white.png) | =`/interface/images/v4_redux/icons/casebuilder/light_white.gif` |
| Círculo Amarelo ![](assets/dot-yellow.png) | =`/interface/images/v4_redux/icons/casebuilder/light_yellow.gif` |

{style=&quot;table-layout:auto&quot;}

### Formatar condicionalmente uma `valueexpression` {#conditionally-format-a-valueexpression}

Para exibir um valor calculado em uma coluna, é possível substituir a variável `valuefield` linha de código na coluna com um `valueexpression`. Um valor calculado permite exibir um novo valor para um objeto com base no cálculo entre dois campos existentes no mesmo objeto.

Para obter mais informações sobre como formatar a variável `valueexpression line`, consulte [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

Não é possível formatar condicionalmente uma coluna que contém uma `valueexpression` linha de código. Em vez disso, você pode adicionar um Campo personalizado calculado a um Formulário personalizado e associá-lo aos objetos exibidos no relatório. Em seguida, é possível formatar condicionalmente as colunas que exibem esse campo.

Para obter mais informações sobre Campos personalizados calculados, consulte [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Adicionar um valor agregador em uma coluna Modo de texto

Recomendamos que você crie a coluna na interface do construtor primeiro, adicione o valor do agregador lá e edite a coluna no modo de texto.

Considere o seguinte ao adicionar agregadores a uma coluna no Modo de texto:

* Os valores na coluna devem ter um formato que possa ser resumido. Por exemplo, eles devem ter um dos seguintes formatos:

   * Número
   * Data
   * Moeda

* É possível adicionar um agregador a uma coluna que exibe um cálculo. O valor agregado é exibido no agrupamento da visualização ou relatório. Para obter mais informações, consulte [Agrupamento: exibir o resultado da agregação de vários valores calculados em um agrupamento](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
* As linhas de código para a definição da coluna devem ser idênticas às linhas de código que introduzem o agregador e precedidas por &quot;agregador&quot;. Por exemplo, se você tiver uma coluna onde exibir Horas Planejadas em um projeto, o modo de texto das linhas principais da coluna será:

   ```
   valuefield=workRequired
   valueformat=compound
   ```

   Quando quiser agregar o valor de todas as linhas no agrupamento da exibição, podemos adicionar o seguinte código para adicionar os valores do agregador: `aggregator.valuefield=workRequired` (a) `aggregator.valuefield` deve ser igual a `valuefield` que descreve a coluna) `aggregator.valueformat=compound` (a) `aggregator.valueformat` a linha deve ter o mesmo valor que a `valueformat` que descreve a coluna) `aggregator.function=SUM` (essa é uma linha obrigatória que indica como você deseja agregar a coluna; nesse caso, você deseja adicionar todas as Horas Planejadas individuais em um número na linha de agrupamento) `aggregator.displayformat=minutesAsHoursString` (como as horas são armazenadas no Workfront em minutos, queremos indicar a variável `displayformat` para horas em que são armazenadas em minutos)
