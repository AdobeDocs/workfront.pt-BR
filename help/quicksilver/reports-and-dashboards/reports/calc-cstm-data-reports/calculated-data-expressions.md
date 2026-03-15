---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Visão geral das expressões de dados calculadas
description: Você pode usar expressões de dados para definir campos de dados personalizados calculados no Adobe Workfront. As expressões calculadas conectam campos existentes do Workfront em instruções que geram um novo campo.
author: Courtney, Lisa
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '2551'
ht-degree: 100%

---

# Visão geral das expressões de dados calculadas

<!--Audited: 12/2023-->

Você pode usar expressões de dados para definir campos personalizados calculados no Adobe Workfront. As expressões calculadas conectam campos existentes do Workfront em instruções que geram um novo campo.

Você pode usar expressões de dados calculados em:

* Um campo personalizado calculado em um formulário personalizado

  Para obter mais informações sobre como criar campos personalizados calculados em formulários personalizados no Workfront, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Uma coluna personalizada calculada em um relatório ou lista, quando você usa o modo de texto

  Para obter mais informações sobre como usar o modo de texto em relatórios e visualizações, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Sintaxe dos campos personalizados calculados vs. colunas personalizadas calculadas

Embora as funções utilizadas sejam as mesmas, a sintaxe para criar uma expressão em um campo personalizado calculado pode ser diferente daquela utilizada para criar uma coluna personalizada calculada.

As diferenças entre as duas sintaxes são:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Campo personalizado calculado</strong></td> 
   <td><strong>Elemento de relatório personalizado calculado</strong></td> 
  </tr> 
   <td>Coloque os nomes dos campos entre chaves</td> 
   <td>Não coloque nomes de campos entre colchetes ou parênteses ao usá-los em uma <p><code>valuefield </code></p>linha. <p>Coloque os nomes dos campos entre chaves quando os utilizar em uma <p><code>valueexpression</code></p> linha.</p> </td> 
  </tr> 
  <tr> 
   <td>Separe os campos por pontos</td> 
   <td> <p>Separe os campos por dois pontos ao usá-los em uma <p><code>valuefield </code></p>linha</p> <p>Separe os campos por pontos ao usá-los em uma <p><code>valueexpression </code></p>linha. </p> </td> 
  </tr> 
 </tbody> 
</table>

Por exemplo:

* Em um campo personalizado, em um formulário personalizado para tarefas, você usaria o seguinte para gerar o nome do projeto principal da tarefa à qual o formulário personalizado está anexado:


  `{project}.{name}`


* Em uma coluna personalizada em um relatório, você usaria o seguinte para adicionar uma coluna personalizada “Nome do projeto” em um relatório de tarefas:


  `valuefield=project:name`


  Ou

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >A mesma sintaxe se aplica a todos os elementos de relatório em modo de texto onde são utilizadas expressões calculadas: visualizações, filtros, agrupamentos, prompts.

Para obter mais informações sobre a sintaxe que você deve usar em uma coluna personalizada calculada, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Expressões de dados que você pode usar

As listas abaixo definem as expressões disponíveis que você pode usar ao criar um dos 3 tipos diferentes de campos personalizados calculados no Workfront:

* [Campos personalizados calculados de data e hora](#date-time-calculated-custom-fields)
* [Campos personalizados calculados matemáticos](#mathematical-calculated-custom-fields)
* [Campos personalizados calculados em texto](#text-calculated-custom-fields)

Você pode usar as expressões listadas abaixo para criar colunas personalizadas calculadas. No entanto, você deve usar a sintaxe correta para uma coluna personalizada calculada, conforme descrito na seção [Sintaxe de campos personalizados calculados vs. colunas personalizadas calculadas](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) neste artigo.

### Campos personalizados calculados de data e hora {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Se você criar um cálculo de data e hora que não inclua uma parte de hora ou que use os curingas de data $$TODAY ou $$NOW, o sistema usará a data de acordo com o fuso horário do Tempo Universal Coordenado (UTC), e não de acordo com o seu fuso horário local. Isso pode causar um resultado inesperado na data.

Você pode criar um campo personalizado calculado de data ou hora usando as seguintes expressões:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expressão</th> 
   <th>Explicação e exemplo</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>Adiciona o número de dias à data. O valor numérico pode incluir dias parciais. Por exemplo, 1,5 adiciona um dia e meio à data.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Adiciona o número de dias úteis à data. Esta expressão apenas adiciona valores inteiros à data, arredondando para baixo. </p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Adiciona o número de meses à data e é formatado da seguinte forma:

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Adiciona o número de anos à data e é formatado da seguinte forma:</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDHOURS</strong> </td> 
   <td> <p>Adiciona o número de horas à data e é formatado da seguinte forma:</p>

<p><code>ADDHOUR(date, number)</code></p>
   <p>Observação: esta expressão não é compatível com o Workfront Planning.</p></td> 
  </tr>
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Apaga a parte da hora de uma data e é formatado da seguinte forma. Neste exemplo, a data é a data de entrada de um objeto de trabalho.</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Converte uma string em uma data e é formatada da seguinte maneira:</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Retorna o número de dias entre as duas datas, levando em consideração os dias de início e fim do período selecionado, bem como os registros de data e hora desses dias. Por exemplo, se a hora de início da data inicial for 15h, o dia de início não é contado como um dia inteiro.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Retorna o dia do mês da data como um número, entre 1 e 31.</p> <p>A expressão é formatada da seguinte maneira. Neste exemplo, a data é a data de entrada de um objeto de trabalho.</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Retorna o dia da semana para a data como um número, entre 1 (domingo) e 7 (sábado).</p> <p>A expressão é formatada da seguinte maneira. Neste exemplo, a data é a data de entrada de um objeto de trabalho.</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Retorna o total de dias no mês da data como um número e é formatado da seguinte maneira. Neste exemplo, a data é a data de entrada de um objeto de trabalho.</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Retorna o total de dias úteis entre a data e o final da semana ou o final do mês, o que ocorrer primeiro. Neste exemplo, a data é a data de entrada de um objeto de trabalho.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Retorna o total de dias no ano da data como um número e é formatado da seguinte maneira. Neste exemplo, a data é a data de entrada de um objeto de trabalho.</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Retorna a data mais recente da lista e é formatada da seguinte maneira:</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Retorna a data mais antiga da lista e é formatada da seguinte maneira:</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>Retorna a hora da data como um número entre 0 e 23.</p> <p>A expressão é formatada da seguinte maneira. Neste exemplo, a data é a data de entrada de um objeto de trabalho.</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Retorna o minuto da data como um número entre 0 e 60, formatado da seguinte maneira. Neste exemplo, a data é a data de entrada de um objeto de trabalho.</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MONTH</strong> </td> 
   <td> <p>Retorna o mês da data como um número entre 1 e 12, formatado da seguinte maneira. Neste exemplo, a data é a data de entrada de um objeto de trabalho.</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Retorna o segundo da data como um número entre 0 e 60, formatado da seguinte maneira. Neste exemplo, a data é a data de entrada de um objeto de trabalho.</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Retorna o número de dias úteis entre duas datas, levando em consideração os dias de início e fim do período selecionado, bem como os registros de data e hora desses dias. Por exemplo, se a hora de início da data inicial for 15h, o dia de início não será contado como um dia inteiro.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Retorna o número de minutos programados entre as datas de acordo com o cronograma padrão.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>YEAR</strong> </td> 
   <td> <p>Retorna o ano da data como um número de 4 dígitos, formatado da seguinte maneira. Neste exemplo, a data é a data de entrada de um objeto de trabalho.</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### Campos personalizados calculados matemáticos {#mathematical-calculated-custom-fields}

Você pode criar um campo personalizado calculado que utilize algumas das seguintes expressões matemáticas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expressão</th> 
   <th>Explicação</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>Retorna o valor absoluto do número e é formatado da seguinte maneira. Este exemplo usa o número de objetos abaixo do objeto ao qual o formulário personalizado está anexado.

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>Retorna a média dos números e é formatado da seguinte forma:

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Arredonda para cima um número inteiro para o mais próximo e é formatado da seguinte maneira. Este exemplo usa o número de objetos abaixo do objeto ao qual o formulário personalizado está anexado.

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Divide todos os números na ordem fornecida e é formatado da seguinte forma:

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Arredonda para baixo um número inteiro para o mais próximo e é formatado da seguinte maneira. Este exemplo usa o número de objetos abaixo do objeto ao qual o formulário personalizado está anexado.

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Retorna o valor do logaritmo natural do número e é formatado da seguinte maneira:

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Retorna o valor logarítmico de número2 na base número1 e é formatado da seguinte maneira:

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Retorna o maior item da lista e é formatado da seguinte maneira:

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Retorna o menor item da lista e é formatado da seguinte maneira:

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>Converte uma string em um número e é formatado da seguinte maneira:<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Retorna um número elevado a uma potência e é formatado da seguinte maneira:

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Multiplica todos os números e é formatado da seguinte forma:

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>NOTA</b></p>

<p>Ao multiplicar campos que contêm horas, certifique-se de compreender se o banco de dados salva as horas nos campos selecionados em minutos, horas ou segundos. Se as horas forem salvas em minutos ou segundos, mas exibidas em horas na interface do Workfront, talvez seja necessário levar em conta a conversão de minutos ou segundos para horas ao escrever uma expressão usando esse cálculo. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Arredonda para cima um número para a quantidade de casas decimais especificadas e é formatado da seguinte forma:

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Ordena os números em ordem crescente e é formatado da seguinte forma:</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Ordena os números em ordem decrescente e é formatado da seguinte forma:

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Retorna a raiz quadrada de um número e é formatado da seguinte maneira. Este exemplo usa o número de objetos abaixo do objeto ao qual o formulário personalizado está anexado.</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Subtrai todos os números na ordem fornecida e é formatado da seguinte forma:

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Soma todos os números e é formatado da seguinte maneira:

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### Campos personalizados calculados em texto {#text-calculated-custom-fields}

Você pode criar um campo personalizado calculado que exiba um valor formatado como texto usando as seguintes expressões:

<table style="table-layout:auto:fixed"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expressão</th> 
   <th>Explicação</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ARRAY</strong> </td> 
   <td> <p>Converte uma string em uma matriz. O delimitador pode ser qualquer string.</p> 
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>ARRAY(string1, "delimiter")</code></p> 
   </td> 
  </tr>

<tr> 
   <td><strong>ARRAYCONTAINS</strong> </td> 
   <td> <p>Procura um valor específico em uma lista ou matriz. Se o valor for encontrado, a função retorna Verdadeiro, caso contrário, retorna Falso. </p> 
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>ARRAYCONTAINS(array, value)</code></p> 
   </td> 
  </tr>


<tr> 
   <td><strong>ARRAYLENGTH</strong> </td> 
   <td> <p>Retorna o número de elementos na matriz e é formatado da seguinte maneira:</p>
   <p><code>ARRAYLENGTH(array)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>ARRAYELEMENT</strong> </td> 
   <td> <p>Retorna o elemento no número especificado na matriz. Se o índice estiver fora dos limites, ele retornará vazio.</p> 
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>ARRAYELEMENT(array, number)</code></p> 
   </td> 
  </tr>

<tr>   
   <td><strong>CASE</strong> </td> 
   <td> <p>É usado com outras expressões para escolher um valor de uma lista, com base em um número de índice. </p>
   <p>Um número de índice é um campo ou função que retorna um valor numérico (geralmente em um intervalo conhecido).</p> 
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>Por exemplo, a expressão a seguir retorna o nome do dia da semana, onde 1 = domingo, 2 = segunda-feira e assim por diante, em uma coluna calculada:</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>Funciona melhor com outras expressões que retornam um número, como DAYOFWEEK, DAYOFMONTH e MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Concatena a string e é formatada da seguinte maneira:</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>A seguir estão alguns exemplos de separadores que você pode incluir:</p> 
    <ul> 
     <li>um espaço: " "</li> 
     <li>um traço: "-"</li> 
     <li>uma barra: "/"</li> 
     <li>uma vírgula: ","</li> 
     <li>uma palavra: "ou", "e"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTAINS</strong> </td> 
   <td>Retorna verdadeiro se a string findText for encontrada dentro da string withinText e estiver formatada da seguinte maneira:

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Escapa quaisquer caracteres especiais na string para que possam ser incluídos em um argumento de URL.<p>A expressão é formatada da seguinte maneira:</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FORMAT</strong> </td> 
   <td><p>Retorna o texto formatado. Apenas as opções de parâmetros listadas aqui são permitidas com FORMAT.</p>
   <p>As opções de cor são $$POSITIVE, $$INFORMATIVE, $$NEGATIVE, $$NOTICE e as outras opções de formatação são $$BOLD, $$ITALIC, $$UNDERLINE. É permitida apenas uma opção de cor, juntamente com até três outras opções de formatação. Se nenhuma opção de cor for especificada, a cor padrão do sistema será aplicada.</p>
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>FORMAT($$POSITIVE, $$BOLD, $$ITALIC)</code></p>
   <p>Observação: esta expressão não é compatível com o Workfront Planning.</p></td> 
  </tr>   
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Avalia uma condição especificada e retorna o valor da trueExpression se ela for verdadeira, ou o valor da falseExpression se ela for falsa.</p>

<p>A expressão é formatada da seguinte maneira:</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>Por exemplo, você pode comparar dois campos de data diferentes seguidos por um resultado Verdadeiro/Falso como uma string de dados:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>Na linguagem cotidiana, essa afirmação significa: “SE a data de conclusão prevista do meu objeto for ‘maior que’ a data de conclusão planejada do mesmo objeto, exiba as palavras ‘Fora do prazo’ neste campo; caso contrário, exiba as palavras ‘Dentro do prazo’”.</p>

<p>Se você não quiser rotular as expressões verdadeiras ou falsas, deve inserir um rótulo em branco em sua declaração, como:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>Ou</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>Para obter mais informações sobre como criar instruções “IF”, consulte <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Visão geral das instruções “IF”</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Permite procurar um valor específico em uma string de valores possíveis. Se o valor que você está procurando for igual a um dos valores fornecidos, a expressão retornará a trueExpression; caso contrário, retornará a falseExpression.</p> 
   <p>A expressão é formatada da seguinte maneira:</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>Por exemplo, você pode encontrar um proprietário de projeto específico e marcar esses projetos com uma etiqueta específica em uma exibição de projeto: <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> Na linguagem cotidiana, essa afirmação significa: “Se o proprietário do projeto for Jennifer Campbell ou Rick Kuvec, marque este projeto com ‘Equipe de Marketing’; caso contrário, marque-o com ‘Outras equipes’.”</p> 
    <p> Se você não quiser rotular as expressões verdadeiras ou falsas, deve inserir um rótulo em branco em sua declaração, como: </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>Ou </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Retorna verdadeiro se o valor for igual a um dos valores fornecidos; caso contrário, a expressão retorna falso.</p> <p>A expressão é formatada da seguinte maneira:

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Retorna verdadeiro se o valor for nulo ou em branco; caso contrário, a expressão retorna falso.</p> <p>A expressão é formatada da seguinte maneira:

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>Retorna um número especificado de caracteres do lado esquerdo de uma string e é formatado da seguinte maneira:</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Retorna o comprimento de uma string e é formatado da seguinte maneira:</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>Retorna a string em minúsculas e formatada da seguinte maneira:

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PASCAL</strong> </td> 
   <td> <p>Converte a string de entrada para PascalCase, colocando em maiúscula a primeira letra de cada palavra e removendo todos os espaços. </p>
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>PASCAL(string) </code></p>
   <p>Por exemplo, “olá mundo” se torna “OláMundo”</p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>REMOVEACCENTS</strong> </td> 
   <td> <p>Remove os sinais diacríticos de todos os caracteres acentuados na string de entrada. </p> 
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>REMOVEACCENTS(string)</code></p> 
   <p>Por exemplo, “Olá mündó com àcentós” torna-se “Ola mundo com acentos”. </p>
   </td> 
  </tr>
  <tr> 
   <td><strong>REPLACE</strong> </td> 
   <td> <p>Substitui todas as ocorrências de string2 por string3 em string1.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr>

<tr> 
   <td><strong>REPLACEPATTERN</strong> </td> 
   <td> <p>Substitui as correspondências do padrão fornecido pela string de substituição. </p> 
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>REPLACEPATTERN (string, pattern, replacement string)</code></p> 
   <p>Por exemplo, REPLACEPATTERN("foo123bar", "\d+", "_") gera a string “foo_bar”.
   </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>Retorna um número especificado de caracteres do lado direito de uma string e é formatado da seguinte maneira:</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>Retorna o índice da primeira ocorrência de findText na string withinText, começando na posição inicial especificada, ou –1 se o texto não for encontrado.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCARRAY</strong> </td> 
   <td> <p>Ordena os elementos da matriz em ordem crescente e os converte para o tipo do primeiro elemento.</p>
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>SORTASCARRAY(array)</code></p>
   <p>Por exemplo, ["–12,6", –13,0] torna-se ["–12,6", "–13"].</p>
   <p>Observação: esta expressão não é compatível com o Workfront Planning.</p></td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCARRAY</strong> </td> 
   <td> <p>Ordena os elementos da matriz em ordem decrescente e os converte para o tipo do primeiro elemento.</p>
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>SORTDESCARRAY(array)</code></p>
   <p>Por exemplo, ["–12,6", –13,0] torna-se ["–13", "–12.6"].</p>
   <p>Observação: esta expressão não é compatível com o Workfront Planning.</p></td> 
  </tr>
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>Converte um número em uma string e é formatado da seguinte maneira:</p>

<p><code>STRING(number)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Classifica uma lista de strings em ordem crescente e é formatada da seguinte maneira:</p>
   <p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Classifica uma lista de strings em ordem decrescente e é formatada da seguinte maneira:</p>
   <p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Retorna caracteres de uma string com base no índice inicial e final especificado e é formatado da seguinte maneira:</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SWITCH</strong> </td> 
   <td> <p>Avalia a expressão em contraste com uma lista de valores e retorna o resultado equivalente ao primeiro valor correspondente.</p>
   <p>A expressão é formatada da seguinte forma:</p>
   <p><code>SWITCH(expression, value1, result1, [value2, result2], ...)</code></p>
   <p>Esta expressão não é suportada no Workfront Planning.</p></td> 
  </tr>   
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Remove os espaços em branco do início e do final de uma string e é formatado da seguinte maneira:</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Retorna uma string em maiúsculas e é formatada da seguinte maneira:</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>

