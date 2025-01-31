---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Visão geral das expressões de dados calculadas
description: Você pode usar expressões de dados para definir campos de dados personalizados calculados no Adobe Workfront. As expressões calculadas conectam campos existentes do Workfront em instruções que geram um novo campo.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: b60a1e74d62e9b3945f69dc590f8cc202302c5af
workflow-type: tm+mt
source-wordcount: '2425'
ht-degree: 0%

---

# Visão geral das expressões de dados calculadas

<!--Audited: 12/2023-->

Você pode usar expressões de dados para definir campos personalizados calculados no Adobe Workfront. As expressões calculadas conectam campos existentes do Workfront em instruções que geram um novo campo.

Você pode usar expressões de dados calculados em:

* Um campo personalizado calculado em um formulário personalizado

  Para obter mais informações sobre como criar campos personalizados calculados em formulários personalizados no Workfront, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Uma coluna personalizada calculada em um relatório ou lista, ao usar o modo de texto

  Para obter mais informações sobre como usar o modo de texto em relatórios e exibições, consulte [Visão geral do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Sintaxe de campos personalizados calculados versus colunas personalizadas calculadas

Embora as funções usadas sejam as mesmas, a sintaxe para criar uma expressão em um campo personalizado calculado pode ser diferente dela para criar uma coluna personalizada calculada.

As diferenças entre as duas sintaxes são:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Campo personalizado calculado</strong></td> 
   <td><strong>Elemento de relatório personalizado calculado</strong></td> 
  </tr> 
   <td>Colocar nomes de campo entre chaves</td> 
   <td>Não coloque os nomes dos campos entre parênteses ou entre parênteses ao usá-los em uma <p><code>valuefield </code></p>linha. <p>Coloque os nomes de campo entre chaves ao usá-los em uma <p><code>valueexpression</code></p> linha.</p> </td> 
  </tr> 
  <tr> 
   <td>Separar os campos por períodos</td> 
   <td> <p>Separe os campos por dois pontos ao usá-los em uma <p><code>valuefield </code></p>linha</p> <p>Separe os campos por pontos ao usá-los em uma <p><code>valueexpression </code></p>linha. </p> </td> 
  </tr> 
 </tbody> 
</table>

Por exemplo:

* Em um campo personalizado, em um formulário personalizado para tarefas, você usaria o seguinte para gerar o nome do projeto principal da tarefa à qual o formulário personalizado está anexado:


  ` {project}.{name}`


* Em uma coluna personalizada em um relatório, você usaria o seguinte para adicionar uma coluna personalizada Nome do projeto em um relatório de tarefa:


  `valuefield=project:name`


  Ou

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >A mesma sintaxe se aplica a todos os elementos de relatório de modo de texto nos quais as expressões calculadas são usadas: exibições, filtros, agrupamentos, prompts.

Para obter mais informações sobre a sintaxe que deve ser usada em uma coluna personalizada calculada, consulte [Visão geral do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Expressões de dados que você pode usar

As listas abaixo definem as expressões disponíveis que podem ser usadas ao criar um dos três diferentes tipos de campos personalizados calculados no Workfront:

* [Campos personalizados calculados de data e hora](#date-time-calculated-custom-fields)
* [Campos personalizados calculados matemáticos](#mathematical-calculated-custom-fields)
* [Campos personalizados calculados em texto](#text-calculated-custom-fields)

Você pode usar as expressões listadas abaixo para criar colunas personalizadas calculadas. No entanto, você deve usar a sintaxe correta para uma coluna personalizada calculada, conforme descrito na seção [Sintaxe de campos personalizados calculados versus colunas personalizadas calculadas](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) deste artigo.

### Campos personalizados calculados de data e hora {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Se você criar um cálculo de data e hora que não inclua uma parte do tempo ou que use os curingas de data $$TODAY ou $$NOW, o sistema usará a data de acordo com o fuso horário Coordenado Universal Time (UTC), não de acordo com o fuso horário local. Isso pode causar um resultado inesperado de data.

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
   <td> <p>Adiciona o número de dias à data. O valor do número pode incluir dias parciais. Por exemplo, 1.5 adiciona um dia e meio à data.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADICIONARDIASDASEMANA</strong> </td> 
   <td> <p>Adiciona o número de dias da semana à data. Essa expressão só adiciona valores inteiros à data, arredondando para baixo. </p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Adiciona o número de meses à data e é formatado da seguinte maneira:

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ANOSSUPLEMENTARES</strong> </td> 
   <td> <p>Adiciona o número de anos à data e é formatado da seguinte maneira:</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>HORA_ADICIONAL</strong> </td> 
   <td> <p>Adiciona o número de horas à data e é formatado da seguinte maneira:</p>

<p><code>ADDHOUR(date, number)</code></p>
   <p>Nota: Esta função não é suportada no Workfront Planning.</p></td> 
  </tr>
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Limpa a parte de tempo de uma data e é formatada da seguinte maneira. Neste exemplo, a data é a Data de Entrada para um objeto de trabalho.</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATA</strong> </td> 
   <td> <p>Converte uma string em uma data e é formatada da seguinte maneira:</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DIFERENÇA</strong> </td> 
   <td> <p>Retorna o número de dias entre as duas datas, levando em conta os dias de início e término do período selecionado, bem como os carimbos de data/hora nesses dias. Por exemplo, se a hora de início da data de início for 15h, o dia de início não será contado como um dia inteiro.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Retorna o dia do mês da data como um número, entre 1 e 31.</p> <p>A expressão é formatada da seguinte maneira. Neste exemplo, a data é a Data de Entrada para um objeto de trabalho.</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Retorna o dia da semana da data como um número, entre 1 (domingo) e 7 (sábado).</p> <p>A expressão é formatada da seguinte maneira. Neste exemplo, a data é a Data de Entrada para um objeto de trabalho.</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Retorna o total de dias no mês da data como um número e é formatado da seguinte maneira. Neste exemplo, a data é a Data de Entrada para um objeto de trabalho.</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Retorna o total de dias da semana entre a data informada e o fim da semana, ou o fim do mês, o qual vier primeiro. Neste exemplo, a data é a Data de Entrada para um objeto de trabalho.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Retorna o total de dias no ano da data como um número e é formatado da seguinte maneira: Neste exemplo, a data é a Data de Entrada para um objeto de trabalho.</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Retorna a data mais recente na lista e é formatado da seguinte maneira:</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Retorna a data mais antiga na lista e é formatado da seguinte maneira:</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>HORA</strong> </td> 
   <td> <p>Retorna a hora da data como um número entre 0 e 23.</p> <p>A expressão é formatada da seguinte maneira. Neste exemplo, a data é a Data de Entrada para um objeto de trabalho.</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTO</strong> </td> 
   <td> <p>Retorna os minutos da data como um número entre 0 e 60, formatado da seguinte maneira: Neste exemplo, a data é a Data de Entrada para um objeto de trabalho.</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MÊS</strong> </td> 
   <td> <p>Retorna o mês da data como um número entre 1 e 12, formatado da seguinte maneira. Neste exemplo, a data é a Data de Entrada para um objeto de trabalho.</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SEGUNDO</strong> </td> 
   <td> <p>Retorna o segundo da data como um número entre 0 e 60, formatado da seguinte maneira: Neste exemplo, a data é a Data de Entrada para um objeto de trabalho.</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DIFERENÇADIASEMANA</strong> </td> 
   <td> <p>Retorna o número de dias da semana entre duas datas, levando em conta os dias de início e término do período selecionado, bem como os carimbos de data/hora nesses dias. Por exemplo, se a hora de início da data de início for 15h, o dia de início não será contado como um dia inteiro.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Retorna o número de minutos agendados entre as datas de acordo com o agendamento padrão.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ANO</strong> </td> 
   <td> <p>Retorna o ano da data como um número de 4 dígitos, formatado da seguinte maneira: Neste exemplo, a data é a Data de Entrada para um objeto de trabalho.</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### Campos personalizados matematicamente calculados {#mathematical-calculated-custom-fields}

Você pode criar um campo personalizado calculado que use algumas das seguintes expressões matemáticas:

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
   <td><strong>MÉDIA</strong> </td> 
   <td>Retorna a média dos números e é formatada da seguinte maneira:

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Arredonda um número para o próximo inteiro imediatamente acima e é formatado da seguinte maneira. Este exemplo usa o número de objetos abaixo do objeto ao qual o formulário personalizado está anexado.

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Divide todos os números na ordem fornecida e é formatado da seguinte maneira:

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ANDAR</strong> </td> 
   <td>Arredonda um número para o próximo inteiro imediatamente abaixo e é formatado da seguinte maneira: Este exemplo usa o número de objetos abaixo do objeto ao qual o formulário personalizado está anexado.

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Retorna o valor logaritmo natural do número e é formatado da seguinte maneira:

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Retorna o logaritmo do número2 com base no número1 e é formatado da seguinte maneira:

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
   <td><strong>NÚMERO</strong> </td> 
   <td>Converte uma string em número e é formatada da seguinte maneira:<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>POTÊNCIA</strong> </td> 
   <td>Retorna um número elevado a potência informada e é formatado da seguinte forma:

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PRODUÇÃO</strong> </td> 
   <td>Multiplica todos os números e é formatado da seguinte maneira:

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>Nota</b></p>

<p>Ao multiplicar campos que contêm horas, certifique-se de que você entende se o banco de dados salva as horas nos campos selecionados em minutos, horas ou segundos. Se as horas forem salvas em minutos ou segundos, mas forem exibidas em horas na interface do Workfront, talvez seja necessário considerar a conversão de minutos ou segundos em horas ao gravar uma expressão usando esse cálculo. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Arredonda o número para cima de acordo com a precisão de casas decimais especificada e é formatado da seguinte maneira:

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Ordena os números em ordem crescente e é formatado da seguinte maneira:</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Ordena os números em ordem decrescente e é formatado da seguinte maneira:

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Retorna a raiz quadrada de um número e é formatada da seguinte maneira. Este exemplo usa o número de objetos abaixo do objeto ao qual o formulário personalizado está anexado.</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Subtrai todos os números na ordem fornecida e é formatado da seguinte maneira:

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SOMA</strong> </td> 
   <td>Adiciona todos os números e é formatado da seguinte maneira:

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### Campos personalizados calculados em texto {#text-calculated-custom-fields}

É possível criar um campo personalizado calculado que exiba um valor de formato de texto usando as seguintes expressões:

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
   <td><strong>MATRIZ</strong> </td> 
   <td> <p>Converte uma string em uma matriz. O delimitador pode ser qualquer string.</p> 
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>ARRAY(string1, "delimiter")</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>COMPRIMENTOARRAY</strong> </td> 
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
   <td><strong>SORTASCARRAY</strong> </td> 
   <td> <p>Ordena os elementos da matriz em ordem crescente e os converte no tipo do primeiro elemento.</p>
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>SORTASCARRAY(array)</code></p>
   <p>Por exemplo, ["-12.6", -13.0] torna-se ["-12.6", "-13"].</p>
   <p>Nota: Esta função não é suportada no Workfront Planning.</p></td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCARRAY</strong> </td> 
   <td> <p>Ordena os elementos da matriz em ordem decrescente e os converte no tipo do primeiro elemento.</p>
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>SORTDESCARRAY(array)</code></p>
   <p>Por exemplo, ["-12.6", -13.0] torna-se ["-13", "-12.6"].</p>
   <p>Nota: Esta função não é suportada no Workfront Planning.</p></td> 
  </tr>
  <tr>   
   <td><strong>CASO</strong> </td> 
   <td> <p>É usado com outras expressões para escolher um valor em uma lista, com base em um número de índice. </p>
   <p>Um número de índice é um campo ou função que retorna um valor numérico (geralmente em um intervalo conhecido).</p> 
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>Por exemplo, a expressão a seguir retorna o nome do dia da semana, em que 1=domingo, 2=segunda-feira e assim por diante, em uma coluna calculada:</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>Funciona melhor com outras expressões que retornam um número, como DAYOFWEEK, DAYOFMONTH e MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Concatena a string e é formatada da seguinte maneira:</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>Veja a seguir exemplos de separadores que podem ser incluídos:</p> 
    <ul> 
     <li>um espaço: " "</li> 
     <li>um traço: "-"</li> 
     <li>uma barra: "/"</li> 
     <li>uma vírgula: ","</li> 
     <li>uma palavra: "ou", "e"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTÉM</strong> </td> 
   <td>Retorna verdadeiro se a string findText for encontrada dentro da string withinText e estiver formatada da seguinte maneira:

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Escapa quaisquer caracteres especiais na string para que eles possam ser incluídos em um argumento de URL.<p>A expressão é formatada da seguinte maneira:</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FORMATO</strong> </td> 
   <td><p>Retorna o texto formatado. As opções de cor são $$POSITIVE, $$INFORMATIVE, $$NEGATIVE, $$NOTICE e as outras opções de formatação são $$BOLD, $$ITALIC, $$UNDERLINE. Somente uma opção de cor pode ser usada por função, juntamente com até três outras opções de formatação. Se nenhuma opção de cor for especificada, a cor padrão do sistema será aplicada.</p>
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>FORMAT($$POSITIVE, $$BOLD, $$ITALIC)</code></p>
   <p>Nota: Esta função não é suportada no Workfront Planning.</p></td> 
  </tr>   
  <tr> 
   <td><strong>SE</strong> </td> 
   <td> <p>Avalia uma condição especificada e retorna o valor da expressãoVerdadeira se for verdadeira, ou o valor da expressãoFalsa se for falsa.</p>

<p>A expressão é formatada da seguinte maneira:</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>Por exemplo, você pode comparar dois campos de data diferentes seguidos por um resultado Verdadeiro/Falso como uma string de dados:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>Na linguagem cotidiana, essa declaração significa: "Se a Data de conclusão projetada do meu objeto for 'Maior que' a Data de conclusão planejada do meu mesmo objeto, exiba as palavras 'Fora do rastreamento' neste campo; caso contrário, exiba as palavras 'No rastreamento'".</p>

<p>Se não quiser rotular as expressões true ou false, insira um rótulo em branco na instrução, como:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>Ou</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>Para obter mais informações sobre a compilação de instruções "IF", consulte a <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref"> visão geral das instruções "IF"</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Permite procurar um valor específico em uma string de valores possíveis. Se o valor que você está procurando for igual a um dos valores fornecidos, a expressão retornará trueExpression; caso contrário, retornará falseExpression.</p> 
   <p>A expressão é formatada da seguinte maneira:</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>Por exemplo, você pode encontrar um Proprietário do projeto específico e marcar esses projetos com uma tag especificada em uma exibição de projeto: <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> No discurso diário, essa declaração significa: "Se o Proprietário do Projeto é Jennifer Campbell ou Rick Kuvec, marque este projeto com 'Equipe de Marketing'; caso contrário, marque-o com 'Outras Equipes'."</p> 
    <p> Se não quiser rotular as expressões true ou false, insira um rótulo em branco na instrução, como: </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>Ou </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>EM</strong> </td> 
   <td> <p>Retornará true se o valor for igual a um dos valores fornecidos; caso contrário, a expressão retornará false.</p> <p>A expressão é formatada da seguinte maneira:

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Retornará true se o valor for nulo ou vazio; caso contrário, a expressão retornará false.</p> <p>A expressão é formatada da seguinte maneira:

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ESQUERDA</strong> </td> 
   <td> <p>Retorna o número especificado de caracteres da parte esquerda de uma cadeia de caracteres e é formatado da seguinte maneira:</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Retorna o comprimento de uma string e é formatado da seguinte maneira:</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>INFERIOR</strong> </td> 
   <td>Retorna a cadeia de caracteres em minúsculas e é formatada da seguinte maneira:

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTITUIR</strong> </td> 
   <td> <p>Substitui todas as ocorrências da string2 pela string3 na string1.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DIREITA</strong> </td> 
   <td> <p>Retorna o número especificado de caracteres da string informada, a partir da direita, e tem a seguinte formatação:</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>PESQUISAR</strong> </td> 
   <td> <p>Retorna o índice da primeira ocorrência do textoPesquisa dentro do textoBase, iniciando na posição inicial informada, ou retorna -1 se o texto não for encontrado.</p> <p>A expressão é formatada da seguinte maneira:</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>CADEIA DE CARACTERES</strong> </td> 
   <td> <p>Converte um número em uma cadeia de caracteres e é formatado da seguinte maneira:</p>

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
   <td> <p>Retorna os caracteres de uma string com base no índice de início e término especificado e é formatado da seguinte maneira:</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ALTERNAR</strong> </td> 
   <td> <p>Avalia a expressão em relação a uma lista de valores e retorna o resultado correspondente ao primeiro valor correspondente.</p>
   <p>A expressão é formatada da seguinte maneira:</p>
   <p><code>SWITCH(expression, value1, result1, [value2, result2], ...)</code></p>
   <p>Esta função não é suportada no Workfront Planning.</p></td> 
  </tr>   
  <tr> 
   <td><strong>CORTAR</strong> </td> 
   <td> <p>Remove os espaços em branco do início e do fim de uma string e é formatado da seguinte maneira:</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUPERIOR</strong> </td> 
   <td> <p>Retorna uma cadeia de caracteres em maiúsculas e é formatada da seguinte maneira:</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
