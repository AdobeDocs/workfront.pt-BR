---
content-type: api
navigation-topic: general-api
title: Noções básicas sobre API
description: Noções básicas sobre API
author: Becky
feature: Workfront API
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '4405'
ht-degree: 0%

---


# Noções básicas sobre API

O objetivo da API do Adobe Workfront é simplificar a criação de integrações com o Workfront, introduzindo uma arquitetura REST-ful que opera via HTTP. Este documento supõe que você está familiarizado com as respostas REST e JSON e descreve a abordagem adotada pela API do Workfront.

Uma familiaridade com o esquema do Workfront ajudará você a entender os relacionamentos do banco de dados que podem ser utilizados para retirar dados do Workfront para fins de integração.

## Limites e diretrizes

Para garantir um desempenho consistente do sistema sob demanda da Workfront, cada cliente está limitado a 10 threads simultâneos de API. O ambiente de sandbox tem o mesmo limite em vigor, permitindo que clientes e parceiros testem com precisão as chamadas de API antes de liberar o código para produção.

Para ambientes de produção, visualização e teste de unidade, as solicitações do usuário final têm um comprimento máximo de URI de 8892 bytes, pois estão sendo roteadas por meio do Workfront CDN (Akamai). Esse limite se aplica somente aos URIs roteados por meio da CDN.

>[!NOTE]
>
>esse limite não é aplicável a ambientes sandbox porque os ambientes sandbox não são roteados por meio da CDN.

### Isenção de responsabilidade

Qualquer uso da API deve ser testado no ambiente beta do Workfront antes de ser executado no ambiente de produção. Se qualquer cliente usar a API para um processo que a Workfront razoavelmente considera ser oneroso para o software sob demanda (ou seja, o processo causa um efeito significativamente negativo no desempenho do software para outros clientes), a Workfront se reserva o direito de solicitar que o cliente interrompa esse processo. Se o cliente não estiver em conformidade e o problema persistir, a Workfront se reserva o direito de encerrar o processo.

## Noções básicas sobre REST

Esta seção fornece uma introdução de alto nível de como interagir com a API REST do Workfront para os seguintes princípios REST:

### URI do objeto

Cada objeto no sistema recebe um URI exclusivo que consiste no tipo de objeto e na ID. Os exemplos a seguir mostram URIs que descrevem três objetos exclusivos:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

O tipo de objeto não diferencia maiúsculas de minúsculas e pode ser o ObjCode abreviado (como proj) ou o nome de objeto alternativo (projeto).

Para obter uma lista de ObjCodes válidos, consulte  [API Explorer](../../wf-api/general/api-explorer.md).

### Operações

Os objetos são manipulados enviando uma solicitação HTTP para seu URI exclusivo. A operação a ser executada é especificada pelo método HTTP .

Os métodos HTTP padrão correspondem às seguintes operações:

* **GET** - Recupera um objeto por ID, pesquisa todos os objetos por uma consulta, executa relatórios ou executa consultas nomeadas
* **POST** - Insere um novo objeto
* **PUT** - Edita um objeto existente
* **DELETE** - Exclui um objeto

Para contornar as deficiências do cliente ou os limites de comprimento do protocolo, o parâmetro de método pode ser usado para substituir o comportamento HTTP. Por exemplo, uma operação do GET pode ser implementada ao postar o seguinte URI:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### Resposta

Cada solicitação recebe uma resposta no formato JSON. A resposta tem um atributo de dados se a solicitação foi bem-sucedida ou um atributo de erro se houver um problema. Por exemplo, a solicitação

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

retorna uma resposta JSON semelhante ao seguinte:


<pre>{<br>    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "Prioridade": 2,<br>            "name": "Novo projeto da marca",<br>            "ID": "4c7c08b2000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Ao executar uma solicitação do GET na barra de endereços do navegador, não é necessário incluir a sessionID como parte da solicitação.

Foi adicionada uma segurança especial às solicitações PUT, POST e DELETE. Qualquer solicitação que resulta na gravação ou exclusão do banco de dados só poderá ser executada se a variável **sessionID=abc123** está incluído no URI. Os exemplos a seguir mostram como isso deve procurar uma solicitação DELETE:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### Autenticação

A API autentica cada solicitação para garantir que o cliente tenha acesso para visualizar ou modificar um objeto solicitado.

A autenticação é executada transmitindo uma ID de sessão que pode ser fornecida usando um dos seguintes métodos:

#### Solicitar Autenticação de Cabeçalho

O método preferido de autenticação é passar um cabeçalho de solicitação chamado SessionID contendo o token de sessão. Isso tem a vantagem de ser seguro contra [Falsificação de solicitação entre sites (CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) e não interferir no URI para fins de armazenamento em cache.

Este é um exemplo de um cabeçalho de solicitação:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Autenticação de parâmetro da solicitação

Você pode autenticar transmitindo um parâmetro de solicitação chamado sessionID, como mostrado no exemplo a seguir: 

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

#### Autenticação baseada em cookies

A API usa a mesma autenticação com cookies usada pela interface do usuário da Web no sistema. Onde, se um cliente fizer logon no Workfront usando a interface do usuário da Web, qualquer chamada de AJAX feita no mesmo navegador usará a mesma autenticação.

>[!NOTE]
>
>Para proteger contra a possibilidade de ataques de CSRF (Cross Site Request Forgery), esse método de autenticação só está disponível para operações de somente leitura.

## Logon

>[!IMPORTANT]
A Workfront não recomenda mais o uso da variável `/login` endpoint ou chaves de API. Em vez disso, use um dos seguintes métodos de autenticação:
* Autenticação de servidor com JWT
* Autenticação do usuário com OAuth2
>
Para obter instruções sobre como configurar esses métodos de autenticação, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)
Para obter instruções sobre como usar a autenticação de servidor no Workfront, consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo JWT](../../wf-api/api/oauth-app-jwt-flow.md)
Para obter instruções sobre como usar a autenticação de usuário no Workfront, consulte [Configure e use os aplicativos OAuth 2 personalizados de sua organização usando o fluxo do código de autorização](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
O procedimento descrito nesta seção aplica-se apenas a organizações que ainda não foram incorporadas à Adobe Business Platform. Fazer logon no Workfront por meio da API do Workfront não estará disponível se sua organização tiver sido integrada à Adobe Business Platform.
Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Plataforma de negócios do Adobe, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Usando um nome de usuário e senha válidos, você pode usar a seguinte solicitação para obter uma ID de sessão:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Isso define um cookie para autenticar solicitações futuras, bem como retornar uma resposta JSON com a sessionID recém-criada, a userID do usuário conectado e outros atributos de sessão.

>[!NOTE]
Se você tiver um usuário designado da API que também seja um administrador, a Workfront recomenda usar uma Chave da API para fazer logon.

**Gerar uma chave de API**

Você pode gerar uma Chave de API ao fazer logon no sistema como esse usuário, conforme mostrado no exemplo a seguir:


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Recuperação de uma chave de API gerada anteriormente**

Você também pode recuperar uma Chave de API que foi gerada anteriormente para um usuário específico executando getApiKey:


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Em seguida, você pode usar esse resultado para autenticar qualquer chamada de API adicionando &quot;apiKey&quot; como parâmetro de solicitação com esse valor no lugar de um sessionID ou nome de usuário e senha. Isto é benéfico do ponto de vista da segurança.

A solicitação a seguir é um exemplo de recuperação de dados de um projeto usando a apiKey:

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Invalidar uma chave de API**

Se o valor de apiKey tiver sido comprometido, você poderá executar &quot;clearApiKey&quot; que invalida a Chave de API atual, como mostrado no exemplo a seguir:

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Depois de limpo, você pode executar getApiKey novamente para gerar uma nova Chave de API.

### Sair

Quando uma sessão é concluída, você pode usar a seguinte solicitação para fazer logoff do usuário, evitando qualquer acesso adicional com a sessionID.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

A sessionID a ser desconectada pode ser especificada como cookie, cabeçalho de solicitação ou parâmetro de solicitação.

Para fazer logoff de um usuário:

1. Navegue até a tela de logon, mas não faça logon.
1. Altere o URL para /attask/api/v15.0/project/search.\
   Observe que a página não pode ser encontrada.
1. Substituir a palavra *pesquisa* com login?username=admin&amp;password=user, substituindo seu nome de usuário e senha por *administrador* e *usuário\
   *Esta sessão é armazenada no navegador como um cookie e não precisa ser redefinida em cada solicitação subsequente do GET.

1. Altere o URL de volta para **/attask/api/v15.0/project/search**.
1. Observe a resposta fornecida.

Você sempre deve incluir a sessionID fornecida após o logon ao executar solicitações PUT, POST e DELETE.

## Comportamento do GET

Use o método HTTP GET para recuperar um objeto ou vários objetos e executar relatórios.

### Recuperação de objetos

É possível aprimorar a pesquisa de objetos usando modificadores e filtros.

#### Recuperação de um objeto usando a ID de objeto

Se você souber a ID de um objeto, poderá recuperar o objeto acessando sua URI exclusiva. Por exemplo, a solicitação

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

retorna uma resposta semelhante à seguinte:

<pre>{<br>    "percentComplete": 0,<br>    "status": "CUR",<br>    "Prioridade": 2,<br>    "name": "Novo projeto da marca",<br>    "ID": "4c7c08b2000002de5ca1ebc19edf2d5" <br>}</pre>


Você pode recuperar vários objetos na mesma solicitação especificando o parâmetro da solicitação de id e fornecendo uma lista separada por vírgulas de IDs, como mostrado no exemplo a seguir:


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

Observe que a solicitação /attask/api/v15.0/project?id=.. é igual à solicitação `/attask/api/v15.0/project/...` solicitação.

#### Recuperação de um objeto usando o URI

Se quiser recuperar um objeto por critérios diferentes da ID, pesquise o URI.

Por exemplo, você pode usar a seguinte solicitação para retornar uma lista de todos os projetos no sistema:

```
GET /attask/api/v15.0/project/search
```

Você pode especificar filtros usando os parâmetros da solicitação como pares de nome-valor. Por exemplo, o exemplo a seguir mostra uma solicitação que encontraria todos os projetos atuais:

```
GET /attask/api/v15.0/project/search?status=CUR
```

A solicitação a seguir encontra todas as tarefas que ainda não foram concluídas e que foram atribuídas a um usuário chamado John.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Usando modificadores de pesquisa

A tabela a seguir lista alguns dos modificadores que podem ser usados com a API do Workfront.

| **Modificador** | **Descrição** | **Exemplo** |
|---|---|---|
| eq | retorna resultados que estão no status de fechado | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | retorna resultados que não estão no status de fechado | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | retorna resultados com uma porcentagem concluída maior ou igual a 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=gte...</pre> |
| lte | retorna resultados com uma porcentagem concluída menor ou igual a 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| null | retorna resultados em que a descrição é Nulo | <pre>...description_Mod=isnull..</pre> |
| notnull | retorna resultados em que a descrição não é Nula | <pre>...description_Mod=notnull..</pre> |
| contém | retorna resultados em que o nome contém &quot;Workfront&quot; | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| entre | retorna resultados com uma data de entrada nos últimos 7 dias | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
As solicitações de pesquisa fazem distinção entre maiúsculas e minúsculas. Se receber um erro, verifique se  **_Mod** e **_Intervalo** têm a capitalização correta.

#### Uso de instruções OR

Você pode aprimorar uma pesquisa adicionando um parâmetro que inclui &quot;OU&quot; e um número para indicar o nível de um filtro ou de uma série de filtros.

Uma instrução OR retorna somente registros na chamada da API que atendem aos critérios de filtragem da instrução OR. Os filtros não são implícitos nos níveis de instrução OR.

Por exemplo, se você deseja filtrar por

* Tarefas com um nome contendo &quot;Planejamento&quot; OU
* Tarefas em um portfólio chamado &quot;FixedAssets&quot; E atribuídas a alguém com um nome contendo &quot;Steve&quot; OU
* Tarefas que têm uma tarefa pai chamada &quot;Tarefa Final&quot;

em seguida, use a seguinte chamada de API com suas várias instruções OR:
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OU:1:portfólio:name=FixedAssets<br>&amp;OU:1:portfólio:name_Mod=eq<br>&amp;OU:1:assignedTo:name=Steve<br>&amp;OU:1:assignedTo:name_Mod=cicontains<br>&amp;OU:2:parent:name=Tarefa Final<br>&amp;OU:2:parent:name_Mod=eq
</pre>

#### Utilização de parâmetros de filtro

Uma possível armadilha com o uso de parâmetros de URL para filtros de pesquisa é que o Workfront analisa determinados parâmetros antes de verificar métodos de autenticação diferentes (ou seja, nome de usuário, senha, apiKey, cookie). Quando isso acontece, os parâmetros não são usados como filtros na chamada . 

Para evitar esse problema, você pode colocar esses valores em parâmetros de filtro com a formatação JSON. Por exemplo, se você deseja filtrar para o nome de usuário testuser, em vez de usar 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>passe o parâmetro do URL em um filtro, como mostrado no exemplo a seguir:
<pre>/attask/api/v15.0/user/search?filters={"nome do usuário":"testuser@workfront.com"}</pre>

#### Uso do parâmetro de solicitação de mapa

Por padrão, os dados retornados de uma pesquisa são uma matriz JSON. Dependendo do caso de uso, pode ser mais eficiente obter o resultado como um objeto JSON indexado pela ID. Isso pode ser feito usando o parâmetro de solicitação de mapa. Por exemplo, a solicitação 
<pre>/attask/api/v15.0/task/search?map=true</pre>retorna uma resposta indexada pela ID semelhante ao seguinte:
<pre>{<br>    "data": {<br>        "4c9a97db000000f13ee446b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "NOVO",<br>            "name": "first task",<br>            "ID": "4c9a97db000000f13ee446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "segunda tarefa",<br>            "ID": "4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### Uso do parâmetro de solicitação de campos

Por padrão, recuperar um objeto retorna somente o subconjunto de campos mais usado.

Você pode usar o parâmetro de solicitação de campos para especificar que uma lista separada por vírgulas de campos específicos seja retornada. Por exemplo, a solicitação
<pre>/attask/api/v15.0/task/search?fields=planStartDate,priority</pre>retorna uma resposta semelhante à seguinte:
<pre>{<br>    "Prioridade": 2,<br>    "name": "first task",<br>    "ID": "4c7c08fa000002ff924e298ee148df4",<br>    "planStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
Esses nomes de campos fazem distinção entre maiúsculas e minúsculas.

Para obter uma lista de possíveis referências de campo, consulte  [API Explorer](../../wf-api/general/api-explorer.md)

#### Pesquisar objetos aninhados

Você pode procurar objetos aninhados. Por padrão, objetos aninhados são retornados somente com o nome e a ID. Por exemplo, para obter todos os problemas com seus proprietários, use a seguinte solicitação:
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>Se mais informações forem necessárias, é possível solicitar um campo aninhado usando a sintaxe de dois pontos. Por exemplo, a solicitação a seguir pesquisa todos os problemas juntamente com o nome, ID, título e número de telefone do proprietário
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>e retorna o seguinte: 
<pre>{<br>    "name": "uma questão importante",<br>    "ID": "4c78285f00000908ea8cfd66e084939f",<br>    "Proprietário": {<br>        "Título": "Especialista em operações",<br>        "phoneNumber": "555-1234",<br>        "name": "Usuário administrador",<br>        "ID": "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### Recuperação de coleções aninhadas

Você pode recuperar coleções aninhadas de objetos. Por exemplo, para obter um projeto com todas as suas tarefas, use a seguinte solicitação:
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>A solicitação a seguir obtém atribuições de tarefa:
<pre>/attask/api/v15.0/task/search?fields=atribuições</pre>

#### Pesquisar por vários campos aninhados

Por padrão, somente o nome e a ID de cada tarefa são retornados, mas campos aninhados adicionais podem ser especificados com sintaxe de dois pontos. Para exibir todos os campos disponíveis para um objeto ou coleção relacionado, basta anexar um sinal de dois pontos e um asterisco à referência objeto/coleção.
<pre>/attask/api/v15.0/task/search?fields=atribuições:*</pre>

#### Recuperação de dados personalizados

Você pode recuperar campos de dados personalizados usando o prefixo &quot;DE:&quot;. Por exemplo, para solicitar um projeto com um parâmetro chamado &quot;CustomText&quot;, use a seguinte solicitação:
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>que retornaria
<pre>{<br>    "name": "projeto de dados personalizados",<br>    "ID": "4c9a954f000001afad0687d7b1b4e43",<br>    "DE:CustomText": "tarefa b" <br>}</pre>Você também pode recuperar todos os dados personalizados de um objeto solicitando o campo parameterValues . Por exemplo, 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>retorna dados semelhantes aos seguintes:
<pre>{<br>    "name": "projeto de dados personalizados",<br>    "ID": "4c9a954f000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "tarefa b", <br>        "DE:CustomNumber": 1.4. <br>        "DE:CustomCheckBoxes": ["primeiro", "segundo", "terceiro"] <br>    } <br>}</pre>

#### Usando Consultas Nomeadas

Alguns tipos de objetos têm pesquisas nomeadas que são normalmente executadas e estão disponíveis ao anexar o nome da consulta ao final do URI do tipo de objeto. Por exemplo, a solicitação a seguir recupera os itens de trabalho (tarefas e problemas) aos quais o usuário está atribuído no momento:
<pre>/attask/api/v15.0/work/myWork</pre>As consultas nomeadas são compatíveis com a solicitação do parâmetro fields para recuperar campos adicionais. Algumas consultas nomeadas também aceitam filtros adicionais. Para obter uma lista de consultas nomeadas permitidas para um objeto, consulte a guia Ação para o objeto no [API Explorer](../../wf-api/general/api-explorer.md).

#### Usar o filtro de contagem

Você pode especificar o número de resultados que deseja retornar por uma determinada pesquisa. Isso permite que o servidor processe a solicitação mais rapidamente e economize largura de banda. Por exemplo, a solicitação
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>retorna o número de resultados no seguinte formato:
<pre>{<br>    "count": 3 <br>}</pre>Esse resultado é um download muito menor do que se os objetos completos fossem enviados. A sintaxe do filtro é idêntica ao comando de pesquisa.

### Solicitar um relatório

É possível executar uma solicitação de relatório, onde somente a agregação de algum campo é desejada com um ou mais agrupamentos. Como mostrado no exemplo a seguir, a sintaxe do relatório é a mesma da API SOAP:
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>que retorna o seguinte resultado
<pre>{<br>    "Primeiro projeto": { <br>        "sum_hours": 15. <br>    }, <br>     "Segundo projeto": { <br>        "sum_hours": 30º <br>    } <br>}</pre>A adição do parâmetro $$ROLLUP=true inclui um total em cada nível de agrupamento:
<pre>{<br>    "Primeiro projeto": { <br>        "sum_hours": 15. <br>    }, <br>    "Segundo projeto": { <br>        "sum_hours": 30º <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45º <br>    } <br>}</pre>

### Classificação dos resultados da consulta na API

Você pode classificar os resultados por qualquer campo se anexar o seguinte à chamada de API:

&amp;entryDate_Sort=asc

Por exemplo, se você deseja classificar por tarefa Data de início planejada, remova entryDate e substitua-a por planCompletionDate.

Isso funciona para a maioria dos campos no Workfront.

### Considerando os limites da consulta

Ao consultar um objeto, deve-se considerar especialmente a relação dos objetos relacionados e as limitações da pesquisa. Por exemplo, como mostrado na tabela a seguir, uma consulta de projetos não pode retornar mais de 2.000 projetos. Esses 2.000 projetos são considerados &quot;objetos primários&quot;. Se você consultar o campo Tarefas nos projetos, o campo Tarefas, que é uma coleção, se tornará um objeto secundário do projeto principal. Um query do campo Tasks pode incluir milhares de tarefas em projetos. No total, o número combinado de objetos (projetos e tarefas) retornados não pode exceder o máximo de 50.000.

Para garantir um desempenho ideal, a tabela a seguir mostra as limitações colocadas em solicitações de pesquisa. 

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
   <td> Se nenhum limite for especificado no filtro de query (ou seja, $$LIMIT), o resultado não poderá conter mais de 100 objetos primários. <br>Consulte <a href="#using-paginated-responses" class="MCXref xref">Uso de Respostas Paginadas</a> para obter instruções sobre como substituir essa limitação. </td> 
  </tr> 
  <tr> 
   <td>Número máximo de resultados</td> 
   <td>2,000</td> 
   <td>O filtro de query (ou seja, $$LIMIT) não pode retornar mais de 2000 resultados. Consulte "Respostas paginadas" para obter mais informações.</td> 
  </tr> 
  <tr> 
   <td>Profundidade máxima do campo</td> 
   <td>4</td> 
   <td>Ao identificar os campos que deseja exibir, não é possível distanciar mais de quatro níveis do objeto consultado.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de objetos</td> 
   <td>50,000</td> 
   <td>O conjunto de resultados não pode incluir 50000 objetos primários e secundários.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de campos</td> 
   <td nowrap>1,000,000</td> 
   <td>Quando o conjunto de resultados tiver menos de 50000 objetos, seus resultados poderão incluir no máximo 1.000.000 campos.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de criações/atualizações de lote</td> 
   <td>100</td> 
   <td>O limite máximo de criação ou atualização de lote é 100.</td> 
  </tr> 
 </tbody> 
</table>

### Uso de Respostas Paginadas {#using-paginated-responses}

Para substituir a limitação Default Number of Results query e permitir 200 resultados, você pode incluir o filtro $$LIMIT=200 em sua query, como mostrado no exemplo a seguir:
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>Para garantir confiabilidade e desempenho para outros locatários no sistema, o limite máximo de resultados permitidos por query é de 2000 objetos. Tentar especificar um limite maior resultará em uma mensagem de erro IllegalArgumentException . 

Portanto, recomendamos que você considere usar respostas paginadas para conjuntos de dados grandes. Para especificar o primeiro resultado que deve ser retornado, adicione o filtro $$FIRST . Por exemplo, a solicitação a seguir retorna os resultados 201-250 para um query:
<pre>GET /attask/api/v15.0/project/search?$$FIRST=201&amp;$$LIMIT=50</pre>

### Criação de uma regra de acesso

Você pode criar uma regra de acesso para determinar quem pode acessar um objeto. A seguir estão exemplos de regras de acesso que podem ser definidas:

Para definir um projeto para que ele seja compartilhado somente com um usuário com a ID &quot;abc123&quot;, use a seguinte solicitação:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessID: 'abc123', accessObjCode: 'USUÁRIO', coreAction: 'VIEW'} ] }</pre>Como alternativa, para compartilhar somente com uma nova pessoa e manter as permissões existentes intactas:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessID=abc123&amp;accessObjCode=USER&amp;coreAction=VIEW</pre>Para recuperar as regras de acesso existentes:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## Comportamento POST

POST insere um novo objeto. A sintaxe é idêntica ao PUT, mas com algumas exceções. Como o novo objeto ainda não existe, ele não tem uma ID. Por esse motivo, o URI não inclui a ID.

### Criação de um objeto

Este é um exemplo de solicitação para criar um novo projeto:
<pre>POST /attask/api/v15.0/project?name=New Project</pre>A resposta inclui o projeto recém-criado, juntamente com sua nova ID e quaisquer outros campos especificados.

### Copiando um objeto

Alguns objetos suportam a cópia. Para esses tipos de objetos, é possível criar novos objetos ao publicar com um parâmetro copySourceID. Por exemplo, a solicitação a seguir copia o projeto e lhe dá um novo nome:

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Fazer upload de documentos

Você pode fazer upload de documentos por meio do seguinte URL da API:
<pre>POST /attask/api/v15.0/upload</pre>A API espera que o tipo de conteúdo seja dados de várias partes/formulários. O nome do parâmetro para o arquivo deve ser uploadFile. O servidor retorna os seguintes dados JSON:
<pre>{<br>    "Identificador": "4c7c08fa000002ff924e298ee148df4"<br>}</pre>Você pode usar o identificador e publicar no seguinte URL ao criar um documento do Workfront:
<pre>POST /attask/api/v15.0/document?updates={<br>    name: aFileName,<br>    identificador: abc...123, (identificador do upload do arquivo)<br>    docObjCode: PROJ, (ou TAREFA, OPTASK etc.)<br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## Comportamento PUT

PUT é usado para atualizar um objeto existente.

A resposta de um PUT é idêntica a um GET. Em ambos os casos, o servidor retorna o novo estado do objeto após a atualização. Todas as regras usadas para alterar uma resposta a uma solicitação de GET também funcionam com o PUT, como especificar campos adicionais a serem retornados, dados personalizados, e assim por diante.

### Editar objetos

As atualizações de objetos são sempre feitas pela ID, usando o URI exclusivo do objeto. Os campos a serem atualizados são especificados como parâmetros de solicitação. Por exemplo, para alterar o nome de um projeto, você pode enviar uma solicitação semelhante ao seguinte:
<pre>PUT /attask/api/v15.0/project/4c7..?name=Novo nome do projeto <br>PUT /attask/api/v15.0/project?id=4c7..&amp;name=Novo nome do projeto</pre>Como a atualização requer uma ID, essa operação falhará (sem inserção) se o objeto não existir no servidor.

### Especificação de edições JSON

Como mostrado no exemplo a seguir, você pode usar o parâmetro de solicitação de atualizações para especificar os campos a serem atualizados usando a sintaxe JSON:
<pre>PUT /attask/api/v15.0/project/4c7..?update= <br>{<br>     name: "Nome do novo projeto", <br>     status: "CUR", <br>     ... <br>}</pre>

### Fazer atualizações aninhadas

Alguns objetos têm coleções privadas que podem ser atualizadas. Por exemplo, o exemplo a seguir demonstra como substituir as atribuições existentes de uma determinada tarefa:
<pre>PUT /attask/api/v15.0/task/4c7...?update= <br>{<br>    atribuições: [ <br>        { <br>            assignedToID: "2222...54d0, <br>            assignPercent: 50,0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br>}</pre>

>[!NOTE]
Embora as atualizações feitas no nível superior sejam esparsas, as atualizações em uma coleção ou em um objeto aninhado substituem completamente a coleção existente. Para editar uma única atribuição em uma tarefa sem afetar os objetos, use o PUT na atribuição em vez de na tarefa.

O exemplo a seguir transforma um projeto em uma fila pública do suporte técnico. Observe que as propriedades da fila existentes são substituídas.
<pre>PUT /attask/api/v15.0/project/4c7..?update= <br>{ <br>    queueDef: { <br>        isPublic: 1 <br>    } <br>}</pre>

### Usar o parâmetro de solicitação de ação

Alguns objetos suportam ações adicionais que podem ser executadas além de edições simples. Você pode especificar essas ações usando o parâmetro de solicitação de ação. Por exemplo, a solicitação a seguir recalcula a linha do tempo de um determinado projeto:
<pre>PUT /attask/api/v15.0/project/4c7..?action=calculateTimeline<br><br>ou<br><br>PUT /attask/api/v15.0/project/4c7../calculateTimeline </pre>

### Mover objetos

A seguir, é exibida a sintaxe para mover uma tarefa de um projeto para outro:
<pre>PUT /attask/api/v15.0/task/4c7../move?projectID=5d8..</pre>Um exemplo para cada tipo de ação é fornecido aqui: (??)
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateLinha do tempo<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/callApproval<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>Somente a ação de mover requer a identificação de atributos adicionais para especificar o projeto onde o item de trabalho será movido.

Este é um exemplo de cada tipo de ação: 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessID: 'abc123', accessObjCode: 'USUÁRIO', coreAction: 'VIEW'}]}</pre>

### Compartilhamento de objetos

O exemplo a seguir demonstra a sintaxe para compartilhar um projeto com uma equipe:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx=access&amp;accessObj&amp;access=ObjObjCode TEAMOB</pre>Ao editar um objeto, você pode substituir todas as regras de acesso em um objeto fazendo um PUT e enviando atualizações semelhantes ao seguinte exemplo:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',accessObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>O exemplo a seguir mostra a sintaxe para mover uma tarefa de um projeto para outro:
<pre>PUT /attask/api/v15.0/task/4c7../move?projectID=5d8..</pre>

## Comportamento DELETE

DELETE remove um objeto. Em cada caso, o URI pode incluir o parâmetro force=true para fazer com que o servidor remova os dados especificados e seus dependentes. No exemplo a seguir, uma tarefa é excluída executando o método DELETE HTTP em um URI:
<pre>DELETE /attask/api/v15.0/task/4c78821c000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c000d6fa8d5e52f07a1d54d0?force=true</pre>

## Atualizações em massa

Uma instrução de atualização em massa atualiza vários objetos ao mesmo tempo em uma única chamada de API. Uma chamada de API de criação em massa é criada de forma semelhante a uma chamada de atualização normal, como mostrado nos exemplos a seguir:
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>que resulte em um retorno semelhante ao seguinte:
<pre>dados: [{<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    name: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    planCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    planStartDate: "2014-08-28T11:00:00:000-0400",<br>    prioridade: 0,<br>    estimatedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    name: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi,<br>    planCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    planStartDate: "2014-08-28T11:00:00:000-0400",<br>    prioridade: 0,<br>    estimatedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>}]</pre>Você também pode fazer uma atualização em massa semelhante ao seguinte:
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx xxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>que resulte em um retorno semelhante ao seguinte:
<pre>dados: [ {<br>     ID: "53ff8e15003b461d4560f7f65a40078",<br>     name: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     planCompletionDate: "2014-08-28T11:00:00:000-0400",<br>     planStartDate: "2014-08-28T11:00:00:000-0400",<br>     prioridade: 0,<br>     estimatedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     status: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    name: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    planCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    planStartDate: "2014-08-28T11:00:00:000-0400",<br>    prioridade: 0,<br>    estimatedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>    status: "CUR"<br>}]</pre>Se quiser que todas as operações aconteçam na mesma transação, adicione "atomic=true" à chamada da API em lote como parâmetro de solicitação. Dessa forma, se alguma das operações falhar, todas as operações foram revertidas.

>[!NOTE]
As operações em lote atômico só podem retornar &quot;success: true&quot; ou um erro.
