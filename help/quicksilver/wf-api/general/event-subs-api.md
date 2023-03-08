---
content-type: api
navigation-topic: general-api
title: API de assinatura de evento
description: API de assinatura de evento
author: Becky
feature: Workfront API
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: e06f6e8ca40da6741982b4ed8c5c53bdbfb253ca
workflow-type: tm+mt
source-wordcount: '2109'
ht-degree: 3%

---


# API de assinatura de evento

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Quando ocorre uma ação em um objeto do Adobe Workfront que é compatível com assinaturas de evento, você pode configurar o Workfront para enviar uma resposta para o endpoint desejado. Isso significa que aplicativos de terceiros podem receber atualizações das interações do Workfront por meio da API do Workfront logo após ocorrerem. Em geral, você pode esperar receber notificações de webhook em menos de 5 segundos a partir da alteração de dados que está sendo registrada. Em média, os clientes recebem notificações de webhook em menos de 1 segundo a partir da alteração de dados que está sendo registrada.  

Para receber payloads de assinatura de evento por meio do firewall, você deve adicionar os seguintes endereços IP à inclui na lista de permissões do:

**Para clientes na Europa:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**Para clientes em locais diferentes da Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

Os seguintes tópicos oferecem suporte à API de assinatura de evento:

## Objetos com Suporte por Assinaturas de Eventos

Os seguintes objetos do Workfront são suportados por assinaturas de evento.

* Atribuição
* Empresa
* Painel de Controle
* Documento
* Despesa
* Hora
* Problema
* Nota
* Portfólio
* Programa
* Projeto
* Relatório
* Tarefa
* Modelo
* Planilha de horas
* Usuário

Para obter uma lista de campos suportados por objetos de assinatura de evento, consulte [Campos de recurso de assinatura do evento](../../wf-api/api/event-sub-resource-fields.md).

## Autenticação de assinatura de evento

Para criar, consultar ou excluir uma assinatura de evento, seu usuário do Workfront precisa do seguinte:

* Um nível de acesso de &quot;Administrador do sistema&quot; é necessário para usar Assinaturas de eventos.
* A `sessionID`  é necessário um cabeçalho para usar a API de Assinaturas de Eventos

   Para obter mais informações, consulte [Autenticação](api-basics.md#authentication) in [Noções básicas sobre API](api-basics.md).

## Formar o recurso de assinatura

O recurso de assinatura contém os seguintes campos.

* objId (opcional)

   * **String** - A ID do objeto do objCode especificado para o qual os eventos são disparados. Se esse campo não for especificado, o usuário receberá eventos para todos os objetos do tipo especificado.

* objCode (obrigatório)

   * **String** - O objCode do objeto que está sendo inscrito para alterações. Os valores possíveis para objCode estão listados na tabela abaixo.

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>Objeto</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">Atribuição</td> 
        <td scope="col"><p>ATRIBUIR</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Empresa </td> 
        <td scope="col"><p>COMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Painel de Controle</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Documento</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Despesa</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Hora</p></td> 
        <td scope="col">HORA</td> 
       </tr> 
       <tr> 
        <td scope="col">Problema</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Nota</td> 
        <td scope="col">Nota</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Portfólio</p></td> 
        <td scope="col"><p>PORTA</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Programa</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Projeto</p></td> 
        <td scope="col"><p>PROJ</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Relatório</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Tarefa</p></td> 
        <td scope="col"><p>TAREFA</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Modelo</p></td> 
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Planilha de horas</td> 
        <td scope="col">FOLHA</td> 
       </tr> 
       <tr> 
        <td scope="col">Usuário</td> 
        <td scope="col">USUÁRIO</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (obrigatório)

   * **String** - Um valor que representa o tipo de evento ao qual o objeto está inscrito. Os tipos de evento disponíveis incluem:

      * CRIAR
      * EXCLUIR 
      * ATUALIZAR

* url (obrigatório)

   * **String** - O URL do endpoint para o qual as cargas do evento de assinatura são enviadas por meio de HTTP.

* authToken (obrigatório)

   * **String** - O token de portador OAuth2 usado para autenticar com o URL especificado no campo &quot;URL&quot;. 

## Criação de solicitações de API de assinatura de evento

Depois de garantir que o usuário tenha acesso de administrador e formar o recurso de assinatura, você estará pronto para criar assinaturas de evento.

Use a sintaxe a seguir para criar o URL.

**URL de solicitação:**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Cabeçalhos de solicitação:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nome do cabeçalho</p> </th> 
   <th> <p>Valor do cabeçalho</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tipo de conteúdo</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valor sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemplo do corpo da solicitação:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

| Código de resposta | Descrição |
|---|---|
| 201 (Criado) | A inscrição no evento foi criada com êxito. |
| 400 (Solicitação inválida) | O campo URL do recurso de assinatura foi considerado inválido. |
| 401 (Não autorizado) | A sessionID fornecida estava vazia ou era considerada inválida. |
| 403 (Proibido) | O usuário que corresponde à sessionID fornecida não tem acesso de administrador. |

Transmitir um recurso de assinatura como o corpo de uma solicitação (com o tipo de conteúdo sendo &quot;application/json&quot;) resulta na criação de uma assinatura de evento para o objeto especificado. Um código de resposta 201 (Criado) indica que a assinatura foi criada. Um código de resposta diferente de 201 significa que a assinatura foi **NOT** criado.

>[!NOTE]
>
> O cabeçalho de resposta &quot;Local&quot; contém o URI da assinatura de evento recém-criada.

**Exemplo de cabeçalhos de resposta:**

| Cabeçalhos de resposta | Exemplo |
|---|---|
| Largura do conteúdo | `→0` |
| Data | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Localização | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Servidor | `→Apache-Coyote/1.1` |

## Consultando Assinaturas de Evento

Ao consultar o HTTP do Workfront, use o método GET. Há duas maneiras de consultar assinaturas de evento: Consultar por ID de assinatura (veja abaixo) ou consultar todas as assinaturas de evento.

### Consultar todas as assinaturas de eventos

É possível consultar todas as assinaturas de eventos para um cliente, conforme especificado pelo valor apiKey. Você também pode usar as seguintes opções para gerenciar a resposta:

* **página**: opção de parâmetro de consulta para especificar o número de páginas a serem retornadas. O padrão é 1.
* **limite**: opção de parâmetro de consulta para especificar o número de resultados a serem retornados por página. O padrão é 100 com um máximo de 1000.

A sintaxe de solicitação para listar todas as assinaturas de evento para um cliente específico é a seguinte:

**URL de solicitação:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Cabeçalhos de solicitação:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nome do cabeçalho</p> </th> 
   <th> <p>Valor do cabeçalho</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valor sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de resposta:**

| Código de resposta | Descrição |
|---|---|
| 200 (OK) | A solicitação retornou com todas as assinaturas de evento encontradas para o cliente que corresponde à sessionID fornecida. |
| 401 (Não autorizado) | A sessionID fornecida estava vazia. |
| 403 (Proibido) | O usuário, que corresponde à sessionID fornecida, não tem acesso de administrador. |


**Exemplo de cabeçalhos de resposta:**

| Cabeçalho de resposta | Exemplo |
|---|---|
| Tipo de conteúdo | `→application/json;charset=UTF-8` |
| Data | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Servidor | `→Apache-Coyote/1.1` |
| Transfer-Encoding | `→chunked` |


**Exemplo de corpo de resposta:**

<!-- [Copy](javascript:void(0);) -->

```
                {
                "subscriptions":                
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": "ObjId1234",
                "objCode": "TASK",
                "url": "http://test.test.net/test/1234",
                "eventType": "UPDATE",
                "authToken": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
                ],
                "meta":
                {
                "page": 1,
                "page_count": 2,
                "limit": 100,
                "total_count": 150
                }
                }            
```

Onde

* **página** e **limite** são os valores fornecidos na solicitação ou o padrão se nenhum valor for fornecido
* **page_count** é o número total de páginas que podem ser consultadas.
* **total_count** é o número total de assinaturas que correspondem à consulta.

### Consulta pela ID de inscrição do evento

Você pode consultar assinaturas de evento pela ID de assinatura de evento. A sintaxe de solicitação para listar assinaturas de evento é a seguinte:

**URL de solicitação:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Cabeçalhos de solicitação:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nome do cabeçalho</p> </th> 
   <th> <p>Valor do cabeçalho</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valor sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de resposta:**

| Código de resposta | Descrição |
|---|---|
| 200 (OK) | A solicitação retornou com a assinatura de evento correspondente à ID de assinatura fornecida. |
| 401 (Não autorizado) | A sessionID fornecida estava vazia. |
| 403 (Proibido) | O usuário, que corresponde à sessionID fornecida, não tem acesso de administrador. |


**Exemplo de corpo de resposta:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
```

## Filtragem de assinatura de evento

A filtragem por assinatura de evento pode ser usada para garantir que você receba apenas mensagens relevantes. Criar filtros para suas assinaturas pode diminuir significativamente o número de mensagens que seu terminal precisa consumir.

Por exemplo, uma variável **ATUALIZAR - TAREFA** a inscrição no evento pode ser definida para acionar somente quando a variável **newState** de uma carga útil do evento define o **taskStatus** as **atual**.

>[!IMPORTANT]
Os seguintes atributos se aplicam à filtragem de assinatura de evento

* Quando um campo de filtro tem um valor não vazio, apenas mensagens com um **newState** contendo as chaves de filtro e os valores são enviados ao URL assinado
* Você pode filtrar pelos dados personalizados incluídos na **newState** E/OU **oldState** do objeto
* Os filtros são avaliados somente se forem iguais ou não a um valor específico
* Se a sintaxe do filtro estiver incorreta ou não corresponder a nenhum dado contido no **newState** da carga, uma mensagem de validação não será retornada para indicar que ocorreu um erro
* Os filtros não podem ser atualizados em uma assinatura existente; uma nova assinatura deve ser criada com novos parâmetros de filtro.
* Vários filtros podem ser aplicados a uma única assinatura, e a assinatura só será entregue quando todas as condições de filtro forem atendidas.
* Aplicar vários filtros a uma única assinatura é uma prática equivalente a usar um **E** operador lógico.
* Várias assinaturas de evento podem ser aplicadas a um único objeto, desde que um ou mais parâmetros de campo de assinatura de evento sejam diferentes em cada assinatura de evento.
* Quando várias assinaturas de evento são atribuídas a um único objeto, todas as assinaturas de evento associadas a esse objeto podem ser retornadas a um único endpoint. Esta prática pode ser usada como um substituto equivalente para o operador lógico **OU** que não podem ser definidas usando parâmetros de filtro.

### Uso de operadores de comparação

Você pode especificar um campo de comparação juntamente com o campo de filtro. Use um operador de comparação neste campo para filtrar por resultados comparativos. Por exemplo, você pode criar uma assinatura UPDATE - TASK que somente envia uma carga se o status da tarefa NÃO for igual ao atual. Você pode usar os seguintes operadores de comparação:

#### eq: equal

Esse filtro permite a entrada de mensagens se a alteração que ocorreu for correspondente `fieldValue` no filtro exatamente. A variável `fieldValue` O valor diferencia maiúsculas de minúsculas.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "eq"
        }
    ]
}
```

#### ne: diferente de

Esse filtro permite a entrada de mensagens se a alteração que ocorreu não corresponder `fieldValue` no filtro exatamente. A variável `fieldValue` O valor diferencia maiúsculas de minúsculas.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "ne"
        }
    ]
}
```

#### gt: maior que

Esse filtro permite a entrada de mensagens se a atualização no `fieldName` é maior que o valor de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gt"
        }
    ]
}
```

#### get: maior que ou igual a

Esse filtro permite a entrada de mensagens se a atualização no `fieldName` é maior que ou igual ao valor de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gte"
        }
    ]
}
```

#### lt: menor que

Esse filtro permite a entrada de mensagens se a atualização no `fieldName` é menor que o valor de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lt"
        }
    ]
}
```

#### lte: menor que ou igual a

Esse filtro permite a entrada de mensagens se a atualização no `fieldName` é menor que ou igual ao valor de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lte"
        }
    ]
}
```

#### contém

Esse filtro permite a entrada de mensagens se a alteração que ocorreu contiver o `fieldValue` no filtro. A variável `fieldValue` o valor diferencia maiúsculas de minúsculas

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        }
    ]
}
```

#### alteração

Esse filtro permite a entrada de mensagens somente se o campo especificado (`fieldName`) tem um valor diferente em oldstate e newstate. Atualização de outros campos além do especificado (`fieldName`) não retornará essa alteração.

>[!NOTE]
`fieldValue` na matriz de filtros abaixo não tem efeito.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "",
            "comparison": "changed"
        }
    ]
}
```

#### state

Esse conector faz com que o filtro se aplique ao novo estado ou ao estado antigo do objeto que foi criado ou atualizado. Isso é útil quando você quer saber onde uma alteração foi feita de algo para outro.
`oldState` não é possível em CREATE `eventTypes`.

>[!NOTE]
A assinatura abaixo com o filtro fornecido só retornará mensagens cujo nome da tarefa contenha `again` no `oldState`, o que era antes de uma atualização ser feita na tarefa.
Um caso de uso para isso seria encontrar as mensagens objCode que mudaram de uma coisa para outra. Por exemplo, para descobrir todas as tarefas que foram alteradas de &quot;Pesquisar algum nome&quot; para &quot;Pesquisar nome da equipe Algum nome&quot;

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains",
            "state": "oldState"
        }
    ]
}
```

### Uso de campos de conector

A variável `filterConnector` no payload da subscrição permite escolher como os filtros devem ser aplicados. O padrão é &quot;E&quot;, onde os filtros devem ser todos `true` para que a mensagem de subscrição seja recebida. Se &quot;OR&quot; for especificado, somente um filtro deverá corresponder para que a mensagem de subscrição seja recebida.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        },
        {
            "fieldName": "name",
            "fieldValue": "also",
            "comparison": "contains"
        }
    ],
    "filterConnector": "AND"
}
```

## Exclusão de Assinaturas de Eventos

Ao excluir o HTTP do Workfront, use o método DELETE. A sintaxe de solicitação para excluir uma única assinatura de evento por ID de assinatura é a seguinte:

**URL de solicitação:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Cabeçalhos de solicitação:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nome do cabeçalho</p> </th> 
   <th> <p>Valor do cabeçalho</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> valor sessionID </p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de resposta:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Código de resposta</p> </th> 
   <th> Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (Sem conteúdo)</td> 
   <td>O servidor removeu com êxito a inscrição de evento correspondente à subscriptionID fornecida.</td> 
  </tr> 
  <tr> 
   <td>401 (Não autorizado)</td> 
   <td>A sessionID fornecida estava vazia.</td> 
  </tr> 
  <tr> 
   <td>403 (Proibido)</td> 
   <td>O usuário que corresponde à sessionID fornecida não tem acesso de administrador.</td> 
  </tr> 
  <tr> 
   <td>404 (Não encontrado)</td> 
   <td>O servidor não pôde localizar uma assinatura de evento correspondente à subscriptionID fornecida para exclusão.</td> 
  </tr> 
 </tbody> 
</table>

**Exemplo de cabeçalhos de resposta:**

| Cabeçalho de resposta | Exemplo |
|---|---|
| Data | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Servidor | `→Apache-Coyote/1.1` |


**Exemplo de corpo de resposta:** N/D

## Exemplos de payloads de evento

A carga útil que um usuário recebe varia dependendo do tipo de objeto, mas há um formato consistente para o qual essas cargas úteis variáveis são entregues.

Por exemplo, as seguintes propriedades permanecem consistentes em todas as cargas do evento:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Embora consistentes no formato, os valores contidos nas propriedades variam entre diferentes objetos e tipos de objeto.

Amostras de cargas para um evento UPDATE e um evento CREATE são mostradas abaixo. Observe que no exemplo UPDATE os objetos oldState e newState são iguais, enquanto no exemplo CREATE o objeto oldState está vazio (não NULL).

Veja a seguir um exemplo de carga para um evento UPDATE:

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "newState": {
                "ID": "59d7ddf7000002322d791eb08bafddfb", 
                       "name": "EventSub Test updated",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,       "categoryID": null,
                      "status": "CUR",
                      "parameterValues": {}
                   },
                   "oldState": {
                       "ID": "59d7ddf7000002322d791eb08bafddfb",
                       "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,<
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,
                       "categoryID": null,
                       "status": "CUR",
                       "parameterValues": {}
                   }
                }
```

Veja a seguir um exemplo de carga para um evento CREATE:

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "newState": {
                "ID": "59caa946000000e07b0afc3383230c67",
                "name": "EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c",
                "objCode": "PROJ",
                "entryDate": "2017-09-26T13:23:50.746-0600",
                "accessorIDs": ["544820df0000142362741fc0c368de19"],
                "lastUpdateDate": "2017-09-26T13:23:50.927-0600",
                "groupID": "544820df0000140f6a9c1faa7cacadd3",
                "sponsorID": null,
                "description": null,
                "plannedCompletionDate": "2017-09-26T09:00:00.000-0600",
                "enteredByID": "544820df0000142362741fc0c368de19",
                "ownerID": "544820df0000142362741fc0c368de19",
                "templateID": null,
                "priority": 0,
                "companyID": null,
                "portfolioID": null,
                "referenceNumber": 1750,
                "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                "customerID": "544820df0000135b7719dcca654391f6",
                "currency": null,
                "categoryID": null,
                "status": "CUR",
                "parameterValues": {}
                },
                "oldState": {}
            }
```

## Codificação de base 64

Se uma assinatura de evento estiver sendo rejeitada devido a um conflito entre os caracteres especiais contidos nas assinaturas de evento e as configurações de rede, você poderá usar a codificação Base64 para enviar as assinaturas de evento. Base64 é um conjunto de esquemas de codificação que podem traduzir quaisquer dados arbitrários em um formato de string ASCII. É importante observar que Base64 não é uma forma de criptografia de segurança.

### Campo de codificação de base 64

O campo base64Encoding é um campo opcional usado para habilitar a codificação Base64 de cargas de assinatura de evento. O valor padrão é false e os valores possíveis são: true, false e &quot; &quot; (em branco).

### Exemplo de uma solicitação usando o campo base64Encoding

Se uma solicitação for feita usando o campo base64Encoding definido como true, o campo **newState** e **oldState** os objetos na carga são entregues como strings de codificação de base 64. Se o campo base64Encoding for definido como false, deixado em branco ou não incluído na solicitação, a carga retornada não será codificada na base 64.

Este é um exemplo de uma solicitação que usa o campo base64Encoding:

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua"",
                "authToken": "EauthTokenWorkfrontRocks1234_",
                "base64Encoding": "true"
            }
```

### Exemplos de cargas de resposta na codificação de base 64

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Método obsoleto para consultar todas as assinaturas de evento

O endpoint da API a seguir está obsoleto e não deve ser usado para novas implementações. Também recomendamos a transição de implementações antigas para o método no **Consultando Assinaturas de Evento** descrito acima.

É possível consultar todas as assinaturas de evento para um cliente, conforme especificado pelo valor sessionID. A sintaxe de solicitação para listar todas as assinaturas de evento para um cliente específico é o seguinte URL:

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**Cabeçalhos de solicitação:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nome do cabeçalho</p> </th> 
   <th> <p>Valor do cabeçalho</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> valor sessionID </p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de resposta:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Código de resposta</p> </th> 
   <th> Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (Sem conteúdo)</td> 
   <td>A solicitação retornou com êxito todas as assinaturas de evento encontradas para o usuário.</td> 
  </tr> 
  <tr> 
   <td>401 (Não autorizado)</td> 
   <td>A sessionID fornecida estava vazia.</td> 
  </tr> 
  <tr> 
   <td>403 (Proibido)</td> 
   <td>O usuário que corresponde à sessionID fornecida não tem acesso de administrador.</td> 
  </tr> 
 </tbody> 
</table>

 

### Exemplo de Corpo de Resposta

<!-- [Copy](javascript:void(0);) -->

```
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customer_id": "504f9640000013401be513579fbebffa",
                "obj_id": "ObjId1234",
                "obj_code": "TASK",
                "url": "http://test.test.net/test/1234",
                "event_type": "UPDATE",
                "auth_token": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customer_d": "504f9640000013401be513579fbebffa",
                "obj_id": null,
                "obj_code": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "event_type": "UPDATE",
                "auth_token": "authTokenWorkfrontRocks1234_"
                }                
                ]
```
