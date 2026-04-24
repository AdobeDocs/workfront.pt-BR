---
content-type: api
navigation-topic: general-api
title: Noções básicas sobre API
description: Noções básicas sobre API
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: be11c7417023ce2f310fce3e0cf77724d101b89e
workflow-type: tm+mt
source-wordcount: '4461'
ht-degree: 96%

---


# Noções básicas sobre API

A meta para a API do Adobe Workfront é simplificar a criação de integrações com o Workfront introduzindo uma arquitetura RESTful que opera via HTTP. Este documento supõe que você esteja familiarizado com as respostas REST e JSON e descreve a abordagem adotada pela API do Workfront.

Uma familiaridade com o esquema do Workfront ajudará a entender as relações de banco de dados que podem ser usadas para obter dados do Workfront para fins de integração.

## Limites e diretrizes

Para garantir um desempenho consistente do sistema sob demanda do Workfront, a API do Workfront limita os threads de API simultâneos. Essa medida de proteção evita problemas do sistema causados por chamadas de API abusivas. O ambiente Sandbox tem o mesmo limite de thread de API simultâneo em vigor, permitindo que clientes e parceiros testem com precisão as chamadas de API antes de liberar o código para produção.

Para ambientes de produção, pré-visualização e test drive, as solicitações de usuários finais têm um tamanho máximo de URI de 8892 bytes, pois estão sendo roteadas por meio da CDN do Workfront (Akamai). Esse limite se aplica somente aos URIs roteados por meio da CDN.

### Isenção de responsabilidade

Qualquer uso da API deve ser testado no ambiente beta do Workfront antes de ser executado no ambiente de produção. Se um cliente usar a API para um processo que o Workfront considere razoavelmente oneroso para o software sob demanda (ou seja, que o processo causa um efeito negativo materialmente no desempenho do software para outros clientes), o Workfront reserva-se o direito de solicitar que o cliente descontinue esse processo. Se o cliente não cumprir e o problema persistir, o Workfront reserva-se o direito de encerrar o processo.

## URL da API do Workfront

Para obter informações sobre o URL que você usará para chamar a API do Workfront, consulte [Formato de domínio para chamadas de API do Adobe Workfront](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md).

## Noções básicas de REST

Esta seção fornece uma introdução de alto nível sobre como interagir com a API REST do Workfront para os seguintes princípios de REST:

### URI do objeto

Cada objeto no sistema recebe um URI exclusivo que consiste no tipo de objeto e na ID. Os exemplos a seguir mostram URIs que descrevem três objetos exclusivos:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

O tipo de objeto não diferencia maiúsculas de minúsculas e pode ser o ObjCode abreviado (como proj) ou o nome alternativo do objeto (projeto).

Para obter uma lista de objetos, ObjCodes válidos e campos de objeto, consulte [API Explorer](../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>No contexto da API do Workfront, um formulário personalizado é um objeto `Category`, e um campo personalizado é um objeto `Parameter`.

### Operações

Os objetos são manipulados enviando uma solicitação HTTP para seu URI exclusivo. A operação a ser executada é especificada pelo método HTTP.

Os métodos HTTP padrão correspondem às seguintes operações:

* **GET**: recupera um objeto por ID, pesquisa todos os objetos por uma consulta, executa relatórios ou executa consultas nomeadas
* **POST**: insere um novo objeto
* **PUT**: edita um objeto existente
* **DELETE**: exclui um objeto

Para contornar deficiências do cliente ou limites de tamanho do protocolo, o parâmetro do método pode ser usado para substituir o comportamento HTTP. Por exemplo, uma operação GET pode ser implementada publicando o seguinte URI:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### Resposta

Cada solicitação recebe uma resposta no formato JSON. A resposta tem um atributo de dados se a solicitação foi bem-sucedida ou um atributo de erro se houve um problema. Por exemplo, a solicitação

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

retorna uma resposta de JSON semelhante à seguinte:


<pre>{<br>    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "priority": 2,<br>            "name": "Brand New Project",<br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Ao executar uma solicitação GET pela barra de endereço do navegador, não é necessário incluir sessionID como parte da solicitação.

Uma segurança especial foi adicionada às solicitações PUT, POST e DELETE. Qualquer solicitação que resulte em gravação ou exclusão do banco de dados só poderá ser executada se **sessionID=abc123** estiver incluído no URI. Os exemplos a seguir mostram como uma solicitação DELETE seria procurada:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### Autenticação

A API autentica cada solicitação para garantir que o cliente tenha acesso para visualizar ou modificar um objeto solicitado.

A autenticação é realizada transmitindo uma ID de sessão que pode ser fornecida usando um dos seguintes métodos:

#### Solicitar autenticação de cabeçalho

O método preferencial de autenticação é transmitir um cabeçalho de solicitação denominado SessionID que contém o token de sessão. Isso tem a vantagem de estar seguro contra ataques de [falsificação de solicitação entre sites (CSRF)](https://pt.wikipedia.org/wiki/Cross-site_request_forgery) e não interferir no URI para fins de armazenamento em cache.

Veja a seguir um exemplo de cabeçalho de solicitação:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Autenticação baseada em cookie

A API usa a mesma autenticação baseada em cookies usada pela interface do usuário da Web para o sistema. Em que, se um cliente fizer logon no Workfront usando a interface da Web, todas as chamadas do AJAX feitas no mesmo navegador usarão a mesma autenticação.

>[!NOTE]
>
>Para proteger contra a possibilidade de ataques CSRF (Falsificação de solicitação entre sites), esse método de autenticação está disponível apenas para operações somente leitura.

## Logon

>[!IMPORTANT]
>
>A Workfront não recomenda mais o uso das chaves de API ou do ponto de acesso `/login`. Em vez disso, use um dos seguintes métodos de autenticação:
>
>* Autenticação do servidor com JWT
>* Autenticação de usuário com OAuth2
>
>Para obter instruções sobre como configurar esses métodos de autenticação, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>
>Para obter instruções sobre como usar a autenticação de servidor no Workfront, consulte [Configurar e usar os aplicativos OAuth2 personalizados da sua organização usando o fluxo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
>
>Para obter instruções sobre como usar a autenticação de usuário no Workfront, consulte [Configurar e usar os aplicativos OAuth2 personalizados de sua organização usando o fluxo de código de autorização](../../wf-api/api/oauth-app-code-token-flow.md).

>[!NOTE]
>
>O procedimento descrito nesta seção se aplicava somente a organizações que ainda não tinham sido integradas à Adobe Business Platform. Como todas as organizações foram integradas à Adobe Business Platform, **fazer logon na Workfront por meio da API Workfront não está mais disponível**.
>
>Para obter uma lista de procedimentos que diferem com base no fato de sua organização ter sido integrada à Adobe Business Platform, consulte [Diferenças de administração entre a Adobe Workfront e a Adobe Business Platform](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Usando um nome de usuário e uma senha válidos, você pode usar a seguinte solicitação para obter uma ID de sessão:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Isso define um cookie para autenticar solicitações futuras, bem como retornar uma resposta JSON com a sessionID recém-criada, a userID do usuário conectado e outros atributos de sessão.

>[!NOTE]
>
>Se você tiver um usuário da API designado que também seja um administrador, o Workfront sugere usar uma chave de API para fazer logon.

**Geração de uma chave de API**

Você pode gerar uma chave de API ao fazer logon no sistema como esse usuário, conforme mostrado no exemplo a seguir:


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Recuperação de uma chave de API gerada anteriormente**

Você também pode recuperar uma chave de API gerada anteriormente para um usuário específico executando getApiKey:


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Você pode usar esse resultado para autenticar qualquer chamada de API adicionando &quot;apiKey&quot; como um parâmetro de solicitação com esse valor no lugar de uma sessionID ou nome de usuário e senha. Isso é benéfico de uma perspectiva de segurança.

A solicitação a seguir é um exemplo de recuperação de dados de um projeto que usa a apiKey:

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Invalidação de uma chave de API**

Se o valor de apiKey tiver sido comprometido, será possível executar &quot;clearApiKey&quot;, que invalida a Chave de API atual, como mostrado no exemplo a seguir:

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Após a limpeza, você pode executar getApiKey novamente para gerar uma nova Chave de API.

### Sair

Quando uma sessão é concluída, você pode usar a seguinte solicitação para fazer o logoff do usuário, impedindo qualquer acesso adicional com a sessionID.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

A sessionID a ser desconectada pode ser especificada como cookie, cabeçalho de solicitação ou parâmetro de solicitação.

Para fazer o logoff de um usuário:

1. Navegue até a tela de logon, mas não faça logon.
1. Altere o URL para /attask/api/v15.0/project/search.\
   Observe que a página não pode ser encontrada.
1. Substitua a palavra *search* por login?username=admin&amp;password=user, substituindo *admin* e *user por seu nome de usuário e senha\
   *Essa sessão é armazenada no navegador como um cookie e não precisa ser reafirmada em cada solicitação GET subsequente.

1. Altere o URL de volta para **/attask/api/v15.0/project/search**.
1. Observe a resposta fornecida.

Você sempre deve incluir a sessionID fornecida após o logon ao executar solicitações PUT, POST e DELETE.

## Comportamento do GET

Use o método GET do HTTP para recuperar um ou vários objetos e executar relatórios.

### Recuperação de objetos

Você pode aprimorar uma pesquisa de objetos usando modificadores e filtros.

#### Recuperando um objeto usando a ID do objeto

Se você souber a ID de um objeto, poderá recuperá-lo acessando seu URI exclusivo. Por exemplo, a solicitação

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

retorna uma resposta semelhante à seguinte:

<pre>{<br>    "percentComplete": 0,<br>    "status": "CUR",<br>    "priority": 2,<br>    "name": "Brand New Project",<br>    "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


Você pode recuperar vários objetos na mesma solicitação especificando o parâmetro de solicitação de ID e fornecendo uma lista de IDs separadas por vírgulas, como mostrado no exemplo a seguir:


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
| ne | retorna resultados que não estão com o status de fechado | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | retorna resultados que têm uma porcentagem concluída maior ou igual a 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=gte...</pre> |
| lte | retorna resultados que têm uma porcentagem concluída menor ou igual a 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | retorna resultados em que a descrição é Nula | <pre>...description_Mod=isnull...</pre> |
| notnull | retorna resultados em que a descrição não é Nula | <pre>...description_Mod=notnull...</pre> |
| contains | retorna resultados em que o nome contém &quot;Workfront&quot; | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| entre | retorna resultados que têm uma data de entrada nos últimos 7 dias | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
>As solicitações de pesquisa diferenciam maiúsculas de minúsculas. Se você receber um erro, verifique se **_Mod** e **_Range** têm as letras maiúsculas corretas.

#### Usando instruções OR

É possível aprimorar uma pesquisa adicionando um parâmetro que inclui &quot;OR&quot;, bem como um número para indicar o nível de um filtro ou uma série de filtros.

Uma instrução OR retorna somente registros na chamada da API que atendam aos critérios de filtragem da instrução OR. Os filtros não estão implícitos entre níveis de instrução OR.

Por exemplo, se você quiser filtrar por

* Tarefas que têm um nome contendo &quot;Planning&quot; OR
* Tarefas em um portfólio chamado &quot;FixedAssets&quot; AND atribuídas a alguém com um nome contendo &quot;Steve&quot; OR
* Tarefas que tenham uma tarefa principal chamada “Final Task”

em seguida, use a seguinte chamada de API com suas várias instruções OR:
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_Mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_Mod=cicontains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### Utilização de parâmetros de filtro

Uma possível armadilha ao usar parâmetros de URL para filtros de pesquisa é que o Workfront analisa determinados parâmetros antes de verificar os diferentes métodos de autenticação (ou seja, nome de usuário, senha, apiKey, cookie). Quando isso acontece, os parâmetros não são usados como filtros na chamada. 

Para evitar esse problema, você pode colocar esses valores em parâmetros de filtro com formatação JSON. Por exemplo, se você deseja filtrar pelo nome de usuário testuser, em vez de usar 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>passe o parâmetro de URL em um filtro, como mostrado no exemplo a seguir:
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### Usando o parâmetro de solicitação Map

Por padrão, os dados retornados de uma pesquisa são uma matriz JSON. Dependendo do caso de uso, pode ser mais eficiente obter o resultado como um objeto JSON indexado pela ID. Isso pode ser feito usando o parâmetro de solicitação map. Por exemplo, a solicitação 
<pre>/attask/api/v15.0/task/search?map=true</pre>retorna uma resposta indexada por ID semelhante à seguinte:
<pre>{<br>    "data": {<br>        "4c9a97db0000000f13ee4446b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "NEW",<br>            "name": "first task",<br>            "ID": "4c9a97db0000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "second task",<br>            "ID": "4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### Uso do parâmetro de solicitação de campos

Por padrão, a recuperação de um objeto retorna apenas o subconjunto de campos mais comumente usado.

Você pode usar o parâmetro de solicitação de campos para especificar uma lista separada por vírgulas de campos específicos a serem retornados. Por exemplo, a solicitação
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate,priority</pre>retorna uma resposta semelhante à seguinte:
<pre>{<br>    "priority": 2,<br>    "name": "first task",<br>    "ID": "4c7c08fa0000002ff924e298ee148df4",<br>    "plannedStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
>
>Esses nomes de campo diferenciam maiúsculas de minúsculas.

Para obter uma lista de possíveis referências de campo, consulte o [API Explorer](../../wf-api/general/api-explorer.md)

#### Pesquisando objetos aninhados

Você pode pesquisar objetos aninhados. Por padrão, objetos aninhados são retornados somente com o nome e a ID. Por exemplo, para obter todas os problemas junto com seus proprietários, use a seguinte solicitação:
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>Se forem necessárias mais informações, você pode solicitar um campo aninhado usando a sintaxe de dois pontos. Por exemplo, a seguinte solicitação pesquisa todas as questões juntamente com o nome, ID, cargo e número de telefone do proprietário
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>e retorna o seguinte: 
<pre>{<br>    "name": "an important issue",<br>    "ID": "4c78285f00000908ea8cfd66e084939f",<br>    "owner": {<br>        "title": "Operations Specialist",<br>        "phoneNumber": "555-1234",<br>        "name": "Admin User",<br>        "ID": "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### Recuperando coleções aninhadas

Você pode recuperar coleções aninhadas de objetos. Por exemplo, para obter um projeto com todas as suas tarefas, use a seguinte solicitação:
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>A solicitação a seguir obtém atribuições de tarefas:
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### Pesquisa de vários campos aninhados

Por padrão, apenas o nome e a ID de cada tarefa são retornados, mas campos aninhados adicionais podem ser especificados com a sintaxe de dois pontos. Para visualizar todos os campos disponíveis para um objeto ou coleção relacionados, basta acrescentar dois pontos e um asterisco à referência do objeto/coleção.
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### Recuperar dados personalizados

Você pode recuperar campos de dados personalizados usando o prefixo “DE:”. Por exemplo, para solicitar um projeto com um parâmetro chamado &quot;CustomText&quot;, use a seguinte solicitação:
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>que retornaria
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText": "task b" <br>}</pre>Você também pode recuperar todos os dados personalizados de um objeto solicitando o campo parameterValues. Por exemplo, 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>retorna dados semelhantes ao seguinte:
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "task b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes": ["first", "second", "third"] <br>    } <br>}</pre>

#### Uso de consultas nomeadas

Alguns tipos de objeto possuem pesquisas nomeadas que são comumente executadas e estão disponíveis ao anexar o nome da consulta ao final do URI do tipo de objeto. Por exemplo, a seguinte solicitação recupera os itens de trabalho (tarefas e problemas) aos quais o usuário está atualmente atribuído:
<pre>/attask/api/v15.0/work/myWork</pre>As consultas nomeadas aceitam a solicitação do parâmetro de campos para recuperar campos adicionais. Algumas consultas nomeadas também aceitam filtros adicionais. Para obter uma lista de consultas nomeadas permitidas para um objeto, consulte a guia Ação do objeto no [API Explorer] (https://developer.adobe.com/workfront/api-explorer/).

#### Usando `Count`

Você pode usar `count` para retornar o número de resultados que correspondem à sua consulta. Isso pode ser útil quando você não precisa dos dados nos resultados. Ao retornar apenas a contagem, o servidor pode processar a solicitação mais rapidamente e economizar largura de banda. Por exemplo, a solicitação
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>retorna o número de resultados no seguinte formato:
<pre>{<br>    "count": 3 <br>}</pre>Retornar uma contagem é uma transferência de dados muito menor do que se os objetos completos fossem retornados. A sintaxe é idêntica à do comando de pesquisa.

### Solicitar um relatório

Você pode realizar uma solicitação de relatório, na qual apenas o agregado de algum campo é desejado com um ou mais agrupamentos. Conforme mostrado no exemplo a seguir, a sintaxe do relatório é a mesma que a sintaxe da API SOAP:
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>que retorna o seguinte resultado
<pre>{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>     "Second Project": { <br>        "sum_hours": 30 <br>    } <br>}</pre>A adição do parâmetro $$ROLLUP=true inclui um total em cada nível de agrupamento:
<pre>{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>    "Second Project": { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br>}</pre>

### Classificação dos resultados da consulta na API

Você pode classificar seus resultados por qualquer campo se acrescentar o seguinte à sua chamada de API:

&amp;entryDate_Sort=asc

Por exemplo, se você deseja classificar por data inicial planejada da tarefa, remova entryDate e substitua-a por plannedCompletionDate.

Isso funciona para a maioria dos campos no Workfront.

### Consideração dos limites de consulta

Ao consultar um objeto, deve-se levar em consideração a relação entre objetos relacionados e as limitações de pesquisa. Por exemplo, conforme mostrado na tabela a seguir, uma consulta por projetos pode retornar no máximo 2.000 projetos. Esses 2.000 projetos são considerados “objetos primários”. Se você consultar o campo Tarefas nos projetos, o campo Tarefas, que é uma coleção, se torna um objeto secundário ao objeto primário Projeto. Uma consulta para o campo Tarefas pode incluir milhares de tarefas em projetos. No total, o número combinado de objetos (projetos e tarefas) retornados não pode exceder o máximo de 50.000.

Para garantir um desempenho ideal, a tabela a seguir mostra as limitações impostas às solicitações de pesquisa. 

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
   <td> Se nenhum limite for especificado no filtro de consulta (ou seja, $$LIMIT), o resultado não poderá conter mais de 100 objetos primários. <br>Consulte <a href="#using-paginated-responses" class="MCXref xref">Usar respostas paginadas</a> para obter instruções sobre como contornar essa limitação. </td> 
  </tr> 
  <tr> 
   <td>Número máximo de resultados</td> 
   <td>2.000</td> 
   <td>O filtro de consulta (ou seja, $$LIMIT) não pode retornar mais de 2000 resultados. Consulte “Respostas paginadas” para obter mais informações.</td> 
  </tr> 
  <tr> 
   <td>Profundidade máxima do campo</td> 
   <td>4</td> 
   <td>Ao identificar os campos que deseja exibir, você não pode se afastar mais do que quatro níveis do objeto que está sendo consultado.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de objetos</td> 
   <td>50.000</td> 
   <td>O conjunto de resultados não pode incluir 50.000 objetos primários e secundários.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de campos</td> 
   <td nowrap>1.000.000</td> 
   <td>Quando o conjunto de resultados for inferior a 50.000 objetos, seus resultados poderão incluir no máximo 1.000.000 de campos.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de criações/atualizações em lote</td> 
   <td>100</td> 
   <td>O limite máximo para criação ou atualização em lote é 100.</td> 
  </tr> 
 </tbody> 
</table>

### Utilização de respostas paginadas {#using-paginated-responses}

Para substituir a limitação da consulta Número padrão de resultados e permitir 200 resultados, você pode incluir o filtro `$$LIMIT=200` na sua consulta, conforme mostrado no exemplo a seguir:
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

Para garantir a confiabilidade e o desempenho para outros locatários no sistema, o limite máximo permitido de resultados por consulta é de 2.000 objetos. Tentar especificar um limite maior resultará em uma mensagem de erro `IllegalArgumentException`. 

Portanto, recomendamos que você considere o uso de respostas paginadas para grandes conjuntos de dados. Para especificar o primeiro resultado que deve ser retornado, adicione o filtro `$$FIRST`. Por exemplo, a solicitação a seguir retorna os resultados 201–250 para uma consulta:
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

Observe que, no exemplo acima, `$$FIRST=200` retorna o 201º resultado. `$$FIRST=0` retornaria o primeiro resultado. Pode ser útil pensar no valor $$FIRST como o número de resultados que você deseja ignorar antes de retornar os resultados.

Para garantir que seus resultados sejam paginados corretamente, use um parâmetro de classificação. Isso permite que os resultados sejam retornados na mesma ordem, para que a paginação não repita ou pule resultados. Por exemplo, para classificar usando a ID do objeto, use `ID_Sort=asc`.

### Criar uma regra de acesso

Você pode criar uma regra de acesso para determinar quem pode acessar um objeto. A seguir estão exemplos de regras de acesso que você pode definir:

Para definir um projeto para que seja compartilhado apenas com um usuário com o ID &quot;abc123&quot;, use a seguinte solicitação:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>Como alternativa, para compartilhar apenas com uma nova pessoa e manter as permissões existentes intactas:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>Para recuperar as regras de acesso já existentes:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## Comportamento POST

POST insere um novo objeto. A sintaxe é idêntica à do PUT, mas com algumas exceções. Como o novo objeto ainda não existe, ele não possui uma ID. Por esse motivo, o URI não inclui a ID.

### Criar um objeto

A seguir, um exemplo de solicitação para criar um novo projeto:
<pre>POST /attask/api/v15.0/project?name=New Project</pre>A resposta inclui o projeto recém-criado, juntamente com sua nova ID e quaisquer outros campos especificados.

### Copiar um objeto

Alguns objetos podem ser copiados. Para esses tipos de objeto, é possível criar novos objetos fazendo uma postagem com um parâmetro copySourceID. Por exemplo, a seguinte solicitação copia o projeto especificado e atribui a ele um novo nome:

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Fazer upload de documentos

Você pode fazer upload de documentos através da seguinte URL da API:
<pre>POST /attask/api/v15.0/upload</pre>A API espera que o tipo de conteúdo seja multipart/form-data. O nome do parâmetro do arquivo deve ser uploadedFile. O servidor retorna os seguintes dados JSON:
<pre>{<br>    "handle": "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>Você pode usar o nome de usuário e publicar no seguinte URL ao criar um documento do Workfront:
<pre>POST /attask/api/v15.0/document?updates={<br>    name: aFileName,<br>    handle: abc...123, (handle from the file upload)<br>    docObjCode: PROJ, (or TASK, OPTASK, etc)<br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## Comportamento PUT

PUT é usado para atualizar um objeto.

A resposta de uma PUT é idêntica a uma GET. Em ambos os casos, o servidor retorna o novo estado do objeto após a atualização. Todas as regras utilizadas para alterar uma resposta a uma solicitação GET também funcionam com PUT, como especificar campos adicionais a serem retornados, dados personalizados e assim por diante.

### Editar objetos

As atualizações dos objetos são sempre feitas por meio de IDs, utilizando o URI exclusivo do objeto. Os campos a serem atualizados são especificados como parâmetros de solicitação. Por exemplo, para alterar o nome de um projeto, você poderia enviar uma solicitação semelhante à seguinte:
<pre>PUT /attask/api/v15.0/project/4c7...?name=Novo nome do projeto <br>PUT /attask/api/v15.0/project?id=4c7...&amp;name=Novo nome do projeto</pre>Como a atualização requer uma ID, essa operação falhará (sem inserção) se o objeto não existir no servidor.

### Especificar edições em JSON

Conforme mostrado no exemplo a seguir, você pode usar o parâmetro de solicitação de atualizações para especificar os campos a serem atualizados usando a sintaxe JSON:
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>&lbrace;<br>     nome: "Novo Nome de Projeto", <br>     status: "CUR", <br>     ... <br></pre>

### Fazer atualizações aninhadas

Alguns objetos possuem coleções particulares que podem ser atualizadas. O exemplo a seguir demonstra como substituir as atribuições existentes para uma determinada tarefa:
<pre>PUT /attask/api/v15.0/task/4c7...?updates= <br>&lbrace;<br>    atribuições: [ <br>        { <br>            assignedToID: "2222...54d0, <br>            assignmentPercent: 50.0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br></pre>

>[!NOTE]
>
>Embora as atualizações feitas no nível superior sejam esparsas, as atualizações em uma coleção ou objeto aninhado substituem completamente a coleção existente. Para editar uma única atribuição em uma tarefa sem afetar os objetos, use PUT na atribuição em vez de na tarefa.

O exemplo a seguir transforma um projeto em uma fila pública de suporte técnico. Observe que as propriedades da fila já existente são substituídas.
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>{ <br>    queueDef: { <br>        isPublic: 1 <br>    } <br>}</pre>

### Usar o parâmetro de solicitação de ação

Alguns objetos aceitam ações adicionais que podem ser realizadas além de edições simples. Você pode especificar essas ações usando o parâmetro de solicitação de ação. Por exemplo, a seguinte solicitação recalcula o cronograma de um determinado projeto:
<pre>PUT /attask/api/v15.0/project/4c7...?action=calculateTimeline<br><br>ou<br><br>PUT /attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### Mover objetos

A seguir, é demonstrada a sintaxe para mover uma tarefa de um projeto para outro:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>Um exemplo para cada tipo de ação é fornecido aqui: (??)
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/recallApproval<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>Apenas a ação de movimentação requer a identificação de atributos adicionais para especificar o projeto para o qual o item de trabalho deve ser movido.

A seguir, apresentamos um exemplo de cada tipo de ação: 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Compartilhar objetos

O exemplo a seguir demonstra a sintaxe para compartilhar um projeto com uma equipe:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>Ao editar um objeto, você pode substituir todas as regras de acesso em um objeto fazendo um PUT e enviando atualizações semelhantes ao exemplo a seguir:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>O exemplo a seguir mostra a sintaxe para mover uma tarefa de um projeto para outro:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## Comportamento DELETE

DELETE remove um objeto. Em todos os casos, a URI pode incluir o parâmetro force=true para fazer com que o servidor remova os dados especificados e seus dependentes. No exemplo a seguir, uma tarefa é excluída executando o método DELETE do HTTP em um URI:
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## Atualizações em massa

Uma instrução de atualização em massa atualiza vários objetos ao mesmo tempo em uma única chamada de API. Uma chamada de API de criação em massa é criada de forma semelhante a uma chamada de atualização normal, conforme mostrado nos exemplos a seguir:
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>ou <pre>PUSH /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>o que resulta em um retorno semelhante ao seguinte:
<pre>data: [{<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    name: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    name: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>}]</pre>Você também pode fazer uma atualização em massa semelhante à seguinte:
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>o que resulta em um retorno semelhante ao seguinte:
<pre>data: [ {<br>     ID: "53ff8e15003b461d4560f7f65a440078",<br>     name: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>     plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>     priority: 0,<br>     projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     status: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    name: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>    status: "CUR"<br>}]</pre>Se você deseja que todas as operações ocorram na mesma transação, adicione “atomic=true” à sua chamada de API em lote como um parâmetro de solicitação. Dessa forma, se alguma das operações falhar, todas as operações serão revertidas.

>[!NOTE]
>
>Operações atômicas em lote só podem retornar &quot;success: true&quot; ou um erro.

