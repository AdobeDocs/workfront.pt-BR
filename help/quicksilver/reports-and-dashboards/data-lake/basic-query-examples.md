---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Exemplos de consulta de Data Connect
description: Exemplos de consultas que você pode usar para se familiarizar com a sintaxe e a estrutura de tipos específicos de consultas.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 364b668f23f5437e5cca0c4cc4793b17d444fb56
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Exemplos de consulta da Workfront Data Connect

Para ajudá-lo a utilizar melhor os dados do Workfront Data Connect, esta página contém exemplos básicos de consultas que você pode usar para se familiarizar com a sintaxe e a estrutura de tipos específicos de consultas.

## Consulta de dados personalizada

Este exemplo demonstra como você pode compor uma consulta para retornar seus dados personalizados no Workfront, como formulários personalizados e campos personalizados.

### Cenário:

Sua organização utiliza um formulário personalizado chamado Integração de finanças. O formulário é anexado a cada projeto e contém os seguintes campos:

* **Unidade de Negócios** - Um campo personalizado que contém uma cadeia de caracteres.
* **IDdoProjeto** - Um campo personalizado que contém uma cadeia de caracteres numérica.
* **Nome do Projeto Expandido** - Um campo de dados personalizado calculado que concatena os valores de Unidade de Negócios, ProjectID e o nome do projeto nativo do Workfront em uma única cadeia de caracteres.

Você precisa incluir essas informações na resposta para uma consulta no Data Connect. Os valores de dados personalizados para um registro no data lake estão contidos em uma coluna intitulada `parametervalues`. Essa coluna é armazenada como um objeto JSON.

### Consulta:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Resposta:

A consulta acima retorna os seguintes dados:

* `projectid` - a ID de projeto nativa do Workfront
* `parametervalues` - uma coluna armazenando um objeto JSON
* `name` - o nome do projeto nativo do Workfront
* `Business Unit` - um valor de dados personalizado incluído no objeto `parametervalues`
* `Project ID` - um valor de dados personalizado incluído no objeto `parametervalues`
* `Expanded Project Name` - um valor de dados personalizado incluído no objeto `parametervalues`

### Explicação:

Ao consultar o objeto JSON `parametervalues`, cada campo de dados personalizado pode ser acessado como uma coluna usando o seguinte:

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` é o nome do objeto JSON na tabela que está sendo consultada. No caso de dados personalizados, sempre será `parametervalues`.
* `<parameter_name>` é a cadeia de caracteres `parametername` encontrada na ferramenta de configuração de formulário, embora nem sempre corresponda a esse valor.

>[!NOTE]
>
>Se o nome do parâmetro for alterado na ferramenta de configuração de formulário do Workfront, ele será representado como uma nova coluna no objeto JSON. Dessa forma, recomendamos não alterar o nome de uma coluna depois de criá-la na ferramenta de configuração de formulário. No entanto, o rótulo pode ser alterado sem afetar o objeto JSON.
>
>Se a string de texto para o nome do parâmetro estiver incorreta, a coluna retornará um valor NULL, em vez de um erro.

* `<data_type>` converte o valor sendo retornado do objeto JSON em um tipo de dados apropriado para o campo. Escolher um tipo de dados incompatível para o valor que está sendo retornado resultará em um erro de incompatibilidade de tipo de dados. Os possíveis tipos de dados incluem:

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (por exemplo, `Number(32,4)` retornaria 1234.0987)
   * `date`
   * `timestamp`

* `<column_name>` é o rótulo que você cria para cada coluna de dados personalizada.

>[!NOTE]
>
>Somente os parâmetros com valores atribuídos a eles no formulário serão incluídos no objeto JSON. Se um campo de dados personalizado estiver vazio no formulário, ele não será exibido.

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
