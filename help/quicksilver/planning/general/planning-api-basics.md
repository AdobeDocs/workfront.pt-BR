---
title: Noções básicas sobre a API de planejamento do Adobe Workfront
description: O objetivo da API de planejamento do Adobe Workfront é simplificar a criação de integrações com o Planning, introduzindo uma arquitetura REST-ful que opera via HTTP. Este documento supõe que você esteja familiarizado com as respostas REST e JSON e descreve a abordagem adotada pela API de Planejamento.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: 083a2bbc49b4679f2c7b828f2726327ea24296b1
workflow-type: tm+mt
source-wordcount: '2206'
ht-degree: 3%

---


# Noções básicas da API do Planejamento do Adobe Workfront

{{planning-important-intro}}

<!--

Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 

-->

O objetivo da API de planejamento do Adobe Workfront é simplificar a criação de integrações com o Planning, introduzindo uma arquitetura RESTful que opera via HTTP. Este documento supõe que você esteja familiarizado com as respostas REST e JSON.

Para obter referência completa do ponto de extremidade, esquemas de solicitação/resposta e detalhes específicos da versão, consulte a [documentação do desenvolvedor da API do Workfront Planning](https://developer.adobe.com/wf-planning).

## Autenticação

A API do Workfront Planning usa o OAuth 2.0 para autenticação. As credenciais são configuradas por meio da Adobe Developer Console.

Dependendo do seu tipo de integração, oferecemos suporte aos dois fluxos a seguir:

* **Autenticação de servidor para servidor (JWT)**: para integrações automatizadas e serviços de back-end sem interação com o usuário. Usa a credencial do servidor para servidor OAuth (concessão de credenciais do cliente — seu aplicativo é autenticado diretamente usando a ID do cliente e o segredo para obter um token de acesso, sem logon do usuário ou etapa de consentimento).

  Para obter informações, consulte [Autenticação de Servidor para Servidor](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/).

* **Autenticação de usuário (Fluxo de código de autorização)**: para integrações que atuam em nome de um usuário específico. Usa a credencial do aplicativo web OAuth ou do aplicativo de página única (concessão de código de autorização — o usuário faz logon e consente, após o qual o aplicativo recebe um código de autorização que troca por um token de acesso).

  Para obter informações, consulte [Autenticação de Usuário](https://developer.adobe.com/developer-console/docs/guides/authentication/UserAuthentication/).

Para começar, crie um projeto no Adobe Developer Console e adicione a API do Workfront Planning para obter suas credenciais.

Para configurar credenciais, crie um aplicativo OAuth2 no Workfront.

Para obter informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

>[!NOTE]
>
>O ponto de extremidade `/login` e a autenticação de chave de API não são compatíveis com o Workfront Planning. Não use `sessionID` ou `apiKey` parâmetros.


## Controle de versão da API

A versão da API do Planning é feita por meio do caminho do URL.

Estas são as versões atuais compatíveis:

| Versão | Data de lançamento |
|-----------|----------------|
| Versão 1 | Julho de 2024 |
| Versão 2 | Maio de 2026 |

<!--

(*****************add deprecation date column above, when we have one*****************)

-->


Para obter mais informações sobre as versões atuais com suporte, consulte o artigo [documentação do desenvolvedor da API do Workfront Planning](https://developer.adobe.com/wf-planning).

Recomendamos o direcionamento explícito de uma versão em todas as integrações:

```
https://{customer-domain}/maestro/api/v2/...
```

Quando uma nova versão principal for lançada, a versão anterior continuará disponível até que uma data de desativação seja comunicada.

Siga as notas de versão do Workfront para se manter informado sobre alterações na API.


## Estrutura e operações de URL

Os objetos são manipulados enviando uma solicitação HTTP para seu URI exclusivo. A operação é especificada pelo método HTTP.

| Método | Operação |
|----------|----------------------------------------------------------------------|
| GET | Recuperar um único objeto por ID ou objetos de pesquisa/lista |
| POST | Criar um novo objeto |
| PUT | Substituir um objeto existente (atualização completa) |
| PATCH | Atualizar parcialmente um objeto existente (somente os campos fornecidos são modificados) |
| EXCLUIR | Excluir um objeto |

>[!NOTE]
>
>Observação de **Versão1:** `PATCH` não tem suporte na Versão 1. Use `PUT` para todas as atualizações.


Para obter caminhos completos de pontos de extremidade e exemplos de solicitação/resposta, consulte a **Referência da API** em [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning).

## Códigos de status HTTP

A API do Planning retorna códigos de status HTTP padrão:

| Código | Significado |
|------------------------|-------------------------------------------------|
| 200 OK | GET, PUT ou PATCH com êxito |
| 201 Criado | POST bem-sucedido (recurso criado) |
| 204 Sem conteúdo | DELETE bem-sucedido |
| Status múltiplo 207 | A operação em massa foi concluída com resultados mistos, em que alguns itens tiveram êxito e alguns falharam. Verifique as respostas de item individual para obter detalhes. |
| 400 Solicitação incorreta | Solicitação inválida — consulte a resposta do erro para obter detalhes |
| 401 Não autorizado | Token de autenticação ausente ou inválido |
| 403 Proibido | Permissões autenticadas, mas insuficientes |
| 404 Não encontrado | O recurso não existe |
| Conflito 409 | Conflito de gravação; o recurso foi modificado por outra solicitação. Tente novamente com a versão mais recente. |
| 429 Muitas solicitações | Limite de taxa excedido |

>[!NOTE]
>
>**Observação da versão 1:** a versão 1 retorna `200 OK` para todas as operações bem-sucedidas, incluindo POST e DELETE.


## Tratamento de erros

A API de Planejamento retorna erros em um formato consistente. Cada resposta de erro inclui uma mensagem legível por humanos, um código de erro legível por computador e uma ID de solicitação para escalonamento de suporte.

Exemplo de resposta de erro:

```
json
{
  "title": "Validation failed",
  "status": 400,
  "detail": "Request validation failed. See 'errors' for details.",
  "errorCode": "VALIDATION_FAILED",
  "requestId": "req-123",
  "errors": [
    { "field": "name", "message": "must not be blank" }
  ]
}
```

Use `errorCode` (não `status`) para direcionar tratamento de erros programáticos. Ela fornece a classificação mais específica da falha.

>[!NOTE]
>
>Observação sobre a **Versão 1:** as respostas de erro da versão 1 usam um campo numérico `type` (por exemplo, `40001`) em vez de uma cadeia de caracteres `errorCode`, e quebra automática de detalhes em um objeto `report` em vez de um campo `detail` de nível superior.

## Filtrar registros

Use o parâmetro `filter` em solicitações de pesquisa de registro para retornar somente registros que correspondam a critérios específicos. Para solicitações POST, `filter` é uma propriedade JSON no corpo da solicitação. Para solicitações GET, `filter` é um parâmetro de consulta que contém um grupo de filtros codificado em JSON. Os filtros usam uma estrutura composta digitada com operadores lógicos explícitos.

```
json
{
  "filter": {
    "operator": "AND",
    "conditions": [
      { "fieldId": "<fieldId>", "condition": "IS", "value": "Active" },
      { "fieldId": "<fieldId>", "condition": "CONTAINS", "value": "marketing" }
    ]
  }
}
```

Filtros podem ser aninhados usando operadores `AND` / `OR` para criar condições compostas:

```
json
{
  "filter": {
    "operator": "OR",
    "conditions": [
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-03-31T20:00:00.000Z", "2024-04-01T20:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "active" }
        ]
      },
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "IS_BETWEEN", "value": ["2024-04-15T00:00:00.000Z", "2024-04-16T00:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "planned" }
        ]
      }
    ]
  }
}
```

>[!NOTE]
>
>**Observação da versão 1:** a versão 1 usa operadores sem tipo de estilo Mongo em um objeto `filters`. Os operadores recebem o prefixo `$` (por exemplo, `$and`, `$or`, `$is`, `$contains`, `$isBetween`). Os parâmetros de paginação (`offset`, `limit`) e `recordTypeId` são passados no corpo da solicitação, em vez de como caminho de URL e parâmetros de consulta.


## Tipos de campo e modificadores de pesquisa

Você pode usar modificadores e filtros com campos para controlar quais dados serão retornados nos resultados.

Para obter exemplos, consulte a [documentação para desenvolvedores da API do Workfront Planning](https://developer.adobe.com/wf-planning/).

### Uso de modificadores de pesquisa

O Workfront Planning suporta os seguintes modificadores de pesquisa:


<table style="table-layout:auto"> 
  <colgroup><col class="c1"><col class="c2"><col class="c3"><col class="c4"></colgroup>
  <thead>
    <tr>
      <th>Modificador</th>
      <th>Exemplo</th>
      <th>Descrição</th>
      <th>Valores possíveis</th>
    </tr>
  </thead>
  <tbody>
    <tr><td class="modifier">CONTÉM</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"CONTAINS","value":"product"}</td><td>Retorna registros cujo valor de campo contém o filtro</td><td class="possible">"Lançamento de novo produto"</td></tr>
    <tr><td class="modifier">DOES_NOT_CONTAIN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"DOES_NOT_CONTAIN","value":"product"}</td><td>Retorna registros em que o valor do campo não contém o filtro</td><td class="possible">"Novo lançamento"</td></tr>
    <tr><td class="modifier">É</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS","value":"new product launch"}</td><td>Retorna registros cujo valor de campo corresponde exatamente ao filtro</td><td class="possible">"Lançamento de novo produto"</td></tr>
    <tr><td class="modifier">IS_NOT</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT","value":"product"}</td><td>Retorna registros cujo valor de campo não corresponde exatamente ao filtro</td><td class="possible">"Lançamento de novo produto"</td></tr>
    <tr><td class="modifier">IS_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EMPTY"}</td><td>Retorna registros cujo valor de campo está vazio</td><td class="possible">"" ou nulo</td></tr>
    <tr><td class="modifier">IS_NOT_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_EMPTY"}</td><td>Retorna registros cujo valor de campo não está vazio</td><td class="possible">"Lançamento de novo produto"</td></tr>
    <tr><td class="modifier">GREATER_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN","value":"10"}</td><td>Retorna registros cujo valor de campo é maior que o filtro</td><td class="possible">"11"</td></tr>
    <tr><td class="modifier">GREATER_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN_OR_EQUAL","value":"10"}</td><td>Retorna registros cujo valor de campo é maior ou igual ao filtro</td><td class="possible">"10", "11"</td></tr>
    <tr><td class="modifier">LESS_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN","value":"10"}</td><td>Retorna registros cujo valor de campo é menor que o filtro</td><td class="possible">"9"</td></tr>
    <tr><td class="modifier">LESS_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN_OR_EQUAL","value":"10"}</td><td>Retorna registros cujo valor de campo é inferior ou igual ao filtro</td><td class="possible">"9", "10"</td></tr>
    <tr><td class="modifier">IS_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>Retorna registros cujo valor de campo está entre os dois valores de filtro</td><td class="possible">["2024-03-01","2024-06-30"]</td></tr>
    <tr><td class="modifier">IS_NOT_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>Retorna registros cujo valor de campo não está entre os dois valores de filtro</td><td class="possible">["2023-01-01","2025-06-30"]</td></tr>
    <tr><td class="modifier">IS_AFTER</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_AFTER","value":"2024-01-01"}</td><td>Retorna registros cujo valor de campo de data está após o filtro</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_BEFORE</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BEFORE","value":"2024-12-31"}</td><td>Retorna registros cujo valor de campo de data é anterior ao filtro</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_ANY_OF","value":["Ative","Planned"]}</td><td>Retorna registros cujo valor de campo corresponde a qualquer valor na lista de filtros</td><td class="possible">["Ativo","Planejado","Concluído"]</td></tr>
    <tr><td class="modifier">IS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NONE_OF","value":["Ative","Planned"]}</td><td>Retorna registros cujo valor de campo não corresponde a nenhum dos valores na lista de filtros</td><td class="possible">["Ativo","Planejado"]</td></tr>
    <tr><td class="modifier">HAS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ANY_OF","value":["Tag1","Tag2"]}</td><td>Retorna registros cujo campo de vários valores contém qualquer um dos valores de filtro</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">HAS_ALL_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ALL_OF","value":["Tag1","Tag2"]}</td><td>Retorna registros cujo campo de vários valores contém todos os valores de filtro</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">IS_EXACTLY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EXACTLY","value":["Tag1"]}</td><td>Retorna registros cujo campo de vários valores contém exatamente os valores de filtro e nenhum outro</td><td class="possible">["Tag1"]</td></tr>
    <tr><td class="modifier">HAS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_NONE_OF","value":["Tag1"]}</td><td>Retorna registros cujo campo de vários valores não contém nenhum dos valores de filtro</td><td class="possible">["Tag1"]</td></tr>
  </tbody>
</table>


>[!NOTE]
>
>Observação sobre a versão 1: os nomes de modificadores V1 usam `$-prefixed camelCase` (por exemplo, `$contains`, `$isNot`, `$isEmpty`, `$greaterThan`, `$greaterThanOrEqual`, `$lessThan`, `$lessThanOrEqual`, `$isBetween`, `$isNotBetween`, `$isAnyOf`, `$hasAllOf`). O comportamento de cada modificador é o mesmo.


## Condições de filtro compatíveis por tipo de campo

| Tipo de campo | Condições suportadas |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| texto, texto longo | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| número, porcentagem, moeda | IS, IS_NOT, GREATER_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN, LESS_THAN_OR_EQUAL, IS_EMPTY, IS_NOT_EMPTY |
| data | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| seleção única | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| multisseleção, usuário | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| booleano | É |
| fórmula | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| created-by | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF |
| atualizado por | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| created-at | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN |
| atualizado-em | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| referência | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| pesquisa | Depende do tipo de campo vinculado |

>[!NOTE]
>
>Observação sobre a **Versão 1:** a Versão 1 usa nomes de operadores com prefixos `$` (por exemplo, `$contains`, `$greaterThan`, `$isAnyOf`, `$hasAllOf`). O conjunto de condições aceitas por tipo de campo é o mesmo.

## Filtragem por campos de pessoas

Os filtros de campo de pessoas (`user`, `created-by`, `updated-by`, `approved-by`) aceitam IDs de usuário do Adobe IMS e IDs de usuário do Workfront. Um valor de string simples é interpretado como uma ID de usuário do Adobe IMS.

Para definir o tipo de identificador para verificar a ID de usuário do Workfront, é necessário passar explicitamente os parâmetros `id` e `idType`. Os valores com suporte para `idType` são &quot;`WF`&quot; para IDs de usuário do Workfront e &quot;`IMS`&quot; para IDs de usuário do Adobe IMS.

```
{ 
  "filter": { 
   "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<userFieldId>", 
        "condition": "HAS_ANY_OF", 
        "value": [ 
          { "id": "63e3b13000078c1795146248182d15dc", "idType": "WF" } 
        ] 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
> Observação da versão 1: V1 oferece suporte somente à filtragem por ID de IMS dos usuários.

## Filtrar campos de referência externa por ID externa

Os campos de referência externa vinculam registros a objetos em outros sistemas Adobe (como projetos Workfront ou AEM Assets). Internamente, o Planning atribui IDs de registro do Planning a esses objetos. Para filtrar esses campos diretamente pela ID de objeto original, adicione `"matchExternalId": true` a uma condição de filtro.

Esse sinalizador só é válido para campos de referência onde `referenceOptions.isExternal` é `true`; ele é ignorado para campos de referência não externos. Se um único valor de cadeia de caracteres não puder ser resolvido, a solicitação falhará com `400 Bad Request`. Se um valor de lista for fornecido, as entradas não resolvidas passarão inalteradas e simplesmente não corresponderão.

```
{ 
  "filter": { 
    "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<externalReferenceFieldId>", 
        "condition": "IS_ANY_OF", 
        "value": [ 
          "5f6a4f6e00000123456789abcdef0123", 
          "/content/dam/wknd/en/adventures/bali-surf-camp" 
        ], 
        "matchExternalId": true 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
>Observação da versão 1: V1 não oferece suporte à filtragem por IDs de objeto externo.

## Campos de conexão externa

Os tipos de registro do Planning podem hospedar campos de referência externa que vinculam registros a objetos em outros sistemas Adobe, em vez de outros tipos de registro do Planning.

Para criar um campo de referência externa por meio da API, defina `referenceOptions.recordTypeId` em um novo campo `REFERENCE` como a ID do tipo de registro externo desejado. O servidor deriva automaticamente `referenceOptions.isExternal=true` e os metadados de conexão (`connectionName, objectName`) do tipo de registro de destino.

Os tipos de objetos externos compatíveis incluem objetos do Workfront (projetos, tarefas, programas, portfólios, empresas, grupos, equipes, usuários) e do AEM Assets (ativos, fragmentos de conteúdo).

>[!NOTE]
>
>Observação da versão 1: V1 não oferece suporte à criação de campos de conexão externa.


## Classificação

Classifique os resultados por qualquer campo incluindo uma matriz `sort` em sua solicitação:

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}
```

Os campos de classificação múltipla são avaliados em ordem. Sempre aplique uma classificação ao paginar para garantir uma ordem consistente entre as páginas.

Para agrupar resultados, inclua uma matriz de grupo ao lado de classificar:

```
{ 
  "sort": [{ "fieldId": "F001", "direction": "asc" }], 
  "group": [{ "fieldId": "F002", "direction": "asc" }] 
} 
```

>[!NOTE]
>
>Observação da versão 1: V1 usa `sorting` (não `sort`), `groupingFieldIds` (matriz de IDs de campo, não objetos `group`) e o `rowOrderViewId` obsoleto agora para aplicar uma ordem de linha de exibição existente. Nenhum desses parâmetros V1 é compatível com a versão

## Projeção de campo

Para limitar quais campos são retornados em uma resposta, use os parâmetros de consulta `fieldIds` ou `fieldAliases` com uma lista separada por vírgulas. Isso reduz o tamanho da carga de resposta e é recomendado para integrações de alto volume ou sensíveis à latência.

>[!NOTE]
>
>Observação sobre a **Versão 1:** a Versão 1 usa `?attributes=` para projeção (por exemplo, `?attributes=data,createdBy`) em vez de `?fieldIds=` ou `?fieldAliases=`.

## Paginação

A API do Planning permite respostas paginadas para gerenciar grandes conjuntos de dados.

* **A paginação baseada em cursor** é usada para espaços de trabalho, tipos de registro, campos e exibições. Passe um valor `cursor` da resposta anterior para recuperar a próxima página. As respostas baseadas em cursor incluem um sinalizador hasMore para indicar se há mais páginas ou não.
* A **paginação baseada em página** é usada para a pesquisa de registro. Use `page` e `size` como parâmetros de consulta. Sempre aplique uma classificação ao paginar para garantir uma ordem consistente entre as páginas. Observe que a paginação é baseada em zero, portanto, para recuperar os resultados da segunda página, use &quot;`page=1`&quot; como parâmetro.

Por exemplo, use a seguinte solicitação para recuperar a segunda página de 500 registros de uma pesquisa de registro:

```
POST /v2/record-types/{recordTypeId}/records/search?page=1&size=500 
{ 
  "sort": [{ "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" }], 
  "filter": { "operator": "AND", "conditions": [ 
    { "fieldId": "<fieldId>", "condition": "IS", "value": "active" } 
  ] } 
} 
```

Todas as respostas paginadas incluem um envelope estruturado indicando se mais resultados estão disponíveis. Sempre aplique uma classificação ao paginar para garantir uma ordem consistente entre as páginas.

>[!NOTE]
>
> **Observação da versão 1:** a V1 usa `offset` e `limit` passados no corpo da solicitação (padrão 500, máx. 2.000). Para recuperar os registros 2001-4000, defina &quot;`offset`&quot;: &quot;`2000`&quot;, &quot;`limit`&quot;: &quot;`2000`&quot; no corpo da solicitação. A resposta retorna uma matriz de registros simples com um campo `totalCount`.

## Operações em massa

A API do Planning permite criar, atualizar, corrigir e excluir registros em massa em uma única solicitação. Consulte a **Referência da API** em [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning) para obter os caminhos de ponto de extremidade, formatos de solicitação e limites de registro por operação.

>[!NOTE]
>
>**Observação sobre a versão 1:** operações em massa não estão disponíveis na versão 1.


## Permissões

As permissões para entidades são gerenciadas por meio de uma API de permissões dedicada, separada dos próprios endpoints de recursos. Isso permite que você leia as permissões atuais, gerencie a lista de compartilhamento e lide com as solicitações de acesso independentemente das operações de dados. Para obter mais informações, consulte a seção &quot;Referências de API&quot; no artigo [API do Workfront Planning](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>**Observação da versão 1:** a versão 1 não expõe uma API de permissões pública. O nível de permissão é incorporado diretamente nos DTOs de resposta do recurso.

## Uso da API do Planning com formulários personalizados do Workfront

Você pode chamar a API do Planning a partir de um campo de pesquisa Externo em um formulário personalizado do Workfront para exibir dados do Planning diretamente nos objetos do Workfront. Para obter mais informações, consulte [Exemplos do campo de pesquisa Externa em um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## Recursos relacionados

Para obter mais documentação relacionada à API, consulte também os seguintes artigos:

* Documentação e referência do desenvolvedor da [API do Workfront Planning](https://developer.adobe.com/wf-planning)
* [Introdução ao Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Visão geral de acesso do Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)
* [Criar aplicativos OAuth2 para integrações do Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

<!--

Our version of this article before Lilit replaced it with the above: 

The goal for the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Planning API.  

A familiarity with the Workfront Planning schema will assist you in understanding the database relationships that can be utilized to pull data out of Workfront Planning for integration purposes. 

You can call the planning API from an External lookup field in a Workfront custom form.

For more information on External lookup fields, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>When using the Planning API, all user-related information will be returned using the Adobe Identity Management System (IMS) user ID, and not the Workfront user ID.
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md). 

## Workfront Planning API versions

* Version 1 - released in July 2024 

  For more information, see the section [Workfront Planning API Version 1](#workfront-planning-api-version-1) in this article. 

* Version 2 - released in May 2026

  For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.


## Workfront Planning API Version 1

Workfront Planning API Version 1 was released in July 2024.

The following sections described functionality that was made available in the Workfront API Version 1. 

All future API version will contain the same functionality, unless otherwise specified. 

### Operations 

Objects are manipulated by sending an HTTP request to their unique URI. The operation to be performed is specified by the HTTP method. 

The standard HTTP methods correspond to the following operations: 

* **GET** - Retrieves an object by ID, searches for all objects by a query 
* **POST** - Inserts a new object 
* **PUT** - Edits an existing object 
* **DELETE** - Deletes an object 

For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Field types and search modifiers used with them 

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

#### Using search modifiers 

Workfront Planning supports the following search modifiers: 

<table>
    <tr>
        <td><b>Modifier</b></td>
        <td><b>Example</b></td>
        <td><b>Description</b></td>
        <td><b>Possible Values</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Returns records whose field value contains the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Returns records where the field value does not contain the filter  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Returns records whose field value exactly match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Returns records whose field value exactly is not match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is empty  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is not empty  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Returns records whose field value is greater than the filter  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is greater than or equal the filter  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Returns records whose field value is less than the filter  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is less than or equal the filter </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is after the filter  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is before the filter </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is between the filter  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is not between the filter  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is any of the filter  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is none of the filter </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has any of the filter  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has all of the filter  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has none of the filter </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is exactly the filter  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>
 
#### Field types 

Below is the list of supported field types and what search modifiers can be used with each of those field types  

| Field Type | Supported search modifiers |
|---|---|
| text |$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| single-select | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolean | $is |
| user | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| formula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| lookup | Depends on the linked field |

### Using "And" and "Or" statements 

In the API call you can have filters that are based on several criteria combined by $and" and "$or" statements  

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

### Using the fields request parameter 

You can use the fields request parameter to specify a comma-separated list of specific fields that should be returned. These field names are case-sensitive.  

For example, the request 

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
..
```

returns a response similar to the following: 

  
```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sorting query results in the API 

You can sort your results by any field if you append the following to your API call: 


`/v1/records/search`

Request body:

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

### Query limits and paginated responses 

By default, Planning API requests return 500 results, starting from the beginning of the list. To override the default limitation for number of results, you can use the `limit` parameter in your requests and set it to a different number, up to 2000 results.  

We recommend that you consider using paginated responses for large datasets by adding the `offset` parameter to your requests. Paginated responses allow you to specify the location of the first result that should be returned. 

For example, if you want to return the results 2001-4000, you can use the following request. This example returns 2000 records that are in active status, starting from the 2001st result: 

`POST /v1/records/search`


Request body: 

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

To make sure your results are properly paginated, use a sorting parameter. This allows the results to be returned in the same order, so that the pagination does not repeat or skip results. 

For more information on sorting, see [Sorting query results in the API](#sorting-query-results-in-the-api) in this article.


Lilit did not want this organized like this - keeping this for reference: 

## Workfront Planning API Version 2

Version of the Workfront Planning API was released in May 2026. 

In addition to all the information contained in Version 1, the following enhancements were added in Version 2: 

* Search by the user's Workfront ID field instead of the user's IMS ID.

    This is applicable to custom People fields, as well as system fields such as Created By and Last Updated By fields.

* Ability to search by external connections (Workfront or AEM objects) via the API.

* Ability to link cross-workspace shared records through API. 

* Support all CRUD operations for workspaces, record types, fields, and views. 

* Enable permissions sharing for all sharable entities via API. 

    This includes workspaces, record types, and views. (***********and in the future also records and fields.*********)

* Support for uploading record thumbnail through API. 

-->