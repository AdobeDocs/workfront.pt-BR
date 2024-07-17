---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Mover objetos de um ambiente para outro
description: O recurso de Promoção do ambiente tem como objetivo fornecer a capacidade de mover objetos relacionados à configuração de um ambiente para outro. Ela não oferece suporte à capacidade de mover objetos transacionais (com exceções limitadas).
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: 6f5da5ede6bb8c98b26d7d37366670c89ded6c49
workflow-type: tm+mt
source-wordcount: '2095'
ht-degree: 2%

---

# Mover objetos entre [!DNL Workfront] ambientes usando a API de promoção de ambiente [!DNL Workfront]

O recurso de Promoção do ambiente permite mover objetos relacionados à configuração de um ambiente para outro. Você pode mover esses objetos usando a API do Workfront, conforme descrito neste artigo.

Para obter instruções sobre como mover objetos entre ambientes usando o aplicativo Workfront, consulte:

* [Criar ou editar um pacote de promoção de ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [Instalar um pacote de promoção de ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)


## Requisitos de acesso

Você deve ter o seguinte:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plano</strong>
   </td>
   <td> Prime ou Ultimate (somente novos planos)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenças</strong>
   </td>
   <td> [!UICONTROL Padrão]
   </td>
  </tr>
   <tr>
   <td>Configurações de nível de acesso
   </td>
   <td>Você deve ser um administrador [!DNL Workfront].
   </td>
  </tr>
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos

O ponto de extremidade Criar pacote de promoção presume que você já configurou o ambiente de origem. Esta chamada de API requer a criação manual de um mapa de objetos de [!DNL Workfront] objCodes e GUIDs de objeto. A estrutura específica deste mapa é descrita abaixo.

## Objetos compatíveis com a promoção do ambiente

O recurso de Promoção do ambiente tem como objetivo fornecer a capacidade de mover objetos relacionados à configuração de um ambiente para outro. Ela não oferece suporte à capacidade de mover objetos transacionais (com exceções limitadas).

Para obter uma lista de objetos promovíveis e seus sub-objetos promovíveis incluídos, consulte [Objetos com suporte para promoção de ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) no artigo [Visão geral da movimentação de objetos entre ambientes do Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## Autenticação

A API autentica cada solicitação para garantir que o cliente tenha acesso para visualizar ou modificar um objeto solicitado.

A autenticação é realizada transmitindo uma ID de sessão ou chave de API, que pode ser fornecida usando o seguinte método:

### Solicitar autenticação de cabeçalho

O método preferido de autenticação é passar um cabeçalho de solicitação chamado SessionID contendo o token de sessão. Isso tem a vantagem de estar seguro contra [ataques de falsificação de solicitação entre sites (CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) e não interferir no URI para fins de armazenamento em cache.

Veja a seguir um exemplo de um cabeçalho de solicitação:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## Endpoints de API

* [Criar um pacote](#create-a-package)
* [Obter uma lista de pacotes](#get-a-list-of-packages)
* [Obter um pacote por ID](#get-a-package-by-id)
* [Atualizar propriedades específicas de um pacote](#update-specific-properties-of-a-package)
* [Excluir um pacote](#delete-a-package)
* [Executar uma pré-execução](#execute-a-pre-run)
* [Executar uma instalação](#execute-an-installation)
* [Obter uma lista de instalações para um pacote específico](#get-a-list-of-installations-for-a-specific-package)
* [Obter os detalhes de uma instalação](#get-the-installation-details-for-an-installation)

### Criar um pacote

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Essa chamada executa um processo de várias etapas.

A primeira etapa resulta na criação de um pacote de promoção vazio no status &quot;MONTANDO&quot;.

A segunda etapa usa a matriz `objectCollections` fornecida no corpo do POST para reunir os registros solicitados do Workfront. Essa etapa pode levar vários minutos para ser concluída, dependendo do número de registros solicitados e da configuração do Workfront. No final deste processo, o pacote de promoção vazio é atualizado com o `packageEntities` e o status é automaticamente definido como &quot;RASCUNHO&quot;.


>[!NOTE]
>
>Anote a estrutura da matriz `objectCollections`.
>
>Cada item na matriz contém uma chave `objCode` que corresponde ao código de objeto documentado no Workfront API Explorer.
>
>Cada item também contém uma coleção `entities`. Isso espera o campo `ID`. Ele também pode aceitar um atributo `name` opcional para facilitar a identificação do que `ID` representa.
>
>Para obter a lista de códigos de objeto permitidos a serem solicitados na lista `objectCollections`, consulte a seção [Objetos com suporte para promoção de ambiente](#supported-objects-for-environment-promotion) neste artigo.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Cabeçalhos

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Ou

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corpo

```json
{
    "name": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### Resposta

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
}
```

### Obter uma lista de pacotes

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Esta chamada retorna uma lista não filtrada de pacotes promocionais pertencentes ao cliente.

A resposta incluirá todos os pacotes criados de qualquer uma das instâncias de sandbox, pré-visualização ou produção do Workfront.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Cabeçalhos

```json
{
    "apikey": "**********"
}
```

Ou

```json
{
    "sessionID": "*****************"
}
```

#### Corpo

_Vazio_

#### Resposta

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "ASSEMBLING",
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

&lt;!—Verifique o &quot;status&quot; acima—ele foi adicionado?—>

### Obter um pacote por ID

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Esta chamada retorna os detalhes de um pacote promocional solicitado.

A solicitação pode ser feita por meio de qualquer ambiente, independentemente da origem do pacote de promoção.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Cabeçalhos

```json
{
    "apikey": "**********"
}
```

Ou

```json
{
    "sessionID": "*****************"
}
```

#### Corpo

_Vazio_

#### Resposta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Atualizar propriedades específicas de um pacote

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Essa chamada atualiza qualquer conteúdo do pacote de promoção fornecido no corpo do PATCH.

Os atributos editáveis são:

1. nome (sequência de caracteres)
1. descrição (sequência de caracteres)
1. status (string com validação de valor)

Para obter uma descrição detalhada dos status disponíveis, consulte [Status de promoção do ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) no artigo [Visão geral da movimentação de objetos entre ambientes do Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### Cabeçalhos

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Ou

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corpo

```json
{
    "status": "ACTIVE"
}
```

#### Resposta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Excluir um pacote

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Essa chamada exclui o registro do pacote promocional. Esta ação é irreversível.

>[!NOTE]
>
>Ao contrário da exclusão de um pacote promocional, a recomendação é alterar o status do pacote para DISABLED. Isso permitirá que o pacote seja recuperável e manterá o histórico de instalação de onde foi implantado.

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Cabeçalhos

```json
{
    "apikey": "**********"
}
```

Ou

```json
{
    "sessionID": "*****************"
}
```

#### Corpo

_Vazio_

#### Resposta

```
200
```

```
Deleted
```

### Executar uma pré-execução

>[!IMPORTANT]
>
>Antes de executar uma instalação, é necessário executar essa pré-execução. Você usará a ID gerada por essa chamada ao executar a instalação.

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

Esta chamada realiza uma comparação entre a definição do pacote e o ambiente de destino identificado no URL.

O resultado é um corpo JSON que identifica se um objeto de promoção é encontrado ou não no ambiente de destino.

Para cada objeto de promoção, um dos `actions` a seguir será definido:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>CRIAR</td> 
   <td><p>Quando um registro correspondente não pode ser encontrado no ambiente de destino, a ação é definida como CRIAR.</p><p>Quando esta ação for definida no <code>translationmap</code> fornecido ao ponto de extremidade <code>/install</code>, o serviço de instalação criará o registro.</p></td> 
  </tr> 
  <tr> 
   <td>USAREXISTENTE</td> 
   <td><p>Quando um registro correspondente é encontrado no ambiente de destino, a ação é definida como USEEXISTING e um <code>targetId</code> também é capturado no <code>translationmap</code>.</p><p>Quando esta ação é definida no <code>translationmap</code> que é fornecido ao ponto de extremidade <code>/install</code>, o serviço de instalação não criará o registro. No entanto, ele usará a <code>targetId</code> incluída na entrada do mapa para outros objetos que possam ter uma referência a este registro.</p><p>Por exemplo, um "Grupo padrão" pode ser encontrado no ambiente de destino no qual um pacote está sendo implantado. Não é possível ter dois registros de "Grupo padrão", portanto, o serviço de instalação usará o GUID do grupo existente em qualquer outra ação de criação de objeto que inclua uma referência ao "Grupo padrão", como um projeto, formulário ou qualquer outra entidade relacionada a esse grupo.</p><p><b>Nota:</b> <ul><li><p>Quando a ação USEEXISTING é atribuída, o registro existente no ambiente de destino não é modificado. </p><p>Por exemplo, se a descrição do "Grupo padrão" tiver sido alterada na sandbox de onde o pacote foi criado e o valor da descrição for diferente no ambiente de destino, o valor permanecerá inalterado após uma instalação com este <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>SUBSTITUIÇÃO</td> 
   <td><p>Esta ação não será definida automaticamente.</p><p>Esta ação fornece a capacidade de atualizar um objeto que existe no ambiente de destino. Ele permite fazer uma substituição manual de uma ação CREATE ou USEEXISTING atribuída antes de executar a chamada <code>/install</code>.<ul><li>Um usuário pode atualizar um objeto no ambiente de teste e, em seguida, usar a ação SUBSTITUIR para atualizar esse objeto no ambiente de destino.</p></li><li><p>Se o usuário instalar um pacote de promoção inicialmente e, em seguida, um novo pacote (ou atualizado) no futuro contiver alterações em objetos no pacote inicial, o usuário poderá usar SUBSTITUIÇÃO para substituir (substituir) objetos instalados anteriormente. </p><p>Para obter mais informações sobre substituição, consulte a seção [Substituição](#overwriting) neste artigo.</li><ul></td> 
  </tr> 
  <tr> 
   <td>IGNORAR</td> 
   <td><p>Esta ação não será definida automaticamente.</p><p>Ele permite fazer uma substituição manual de uma ação CREATE ou USEEXISTING atribuída antes de executar a chamada <code>/install</code>.</p><p><b>Notas: </b><ul><li><p>Se um registro originalmente definido como CREATE for definido como IGNORE, quaisquer registros secundários também deverão ser definidos como IGNORE.</p><p>Por exemplo, se um registro de Modelo foi mapeado com uma ação CRIAR e o usuário que estiver instalando deseja excluí-lo da implantação, ele pode definir a ação do Modelo como IGNORAR.</p><p>Nesse caso, se o usuário que estiver instalando também não definir as Tarefas de Modelo, Atribuições de Tarefa de Modelo, Predecessoras de Tarefa de Modelo, Definição de Fila, Tópicos de Fila, Regras de Roteamento etc. como IGNORAR, a implantação resultará em uma falha na tentativa de instalação.</p></li><li><p>Se um registro originalmente definido como USEEXISTING for definido como IGNORE, poderá haver alguns efeitos adversos durante o processo de instalação.</p><p>Por exemplo, se um registro de Grupo foi mapeado com a ação USEEXISTING e o usuário que instalou altera a ação para IGNORE, para objetos que exigem um grupo (por exemplo, um Projeto não pode existir sem um grupo atribuído), o grupo padrão do sistema será atribuído a esse projeto.</p></li><li><p>Se um registro originalmente definido como USEEXISTING for definido como CREATE, poderá haver alguns efeitos adversos durante o processo de instalação, pois muitas entidades do Workfront têm restrições de nome exclusivo.</p><p>Por exemplo, se um registro "Grupo padrão" foi mapeado com a ação USEEXISTING e o usuário que instalou altera a ação para CREATE, porque já existe um "Grupo padrão", a tentativa de instalação não concluirá todas as etapas. Os nomes dos grupos devem ser exclusivos.</p><p>Algumas entidades não têm uma restrição de nome exclusivo. Para esses objetos, fazer essa alteração resultará em dois registros com nomes idênticos. Por exemplo, Modelos, Projetos, Visualizações, Filtros, Agrupamentos, Relatórios e Painéis não exigem restrições de nome exclusivo. É uma prática recomendada ter nomes exclusivos para esses registros, mas não é aplicada.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

No momento, não há suporte para UPDATE `action` nos recursos alfa deste serviço. A opção para permitir uma ATUALIZAÇÃO `action` é algo que estamos pesquisando.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```

#### Cabeçalhos

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Ou

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corpo

```json
{}
```

#### Resposta

```
200
```

```json
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
```

>[!NOTE]
>
>A ID necessária para executar a instalação é o campo `id`. Neste exemplo, o campo `id` é o terceiro da parte superior e tem um valor começando com `c0bc79bd`.

### Executar uma instalação

>[!IMPORTANT]
>
>Antes de executar uma instalação, é necessário executar uma pré-execução. Você usará a ID gerada na pré-execução ao executar a instalação.
>
>Se alguma alteração tiver sido feita no ambiente de destino (o ambiente no qual o pacote está sendo implantado) após a execução da pré-execução, recomendamos executar a pré-execução novamente. Se você não executar a pré-execução novamente, a execução poderá não ser concluída com precisão ou a instalação poderá falhar.
>
>Para obter instruções sobre como executar uma pré-execução, consulte [Executar uma pré-execução](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Esta chamada inicia uma tentativa de instalação de um pacote de promoção no ambiente de destino identificado no URL do POST.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### Cabeçalhos

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Ou

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corpo

```json
{
}
```

#### Resposta

```
202
```


```json
{}
```

### Obter uma lista de instalações para um pacote específico

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

Os resultados incluem eventos de instalação de todos os ambientes nos quais o pacote foi implantado. Elas não se limitam às instalações para o ambiente pelo qual a solicitação está sendo feita. Isso permite identificar quais ambientes receberam esse pacote.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### Cabeçalhos

```json
{
    "apikey": "**********"
}
```

Ou

```json
{
    "sessionID": "*****************"
}
```

#### Corpo

_Vazio_

#### Resposta

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "INSTALLED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### Obter os detalhes de uma instalação

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Esta chamada retornará o `translationMap` final produzido pelo serviço de instalação para uma instalação específica.

Cada registro indicará qual foi o `action` prescrito e se essa ação foi bem-sucedida ou não.

Para registros com um CREATE `action`, o campo `targetId` será definido com o valor do registro recém-criado no sistema de destino. Além disso, o campo `installationStatus` será definido como INSTALADO.

Para registros com USEEXISTING `action`, o campo `targetId` também será definido, e o campo `installationStatus` será definido como REGISTERED. Isso significa que o processo de mapeamento foi concluído e o serviço de instalação reconhece que avaliou o registro e não há nada para ser feito.

Se o registro tiver um CREATE `action`, mas ele não conseguir criar o registro com êxito, o `installationStatus` será definido como FAILED e o motivo da falha também será fornecido.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### Cabeçalhos

```json
{
    "apikey": "**********"
}
```

Ou

```json
{
    "sessionID": "*****************"
}
```

#### Corpo

_Vazio_

#### Resposta

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "INSTALLED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
}
```

## Substituição

Este é um processo de três etapas.

1. Criar um mapa de tradução (análogo à fase &quot;preparar instalação&quot;)
1. Edite o mapa de tradução gerado, definindo os campos `action` e `targetId` para qualquer objeto que eles desejem substituir. A ação deve ser `OVERWRITING` e `targetId` deve ser a uuid do objeto que deve ser substituído
1. Execute a instalação.

* [Etapa 1 - Criar um mapa de tradução](#step-1---create-a-translation-map)
* [Etapa 2 - Modificar o mapa de tradução](#step-2---modify-the-translation-map)
* [Etapa 3 - Instalar](#step-3---install)

### **Etapa 1 - Criar um Mapa de Tradução**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/translation-map
```

#### Corpo

Nenhum(a)

#### Resposta

Um mapa de tradução, com status `202 - OK`

```json
{
    {objcode}: {
        {object uuid}: {
            "targetId": {uuid of object in destination},
            "action": {installation action},
            "name": {name of the object},
            "isValid": true
        },
        {...more objects}
    },
    {...more objcodes}
}
```


#### Exemplo

```json
{
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "CREATE",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
```

### Etapa 2 - Modificar o mapa de tradução

Não há um terminal para esta etapa.

1. No mapa de tradução retornado em [Etapa 1 - Criar um Mapa de Tradução](#step-1---create-a-translation-map), inspecione a lista de objetos que serão instalados.
1. Atualize o campo de ação em cada objeto para a ação de instalação desejada.
1. Valide o `targetId` em cada objeto. Se a ação definida for `USEEXISTING` ou `OVERWRITING`, `targetId` deverá ser definido como a UUID do objeto de destino no ambiente de destino. Para qualquer outra ação, o targetId deve ser uma cadeia de caracteres vazia.

   >[!NOTE]
   >
   >O `targetId` já está preenchido se uma colisão foi detectada.

### **Etapa 3 - Instalar**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/install
```

#### Corpo

Este é um objeto com um único campo `translationMap`, que deve ser igual ao mapa de tradução modificado de [Etapa 2 - Modificar o Mapa de Tradução](#step-2---modify-the-translation-map).

```json
{
    "translationMap": {
        {objcode}: {
            {object uuid}: {
                "targetId": {uuid of object in destination},
                "action": {installation action},
                "name": {name of the object},
                "isValid": true
            },
            {...more objects}
        },
        {...more objcodes}
    }
}
```


#### Exemplo

```json
{
    "translationMap": {
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "OVERWRITING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
}
```

#### Resposta

A resposta inclui o `{uuid of the created installation}` e um status `202 - ACCEPTED`.

Exemplo: `b6aa0af8-3520-4b25-aca3-86793dff44a6`

<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->
