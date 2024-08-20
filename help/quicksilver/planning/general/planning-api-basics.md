---
title: Noções básicas sobre a API do Adobe Workfront Planning
description: O objetivo da API de planejamento do Adobe Workfront é simplificar a criação de integrações com o Planning, introduzindo uma arquitetura REST-ful que opera via HTTP. Este documento supõe que você esteja familiarizado com as respostas REST e JSON e descreve a abordagem adotada pela API de Planejamento.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: 83ea00f63f597731f808673d45b6103522995fb1
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 2%

---

# Noções básicas sobre a API do Adobe Workfront Planning

O objetivo da API de planejamento do Adobe Workfront é simplificar a criação de integrações com o Planning, introduzindo uma arquitetura REST-ful que opera via HTTP. Este documento supõe que você esteja familiarizado com as respostas REST e JSON e descreve a abordagem adotada pela API de Planejamento.

Uma familiaridade com o esquema do Workfront Planning o ajudará a entender os relacionamentos de banco de dados que podem ser utilizados para extrair dados do Workfront Planning para fins de integração.

## URL da API do Workfront Planning

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### Operações

Os objetos são manipulados enviando uma solicitação HTTP para seu URI exclusivo. A operação a ser executada é especificada pelo método HTTP.

Os métodos HTTP padrão correspondem às seguintes operações:

* **GET** - Recupera um objeto por ID, pesquisa todos os objetos por uma consulta
* **POST** - Insere um novo objeto
* **PUT** - Edita um objeto existente
* **DELETE** - Exclui um objeto

Para obter mais detalhes e exemplos de cada operação, consulte a [documentação do desenvolvedor da API do Workfront Planning](https://developer.adobe.com/wf-planning/).

### Tipos de campo e modificadores de pesquisa usados com eles

Você pode usar modificadores e filtros com campos para controlar quais dados serão retornados nos resultados.

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### Uso de modificadores de pesquisa

O Workfront Planning suporta os seguintes modificadores de pesquisa:

<table>
    <tr>
        <td><b>Modificador</b></td>
        <td><b>Exemplo</b></td>
        <td><b>Descrição</b></td>
        <td><b>Valores possíveis</b></td>
    </tr>
    <tr>
        <td>$contém </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Retorna registros cujo valor de campo contém o filtro  </td>
        <td>"Lançamento de novo produto"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Retorna registros em que o valor do campo não contém o filtro  </td>
        <td>"Novo lançamento"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Retorna registros cujo valor de campo corresponde exatamente ao filtro  </td>
        <td>"Lançamento de novo produto"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Retorna registros cujo valor de campo não corresponde exatamente ao filtro  </td>
        <td>"Lançamento de novo produto"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Retorna registros cujo valor de campo não está vazio  </td>
        <td><ul><li>“” </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Retorna registros cujo valor de campo não está vazio  </td>
        <td>"Lançamento de novo produto"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Retorna registros cujo valor de campo é maior que o filtro  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Retorna registros cujo valor de campo é maior ou igual ao filtro  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Retorna registros cujo valor de campo é menor que o filtro  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Retorna registros cujo valor de campo é inferior ou igual ao filtro </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Retorna registros cujo valor de campo está após o filtro  </td>
        <td>"05-2024-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Retorna registros cujo valor de campo é anterior ao filtro </td>
        <td>"05-2024-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Retorna registros cujo valor de campo está entre o filtro  </td>
        <td><ul><li>"05-2024-12T20:00:00.000Z" </li><li>"05-2024-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Retorna registros cujo valor de campo não está entre o filtro  </td>
        <td><ul><li>"05/2024/09T20:00:00.000Z"  </li><li>"05-2024-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Retorna registros cujo valor de campo é qualquer um dos filtros  </td>
        <td><ul><li>"ativo" </li><li>"concluído" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Retorna registros cujo valor de campo é none no filtro </td>
        <td><ul><li>"concluído"  </li><li>"fixo"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Retorna registros cujo valor de campo tem qualquer um dos filtros  </td>
        <td><ul><li>["ativo", "fixo"]  </li><li>["fixo", "concluído", "concluído"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Retorna registros cujo valor de campo tem todo o filtro  </td>
        <td><ul><li>["ativo", "concluído"]   </li><li>["ativo", "concluído", "concluído"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Retorna registros cujo valor de campo não tem nenhum do filtro </td>
        <td>["fixo", "concluído"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Retorna registros cujo valor de campo é exatamente o filtro  </td>
        <td>["ativo", "concluído"]  </td>
    </tr>
</table>

#### Tipos de campo

Abaixo está a lista de tipos de campo suportados e quais modificadores de pesquisa podem ser usados com cada um desses tipos de campo

| Tipo de campo | Modificadores de pesquisa suportados |
|---|---|
| texto | $contém, $nãoContém, $é, $nãoÉ, $estáVazio, $nãoVazio |
| long-text | $contém, $nãoContém, $é, $nãoÉ, $estáVazio, $nãoVazio |
| número | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| porcentagem | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| moeda | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| data | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| seleção única | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| seleção múltipla | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| booleano | $is |
| usuário | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| fórmula | $contém, $nãoContém, $é, $nãoÉ, $estáVazio, $nãoVazio |
| url | $contém, $nãoContém, $é, $nãoÉ, $estáVazio, $nãoVazio |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| atualizado por | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| atualizado-em | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| referência | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| pesquisa | Depende do campo vinculado |

### Uso de instruções &quot;And&quot; e &quot;Or&quot;

Na chamada da API, você pode ter filtros baseados em vários critérios combinados por instruções $and&quot; e &quot;$or&quot;

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### Uso do parâmetro de solicitação de campos

Você pode usar o parâmetro de solicitação de campos para especificar uma lista separada por vírgulas de campos específicos que devem ser retornados. Esses nomes de campos fazem distinção entre maiúsculas e minúsculas.

Por exemplo, a solicitação

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
....
```

retorna uma resposta semelhante à seguinte:


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Classificação dos resultados da consulta na API

Você pode classificar os resultados por qualquer campo se anexar o seguinte à chamada de API:


`/v1/records/search`

Corpo da solicitação:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Limites de consulta e respostas paginadas

Por padrão, as solicitações da API de Planejamento retornam 500 resultados, começando do início da lista. Para substituir a limitação padrão do número de resultados, você pode usar o parâmetro `limit` em suas solicitações e defini-lo como um número diferente, até 2000 resultados.

Recomendamos que você considere usar respostas paginadas para conjuntos de dados grandes adicionando o parâmetro `offset` às suas solicitações. As respostas paginadas permitem especificar o local do primeiro resultado que deve ser retornado.

Por exemplo, se quiser retornar os resultados 2001-4000, você poderá usar a solicitação a seguir. Este exemplo retorna 2000 registros que estão no status ativo, a partir do resultado 2001:

`POST /v1/records/search `



Corpo da solicitação:

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

Para garantir que seus resultados sejam paginados corretamente, use um parâmetro de classificação. Isso permite que os resultados sejam retornados na mesma ordem, para que a paginação não repita ou ignore os resultados.

Para obter mais informações sobre classificação, consulte [Classificar resultados da consulta na API](#sorting-query-results-in-the-api) neste artigo.
