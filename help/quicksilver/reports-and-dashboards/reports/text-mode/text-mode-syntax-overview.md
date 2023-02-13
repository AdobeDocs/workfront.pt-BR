---
product-area: reporting
navigation-topic: text-mode-reporting
title: Visão geral da sintaxe do modo de texto
description: Você pode usar a interface do modo de texto para criar exibições, filtros, agrupamentos e prompts personalizados mais complexos em listas e relatórios. Ao usar o modo de texto, é possível acessar os campos e seus atributos que não estão disponíveis na interface do modo padrão.
author: Nolan
feature: Reports and Dashboards
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1498'
ht-degree: 0%

---

# Visão geral da sintaxe do modo de texto

Você pode usar a interface do modo de texto para criar exibições, filtros, agrupamentos e prompts personalizados mais complexos em listas e relatórios. Ao usar o modo de texto, é possível acessar os campos e seus atributos que não estão disponíveis na interface do modo padrão.

Para obter informações e considerações sobre o modo de texto antes de começar, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obter uma lista completa de todos os campos relatáveis e seus atributos, consulte [API Explorer](../../../wf-api/general/api-explorer.md).

## Considerações sobre a sintaxe do modo de texto

* Você deve entender a sintaxe do Adobe Workfront antes de começar a criar elementos de relatório no modo de texto. A sintaxe do Workfront para o modo de texto é exclusiva deste aplicativo e tem características exclusivas que você deve conhecer.
* Antes de começar a usar o modo de texto em seus relatórios, recomendamos que você utilize nossas classes em relatórios avançados para obter uma compreensão mais profunda de nosso idioma do modo de texto. Para obter materiais de treinamento em relatórios, consulte [Caminhos de aprendizagem de relatórios e painéis do Workfront](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).
* Você pode personalizar exibições, filtros e agrupamentos usando a interface de modo padrão. No entanto, você pode criar Prompts personalizados somente usando o modo de texto.

## Orientações comuns para a criação de elementos de relatório no modo de texto

A seguir estão as diretrizes comuns ao criar qualquer elemento de relatório ou lista no modo de texto:

* Sempre use camel case ao fazer referência a objetos ou atributos no banco de dados do Workfront.
* Lembre-se da hierarquia de objetos no Workfront. As seguintes diferenças existem entre exibições, filtros e agrupamentos:

   * É possível exibir um objeto distante três objetos do relatório ou de lista em uma visualização.
   * Não é possível fazer referência a objetos que estão a mais de 2 objetos do objeto principal em um agrupamento, filtro ou prompt personalizado.

   **Exemplo:** Você pode exibir o nome ou o GUID do Proprietário do Portfolio em uma visualização de tarefa:

   ```
   valuefield=project:portfolio:ownerID
   ```

   Não é possível agrupar, filtrar ou solicitar o Proprietário do Portfolio em uma exibição de tarefa:

   ```
   project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa
   ```

   Nesses exemplos, a ID do proprietário do Portfolio está a três objetos da lista.

   Para obter informações sobre a hierarquia de objetos no Workfront, consulte:

   * [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API Explorer](../../../wf-api/general/api-explorer.md)


* Use curingas sempre que possível para tornar seus relatórios e listas mais dinâmicos e evitar a duplicação para usuários diferentes e linhas do tempo semelhantes.

## Visão geral do caso de Camel

Ao referenciar campos Workfront ou seus atributos no modo de texto, o Workfront exige que você digite seus nomes em camel case. Nesse caso, os campos de nome único são digitados em minúsculas. Campos compostos são escritos de acordo com o seguinte padrão:

```
camelCaseSyntax
```

>[!IMPORTANT]
>
>Todos os elementos do relatório seguem esse padrão de capitalização.

As características do caso de camelo são:

* A primeira palavra sempre começa com uma letra minúscula.
* As palavras a seguir sempre começam com uma letra maiúscula.
* Não há espaços entre as palavras.

**Exemplo:** Para fazer referência à Data de conclusão real de um projeto, o nome do campo que você usaria ao criar elementos de relatório do modo de texto é

```
actualCompletionDate
```

.

## Sintaxe do modo de texto para vários elementos de relatório

As seguintes semelhanças existem entre a sintaxe dos conjuntos de elementos de relatório abaixo, ao criá-los usando o modo de texto:

* As linhas de código e sintaxe são semelhantes para exibições e agrupamentos.

   Para obter informações sobre as linhas principais de códigos para exibições e agrupamentos ao criá-los no modo de texto, consulte:

   * [Editar uma exibição usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Editar modo de texto em um agrupamento](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* As linhas de código e sintaxe são semelhantes para filtros e prompts personalizados.

   Para obter mais informações, consulte:

   * [Editar um filtro usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Sintaxe para exibições e agrupamentos

Observe que as linhas de código ao criar exibições e agrupamentos são semelhantes.

Para obter informações sobre como criar exibições e agrupamentos, consulte os seguintes artigos:

* [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

A linha de código mais importante para uma exibição ou agrupamento é a linha que identifica o objeto referenciado na coluna da exibição ou no agrupamento. Se esse campo for uma referência direta a um campo de banco de dados do Workfront ou um cálculo entre vários campos, a linha de código poderá começar com

```
valuefield
```

ou

```
valueexpression
```

.

* [Visão geral da sintaxe do campo de valor para exibições e agrupamentos](#valuefield-syntax-overview-for-views-and-groupings)
* [Visão geral da sintaxe de expressão de valor para exibições e agrupamentos](#valueexpression-syntax-overview-for-views-and-groupings)

>[!TIP]
>
>* Embora as linhas de código nos exemplos abaixo sejam semelhantes entre exibições e agrupamentos, sempre lembre-se de que cada linha de código para um agrupamento começa com o número de agrupamento.
>
>  Para agrupar por Nome de Projeto em uma lista de projeto ou relatório, use a seguinte linha para o agrupamento de primeira camada:
>
>  
```>
>  group.0.valuefield=name
>  ```>
>* If you edit multiple columns in a view in the same column (as it is the case of shared columns), remember that every line of code for each column starts with the column number. 
>
>  
Use the following format to identify the first column of a view: 
>
>  
```>
>  column.0.valuefield=name
>  ```>
>  For information about sharing columns, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md). 
>



```
Valuefield
```

visão geral da sintaxe para exibições e agrupamentos {#valuefield-syntax-overview-for-views-and-groupings}

```
Valuefield=
```

é uma linha chave do código em exibições e agrupamentos que identifica o objeto que você está referenciando diretamente.

A sintaxe para campos de referência direta é idêntica para agrupamentos e visualizações.

As seguintes regras se aplicam ao fazer referência a objetos Workfront usando um

```
valuefield
```

linha:

* Use camel case para fazer referência direta aos campos.

   **Exemplo:** Para fazer referência à Data de Conclusão Real da Tarefa em uma exibição de tarefa, use a seguinte linha:

   ```
   valuefield=actualCompletionDate
   ```

* Use camel case e dois pontos para separar campos relacionados para o mesmo objeto.

   **Exemplo:** Para fazer referência à Data de Conclusão Planejada do Projeto em uma exibição de tarefa, use a seguinte linha:

   ```
   valuefield=project:plannedCompletionDate
   ```

   Para obter informações sobre como os objetos estão fazendo referência uns aos outros no banco de dados do Workfront, consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

* Ao fazer referência a um campo personalizado, use o nome do campo exatamente como ele aparece na interface.

   **Exemplo:** Para fazer referência a um campo personalizado do projeto chamado Detalhes adicionais em uma exibição de tarefa, use a seguinte linha:

   ```
   valuefield=project:Additional Details
   ```

 

```
Valueexpression
```

visão geral da sintaxe para exibições e agrupamentos {#valueexpression-syntax-overview-for-views-and-groupings}

Você pode substituir a variável

```
valuefield=
```

linha de código com

```
valueexpression=
```

ao criar exibições e agrupamentos no modo de texto, quando quiser fazer referência a um cálculo entre 2 ou mais campos.

>[!TIP]
>
>Embora seja possível criar campos calculados que podem ser exibidos em relatórios, exibições calculadas e agrupamentos são mais dinâmicos. As exibições e agrupamentos calculados são atualizados com novas informações sempre que você executa o relatório ou exibe uma lista.
>
>Para obter informações sobre como criar colunas calculadas em uma exibição, consulte [Campos personalizados calculados vs. colunas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Criar um agrupamento calculado é semelhante a criar uma coluna calculada em uma visualização.

As seguintes regras se aplicam ao fazer referência a objetos Workfront usando um

```
valueexpression
```

linha:

* Use camel case para fazer referência aos campos diretamente e coloque cada campo entre colchetes.

   **Exemplo:** Para exibir o campo Nome da tarefa em uma coluna de tarefa usando

   ```
   valueexpression
   ```

   , use a seguinte linha:

   ```
   valueexpression={name}
   ```

* Use camel case e pontos para separar campos relacionados entre si.

   **Exemplo:** Para exibir o nome de um projeto concatenado com o nome da tarefa em um relatório de tarefa, use as seguintes linhas:

   * Em uma exibição:

      ```
      valueexpression=CONCAT({project}.{name},' - ',{name})
      ```

   * Em um agrupamento:

      ```
      group.0.valueexpression=CONCAT({project}.{name},' - ',{name})
      ```
   Para obter informações sobre como os objetos estão fazendo referência uns aos outros no banco de dados do Workfront, consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

* Ao fazer referência a um campo personalizado, use as seguintes regras:

   * Use o nome do campo exatamente como ele aparece na interface.
   * Preceda o nome do campo com &quot;DE:&quot;.
   * Insira o campo entre chaves.
   * Separe os campos relacionados ao objeto por períodos.

   **Exemplo:** Para exibir o campo personalizado do projeto Detalhes Adicionais em uma exibição de tarefa em uma linha de expressão de valor, use a seguinte linha:

   ```
   valueexpression={project}.{DE:Additional Details}
   ```

* Você pode usar um curinga em um

   ```
   valueexpression
   ```

   mas não em um

   ```
   valuefield
   ```

   linha.

   Para obter informações sobre curingas, consulte [Variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

```
Valueformat
```

visão geral

A segunda linha de código mais importante em uma visualização ou agrupamento é a variável

```
valueformat=
```

linha. Isso informa ao Workfront em qual formato retornar o valor especificado na variável

```
valuefield
```

ou de expressão de valor. Embora você possa usar vários formatos para a variável

```
valueformat
```

, recomendamos que você sempre use o seguinte valor ao usar

```
valueexpression
```

:

```
valueformat=HTML
```

### Sintaxe para filtros e prompts personalizados

A sintaxe para criação de filtros é semelhante àquela para criação de prompts personalizados.

>[!TIP]
>
>Você pode criar um prompt personalizado criando primeiro um filtro para a instrução que deseja incluir no prompt. Conecte todas as linhas de código em um filtro usando &quot;&amp;&quot; sem espaços entre as linhas e que se tornam seu prompt personalizado.

Para obter informações sobre como criar filtros e prompts personalizados, consulte:

* [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Para obter informações sobre como criar filtros no modo de texto, consulte [Editar um filtro usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

Você pode usar os seguintes elementos para criar filtros e prompts personalizados no modo de texto:

* Uma linha de código que faz referência ao objeto da instrução de filtro. Use camel case para o objeto de filtro.
* Uma linha de código que faz referência ao objeto de filtro e ao modificador do valor do objeto de filtro. Use camel case para o objeto de filtro nesta linha.

   >[!TIP]
   >
   >Ao fazer referência a intervalos, isso requer 2 linhas modificadoras.

* Um conector de instrução que conecta várias instruções de filtro:

   * AND

      Esse é o conector padrão entre instruções de filtro.

   * OU

      >[!TIP]
      >
      >Os conectores de declaração fazem distinção entre maiúsculas e minúsculas e sempre maiúsculas. &quot;AND&quot; pode ser omitido no modo de texto.

* Curingas para tornar os filtros mais dinâmicos e personalizá-los pelo tempo atual ou pelo usuário que está conectado. Para obter informações sobre curingas, consulte [Variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
