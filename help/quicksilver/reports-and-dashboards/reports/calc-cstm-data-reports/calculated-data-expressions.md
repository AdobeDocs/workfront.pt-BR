---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Expressões de dados calculadas
description: Você pode usar expressões de dados para definir campos de dados personalizados calculados no Adobe Workfront. Eles conectam campos existentes do Workfront em instruções que geram um novo campo.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '2368'
ht-degree: 7%

---

# Expressões de dados calculadas

Você pode usar expressões de dados para definir campos de dados personalizados calculados no Adobe Workfront. Eles conectam campos existentes do Workfront em instruções que geram um novo campo.

Você pode usar expressões de dados calculados em:

* Um formulário personalizado

   Para obter mais informações sobre como criar campos de dados personalizados calculados em formulários personalizados no Workfront, consulte [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Uma coluna personalizada calculada em um relatório ou lista, ao usar o modo de texto

   Para obter mais informações sobre como usar o modo de texto em relatórios e visualizações, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Sintaxe de campos personalizados calculados versus colunas personalizadas calculadas

Embora as funções usadas sejam as mesmas, a sintaxe para criar uma expressão em um campo personalizado calculado pode ser diferente do que é para criar uma coluna personalizada calculada.

Por exemplo:

* Em um campo personalizado, em um formulário personalizado para tarefas, você usaria o seguinte para gerar o nome do projeto principal da tarefa à qual o formulário personalizado está anexado:

   ```
   {project}.{name}
   ```

* Em uma coluna personalizada em um relatório, você usaria o seguinte para adicionar uma coluna personalizada Nome do projeto em um relatório de tarefa:

   ```
   valuefield=project:name
   ```

   Ou

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >A mesma sintaxe se aplica a todos os elementos de relatório de modo de texto nos quais as expressões calculadas são usadas: exibições, filtros, agrupamentos, prompts.

As diferenças entre as duas sintaxes são:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Campo personalizado calculado</strong></td> 
   <td><strong>Elemento de relatório personalizado calculado</strong></td> 
  </tr> 
   <td>Coloque os nomes de campo entre chaves.</td> 
   <td>Não coloque os nomes dos campos entre parênteses ou entre parênteses ao usá-los em uma <code>valuefield </code>linha. <p>Coloque os nomes de campo entre chaves ao usá-los em uma <code>valueexpression</code> linha.</p> </td> 
  </tr> 
  <tr> 
   <td>Separe os campos por pontos.</td> 
   <td> <p>Separe os campos por dois pontos ao usá-los em uma <code>valuefield </code>linha</p> <p>Separe os campos por pontos ao usá-los em uma <code>valueexpression </code>linha. </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações sobre a sintaxe que deve ser usada em uma coluna personalizada calculada, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Expressões de dados que você pode usar

As listas abaixo definem as expressões disponíveis que podem ser usadas ao criar um dos três diferentes tipos de campos personalizados calculados no Workfront:

* [Campos personalizados calculados de data e hora](#date-time-calculated-custom-fields)
* [Campos personalizados matematicamente calculados](#mathematical-calculated-custom-fields)
* [Campos personalizados calculados em texto](#text-calculated-custom-fields)

### Campos personalizados calculados de data e hora {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Se você criar um cálculo de data e hora que não inclua uma parte do tempo ou que use os curingas de data $$TODAY ou $$NOW, o sistema usará a data de acordo com o fuso horário Coordenado Universal Time (UTC), não de acordo com o fuso horário local. Isso pode causar um resultado inesperado de data.

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
   <td> <p>Essa expressão adiciona o número de dias à data. O valor do número pode incluir dias parciais (por exemplo, 1,5 adicionará um dia e meio à data).</p> <p>A expressão é formatada da seguinte maneira:</p><pre>ADDDAYS(data, número)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADICIONARDIASDASEMANA</strong> </td> 
   <td> <p>Essa expressão adiciona o número de dias da semana à data. Essa expressão só adiciona valores inteiros à data, arredondando para baixo. </p> <p>A expressão é formatada da seguinte maneira:</p><pre>ADICIONARDIASDASEMANA(data, número)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Essa expressão adiciona o número de meses à data e é formatada da seguinte maneira:</p><pre>ADDMONTHS(data, número)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Essa expressão adiciona o número de anos à data e é formatada da seguinte maneira:</p><pre>ADDYEARS(data, número)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Essa expressão limpa a parte de tempo de uma data e é formatada da seguinte maneira. Neste exemplo, a data é a data de entrada para um objeto de trabalho.</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATA</strong> </td> 
   <td> <p>Essa expressão converte uma string em uma data e é formatada da seguinte maneira:</p><pre>DATE(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Essa expressão retorna o número de dias entre as duas datas, levando em conta os dias de início e término do período selecionado, bem como os carimbos de data e hora nesses dias. Por exemplo, se a hora de início da data de início for 15h, o dia de início não será contado como um dia inteiro.</p> <p>A expressão é formatada da seguinte maneira:</p><pre>DATEDIFF(data1, data2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Essa expressão retorna o dia do mês da data como um número, entre 1 e 31.</p> <p>A expressão é formatada da seguinte maneira. Neste exemplo, a data é a data de entrada para um objeto de trabalho.</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Essa expressão retorna o dia da semana da data como um número, entre 1 (domingo) e 7 (sábado).</p> <p>A expressão é formatada da seguinte maneira. Neste exemplo, a data é a data de entrada para um objeto de trabalho.</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Essa expressão retorna o total de dias no mês da data como um número e é formatada da seguinte maneira. Neste exemplo, a data é a data de entrada para um objeto de trabalho.</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Essa expressão retorna o total de dias da semana entre a data e o fim da semana, ou o fim do mês, o que ocorrer primeiro. Neste exemplo, a data é a data de entrada para um objeto de trabalho.</p> <p>A expressão é formatada da seguinte maneira:</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Essa expressão retorna o total de dias no ano da data como um número e é formatada da seguinte maneira. Neste exemplo, a data é a data de entrada para um objeto de trabalho.</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Essa expressão retorna a data mais recente na lista e é formatada da seguinte maneira:</p><pre>DMAX(data1, data2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Essa expressão retorna a data mais antiga na lista e é formatada da seguinte maneira:</p><pre>DMIN(data1, data2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HORA</strong> </td> 
   <td> <p>Essa expressão retorna a hora da data como um número entre 0 e 23.</p> <p>A expressão é formatada da seguinte maneira. Neste exemplo, a data é a data de entrada para um objeto de trabalho.</p><pre>HORA({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Essa expressão retorna os minutos da data como um número entre 0 e 60, formatado da seguinte maneira. Neste exemplo, a data é a data de entrada para um objeto de trabalho.</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MÊS</strong> </td> 
   <td> <p>Essa expressão retorna o mês da data como um número entre 1 e 12, formatado da seguinte maneira. Neste exemplo, a data é a data de entrada para um objeto de trabalho.</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Essa expressão retorna o segundo dia da data como um número entre 0 e 60, formatado da seguinte maneira. Neste exemplo, a data é a data de entrada para um objeto de trabalho.</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Essa expressão retorna o número de dias da semana entre duas datas, levando em conta os dias de início e término do período selecionado, bem como os carimbos de data e hora nesses dias. Por exemplo, se a hora de início da data de início for 15h, o dia de início não será contado como um dia inteiro.</p> <p>A expressão é formatada da seguinte maneira:</p><pre>WEEKDAYDIFF(data2, data1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Essa expressão retorna o número de minutos agendados entre as datas de acordo com o agendamento padrão.</p> <p>A expressão é formatada da seguinte maneira:</p><pre>WORKMINUTESDIFF(data1, data2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ANO</strong> </td> 
   <td> <p>Essa expressão retorna o ano da data como um número de 4 dígitos, formatado da seguinte maneira. Neste exemplo, a data é a data de entrada para um objeto de trabalho.</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### Campos personalizados matematicamente calculados {#mathematical-calculated-custom-fields}

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
   <td>Essa expressão retorna o valor absoluto do número e é formatada da seguinte maneira. Este exemplo usa o número de objetos abaixo do objeto ao qual o formulário personalizado está anexado.<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>Essa expressão retorna a média dos números e é formatada da seguinte maneira:<pre>AVERAGE(número1, número2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Essa expressão arredonda um número para cima até o inteiro mais próximo e é formatada da seguinte maneira. Este exemplo usa o número de objetos abaixo do objeto ao qual o formulário personalizado está anexado.<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Essa expressão divide todos os números na ordem fornecida e é formatada da seguinte maneira:<pre>DIV(número1, número2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Essa expressão arredonda um número para o número inteiro mais próximo e é formatada da seguinte maneira. Este exemplo usa o número de objetos abaixo do objeto ao qual o formulário personalizado está anexado.<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Essa expressão retorna o valor logaritmo natural do número e é formatada da seguinte maneira:<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Essa expressão retorna o logaritmo do número2 com base no número1 e é formatada da seguinte maneira:<pre>LOG(número1, número2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Essa expressão retorna o maior item da lista e é formatada da seguinte maneira:<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Essa expressão retorna o menor item da lista e é formatada da seguinte maneira:<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>NÚMERO</strong> </td> 
   <td>Essa expressão converte uma string em um número e é formatada da seguinte maneira:<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Essa expressão retorna um número elevado a uma potência e é formatada da seguinte maneira:<pre>POWER(número, potência)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Essa expressão multiplica todos os números e é formatada da seguinte maneira:<pre>PROD(número1, número2, ....)</pre>
   <b>Nota</b>

Ao multiplicar campos que contêm horas, certifique-se de entender se as horas nos campos selecionados são salvas em minutos, horas ou segundos no banco de dados. Se as horas forem salvas em minutos ou segundos, mas forem exibidas em horas na interface do Workfront, talvez seja necessário considerar a conversão de minutos ou segundos em horas ao gravar uma expressão usando esse cálculo.
</td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Essa expressão arredonda o número para cima de acordo com a precisão de decimais especificada e é formatada da seguinte maneira:<p>ROUND(número, precisão)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Essa expressão ordena os números em ordem crescente e é formatada da seguinte maneira:</p><pre>SORTASCNUM(número1, número2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Essa expressão ordena os números em ordem decrescente e é formatada da seguinte maneira:<pre>SORTDESCNUM(numbero1, numbero2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Essa expressão retorna uma raiz quadrada de um número e é formatada da seguinte maneira. Este exemplo usa o número de objetos abaixo do objeto ao qual o formulário personalizado está anexado.</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Essa expressão subtrai todos os números na ordem fornecida e é formatada da seguinte maneira:<pre>SUB(número1, número2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Essa expressão adiciona todos os números e é formatada da seguinte maneira:<pre>SUM(número1, número2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### Campos personalizados calculados em texto {#text-calculated-custom-fields}

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
   <td><strong>CASE</strong> </td> 
   <td> <p>Essa expressão é usada com outras expressões para escolher um valor em uma lista, com base em um número de índice. Um número de índice é um campo ou função que retorna um valor numérico (geralmente em um intervalo conhecido).</p> <p>A expressão é formatada da seguinte maneira:</p><pre>CASE(número_do_índice, value1, value2, ...)</pre> <p>Por exemplo, a expressão a seguir retorna o nome do dia da semana, em que 1=domingo, 2=segunda-feira e assim por diante, em uma coluna calculada:</p><pre>CASE(DAYOFWEEK({entryDate}),"domingo","segunda-feira","terça-feira","quarta-feira","quinta-feira","sexta-feira","sábado")</pre> <p>Essa expressão funciona melhor com outras expressões que retornam um número, como DAYOFWEEK, DAYOFMONTH e MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Essa expressão concatena a sequência de caracteres e é formatada da seguinte maneira:</p><pre>CONCAT(sequência1,"separador", sequência2)</pre> <p>Veja a seguir exemplos de separadores que podem ser incluídos:</p> 
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
   <td>Essa expressão retornará true se a string findText for encontrada na string withinText e estiver formatada da seguinte maneira:<pre>CONTAINS(textoPesquisa, textoBase)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Essa expressão escapa todos os caracteres especiais na string para que eles possam ser incluídos em um argumento de URL.<p>A expressão é formatada da seguinte maneira:</p><pre>ENCODEURL(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SE</strong> </td> 
   <td> <p>Essa expressão avalia uma condição especificada e retorna o valor da expressãoVerdadeira se for verdadeira, ou o valor da expressãoFalsa se for falsa.</p> <p>A expressão é formatada da seguinte maneira:</p><pre>IF(condição, expressãoVerdadeira, expressãoFalsa)</pre> <p>Por exemplo, você pode comparar dois campos de data diferentes seguidos por um resultado Verdadeiro/Falso como uma string de dados:</p><pre>IF({projectionCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</pre> <p>Na linguagem cotidiana, essa declaração significa: "Se a Data de conclusão projetada do meu objeto for 'Maior que' a Data de conclusão planejada do meu mesmo objeto, exiba as palavras 'Fora do rastreamento' neste campo; caso contrário, exiba as palavras 'No rastreamento'".</p> <p>Se não quiser rotular as expressões true ou false, insira um rótulo em branco na instrução, como:</p><pre>IF({projectionCompletionDate}&gt;{plannedCompletionDate},"","No caminho")</pre> <p>Ou</p><pre>IF({projectionCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</pre> <p>Para obter mais informações sobre a criação de instruções "IF", consulte <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Visão geral das instruções "IF"</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Essa expressão permite procurar um valor específico em uma cadeia de caracteres de valores possíveis. Se o valor que você está procurando for igual a um dos valores fornecidos, a expressão retornará trueExpression; caso contrário, retornará falseExpression.</p> <p>A expressão é formatada da seguinte maneira:</p><pre>IFIN(valor, valor1, valor2,..., expressãoVerdadeira, expressãoFalsa)</pre> <p>Por exemplo, você pode encontrar um Proprietário do projeto específico e marcar esses projetos com uma tag especificada em uma exibição de projeto: <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> No discurso diário, essa declaração significa: "Se o Proprietário do Projeto é Jennifer Campbell ou Rick Kuvec, marque este projeto com 'Equipe de Marketing'; caso contrário, marque-o com 'Outras Equipes'."</p> <p> Se não quiser rotular as expressões true ou false, insira um rótulo em branco na instrução, como: </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>Ou </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>EM</strong> </td> 
   <td> <p>Esta expressão retornará true se o valor for igual a um dos valores fornecidos; caso contrário, a expressão retornará false.</p> <p>A expressão é formatada da seguinte maneira:</p><pre>IN(valor, valor1[, valor2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Essa expressão retornará true se o valor for nulo ou estiver vazio; caso contrário, a expressão retornará false.</p> <p>A expressão é formatada da seguinte maneira:</p><pre>ISBLANK(valor)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ESQUERDO</strong> </td> 
   <td> <p>Essa expressão retorna um número especificado de caracteres do lado esquerdo de uma cadeia de caracteres e é formatada da seguinte maneira:</p><pre>LEFT(string, tamanho)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Essa expressão retorna o comprimento de uma string e é formatada da seguinte maneira:</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>Essa expressão retorna a cadeia de caracteres em minúsculas e é formatada da seguinte maneira:<pre>LOWER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTITUIR</strong> </td> 
   <td> <p>Essa expressão substitui todas as ocorrências da sequência2 pela sequência3 na sequência1.</p> <p>A expressão é formatada da seguinte maneira:</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DIREITO</strong> </td> 
   <td> <p>Essa expressão retorna um número especificado de caracteres do lado direito de uma cadeia de caracteres e é formatada da seguinte maneira:</p><pre>RIGHT(string, tamanho)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>Esta expressão retorna o índice da primeira ocorrência de findText na string withinText, iniciando na posição inicial fornecida, ou -1 se o texto não for encontrado.</p> <p>A expressão é formatada da seguinte maneira:</p><pre>SEARCH(textoPesquisa, textoBase, início)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>Essa expressão converte um número em uma string e é formatada da seguinte maneira:</p><pre>STRING(número)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Essa expressão classifica uma lista de cadeias de caracteres em ordem crescente e é formatada da seguinte maneira:</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Essa expressão classifica uma lista de cadeias de caracteres em ordem decrescente e é formatada da seguinte maneira:</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Essa expressão retorna os caracteres de uma string com base no índice de início e término especificado e é formatada da seguinte maneira:</p><pre>SUBSTR({string}, número da posição inicial, número da posição final)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Essa expressão remove os espaços em branco do início e do fim de uma string e é formatada da seguinte maneira:</p><pre>TRIM(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Essa expressão retorna uma string em maiúsculas e é formatada da seguinte maneira:</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>
