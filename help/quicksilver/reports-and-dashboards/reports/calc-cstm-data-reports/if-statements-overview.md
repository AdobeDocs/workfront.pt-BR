---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Visão geral de instruções IF
description: Você pode usar instruções "IF" em linguagens de programação gerais. No Adobe Workfront, as instruções "IF" permitem comparar, formatar e reunir campos de dados para fins de relatório e dados personalizados. Além disso, pensar matematicamente sobre declarações "IF" leva a uma melhor compreensão conceitual, uma vez que as variáveis para expressões são comumente usadas.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 23b5ba9564b514e11c1ca9d5cca276238ef11066
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Visão geral das instruções &quot;IF&quot;

<!-- Audited: 1/2024 -->

Você pode usar instruções &quot;IF&quot; em linguagens de programação gerais. No Adobe Workfront, as instruções &quot;IF&quot; permitem comparar, formatar e reunir campos de dados para fins de relatório e dados personalizados. Além disso, pensar matematicamente sobre declarações &quot;IF&quot; leva a uma melhor compreensão conceitual, uma vez que as variáveis para expressões são comumente usadas.

## Recommendations para instruções &quot;IF&quot;

Considere o seguinte antes de criar uma instrução &quot;IF&quot;:

* Recomendamos uma compreensão básica de qualquer linguagem de programação geral, mas não a exigimos, para este guia.
* Precisamos de uma compreensão avançada da sintaxe do modo de texto do Workfront. Isso ajuda a compreender a terminologia da API do Workfront e a entender a sintaxe dos dados personalizados nesses formatos específicos.

  Para obter informações sobre a API do Workfront, consulte [noções básicas sobre API](../../../wf-api/general/api-basics.md).

  Para obter informações sobre como usar o modo de texto, consulte [Visão geral do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* Você pode criar instruções &quot;IF&quot; para os seguintes elementos do Workfront:

   * Visualizações
   * Agrupamento
   * Campos personalizados calculados

* Não é possível criar instruções &quot;IF&quot; para filtros. Isso resulta em um erro &quot;Ops&quot; no Workfront.
* A Equipe de suporte não ajuda na criação de dados personalizados. Você pode entrar em contato com a equipe de suporte depois de criar os campos ou colunas personalizados e não estiver vendo os resultados desejados. Para obter ajuda sobre como criar uma expressão, entre em contato com o seu Executivo de contas para saber mais sobre nossas opções de consultoria.
* Recomendamos escrever essas expressões primeiro em um editor de texto, como Sublime ou Visual Studio Code, pois isso ajuda a ver os dados com mais clareza do que apareceria no Workfront.

## Componentes de uma instrução &quot;IF&quot;

Você pode criar instruções &quot;IF&quot; no Workfront usando o seguinte formato:
<pre>IF(Condição,Expressão Verdadeira,Expressão Falsa)</pre>Os componentes de uma instrução "IF" são:

* **IF** = Esta é a expressão de dados calculados Workfront para &quot;função&quot;. Semelhante às expressões SUM e PROD, isso informa primeiro o sistema a entender a função como uma instrução &quot;IF&quot;. Use sempre letras maiúsculas para &quot;IF&quot; neste demonstrativo.\
  Para obter uma lista de todas as expressões de dados calculados, consulte [Visão geral das expressões de dados calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Condição** = Essa é a condição que a variável Workfront deve atender e é a base dessa equação. Tudo que pode ser especificado posteriormente na equação depende da condição. Você pode usar várias referências, comparações ou expressões matemáticas para iniciar uma equação. Alguns exemplos de condições são:

   * Uma data é posterior a outra data em um objeto especificado.
   * Um status é igual a um dos status disponíveis em um objeto especificado.
   * O percentual concluído de uma tarefa é menor ou maior que um determinado percentual.

* **Operador de Condição** = este é o operador que ajuda a criar a condição da sua instrução &quot;IF&quot;. Por exemplo, &quot;é igual a&quot; ou &quot;é maior que&quot; são operadores de condição. Para obter uma lista de operadores de condição que você pode usar em instruções, consulte [Operadores de condição em expressões personalizadas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True**&#x200B;**Expression** = Esta é a variável &quot;True&quot;, que informa à equação qual indicador será exibido quando os critérios da condição forem atendidos (indicadores true).

* **Expressão Falsa** = Essa é a variável &quot;False&quot;, que informa à equação qual indicador exibir quando os critérios da condição não forem atendidos (indicadores falsos).

No exemplo a seguir, o formato da instrução original é usado para escrever uma expressão de dados simples para uma instrução &quot;IF&quot;. A expressão compara dois campos de data diferentes no Workfront seguidos por um resultado Verdadeiro/Falso como uma string de dados:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

Na linguagem cotidiana, essa declaração significaria: Se a Data de conclusão projetada do meu objeto for &quot;Maior que&quot; a Data de conclusão planejada do mesmo objeto, exibir as palavras &quot;Fora do rastreamento&quot; neste campo. Caso contrário, exiba as palavras &quot;On Track&quot;.

## Criar campos calculados em formulários personalizados ou colunas personalizadas usando instruções &quot;IF&quot;

Você pode criar declarações &quot;IF&quot; em um campo calculado em um formulário personalizado ou em uma coluna personalizada.

Há uma diferença na sintaxe usada em um formulário personalizado calculado em comparação a uma coluna personalizada calculada. Consulte os seguintes exemplos:

* [Instruções &quot;IF&quot; simples](#single-if-statements)
* [Várias instruções &quot;IF&quot;](#multiple-if-statements)

### Instruções &quot;IF&quot; únicas {#single-if-statements}

Veja a seguir exemplos de um campo personalizado calculado e sua coluna correspondente usando uma instrução &quot;IF&quot;:

* Campo personalizado calculado:

Ao criar um campo personalizado, use a seguinte sintaxe para uma instrução &quot;IF&quot;:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Coluna personalizada calculada:

Ao criar uma coluna personalizada, você deve usar a seguinte sintaxe para a instrução &quot;IF&quot; na linha de expressão de valor:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Várias instruções &quot;IF&quot; {#multiple-if-statements}

Você pode reunir várias instruções &quot;IF&quot; com a seguinte instrução para criar uma expressão mais complexa e dinâmica:

<pre>IF(Condição1,Expressão Verdadeira,IF(Condição2,Expressão Verdadeira,Expressão Falsa))</pre>Observe que agora não há nenhuma declaração falsa para o primeiro "IF". Em vez disso, o substituímos pelo início de um segundo "IF".

Veja a seguir exemplos de um campo personalizado calculado e sua coluna personalizada correspondente usando várias instruções &quot;IF&quot;:

* Campo personalizado calculado:

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* Coluna personalizada calculada:

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

Neste exemplo, a mesma coisa foi realizada, reunindo duas variáveis de critério diferentes.\
Você pode explorar ainda mais essas opções recriando esses exemplos em seu próprio ambiente.

A melhor maneira de aprender isso é experimentando com vários campos e cenários. Além disso, familiarize-se com o API Explorer, que revela os nomes de campo que podem ser usados. Para obter informações sobre o API Explorer, consulte [API Explorer](../../../wf-api/general/api-explorer.md).

Para obter mais informações sobre a sintaxe Workfront de expressões de dados calculados, consulte [Visão geral de expressões de dados calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
