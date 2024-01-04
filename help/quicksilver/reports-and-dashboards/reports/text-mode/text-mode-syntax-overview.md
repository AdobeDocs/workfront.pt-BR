---
product-area: reporting
navigation-topic: text-mode-reporting
title: Visão geral da sintaxe do modo de texto
description: Você pode usar a interface do modo de texto para criar exibições, filtros, agrupamentos e prompts mais complexos em listas e relatórios. Ao usar o modo de texto, você pode acessar campos e seus atributos que não estão disponíveis na interface do modo padrão.
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1862'
ht-degree: 0%

---

# Visão geral da sintaxe do modo de texto

<!--Audited: 12/2023-->

Você pode usar a interface do modo de texto para criar exibições, filtros, agrupamentos e prompts mais complexos em listas e relatórios. Ao usar o modo de texto, você pode acessar campos e seus atributos que não estão disponíveis na interface do modo padrão.

Para obter informações e considerações sobre o modo de texto antes de começar, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obter uma lista completa de todos os campos reportáveis e seus atributos, consulte [API Explorer](../../../wf-api/general/api-explorer.md).

Para obter mais informações sobre como criar relatórios usando o modo de texto, incluindo classes, vídeos e tutoriais, visite a seção Saiba mais no site do Adobe Experience League.

## Considerações sobre a sintaxe do modo de texto

* Você deve entender a sintaxe do Adobe Workfront antes de começar a criar elementos de relatórios no modo de texto. A sintaxe do Workfront para o modo de texto é exclusiva desse aplicativo e tem características exclusivas que você deve conhecer.
* Antes de começar a usar o modo de texto em seus relatórios, recomendamos que você faça nossas aulas sobre relatórios avançados para obter uma compreensão mais profunda da linguagem do modo de texto. <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* É possível personalizar exibições, filtros e agrupamentos usando a interface do modo padrão. No entanto, é possível criar Solicitações personalizadas apenas usando o modo de texto.

## Diretrizes comuns para a criação de elementos de relatórios no modo de texto

As diretrizes a seguir são comuns ao criar qualquer elemento de relatório ou lista no modo de texto:

* Sempre use camel case ao referenciar objetos ou atributos no banco de dados do Workfront.
* Lembre-se da hierarquia de objetos no Workfront. As seguintes diferenças existem entre exibições, filtros e agrupamentos:

   * Você pode exibir um objeto que esteja a três objetos de distância do relatório ou da lista em uma visualização.
   * Você não pode fazer referência a objetos que estejam a mais de 2 objetos de distância do objeto principal em um prompt de agrupamento, filtro ou personalizado.

  **Exemplo:** Você pode exibir o nome ou o GUID do Proprietário do Portfolio em uma exibição de tarefa:


  `valuefield=project:portfolio:ownerID`

  Não é possível agrupar, filtrar ou solicitar o Proprietário do Portfolio em uma exibição de tarefa:

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`


  Nesses exemplos, a ID do proprietário do Portfolio está a três objetos de distância do objeto da lista.

  Para obter informações sobre a hierarquia de objetos no Workfront, consulte:

   * [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API Explorer](../../../wf-api/general/api-explorer.md)

* Use curingas sempre que possível para tornar seus relatórios e listas mais dinâmicos e evitar a duplicação deles para usuários diferentes e linhas do tempo semelhantes.

## Visão geral do Camel case

Ao referenciar campos do Workfront ou seus atributos no modo de texto, o Workfront exige que você digite seus nomes em caixa de camelo. Nesse caso, os campos de nome único são escritos em minúsculas. Os campos compostos são escritos de acordo com o seguinte padrão:

`camelCaseSyntax`

>[!IMPORTANT]
>
>Todos os elementos de relatórios seguem esse padrão de maiúsculas e minúsculas.

As características da caixa de camelo são:

* A primeira palavra sempre começa com uma letra minúscula.
* As palavras a seguir sempre começam com uma letra maiúscula.
* Não há espaços entre as palavras.

**Exemplo:** Para fazer referência à Data de conclusão real de um projeto, o nome do campo que você usaria ao criar elementos de relatório no modo de texto é

`actualCompletionDate`

## Sintaxe do modo de texto para vários elementos de relatórios

Existem as seguintes semelhanças entre a sintaxe dos conjuntos de elementos de relatório abaixo, ao criá-los usando o modo de texto:

* As linhas de código e sintaxe são semelhantes para exibições e agrupamentos.

  Para obter informações sobre as linhas principais dos códigos para exibições e agrupamentos ao criá-los no modo de texto, consulte:

   * [Editar uma visualização usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Modo de edição de texto em um agrupamento](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* As linhas de código e sintaxe são semelhantes para filtros e prompts personalizados.

  Para obter mais informações, consulte:

   * [Editar um filtro usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Sintaxe para exibições e agrupamentos

As linhas de código ao criar exibições e agrupamentos são semelhantes.

Para obter informações sobre como criar exibições e agrupamentos, consulte os seguintes artigos:

* [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Visão geral de agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

A linha de código mais importante para uma exibição ou um agrupamento é a linha que identifica o objeto referenciado na coluna da exibição ou no agrupamento. Esta linha de código pode começar com `valuefield` ou `valueexpression` se esse campo for uma referência direta a um campo de banco de dados do Workfront ou um cálculo entre vários campos.

A tabela a seguir lista as linhas de códigos mais comuns em uma exibição ou agrupamento:

| Linha de código | Descrição |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | Identifica o objeto referenciado na coluna da exibição ou no agrupamento. Esta é uma referência direta ao objeto referenciado. |
| `valueexpression` | Identifica o objeto referenciado na coluna da exibição ou no agrupamento. Este é um cálculo entre vários campos. |
| `valueformat` | Identifica o formato em que o Workfront retorna o valor especificado nas linhas de expressão valuefield ou valuefield. |
| `width` | Identifica a largura de uma coluna em pixels. |
| `stretch` | Identifica quais colunas ocupam espaço extra não necessário para a exibição. |

>[!TIP]
>
>* Embora as linhas de código nos exemplos abaixo sejam semelhantes entre exibições e agrupamentos, sempre lembre-se de que cada linha de código de um agrupamento começa com o número do agrupamento.
>
>  Para agrupar por Nome do Projeto em uma lista de projeto ou relatório, use a seguinte linha para o agrupamento de primeira camada:
>
>  `group.0.valuefield=name`
>  
>* Se você editar várias colunas em uma visualização na mesma coluna (como no caso de colunas compartilhadas), lembre-se de que cada linha de código para cada coluna começa com o número da coluna.
>
>  Use o formato a seguir para identificar a primeira coluna de uma view:
>
>  `column.0.valuefield=name`
>  
>  Para obter informações sobre como compartilhar colunas, consulte [Exibição: mesclar informações de várias colunas em uma coluna compartilhada](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### `Valuefield` visão geral de sintaxe para exibições e agrupamentos

`Valuefield=` é uma linha principal de código em exibições e agrupamentos que identifica o objeto que você está referenciando diretamente.

A sintaxe para campos de referência direta é idêntica para agrupamentos e visualizações.

As seguintes regras se aplicam ao referenciar objetos do Workfront usando um `valuefield` linha:

* Use camel case para fazer referência a campos diretamente.

  **Exemplo:** Para fazer referência à Data de Término Efetivo da Tarefa em uma exibição de tarefa, use a seguinte linha:

  `valuefield=actualCompletionDate`

* Use camel case e dois pontos para separar campos relacionados um ao outro para o mesmo objeto.

  **Exemplo:** Para fazer referência à Data de Conclusão Planejada do Projeto em uma exibição de tarefa, use a seguinte linha:

  `valuefield=project:plannedCompletionDate`

  Para obter informações sobre como os objetos estão se referenciando no banco de dados do Workfront, consulte [API Explorer](../../../wf-api/general/api-explorer.md).

* Ao fazer referência a um campo personalizado, use o nome do campo exatamente como ele aparece na interface.

  **Exemplo:** Para fazer referência a um campo personalizado do projeto rotulado como Detalhes Adicionais em uma exibição de tarefa, use a seguinte linha:

  `valuefield=project:Additional Details`

#### `Valueexpression` visão geral de sintaxe para exibições e agrupamentos

Você pode substituir o `valuefield=` linha de código com `valueexpression=` ao criar exibições e agrupamentos no modo texto quando quiser fazer referência a um cálculo entre 2 ou mais campos.

>[!TIP]
>
>Embora seja possível criar campos calculados que podem ser exibidos em relatórios, as exibições calculadas e os agrupamentos são mais dinâmicos. As exibições e os agrupamentos calculados são atualizados com novas informações sempre que você executa o relatório ou exibe uma lista.
>
>Para obter informações sobre como criar colunas calculadas em uma exibição, consulte [Campos personalizados calculados versus colunas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Criar um agrupamento calculado é semelhante a criar uma coluna calculada em uma exibição.

As seguintes regras se aplicam ao referenciar objetos do Workfront usando um `valueexpression` linha:

* Use camel case para fazer referência a campos diretamente e colocar cada campo entre chaves.

  **Exemplo:** Para exibir o campo Nome da Tarefa em uma coluna de tarefa usando `valueexpression`, use a seguinte linha:

  `valueexpression={name}`


* Use camel case e pontos para separar campos relacionados uns aos outros.

  **Exemplo:** Para exibir o nome de um projeto concatenado com o nome da tarefa em um relatório de tarefas, use as seguintes linhas:

   * Em uma exibição:

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * Em um agrupamento:

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  Para obter informações sobre como os objetos estão se referenciando no banco de dados do Workfront, consulte [API Explorer](../../../wf-api/general/api-explorer.md).

* Ao fazer referência a um campo personalizado, use as seguintes regras:

   * Use o nome do campo exatamente como ele aparece na interface.
   * Coloque &quot;DE:&quot; antes do nome do campo.
   * Coloque o campo entre chaves.
   * Separe os campos relacionados ao objeto por pontos.

  **Exemplo:** Para exibir o campo personalizado do projeto Detalhes Adicionais em uma exibição de tarefa em uma linha de expressão de valor, use a seguinte linha:

  `valueexpression={project}.{DE:Additional Details}`

* É possível usar um curinga em uma `valueexpression` mas não em um `valuefield` linha.

  Para obter informações sobre curingas, consulte [Visão geral das variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` visão geral para exibições e agrupamentos

A segunda linha de código mais importante em uma visualização ou agrupamento é o `valueformat=` linha. Isso informa ao Workfront em que formato retornar o valor especificado na variável `valuefield` ou `valueexpression` linhas. Embora você possa usar vários formatos para a variável `valueformat` recomendamos que você sempre use o seguinte valor ao usar `valueexpression`:

`valueformat=HTML`

Para obter `valueformat` valores, consulte também os seguintes artigos:

* [Formatar datas em relatórios do modo texto](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [Formatar números, valores de moeda e porcentagem em relatórios de modo de texto](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` visão geral para exibições

`width=` é a linha de código em que você pode especificar a largura de cada coluna em pixels. O Workfront fornece uma largura sugerida para cada campo, embora dependendo do tipo de campo e do formato, talvez você queira fazer ajustes.

Você deve usar o adicional `usewidths=true` linha de código para aplicar a largura especificada para a coluna.

**Exemplo:** Para exibir uma coluna com largura de 80 pixels, use as seguintes linhas:

`width=80`

`usewidths=true`

#### `stretch` visão geral para exibições

A variável `stretch` é usado para identificar quais colunas ocupam espaço extra não necessário para a exibição. A largura da interface do usuário do espaço de trabalho para um usuário típico é de cerca de 850 pixels. Isso significa que se você tiver uma exibição com quatro colunas (150 pixels cada), sua exibição ocupará 600 de 850 pixels. Há 250 pixels extras na interface do usuário que serão adicionados às colunas com uma porcentagem de ampliação fornecida.

O alongamento de uma coluna é aplicado ao usar a linha de código adicional: `usewidths=true` para pelo menos uma das colunas na exibição.

**Exemplo:** Para indicar que uma coluna poderia usar 70% do espaço vazio em uma exibição, use as seguintes linhas:

`stretch=70`

`usewidths=true`

### Sintaxe para filtros e prompts personalizados

A sintaxe para a criação de filtros é semelhante àquela para a criação de prompts personalizados.

>[!TIP]
>
>Você pode criar um prompt personalizado criando primeiro um filtro para a instrução que deseja incluir no prompt. Conecte todas as linhas de código em um filtro usando &quot;&amp;&quot;, sem espaços entre as linhas, e esse se tornará seu prompt personalizado.

Para obter informações sobre a criação de filtros e prompts personalizados, consulte:

* [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Para obter informações sobre como criar filtros no modo de texto, consulte [Editar um filtro usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

Você pode usar os seguintes elementos para criar filtros e prompts personalizados no modo de texto:

* Uma linha de código que faz referência ao objeto da instrução de filtro. Use camel case para o objeto de filtro.
* Uma linha de código que faz referência ao objeto de filtro e ao modificador para o valor do objeto de filtro. Use camel case para o objeto de filtro nesta linha.

  >[!TIP]
  >
  >Ao fazer referência a intervalos, isso requer duas linhas do modificador.

* Um conector de instrução que conecta várias instruções de filtro:

   * E

     Este é o conector padrão entre as instruções de filtro.

   * OU

     >[!TIP]
     >
     >Os conectores de instrução fazem distinção entre maiúsculas e minúsculas. &quot;AND&quot; pode ser omitido no modo de texto.

* Curingas para tornar os filtros mais dinâmicos e personalizá-los para o horário atual ou para o usuário que está conectado. Para obter informações sobre curingas, consulte [Visão geral das variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
