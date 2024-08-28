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
source-git-commit: 84f7f80314e4acafb0414b806f7b1e1e4b2845fc
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Exemplos de consulta da Workfront Data Connect

Para ajudá-lo a utilizar melhor os dados do Workfront Data Connect, esta página contém exemplos básicos de consultas que você pode usar para se familiarizar com a sintaxe e a estrutura de tipos específicos de consultas.

## Consulta de dados personalizada

Este exemplo demonstra como você pode compor uma consulta para retornar seus dados personalizados no Workfront, como formulários personalizados e campos personalizados.

### Cenário:

Sua organização que utiliza um formulário personalizado chamado Integração de finanças. O formulário é anexado a cada projeto e contém os seguintes campos:

* **Unidade de Negócios** - Um campo personalizado que contém uma cadeia de caracteres.
* **IDdoProjeto** - Um campo personalizado que contém uma cadeia de caracteres numérica.
* **Nome do Projeto Expandido** - Um campo de dados personalizado calculado que concatena os valores de Unidade de Negócios, ProjectID e o nome do projeto nativo do Workfront em uma única cadeia de caracteres.

Você precisa incluir essas informações na resposta para uma consulta no Data Connect. Os valores de dados personalizados para um registro no data lake estão contidos em uma coluna intitulada `parameterValues`. Essa coluna é armazenada como um objeto JSON.

### Consulta:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit" :: int as BusinessUnit,
    parametervalues:"DE:Project ID" :: int as ProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Resposta

A consulta acima retorna os seguintes dados:

* `projectid` - a ID de projeto nativa do Workfront
* `parametervalues` - uma coluna armazenando um objeto JSON
* `name` - o nome do projeto nativo do Workfront
* `Business Unit` - um valor de dados personalizado incluído no objeto `parametervalues`
* `Project ID` - um valor de dados personalizado incluído no objeto `parametervalues`
* `Expanded Project Name` - um valor de dados personalizado incluído no objeto `parametervalues`

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
