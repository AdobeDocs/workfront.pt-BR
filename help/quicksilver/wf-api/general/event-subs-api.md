---
content-type: api
navigation-topic: general-api
title: API de Assinatura de evento
description: API de Assinatura de evento
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: 159c3b4a3627e29123afd96115e965d3bba8329c
workflow-type: tm+mt
source-wordcount: '3387'
ht-degree: 93%

---


# API de Assinatura de evento

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Quando ocorre uma ação em um objeto do Adobe Workfront que é compatível com assinaturas de evento, você pode configurar o Workfront para enviar uma resposta para o ponto de acesso desejado. Isso significa que aplicativos de terceiros podem receber atualizações das interações do Workfront por meio da API do Workfront, logo após ocorrerem. Em geral, você pode esperar receber notificações de webhook em menos de 5 segundos após a alteração de dados que está sendo registrada. Em média, clientes recebem notificações de webhook em menos de 1 segundo após a alteração de dados que está sendo registrada.

Como as assinaturas de evento enviam dados para outro serviço, elas são gerenciadas por meio de comandos, não pelo aplicativo do Workfront.

Para receber conteúdos de assinaturas de evento por meio do firewall, você deve adicionar os seguintes endereços IP à lista de permissões:

**Para clientes na Europa:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**Para clientes fora da Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

Os seguintes tópicos servem de auxílio para a API de Assinatura de evento:

## Objetos compatíveis com assinaturas de evento

Os seguintes objetos do Workfront são compatíveis com assinaturas de evento.

* Aprovação
* Estágio de aprovação
* Participante do estágio de aprovação
* Atribuição
* Empresa
* Painel
* Documento
* Versão do documento
* Despesa
* Campo
* Hora
* Problema
* Nota
* Portfólio
* Programa
* Projeto
* Aprovação da prova
* Registro
* Tipo de registro
* Relatório
* Plano de recrutamento
* Valor do parâmetro do plano de recrutamento
* Recurso do plano de recrutamento
* Valor do atributo de recurso do plano de recrutamento
* Conjunto de valores de atributo de recurso do plano de recrutamento
* Valor do parâmetro de recurso do plano de recrutamento
* Tarefa
* Modelo
* Folha de horas
* Usuário
* Espaço de trabalho

>[!NOTE]
>
>Para obter uma lista de campos compatíveis com objetos de assinatura de evento, consulte [Campos de recursos de assinatura de evento](../../wf-api/api/event-sub-resource-fields.md).

## Autenticação da assinatura de evento

Para criar, consultar ou excluir uma assinatura de evento, o usuário do Workfront precisa do seguinte:

* Um nível de acesso de “Admin do sistema” é exigido para usar assinaturas de evento.
* Um cabeçalho `sessionID` é exigido para usar a API de assinaturas de evento

  Para obter mais informações, consulte [Autenticação](api-basics.md#authentication) em [Noções básicas sobre API](api-basics.md).

## Evitar sobrecarregar as assinaturas de evento

O serviço de assinatura de evento foi projetado para fornecer entrega confiável de eventos para todos os usuários. Para garantir isso, foram implementadas proteções para evitar uma produção excessiva de eventos por parte de um mesmo usuário, o que poderia causar possíveis problemas de qualidade do serviço para todos os usuários. Como resultado, um usuário que está produzindo eventos demais em um curto período de tempo pode enfrentar sandboxing e atrasos de entrega de eventos.

## Formar o recurso de assinatura

O recurso de assinatura contém os seguintes campos.

* objId (opcional)

   * **String** — A identificação do objeto do objCode especificado para o qual os eventos são disparados. Se esse campo não for especificado, o usuário receberá eventos para todos os objetos do tipo especificado.

* objCode (exigido)

   * **String** — O objCode do objeto que está sendo assinado para alterações. Os valores possíveis para objCode estão listados na tabela abaixo.

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
        <td scope="col">Aprovação</td> 
        <td scope="col"><p>aprovação</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Estágio de aprovação</td> 
        <td scope="col"><p>approval_stage</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Participante do estágio de aprovação</td> 
        <td scope="col"><p>approval_stage_participant</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Atribuição</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Empresa </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Painel</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Documento</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Versão do documento</p></td> 
        <td scope="col">DOCV </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Despesa</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Campo</p></td> 
        <td scope="col"><p>CAMPO</p></td> 
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
        <td scope="col">NOTA</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Portfólio</p></td> 
        <td scope="col"><p>PORT</p></td> 
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
        <td scope="col"><p>Aprovação da prova</p></td> 
        <td scope="col"><p>PRFAPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Registro</p></td> 
        <td scope="col"><p>REGISTRO</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Tipo de registro</p></td> 
        <td scope="col"><p>RECORD_TYPE</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Relatório</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Plano de recrutamento</p></td> 
        <td scope="col"><p>STAFFP</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Valor do parâmetro do plano de recrutamento</p></td> 
        <td scope="col"><p>SPVAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Recurso do plano de recrutamento</p></td> 
        <td scope="col"><p>STAFFR</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Valor do atributo de recurso do plano de recrutamento</p></td> 
        <td scope="col"><p>SPAVAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Conjunto de valores de atributo de recurso do plano de recrutamento</p></td> 
        <td scope="col"><p>SAVSET</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Valor do parâmetro de recurso do plano de recrutamento</p></td> 
        <td scope="col"><p>SRPVAL</p></td> 
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
        <td scope="col">Folha de horas</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">Usuário</td> 
        <td scope="col">USUÁRIO</td> 
       </tr> 
       <tr> 
        <td scope="col">Espaço de trabalho</td> 
        <td scope="col">ESPAÇO DE TRABALHO</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (exigido)

   * **String** — Um valor que representa o tipo de evento ao qual o objeto está assinado. Os tipos de evento disponíveis incluem:

      * CREATE
      * EXCLUIR
      * UPDATE

* url (exigido)

   * **String** — A URL do ponto de acesso para a qual os conteúdos do evento de assinatura são enviados via HTTP.

* authToken (exigido)

   * **String** — O token do portador OAuth2 usado para a autenticação com a URL especificada no campo &quot;URL&quot;.

## Criação de solicitações de API de assinatura de evento

Depois de garantir que o usuário tenha acesso de administrador e formar o recurso de assinatura, você está com tudo pronto para criar assinaturas de evento.

Use a sintaxe a seguir para criar o URL.

**URL da solicitação**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Cabeçalhos da solicitação**

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
   <td> <p>content-type</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valor sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemplo de corpo da solicitação:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

**Exemplo de corpo de resposta**

```
{
    "id": <NEW SUBSCRIPTION ID>,
    "version": <NEW SUBSCRIPTION VERSION>
}
```

| Código de resposta | Descrição |
|---|---|
| 201 (criado) | A assinatura de evento foi criada com sucesso. |
| 400 (solicitação inválida) | O campo de URL do recurso de assinatura foi considerado inválido. |
| 401 (não autorizado) | A sessionID fornecida estava vazia ou foi considerada inválida. |
| 403 (proibido) | O usuário que corresponde à sessionID fornecida não tem acesso de administrador. |

Transmitir um recurso de assinatura como o corpo de uma solicitação (com content-type sendo &quot;application/json&quot;) resulta na criação de uma assinatura de evento para o objeto especificado. Um código de resposta 201 (criado) indica que a assinatura foi criada. Um código de resposta diferente de 201 significa que a assinatura **NÃO** foi criada.

>[!NOTE]
>
> O cabeçalho de resposta &quot;Local&quot; contém o URI da assinatura de evento recém-criada.

**Exemplo de cabeçalhos de resposta:**

| Cabeçalhos de resposta | Exemplo |
|---|---|
| Tamanho do conteúdo | `→0` |
| Data | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Localização | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Servidor | `→Apache-Coyote/1.1` |

## Consulta de assinaturas de evento

Ao consultar o HTTP do Workfront, use o método GET. Há duas maneiras de consultar assinaturas de evento: consultar por ID de assinatura (veja abaixo) ou consultar todas as assinaturas de evento.

### Consultar todas as assinaturas de evento

Você pode consultar todas as assinaturas de evento para um cliente ou usar o seguinte para gerenciar a resposta. Você também pode usar as seguintes opções para gerenciar a resposta:

* **página**: opção de parâmetro de consulta para especificar o número de páginas a serem retornadas. O valor padrão é 1.
* **limite**: opção de parâmetro de consulta para especificar o número de resultados a serem retornados por página. O padrão é 100, com um máximo de 1000.

A sintaxe de solicitação para listar todas as assinaturas de evento para um cliente específico é a seguinte:

**URL da solicitação**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Cabeçalhos da solicitação:**

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

**Códigos de resposta**

| Código de resposta | Descrição |
|---|---|
| 200 (OK) | A solicitação retornou com todas as assinaturas de evento encontradas para o cliente que corresponde à sessionID fornecida. |
| 401 (não autorizado) | A sessionID fornecida estava vazia. |
| 403 (proibido) | O usuário que corresponde à sessionID fornecida não tem acesso de administrador. |


**Exemplo de cabeçalhos de resposta**

| Cabeçalho de resposta | Exemplo |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| Data | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Servidor | `→Apache-Coyote/1.1` |
| Transfer-Encoding | `→chunked` |


**Exemplo de corpo de resposta**

```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```

Onde

* **page** e **limit** são os valores fornecidos na solicitação, ou o padrão se nenhum valor for fornecido
* **page_count** é o número total de páginas que podem ser consultadas.
* **total_count** é o número total de assinaturas que correspondem à consulta.

### Consulta por ID de assinatura de evento

Você pode consultar assinaturas de evento pela ID de assinatura de evento. A sintaxe da solicitação para listar assinaturas de evento é a seguinte:

**URL da solicitação**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Cabeçalhos da solicitação**

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

**Códigos de resposta**

| Código de resposta | Descrição |
|---|---|
| 200 (OK) | A solicitação retornou com a assinatura de evento correspondente à ID de assinatura fornecida. |
| 401 (não autorizado) | A sessionID fornecida estava vazia. |
| 403 (proibido) | O usuário que corresponde à sessionID fornecida não tem acesso de administrador. |


**Exemplo de corpo de resposta**



```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```


## Controle de versão da assinatura de evento

O Workfront tem duas versões de assinaturas de evento.

A capacidade de atualizar ou fazer downgrade de assinaturas de evento garante que, quando alterações forem feitas na estrutura dos eventos, as assinaturas existentes não sejam interrompidas, permitindo testar e atualizar para a nova versão sem uma lacuna na assinatura do evento.

Para obter mais informações sobre o controle de versão de assinaturas de evento, incluindo diferenças específicas entre a versão e datas importantes, consulte [Controle de versão de assinaturas de evento](/help/quicksilver/wf-api/general/event-subs-versioning.md).

>[!NOTE]
>
>Ao atualizar ou fazer downgrade da assinatura de evento para outra versão, você recebe eventos duplicados para cada entrega de evento por uma janela de cinco minutos após a alteração da versão. Os duplicados incluem um de cada versão da assinatura de eventos: versão 1 e versão 2. Isso garante que você não perca nenhum evento devido à alteração da versão de assinatura do evento.

### Alteração de versão de assinatura única

A sintaxe de solicitação para alterar a versão de uma única assinatura é:

**URL da solicitação**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>/version 
```

**Exemplo de corpo de solicitação**

```
{
    "version": "v2" 
}
```


**Exemplo de corpo de resposta (200)**

```
{
    "id": <SUBSCRIPTION ID>,
    "version": "v2" 
}
```

**Códigos de resposta possíveis**

* 200
* 400
* 404


### Alteração de versão de assinatura múltipla

Esse ponto de acesso altera a versão de várias assinaturas, por lista de assinaturas ou pelo sinalizador de todas as assinaturas do cliente.

A sintaxe de solicitação para alterar a versão de uma única assinatura é:

**URL da solicitação**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/version
```

**Exemplo de corpos de solicitação**

* Corpo da solicitação para a lista de assinaturas

  ```
  {
      "subscriptionIds": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>],
      "version": "v2" 
  }
  ```

* Corpo da solicitação para todas as assinaturas do cliente

  ```
  {
      "allCustomerSubscriptions": true,
      "version": "v2" 
  }
  ```

**Exemplo de corpo de resposta (200)**

```
{
    "subscription_ids": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>, ...],
    "version": "v2" 
}
```

**Códigos de resposta possíveis**

* 200
* 400

## Filtragem de assinatura de evento

Você pode usar a filtragem de assinatura de evento para garantir que receba apenas mensagens relevantes. Criar filtros para as assinaturas pode diminuir significativamente o número de mensagens que o ponto de acesso precisa consumir.

Por exemplo, uma assinatura de evento **UPDATE - TASK** pode ser definida para disparar somente quando o **newState** de um conteúdo de evento define o **taskStatus** como **current**.

>[!IMPORTANT]
>
>Os seguintes atributos se aplicam à filtragem de assinatura de evento

* Quando um campo de filtro tem um valor não vazio, somente as mensagens com um **newState** contendo as chaves e os valores do filtro serão enviadas para a URL assinada
* Você pode filtrar pelos dados personalizados incluídos no **newState** E/OU no **oldState** do objeto
* Os filtros são avaliados exclusivamente com base em serem ou não iguais a um valor específico
* Se a sintaxe do filtro estiver incorreta ou não corresponder aos dados contidos no **newState** da carga, uma mensagem de validação não será retornada para indicar que ocorreu um erro
* Os filtros não podem ser atualizados em uma assinatura já existente. Uma nova assinatura deve ser criada com novos parâmetros de filtro.
* Vários filtros podem ser aplicados a uma única assinatura, que será entregue apenas quando todas as condições de filtro forem atendidas.
* Aplicar vários filtros a uma única assinatura é uma prática equivalente ao uso de um operador lógico **AND**.
* Várias assinaturas de evento podem ser aplicadas a um único objeto, desde que um ou mais parâmetros de campo de assinatura de evento sejam diferentes em cada assinatura de evento.
* Quando várias assinaturas de evento forem atribuídas a um único objeto, todas as assinaturas de evento associadas a esse objeto poderão ser retornadas a um único ponto de acesso. Essa prática pode ser usada como um substituto equivalente para o operador lógico **OR**, que não pode ser definido usando parâmetros de filtro.
* Os seguintes campos não são filtráveis:

   * DOCU.groups
   * RECORD.data
   * RECORD_TYPE.data
   * RECORD_TYPE.fields

### Uso de operadores de comparação

Você pode especificar um campo de comparação juntamente com o campo de filtro. Use um operador de comparação nesse campo para filtrar por resultados comparativos. Por exemplo, você pode criar uma assinatura UPDATE - TASK que envia um conteúdo somente se o status da tarefa NÃO for igual ao atual. Você pode usar os seguintes operadores de comparação:

#### eq: igual

Esse filtro permite a entrada das mensagens se a alteração que ocorreu corresponder exatamente a `fieldValue` no filtro. O valor `fieldValue` diferencia entre maiúsculas e minúsculas.

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

#### ne: não é igual

Esse filtro permite a entrada das mensagens se a alteração que ocorreu não corresponder exatamente a `fieldValue` no filtro. O valor `fieldValue` diferencia entre maiúsculas e minúsculas.

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

Esse filtro permite a entrada das mensagens se a atualização no `fieldName` especificado for maior que o valor de `fieldValue`.

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

#### gte: é maior ou igual a

Esse filtro permite a entrada das mensagens se a atualização no `fieldName` especificado for maior ou igual ao valor de `fieldValue`.

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

Esse filtro permite a entrada das mensagens se a atualização no `fieldName` especificado for menor que o valor de `fieldValue`.

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

#### let: é menor ou igual a

Esse filtro permite a entrada de mensagens se a atualização no `fieldName` especificado for menor ou igual ao valor de `fieldValue`.

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

#### contains

Esse filtro permite a entrada das mensagens se a alteração que ocorreu contiver o `fieldValue` no filtro. O valor `fieldValue` diferencia entre maiúsculas e minúsculas

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

#### containsOnly

Esse filtro permite a entrada das mensagens somente quando o conjunto completo de valores selecionados corresponde exatamente a fieldValue no filtro, independentemente da ordem. Não deve haver valores extras ou ausentes.

>[!NOTE]
>
>Usado para campos do tipo matriz (seleção múltipla). O exemplo de assinatura abaixo permite o envio de mensagens somente quando o campo `groups` contém exatamente &quot;Escolha 3&quot; e &quot;Escolha 4&quot;, sem valores adicionais ou ausentes e independentemente da ordem. Se uma string ou um número inteiro for especificado em `fieldValue`, em vez de em uma matriz, a assinatura permitirá que as mensagens sejam enviadas apenas quando o campo `groups` contiver exatamente uma única opção e esta corresponder exatamente à string ou ao número inteiro especificado em `fieldValue`&quot;


```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": [
                "Choice 3",
                "Choice 4"
            ],
            "state": "newState",
            "comparison": "containsOnly"
        }
    ]
}
```

#### notContains

Esse filtro permite a entrada das mensagens somente quando o campo especificado (`fieldName`) não contiver o valor especificado (`fieldValue`).

>[!NOTE]
>
>Usado para campos do tipo matriz (seleção múltipla) ou string. Se o campo for uma string, verificaremos se o valor especificado não está contido na string (por exemplo, &quot;Novo&quot; não está na string &quot;Projeto - Atualizado&quot;). Se o campo for uma matriz e o valor do campo especificado for uma string ou um número inteiro, verificaremos se a matriz não contém o valor especificado (por exemplo, &quot;Opção 1&quot; não está na [&quot;Opção 2&quot;, &quot;Opção 3&quot;]). O exemplo de assinatura abaixo permite o envio de mensagens somente quando os campos `groups` não contêm a string &quot;Grupo 2&quot;.

```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": "Group 2",
            "state": "newState",
            "comparison": "notContains"
        }
    ]
}
```

#### alteração

Esse filtro permite a entrada das mensagens somente se o campo especificado (`fieldName`) tiver um valor diferente em oldstate e newstate. Atualizar outros campos além do especificado (`fieldName`) não retornará essa alteração.

>[!NOTE]
>
>`fieldValue` na matriz de filtros abaixo não tem efeito.

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

#### estado

Esse conector faz com que o filtro se aplique ao novo estado ou ao estado antigo do objeto que foi criado ou atualizado. Isso é útil quando você quer saber de onde uma alteração foi feita.
`oldState` não é possível em CREATE `eventTypes`.

>[!NOTE]
>
>A assinatura abaixo com o filtro fornecido só retornará mensagens em que o nome da tarefa contém `again` no `oldState`, como era antes de uma atualização ser feita na tarefa.
>Um caso de uso seria encontrar as mensagens objCode que mudaram de uma coisa para outra. Por exemplo, para descobrir todas as tarefas que foram alteradas de &quot;Pesquisar algum nome&quot; para &quot;Pesquisar algum nome de equipe&quot;

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

### Uso de filtros aninhados

A Assinatura de evento é compatível com filtragem em campos aninhados de eventos, usando os nomes de campos aninhados. Por exemplo, para filtrar uma mensagem em que `newState.data.customField1 = 'myCustomFieldValue'`, a seguinte assinatura com filtro pode ser criada:

```
{
    "objCode": "RECORD",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedRecords",
    "filters": [
        {
            "fieldName": "data",
            "fieldValue": {
                    "customField1": "myCustomFieldValue"
            },
            "comparison": "eq",
            "state": "newState"
        }
    ]
}
```

Filtros duplamente aninhados também podem ser endereçados.

```
"filters": [
    {
        "fieldName": "data",
        "fieldValue": {
            "fields": {
                "children": {
                    "customerId":"customer1234",
                    "name":"New Campaign"
                }
            }
        },
        "comparison": "eq",
        "state": "newState"
    }
],
"filterConnector": 'AND'
```

### Utilização de grupos de filtros (filtros de combinação)

As assinaturas de evento são compatíveis com grupos de filtros, juntamente com filtros padrão, para oferecer suporte a condições lógicas aninhadas.

Os grupos de filtros permitem criar condições lógicas aninhadas (AND/OR) nos filtros de subscrição do evento.

Cada grupo de filtros pode ter:

* Seu próprio conector: `AND` ou `OR`
* Vários filtros, cada um seguindo a mesma sintaxe e comportamento que os filtros independentes

Todos os filtros dentro de um grupo são compatíveis:

* Operadores de comparação: `eq`, `ne`, `gt`, `gte`, `lt`, `lte`, `contains`, `notContains`, `containsOnly`, `changed`
* Opções de estado: `newState`, `oldState`
* Direcionamento de campo: qualquer nome de campo de objeto válido

Um grupo deve conter no mínimo 2 filtros

```
{
  "objCode": "TASK",
  "eventType": "UPDATE",
  "authToken": "token",
  "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
  "filters": [
    {
      "fieldName": "percentComplete",
      "fieldValue": "100",
      "comparison": "lt"
    },
    {
      "type": "group",
      "connector": "OR",
      "filters": [
        {
          "fieldName": "status",
          "fieldValue": "CUR",
          "comparison": "eq"
        },
        {
          "fieldName": "priority",
          "fieldValue": "1",
          "comparison": "eq"
        }
      ]
    }
  ],
  "filterConnector": "AND"
}
```

Este exemplo mostra:


* Filtro de nível superior (fora do grupo):

  `fieldName`: `percentComplete`, `fieldValue`: `100`, `comparison`: `lt`

  Esse filtro verifica se o campo percentComplete da tarefa atualizada é menor que 100.

* Grupo de Filtros (filtros aninhados com `OR`):

  { &quot;`type`&quot;: &quot;`group`&quot;, &quot;`connector`&quot;: &quot;`OR`&quot;, &quot;`filters`&quot;: [{ &quot;`fieldName`&quot;: &quot;`status`&quot;, &quot;`fieldValue`&quot;: &quot;`CUR`&quot;, &quot;`comparison`&quot;: &quot;`eq`&quot; }, { &quot;`fieldName`&quot;: &quot;`priority`&quot;, &quot;`fieldValue`&quot;: &quot;`1`&quot;, &quot;`comparison`&quot;: &quot;`eq`&quot; }] }

  Esse grupo avalia dois filtros internos:

   * O primeiro verifica se o status da tarefa é igual a &quot;CUR&quot; (atual).

   * O segundo verifica se a prioridade é igual a &quot;1&quot; (alta prioridade).

  Como o conector é &quot;OR&quot;, esse grupo será aprovado se qualquer uma das condições for verdadeira.

* Conector de Nível Superior (filterConnector: `AND`):

  O conector mais externo entre os filtros de nível superior é `AND`.

  Isso significa que o filtro de nível superior e o grupo devem passar para que o evento corresponda.

* A assinatura é acionada quando:

  O percentual de Término é inferior a 100

  E

  O status é &quot;CUR&quot; OU a prioridade é &quot;1&quot;.

#### Desempenho e limites

Para garantir desempenho e capacidade de manutenção consistentes:

* Cada assinatura suporta até 10 grupos de filtros (cada grupo contendo vários filtros).
* Cada grupo de filtros pode incluir até 5 filtros para evitar uma possível degradação do desempenho durante o processamento de eventos.
* Embora haja suporte para até 10 grupos de filtros (cada um com 5 filtros), observe que um grande número de assinaturas ativas com lógica de filtro complexa pode resultar em um atraso durante a avaliação do evento.

Se você ultrapassar esses limites, considere simplificar sua lógica ou dividir a assinatura em várias menores.

### Uso de campos de conector

O campo `filterConnector` no conteúdo da assinatura permite escolher como os filtros devem ser aplicados. O padrão é &quot;AND&quot;, em que os filtros devem ser `true` para que a mensagem de assinatura seja recebida. Se &quot;OR&quot; for especificado, somente um filtro deverá corresponder para que a mensagem de assinatura passe.

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

### Uso de grupos de filtros

Os grupos de filtros permitem criar condições lógicas (AND/OR) aninhadas nos filtros de assinatura de evento.

Cada grupo de filtros pode ter o seguinte:

* O próprio conector (AND ou OR).
* Vários filtros, cada um seguindo a mesma sintaxe e comportamento como filtros independentes.

>[!IMPORTANT]
>
>Um grupo deve ter no mínimo dois filtros.


Todos os filtros dentro de um grupo são compatíveis com o seguinte:

* Operadores de comparação: eq, ne, gt, gte, lt, lte, contains, notContains, containsOnly, changed.
* Opções de estado: newState, oldState.
* Direcionamento de campo: qualquer nome de campo de objeto válido.

```
{
  "objCode": "TASK",
  "eventType": "UPDATE",
  "authToken": "token",
  "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
  "filters": [
    {
      "fieldName": "percentComplete",
      "fieldValue": "100",
      "comparison": "lt"
    },
    {
      "type": "group",
      "connector": "OR",
      "filters": [
        {
          "fieldName": "status",
          "fieldValue": "CUR",
          "comparison": "eq"
        },
        {
          "fieldName": "priority",
          "fieldValue": "1",
          "comparison": "eq"
        }
      ]
    }
  ],
  "filterConnector": "AND"
}
```

O exemplo acima contém os seguintes componentes:

1. O filtro de nível superior (fora do grupo):

   * `{ "fieldName": "percentComplete", "fieldValue": "100", "comparison": "lt" }`
   * Esse filtro verifica se o campo percentComplete da tarefa atualizada é menor que 100.

1. Grupo de filtros (filtros aninhados com OR):

   * `{ "type": "group", "connector": "OR", "filters": [ { "fieldName": "status", "fieldValue": "CUR", "comparison": "eq" }, { "fieldName": "priority", "fieldValue": "1", "comparison": "eq" } ] }`
   * Esse grupo avalia dois filtros internos:

      * O primeiro verifica se o status da tarefa é igual a &quot;CUR&quot; (atual).
      * O segundo verifica se a prioridade é igual a &quot;1&quot; (alta prioridade).
   * Como o conector é &quot;OR&quot;, esse grupo será aprovado se qualquer uma das condições for verdadeira.

1. Conector de nível superior (filterConnector: AND):
   * O conector mais externo entre os filtros de nível superior é &quot;AND&quot;. Isso significa que o filtro de nível superior e o grupo devem passar para que o evento corresponda.

1. A assinatura será acionada quando as seguintes condições forem atendidas:
   * A percentComplete é menor que 100.
   * O status é &quot;CUR&quot; ou a prioridade é &quot;1&quot;.

>[!NOTE]
>
>Existem limites para garantir um desempenho consistente do sistema ao usar grupos de filtros, que incluem o seguinte:
>
>* Cada assinatura suporta até 10 grupos de filtros (cada grupo contendo vários filtros).
>* Cada grupo de filtros pode incluir até 5 filtros para evitar uma possível degradação do desempenho durante o processamento de eventos.
>* Embora seja possível ter até 10 grupos de filtros (cada um com 5 filtros), um grande número de assinaturas ativas com lógica de filtro complexa pode resultar em um atraso durante a avaliação do evento.

## Exclusão de assinaturas de eventos

Ao excluir o HTTP do Workfront, use o método DELETE. A sintaxe da solicitação para excluir uma única assinatura de evento por ID de assinatura é a seguinte:

**Solicitar URL:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Solicitar Cabeçalhos:**

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

**Códigos de Resposta:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Código de resposta</p> </th> 
   <th> Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (Sem conteúdo)</td> 
   <td>O servidor removeu com sucesso a assinatura do evento correspondente ao subscriptionID fornecido.</td> 
  </tr> 
  <tr> 
   <td>401 (não autorizado)</td> 
   <td>A sessionID fornecida estava vazia.</td> 
  </tr> 
  <tr> 
   <td>403 (proibido)</td> 
   <td>O usuário que corresponde à sessionID fornecida não tem acesso de administrador.</td> 
  </tr> 
  <tr> 
   <td>404 (Não encontrado)</td> 
   <td>O servidor não pôde localizar uma assinatura de evento correspondente à subscriptionID fornecida para exclusão.</td> 
  </tr> 
 </tbody> 
</table>

**Exemplo de Cabeçalhos de Resposta:**

| Cabeçalho de resposta | Exemplo |
|---|---|
| Data | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Servidor | `→Apache-Coyote/1.1` |


**Exemplo de corpo de resposta:** N/D

## Exemplos de conteúdos de evento

O conteúdo que um usuário recebe varia dependendo do tipo de objeto, mas existe um formato consistente para o qual esses conteúdos variáveis são entregues.

Por exemplo, as seguintes propriedades permanecem consistentes em todos os conteúdos de eventos:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Embora consistentes em formato, os valores contidos nas propriedades variam entre diferentes objetos e tipos de objetos.

Exemplos dos conteúdos evento UPDATE, e evento CREATE são mostrados abaixo Observe que, no exemplo de UPDATE, os objetos oldState e newState são iguais, enquanto, no exemplo de CREATE, o objeto oldState está vazio (não NULL).

A seguir, um exemplo de conteúdo para um evento de UPDATE:

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "eventVersion": "v2",
                   "subscriptionVersion": "v2",
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

A seguir, um exemplo de conteúdo para um evento de CREATE:

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
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

## Codificação Base64

Se uma assinatura de evento estiver sendo rejeitada devido a um conflito entre caracteres especiais contidos em suas assinaturas de evento e suas configurações de rede, você poderá usar a codificação Base64 para passar suas assinaturas de evento. Base64 é um conjunto de esquemas de codificação que pode traduzir qualquer dado arbitrário para o formato de string ASCII. É importante observar que Base64 não é uma forma de criptografia de segurança.

### Campo de Codificação Base64

O campo base64Encoding é um campo opcional usado para habilitar a codificação Base64 de conteúdos de assinaturas de eventos. O valor padrão é falso, e os valores possíveis são: verdadeiro, falso e &quot; &quot; (em branco).

### Exemplo de uma solicitação usando o campo base64Encoding

Se uma solicitação for feita usando o campo base64Encoding definido como verdadeiro, os objetos **newState** e **oldState** no conteúdo serão entregues como strings codificadas em Base64. Se o campo base64Encoding for definido como falso, deixado em branco ou não incluído na solicitação, o conteúdo retornado não será codificado em Base64.

A seguir está um exemplo de uma solicitação que usa o campo base64Encoding:

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

### Exemplos de conteúdos de resposta em codificação Base64

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Método obsoleto para consultar todas as assinaturas de eventos

O seguinte ponto de acesso da API está obsoleto e não deve ser usado para novas implementações. Também recomendamos a transição de implementações antigas para o método na seção **Consulta de assinaturas de eventos** descrita acima.

É possível consultar todas as assinaturas de evento para um cliente, conforme especificado pelo valor sessionID. A sintaxe da solicitação para listar todas as assinaturas de eventos de um cliente específico é a seguinte URL:

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**Solicitar Cabeçalhos:**

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

**Códigos de Resposta:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Código de resposta</p> </th> 
   <th> Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (Sem conteúdo)</td> 
   <td>A solicitação retornou com sucesso todas as assinaturas de eventos encontradas para o usuário.</td> 
  </tr> 
  <tr> 
   <td>401 (não autorizado)</td> 
   <td>A sessionID fornecida estava vazia.</td> 
  </tr> 
  <tr> 
   <td>403 (proibido)</td> 
   <td>O usuário que corresponde à ID de sessão fornecida não tem acesso de administrador.</td> 
  </tr> 
 </tbody> 
</table>



### Exemplo de corpo de resposta

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
