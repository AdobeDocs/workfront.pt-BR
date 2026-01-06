---
content-type: api
navigation-topic: general-api
title: Noções básicas sobre API
description: Noções básicas sobre API
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 319c45bc6617269f358af1e7b5f6132a8694710b
workflow-type: tm+mt
source-wordcount: '4396'
ht-degree: 0%

---


# Noções básicas sobre API

O objetivo da API do Adobe Workfront é simplificar a criação de integrações com o Workfront, introduzindo uma arquitetura REST-ful que opera via HTTP. Este documento supõe que você esteja familiarizado com as respostas REST e JSON e descreve a abordagem adotada pela API do Workfront.

Uma familiaridade com o esquema do Workfront ajudará você a entender as relações de banco de dados que podem ser usadas para obter dados do Workfront para fins de integração.

## Limites e diretrizes

Para garantir um desempenho consistente do sistema sob demanda do Workfront, a API do Workfront limita as threads de API simultâneas. Essa proteção evita problemas do sistema causados por chamadas de API abusivas. O ambiente de sandbox tem o mesmo limite de thread de API simultâneo em vigor, permitindo que clientes e parceiros testem com precisão as chamadas de API antes de lançar o código para produção.

Para ambientes de produção, pré-visualização e teste de unidades, as solicitações de usuários finais têm um comprimento máximo de URI de 8892 bytes, pois estão sendo roteadas por meio do Workfront CDN (Akamai). Esse limite se aplica somente aos URIs roteados por meio da CDN.

### Isenção de responsabilidade

Qualquer uso da API deve ser testado no ambiente beta do Workfront antes de ser executado no ambiente de produção. Se qualquer cliente usar a API para um processo que a Workfront considere razoavelmente oneroso para o software sob demanda (ou seja, o processo causa um efeito materialmente negativo no desempenho do software para outros clientes), a Workfront se reserva o direito de solicitar que o cliente descontinue esse processo. Se o cliente não estiver em conformidade e o problema persistir, a Workfront se reserva o direito de encerrar o processo.

## URL da API Workfront

Para obter informações sobre a URL que você usará para chamar a API do Workfront, consulte [Formato de domínio para chamadas de API do Adobe Workfront](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md).

## Noções básicas de REST

Esta seção fornece uma introdução de alto nível sobre como interagir com a API REST do Workfront para os seguintes princípios REST:

### URI do objeto

Cada objeto no sistema recebe um URI exclusivo que consiste no tipo de objeto e na ID. Os exemplos a seguir mostram URIs que descrevem três objetos únicos:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

O tipo de objeto não diferencia maiúsculas de minúsculas e pode ser o ObjCode abreviado (como proj) ou o nome de objeto alternativo (projeto).

Para obter uma lista de objetos, Códigos de Obj válidos e campos de objeto, consulte  [API Explorer](../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>No contexto da API do Workfront, um formulário personalizado é um objeto `Category`, e um campo personalizado é um objeto `Parameter`.

### Operações

Os objetos são manipulados enviando uma solicitação HTTP para seu URI exclusivo. A operação a ser executada é especificada pelo método HTTP.

Os métodos HTTP padrão correspondem às seguintes operações:

* **GET** - Recupera um objeto por ID, pesquisa todos os objetos por uma consulta, executa relatórios ou executa consultas nomeadas
* **POST** - Insere um novo objeto
* **PUT** - Edita um objeto existente
* **DELETE** - Exclui um objeto

Para contornar deficiências do cliente ou limites de comprimento do protocolo, o parâmetro do método pode ser usado para substituir o comportamento HTTP. Por exemplo, uma operação do GET pode ser implementada publicando o seguinte URI:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### Resposta

Cada solicitação recebe uma resposta no formato JSON. A resposta tem um atributo de dados se a solicitação tiver sido bem-sucedida ou um atributo de erro se houver um problema. Por exemplo, a solicitação

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

retorna uma resposta JSON semelhante ao seguinte:


<pre>{<br>    "dados": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "priority": 2,<br>            "name": "Novo projeto",<br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br></pre>

>[!NOTE]
>
>Ao executar uma solicitação do GET pela barra de endereços do navegador, não é necessário incluir a sessionID como parte da solicitação.

Uma segurança especial foi adicionada às solicitações do PUT, POST e DELETE. Qualquer solicitação que resulte em gravação ou exclusão do banco de dados só poderá ser executada se **sessionID=abc123** estiver incluída no URI. Os exemplos a seguir mostram como isso procuraria uma solicitação DELETE:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### Autenticação

A API autentica cada solicitação para garantir que o cliente tenha acesso para visualizar ou modificar um objeto solicitado.

A autenticação é realizada transmitindo uma ID de sessão que pode ser fornecida usando um dos seguintes métodos:

#### Solicitar autenticação de cabeçalho

O método preferido de autenticação é passar um cabeçalho de solicitação chamado SessionID contendo o token de sessão. Isso tem a vantagem de estar seguro contra [ataques de falsificação de solicitação entre sites (CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) e não interferir no URI para fins de armazenamento em cache.

Veja a seguir um exemplo de um cabeçalho de solicitação:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Autenticação baseada em cookie

A API usa a mesma autenticação baseada em cookies usada pela interface do usuário da Web para o sistema. Onde, se um cliente fizer logon no Workfront usando a interface da Web, quaisquer chamadas do AJAX feitas no mesmo navegador usarão a mesma autenticação.

>[!NOTE]
>
>Para proteger contra a possibilidade de ataques CSRF (Cross Site Request Forgery), esse método de autenticação está disponível somente para operações somente leitura.

## Logon

>[!IMPORTANT]
>
>A Workfront não recomenda mais o uso do ponto de extremidade ou das chaves de API `/login`. Em vez disso, use um dos seguintes métodos de autenticação:
>
>* Autenticação do servidor com JWT
>* Autenticação de usuário com OAuth2
>
>Para obter instruções sobre como configurar esses métodos de autenticação, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>
>Para obter instruções sobre como usar a autenticação de servidor no Workfront, consulte [Configurar e usar os aplicativos OAuth 2 personalizados da sua organização usando o fluxo JWT](../../wf-api/api/oauth-app-jwt-flow.md)
>
>Para obter instruções sobre como usar a autenticação de usuário no Workfront, consulte [Configurar e usar os aplicativos OAuth 2 personalizados de sua organização usando o fluxo de código de autorização](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
>
>O procedimento descrito nesta seção se aplica apenas a organizações que ainda não foram integradas à Adobe Business Platform. Fazer logon no Workfront por meio da API do Workfront não estará disponível se sua organização tiver sido integrada à Adobe Business Platform.
>
>Para obter uma lista de procedimentos que diferem dependendo de sua organização ter sido integrada à Adobe Business Platform, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Usando um nome de usuário e senha válidos, você pode usar a seguinte solicitação para obter uma ID de sessão:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Isso define um cookie para autenticar solicitações futuras, bem como retornar uma resposta JSON com a sessionID recém-criada, a userID do usuário conectado e outros atributos de sessão.

>[!NOTE]
>
>Se você tiver um usuário da API designado que também seja um administrador, a Workfront sugere usar uma chave de API para fazer logon.

**Gerando uma Chave de API**

Você pode gerar uma Chave de API ao fazer logon no sistema como esse usuário, conforme mostrado no exemplo a seguir:


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Recuperando uma Chave de API Gerada Anteriormente**

Você também pode recuperar uma Chave de API que foi gerada anteriormente para um usuário específico executando getApiKey:


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Você pode usar esse resultado para autenticar qualquer chamada de API adicionando &quot;apiKey&quot; como um parâmetro de solicitação com esse valor no lugar de uma sessionID ou nome de usuário e senha. Isso é benéfico do ponto de vista da segurança.

A solicitação a seguir é um exemplo de recuperação de dados de um projeto usando a apiKey:

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Invalidando uma Chave de API**

Se o valor apiKey tiver sido comprometido, será possível executar &quot;clearApiKey&quot;, que invalida a Chave de API atual, como mostrado no exemplo a seguir:

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Depois de limpa, você pode executar getApiKey novamente para gerar uma nova Chave de API.

### Sair

Quando uma sessão é concluída, você pode usar a seguinte solicitação do para fazer logoff do usuário, impedindo qualquer acesso adicional com a sessionID.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

A sessionID a ser desconectada pode ser especificada como um cookie, cabeçalho de solicitação ou parâmetro de solicitação.

Para fazer logoff de um usuário:

1. Navegue até a tela de logon, mas não faça logon.
1. Altere o URL para /attask/api/v15.0/project/search.\
   Observe que a página não pode ser encontrada.
1. Substitua a palavra *search* por login?username=admin&amp;password=user, substituindo seu nome de usuário e senha por *admin* e *user\
   *Essa sessão é armazenada no navegador como um cookie e não precisa ser reafirmada em cada solicitação subsequente do GET.

1. Altere a URL de volta para **/attask/api/v15.0/project/search**.
1. Observe a resposta fornecida.

Você sempre deve incluir a sessionID fornecida após o logon ao executar solicitações do PUT, POST e DELETE.

## Comportamento do GET

Use o método GET do HTTP para recuperar um ou vários objetos e executar relatórios.

### Recuperando Objetos

Você pode aprimorar uma pesquisa por objetos usando modificadores e filtros.

#### Recuperando um objeto usando a ID do objeto

Se você souber a ID de um objeto, poderá recuperá-lo acessando seu URI exclusivo. Por exemplo, a solicitação

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

retorna uma resposta semelhante à seguinte:

<pre>{<br>    "percentComplete": 0,<br>    "status": "CUR",<br>    "priority": 2,<br>    "name": "Novo projeto",<br>    "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br></pre>


Você pode recuperar vários objetos na mesma solicitação especificando o parâmetro de solicitação de id e fornecendo uma lista de IDs separadas por vírgulas, como mostrado no exemplo a seguir:


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

Observe que a solicitação /attask/api/v15.0/project?id=... é igual à solicitação `/attask/api/v15.0/project/...`.

#### Recuperando um objeto usando o URI

Se quiser recuperar um objeto por critérios diferentes da ID, procure o URI.

Por exemplo, você pode usar a seguinte solicitação para retornar uma lista de todos os projetos no sistema:

```
GET /attask/api/v15.0/project/search
```

Você pode especificar filtros usando os parâmetros da solicitação como pares de nome-valor. Por exemplo, o exemplo a seguir mostra uma solicitação que localizaria todos os projetos atuais:

```
GET /attask/api/v15.0/project/search?status=CUR
```

A solicitação a seguir encontra todas as tarefas que ainda não foram concluídas e que foram atribuídas a um usuário chamado John.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Uso de Modificadores de Pesquisa

A tabela a seguir lista alguns dos modificadores que podem ser usados com a API do Workfront.

| **Modificador** | **Descrição** | **Exemplo** |
| --- | --- | --- |
| eq | retorna resultados que estão com o status de fechado | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | retorna resultados que não estão no status de fechado | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| get | retorna resultados que têm uma porcentagem concluída maior ou igual a 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=get...</pre> |
| lte | retorna resultados que têm uma porcentagem concluída menor ou igual a 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | retorna resultados em que a descrição é Null | <pre>...description_Mod=isnull...</pre> |
| notnull | retorna resultados em que a descrição não é Nula | <pre>...description_Mod=notnull...</pre> |
| contém | retorna resultados em que o nome contém &quot;Workfront&quot; | <pre>...name=Workfront&amp;name_Mod=contém...</pre> |
| entre | retorna resultados que têm uma data de entrada nos últimos 7 dias | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
>As solicitações de pesquisa fazem distinção entre maiúsculas e minúsculas. Se você receber um erro, verifique se  **_Mod** e **_Range** têm as letras maiúsculas corretas.

#### Uso de instruções OR

É possível aprimorar uma pesquisa adicionando um parâmetro que inclui &quot;OU&quot;, bem como um número para indicar o nível de um filtro ou uma série de filtros.

Uma instrução OR retorna somente registros na chamada à API que atendam aos critérios de filtragem da instrução OR. Os filtros não estão implícitos nos níveis de instrução OU.

Por exemplo, se você deseja filtrar por

* Tarefas que têm um nome contendo &quot;Planning&quot; OR
* Tarefas em um portfólio chamado &quot;FixedAssets&quot; E atribuídas a alguém com um nome contendo &quot;Steve&quot; OU
* Tarefas que têm uma tarefa pai chamada &quot;Tarefa Final&quot;

Em seguida, use a seguinte chamada de API com suas várias instruções OR:
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_Mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_Mod=cicontains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### Utilização de parâmetros de filtro

Uma possível armadilha no uso de parâmetros de URL para filtros de pesquisa é que o Workfront analisa determinados parâmetros antes de verificar se há diferentes métodos de autenticação (ou seja, nome de usuário, senha, apiKey, cookie). Quando isso acontece, os parâmetros não são usados como filtros na chamada. 

Para evitar esse problema, você pode colocar esses valores em parâmetros de filtro com formatação JSON. Por exemplo, se você deseja filtrar pelo nome de usuário testuser, em vez de usar 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>passe o parâmetro de URL em um filtro, como mostrado no exemplo a seguir:
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### Uso do Parâmetro de solicitação de mapa

Por padrão, os dados retornados de uma pesquisa são uma matriz JSON. Dependendo do caso de uso, pode ser mais eficiente obter o resultado como um objeto JSON indexado pela ID. Isso pode ser feito usando o parâmetro de solicitação map. Por exemplo, a solicitação 
<pre>/attask/api/v15.0/task/search?map=true</pre>retorna uma resposta indexada por ID semelhante à seguinte:
<pre>{<br>    "dados": {<br>        "4c9a97db0000000f13ee4446b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "NEW",<br>            "name": "primeira tarefa",<br>            "ID": "4c9a97db0000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "segunda tarefa",<br>            "ID": "4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### Uso do parâmetro de solicitação de campos

Por padrão, a recuperação de um objeto retorna somente o subconjunto de campos usado com mais frequência.

Você pode usar o parâmetro de solicitação de campos para especificar que uma lista separada por vírgulas de campos específicos seja retornada. Por exemplo, a solicitação
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate,priority</pre>retorna uma resposta semelhante à seguinte:
<pre>{<br>    "priority": 2,<br>    "name": "primeira tarefa",<br>    "ID": "4c7c08fa0000002ff924e298ee148df4",<br>    "plannedStartDate": "30/08/2010:00:00:000-0600" <br></pre>

>[!NOTE]
>
>Esses nomes de campos fazem distinção entre maiúsculas e minúsculas.

Para obter uma lista de referências de campo possíveis, consulte  [API Explorer](../../wf-api/general/api-explorer.md)

#### Pesquisando Objetos Aninhados

Você pode pesquisar objetos aninhados. Por padrão, objetos aninhados são retornados somente com o nome e a ID. Por exemplo, para obter todos os problemas junto com seus proprietários, use a seguinte solicitação:
<pre>/attask/api/v15.0/issue/search?fields=proprietário</pre>Se forem necessárias mais informações, é possível solicitar um campo aninhado usando a sintaxe de dois pontos. Por exemplo, a solicitação a seguir pesquisa todos os problemas, juntamente com o nome, a ID, o título e o número de telefone do proprietário
<pre>/attask/api/v15.0/issue/search?fields=proprietário:título,proprietário:phoneNumber</pre>e retorna o seguinte: 
<pre>{<br>    "name": "um problema importante",<br>    "ID": "4c78285f00000908ea8cfd66e084939f",<br>    "proprietário": {<br>        "title": "Especialista em Operações",<br>        "phoneNumber": "555-1234",<br>        "name": "Usuário administrador",<br>        "ID": "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br></pre>

#### Recuperando coleções aninhadas

Você pode recuperar coleções aninhadas de objetos. Por exemplo, para obter um projeto com todas as suas tarefas, use a seguinte solicitação:
<pre>/attask/api/v15.0/project/search?fields=tarefas</pre>A solicitação a seguir obtém atribuições de tarefas:
<pre>/attask/api/v15.0/task/search?fields=atribuições</pre>

#### Pesquisa de vários campos aninhados

Por padrão, somente o nome e a ID de cada tarefa são retornados, mas campos aninhados adicionais podem ser especificados com a sintaxe de dois pontos. Para exibir todos os campos disponíveis para um objeto ou coleção relacionada, basta anexar dois pontos e um asterisco à referência do objeto/coleção.
<pre>/attask/api/v15.0/task/search?fields=atribuições:*</pre>

#### Recuperação de dados personalizados

Você pode recuperar campos de dados personalizados usando o prefixo &quot;DE:&quot;. Por exemplo, para solicitar um projeto com um parâmetro chamado &quot;CustomText&quot;, use a seguinte solicitação:
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>que retornaria
<pre>{<br>    "name": "projeto de dados personalizado",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText": "task b" <br>}</pre>Você também pode recuperar todos os dados personalizados de um objeto solicitando o campo parameterValues. Por exemplo, 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>retorna dados semelhantes ao seguinte:
<pre>{<br>    "name": "projeto de dados personalizado",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "tarefa b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes": ["first", "second", "third"] <br>    } <br></pre>

#### Uso de Consultas Nomeadas

Alguns tipos de objeto têm pesquisas nomeadas que são executadas com frequência e estão disponíveis ao anexar o nome da consulta ao final do URI do tipo de objeto. Por exemplo, a solicitação a seguir recupera os itens de trabalho (tarefas e problemas) aos quais o usuário está atribuído no momento:
<pre>/attask/api/v15.0/work/myWork</pre>As consultas nomeadas suportam a solicitação do parâmetro de campos para recuperar campos adicionais. Algumas consultas nomeadas também aceitam filtros adicionais. Para obter uma lista de consultas nomeadas permitidas para um objeto, consulte a guia Ação para o objeto na  [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

#### Usando o `Count`

Você pode usar `count` para retornar o número de resultados que correspondem à sua consulta. Isso pode ser útil quando você não precisa dos dados nos resultados. Ao retornar apenas a contagem, o servidor pode processar a solicitação mais rapidamente e economizar largura de banda. Por exemplo, a solicitação
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>retorna o número de resultados no seguinte formato:
<pre>{<br>    "count": 3 <br>}</pre>Retornar uma contagem é uma transferência de dados muito menor do que se os objetos completos forem retornados. A sintaxe é idêntica ao comando search.

### Solicitar um relatório

Você pode executar uma solicitação de relatório, onde somente a agregação de algum campo é desejada com um ou mais agrupamentos. Como mostrado no exemplo a seguir, a sintaxe do relatório é igual à sintaxe da API do SOAP:
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>que retorna o seguinte resultado
<pre>{<br>    "Primeiro projeto": { <br>        "sum_hours": 15 <br>    }, <br>     "Segundo projeto": { <br>        "sum_hours": 30 <br>    } <br></pre>A adição do parâmetro $$ROLLUP=true inclui um total em cada nível de agrupamento:
<pre>{<br>    "Primeiro projeto": { <br>        "sum_hours": 15 <br>    }, <br>    "Segundo projeto": { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br></pre>

### Classificação dos resultados da consulta na API

Você pode classificar os resultados por qualquer campo se anexar o seguinte à chamada de API:

&amp;entryDate_Sort=asc

Por exemplo, se você deseja classificar por Data de início planejada da tarefa, remova entryDate e substitua-a por plannedCompletionDate.

Isso funciona para a maioria dos campos no Workfront.

### Consideração dos limites de consulta

Ao consultar um objeto, deve-se levar em consideração a relação entre objetos relacionados e as limitações de pesquisa. Por exemplo, como mostrado na tabela a seguir, uma consulta de projetos não pode retornar mais de 2.000 projetos. Esses 2.000 projetos são considerados &quot;objetos principais&quot;. Se você consultar o campo Tasks nos projetos, o campo Tasks, que é uma coleção, se tornará um objeto secundário ao projeto de objeto principal. Uma consulta para o campo Tarefas pode incluir milhares de tarefas em projetos. No total, o número combinado de objetos (projetos e tarefas) retornados não pode exceder o máximo de 50.000.

Para garantir o desempenho ideal, a tabela a seguir mostra as limitações impostas às solicitações de pesquisa. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Resultado da consulta</th> 
   <th>Limitação</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">Número padrão de resultados</td> 
   <td>100</td> 
   <td> Se nenhum limite for especificado no filtro de query (ou seja, $$LIMIT), o resultado não poderá conter mais de 100 objetos primários. <br>Consulte <a href="#using-paginated-responses" class="MCXref xref">Usar respostas paginadas</a> para obter instruções sobre como substituir essa limitação. </td> 
  </tr> 
  <tr> 
   <td>Número máximo de resultados</td> 
   <td>2.000</td> 
   <td>O filtro de query (ou seja, $$LIMIT) não pode retornar mais de 2000 resultados. Consulte "Respostas paginadas" para obter mais informações.</td> 
  </tr> 
  <tr> 
   <td>Profundidade máxima do campo</td> 
   <td>4</td> 
   <td>Ao identificar os campos que deseja exibir, não é possível distanciar mais de quatro níveis do objeto que está sendo consultado.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de objetos</td> 
   <td>50.000</td> 
   <td>O conjunto de resultados não pode incluir 50000 objetos principais e secundários.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de campos</td> 
   <td nowrap>1.000.000</td> 
   <td>Quando o conjunto de resultados tiver menos de 50.000 objetos, seus resultados poderão incluir no máximo 1.000.000 campos.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de criações/atualizações em lote</td> 
   <td>100</td> 
   <td>O limite máximo de criação ou atualização de lote é 100.</td> 
  </tr> 
 </tbody> 
</table>

### Utilização de respostas paginadas {#using-paginated-responses}

Para substituir a limitação de consulta Número Padrão de Resultados e permitir 200 resultados, você pode incluir o filtro `$$LIMIT=200` em sua consulta, como mostrado no exemplo a seguir:
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

Para garantir a confiabilidade e o desempenho de outros locatários no sistema, o limite máximo de resultados permitido por consulta é de 2000 objetos. Tentar especificar um limite maior resultará em uma mensagem de erro `IllegalArgumentException`. 

Portanto, recomendamos que você considere usar respostas paginadas para grandes conjuntos de dados. Para especificar o primeiro resultado que deve ser retornado, adicione o filtro `$$FIRST`. Por exemplo, a solicitação a seguir retorna os resultados 201-250 para uma consulta:
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

Observe que no exemplo acima, `$$FIRST=200` retorna o 201º resultado. `$$FIRST=0` retornaria o primeiro resultado. Pode ser útil pensar no valor $$FIRST como o número de resultados que você deseja ignorar antes de retornar os resultados.

Para garantir que seus resultados sejam paginados corretamente, use um parâmetro de classificação. Isso permite que os resultados sejam retornados na mesma ordem, para que a paginação não repita ou ignore os resultados. Por exemplo, para classificar usando a ID de objeto, use `ID_Sort=asc`.

### Criação de uma regra de acesso

Você pode criar uma regra de acesso para determinar quem pode acessar um objeto. Veja a seguir exemplos de regras de acesso que você pode definir:

Para definir um projeto para que ele seja compartilhado somente com um usuário com ID &quot;abc123&quot;, use a seguinte solicitação:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>Como alternativa, para compartilhar somente com uma nova pessoa e manter as permissões existentes intactas:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>Para recuperar as regras de acesso existentes:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=regras de acesso:*</pre>

## Comportamento do POST

POST insere um novo objeto. A sintaxe é idêntica à do PUT, mas com algumas exceções. Como o novo objeto ainda não existe, ele não tem uma ID. Por esse motivo, o URI não inclui a ID.

### Criação de um objeto

Veja a seguir um exemplo de uma solicitação para criar um novo projeto:
<pre>POST /attask/api/v15.0/project?name=Novo projeto</pre>A resposta inclui o projeto recém-criado, a nova ID e todos os outros campos especificados.

### Copiando um Objeto

Alguns objetos oferecem suporte à cópia. Para esses tipos de objeto, é possível criar novos objetos publicando com um parâmetro copySourceID. Por exemplo, a solicitação a seguir copia o projeto fornecido e lhe dá um novo nome:

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Carregando Documentos

Você pode fazer upload de documentos por meio do seguinte URL da API:
<pre>POST /attask/api/v15.0/upload</pre>A API espera que o tipo de conteúdo seja multipart/form-data. O nome do parâmetro do arquivo deve ser uploadedFile. O servidor retorna os seguintes dados JSON:
<pre>{<br>    "handle": "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>Você pode usar o identificador e publicar no seguinte URL ao criar um documento do Workfront:
<pre>POST /attask/api/v15.0/document?updates={<br>}    nome: aFileName,<br>    handle: abc...123, (identificador do carregamento de arquivo)<br>    docObjCode: PROJ, (ou TASK, OPTASK, etc.)<br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br></pre>

## Comportamento do PUT

O PUT é usado para atualizar um objeto existente.

A resposta de uma PUT é idêntica a uma GET. Em ambos os casos, o servidor retorna o novo estado do objeto após a atualização. Todas as regras usadas para alterar uma resposta a uma solicitação do GET também funcionam com o PUT, como especificar campos adicionais a serem retornados, dados personalizados etc.

### Editando Objetos

As atualizações de objetos são sempre feitas por ID usando o URI exclusivo do objeto. Os campos que serão atualizados são especificados como parâmetros de solicitação. Por exemplo, para alterar o nome de um projeto, você pode enviar uma solicitação semelhante à seguinte:
<pre>PUT /attask/api/v15.0/project/4c7...?name=Novo nome do projeto <br>PUT /attask/api/v15.0/project?id=4c7...&amp;name=Novo nome do projeto</pre>Como a atualização requer uma ID, essa operação falhará (sem inserção) se o objeto não existir no servidor.

### Especificação de edições de JSON

Como mostrado no exemplo a seguir, você pode usar o parâmetro de solicitação de atualizações para especificar os campos a serem atualizados usando a sintaxe JSON:
<pre>PUT /attask/api/v15.0/project/4c7...?atualizações= <br>{<br>     nome: "Novo Nome de Projeto", <br>     status: "CUR", <br>     ... <br></pre>

### Fazer atualizações aninhadas

Alguns objetos têm coleções de propriedade privada que podem ser atualizadas. Por exemplo, o exemplo a seguir demonstra como substituir as atribuições existentes para uma determinada tarefa:
<pre>PUT /attask/api/v15.0/task/4c7...?atualizações= <br>{<br>    atribuições: [ <br>        { <br>            assignedToID: "2222...54d0, <br>            assignmentPercent: 50.0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br></pre>

>[!NOTE]
>
>Enquanto as atualizações feitas no nível superior são esparsas, as atualizações em uma coleção ou objeto aninhado substituem completamente a coleção existente. Para editar uma única atribuição em uma tarefa sem afetar os objetos, use o PUT na atribuição em vez da tarefa.

O exemplo a seguir torna um projeto uma fila de Help Desk pública. Observe que as propriedades existentes da fila são substituídas.
<pre>PUT /attask/api/v15.0/project/4c7...?atualizações= <br>{ <br>    queueDef: { <br>        isPublic: 1 <br>    } <br>}</pre>

### Uso do Parâmetro de Solicitação de Ação

Alguns objetos oferecem suporte a ações adicionais que podem ser executadas, além de edições simples. Você pode especificar essas ações usando o parâmetro action request. Por exemplo, a solicitação a seguir recalcula a linha do tempo de um determinado projeto:
<pre>PUT /attask/api/v15.0/project/4c7...?action=calculateTimeline<br><br>ou<br><br>PUT /attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### Movendo Objetos

A seguir é apresentada a sintaxe para mover uma tarefa de um projeto para outro:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>Um exemplo para cada tipo de ação é fornecido aqui: (??)
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/recallApproval<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>Somente a ação de mover requer a identificação de atributos adicionais para especificar o projeto para o qual o item de trabalho deve ser movido.

Veja a seguir um exemplo de cada tipo de ação: 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Objetos de Compartilhamento

O exemplo a seguir demonstra a sintaxe para o compartilhamento de um projeto com uma equipe:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>Ao editar um objeto, você pode substituir todas as regras de acesso em um objeto fazendo uma PUT e enviando atualizações semelhantes ao seguinte exemplo:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>O exemplo a seguir mostra a sintaxe para mover uma tarefa de um projeto para outro:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## Comportamento do DELETE

O DELETE remove um objeto. Em todos os casos, o URI pode incluir o parâmetro force=true para fazer com que o servidor remova os dados especificados e seus dependentes. No exemplo a seguir, uma tarefa é excluída executando o método HTTP DELETE em um URI:
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=pt</pre>

## Atualizações em massa

Uma instrução de atualização em massa atualiza vários objetos ao mesmo tempo em uma única chamada de API. Uma chamada de API de criação em massa é criada de forma semelhante a uma chamada de atualização normal, como mostrado nos exemplos a seguir:
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>ou <pre>PUSH /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>que resulta em um retorno semelhante ao seguinte:
<pre>dados: [{<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    nome: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "28/08/2014 T11:00:00:000-0400",<br>    plannedStartDate: "28/08/2014 T11:00:00:000-0400",<br>    prioridade: 0,<br>    projectsCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    nome: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi,<br>    plannedCompletionDate: "28/08/2014 T11:00:00:000-0400",<br>    plannedStartDate: "28/08/2014 T11:00:00:000-0400",<br>    prioridade: 0,<br>    projectsCompletionDate: "28/08/2014 T16:12:00:000-0400",<br>    status: "CUR"<br>]</pre>Você também pode fazer uma atualização em massa semelhante ao seguinte:
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Editar"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>que resulta em um retorno semelhante ao seguinte:
<pre>dados: [<br>     ID: "53ff8e15003b461d4560f7f65a440078",<br>     name: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     plannedCompletionDate: "28/08/2014 T11:00:00:000-0400",<br>     plannedStartDate: "28/08/2014 T11:00:00:000-0400",<br>     prioridade: 0,<br>     projectsCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     status: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    name: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "28/08/2014 T11:00:00:000-0400",<br>    plannedStartDate: "28/08/2014 T11:00:00:000-0400",<br>    prioridade: 0,<br>    projectsCompletionDate: "28/08/2014 T16:16:00:000-0400",<br>    status: "CUR"<br>]</pre>Se quiser que todas as operações aconteçam na mesma transação, adicione "atomic=true" à chamada da API em lote como um parâmetro de solicitação. Dessa forma, se qualquer uma das operações falhar, todas as operações serão revertidas.

>[!NOTE]
>
>As operações atômicas em lote só podem retornar &quot;success: true&quot; ou um erro.

