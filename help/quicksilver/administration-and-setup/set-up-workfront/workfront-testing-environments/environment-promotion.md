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
hide: true
hidefromtoc: true
source-git-commit: b0142b75e507081ebfb6ce700f37d5c287c72cde
workflow-type: tm+mt
source-wordcount: '2334'
ht-degree: 3%

---

# Mover objetos de um [!DNL Workfront] ambiente para outro

<!-- 
TO DO

Overview of value
Check for any code changes
Fix {}
Add to tocs
-->

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plano</td> 
   <td> <p>Enterprise, Prime ou Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licença</p> </td> 
   <td> <p>[!UICONTROL Plano] </p> <p>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Permissões de objeto</p> </td> 
   <td> <p>Todos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pacote de suporte</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferencial] ou [!UICONTROL Enterprise]</p> <p>O pacote de suporte padrão não tem acesso à sandbox de atualização personalizada, mas tem acesso à sandbox de visualização.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Pré-requisitos

O ponto de extremidade Criar pacote de promoção presume que você já configurou o ambiente de origem. Esta chamada de API requer a criação manual de um mapa de objetos de [!DNL Workfront] objCodes e GUIDs de objeto. A estrutura específica deste mapa é descrita abaixo.

## Objetos compatíveis com a promoção do ambiente

O recurso de Promoção do ambiente tem como objetivo fornecer a capacidade de mover objetos relacionados à configuração de um ambiente para outro. Ela não oferece suporte à capacidade de mover objetos transacionais (com exceções limitadas).

* [Objetos de trabalho](#work-objects)
* [Objetos de relatório](#reporting-objects)
* [Objetos de dados personalizados](#custom-data-objects)
* [Objetos da organização](#organization-objects)
* [Outros objetos de configuração](#other-configuration-objects)


### Objetos de trabalho

| Objeto promovível | Sub-objetos promovíveis incluídos |
| --- | --- |
| Projeto (PROJ) | Projeto<br>Tarefa<br>Atribuição<br>Predecessora<br>Empresa<br>Taxa de substituição<br>Grupo<br>Função<br>Equipe<br>Processo de aprovação<br>Caminho de aprovação<br>Etapa de aprovação<br>Aprovador da etapa<br>Agendar<br>Dia Não Útil<br>Definição da fila<br>Grupo de Tópicos de Fila<br>Enfileirar tópico<br>Regra de Encaminhamento<br>Caminho de Etapas<br>Etapa<br>Tipo de Hora<br>Conjunto de recursos<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria |
| Modelo (TMPL) | Modelo<br>Modelo de Tarefa<br>Atribuição de Modelo de Tarefa<br>Predecessora da Tarefa de Modelo<br>Empresa<br>Taxa de substituição<br>Grupo<br>Função<br>Equipe<br>Processo de aprovação<br>Caminho de aprovação<br>Etapa de aprovação<br>Aprovador da etapa<br>Agendar<br>Dia Não Útil<br>Definição da fila<br>Grupo de Tópicos de Fila<br>Enfileirar tópico<br>Regra de Encaminhamento<br>Caminho de Etapas<br>Etapa<br>Tipo de Hora<br>Conjunto de recursos<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria |

### Objetos de relatório

| Objeto promovível | Sub-objetos promovíveis incluídos |
| --- | --- |
| Modelo de layout (UITMPL) | Modelo de layout<br>Painel<br>Calendário<br>Seção de calendário<br>Página externa<br>Relatório<br>Filtro<br>Agrupamento<br>Exibir<br>Parâmetro |
| Painel (PTLTAB) | Painel<br>Calendário<br>Seção de calendário<br>Página externa<br>Relatório<br>Filtro<br>Agrupamento<br>Exibir<br>Parâmetro |
| Calendário (CALEND) | Calendário<br>Seção de calendário |
| Página externa (EXTSEC) | Página Externa |
| Relatório (PTLSEC) | Relatório<br>Filtro<br>Agrupamento<br>Exibir<br>Parâmetro |
| Filtro (UIFT) | Filtro<br>Parâmetro |
| Agrupamento (UIGB) | Agrupamento<br>Parâmetro |
| Visualização (UIVW) | Exibir<br>Parâmetro |

### Objetos de dados personalizados

| Objeto promovível | Sub-objetos promovíveis incluídos |
| --- | --- |
| Categoria (CTGY) | Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria<br>Grupo |
| Parâmetro (PARAM) | Parâmetro<br>Opção de parâmetro |
| Grupo de Parâmetros (PGRP) | Grupo de Parâmetros |

### Objetos da organização

| Objeto promovível | Sub-objetos promovíveis incluídos |
| --- | --- |
| Grupo (GRUPO) | Grupo <br>Subgrupos (até 5 níveis)<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria |
| Função (ROLE) | Função |
| Equipe (TEAM) | Equipe<br>Grupo |
| Empresa (CMPY) | Empresa<br>Taxa de substituição<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Parâmetro <br>Lógica de exibição da categoria<br>Grupo |
| Portfolio (PORTA) | Portfolio<br>Programa<br>Grupo<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria |
| Programa (PRGM) | Programa<br>Portfolio<br>Grupo<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria |

### Outros objetos de configuração

| Objeto promovível | Sub-objetos promovíveis incluídos |
| --- | --- |
| Processo de aprovação (ARVPRC) | Processo de aprovação<br>Caminho de aprovação<br>Etapa de aprovação<br>Aprovador da etapa<br>Função<br>Equipe<br>Grupo |
| Agendamento (SCHED) | Agendar<br>Dia Não Útil<br>Grupo |
| Caminho de Etapas (MPATH) | Caminho de Etapas<br>Etapa |
| Perfil da planilha de horas (TSPRO) | Perfil da Planilha de Horas<br>Tipo de Hora |
| Tipo de Hora (HOURT) | Tipo de hora |
| Tipo de Despesa (EXPTYP) | Tipo de Despesa |
| Tipo de Risco (RSKTYP) | Tipo de Risco |
| Conjunto de Recursos (RSPL) | Conjunto de Recursos |

## Autenticação

A API autentica cada solicitação para garantir que o cliente tenha acesso para visualizar ou modificar um objeto solicitado.

A autenticação é realizada transmitindo uma ID de sessão ou chave de API, que pode ser fornecida usando o seguinte método:

### Solicitar autenticação de cabeçalho

O método preferido de autenticação é passar um cabeçalho de solicitação chamado SessionID contendo o token de sessão. Isso tem a vantagem de ser seguro contra [Falsificação de solicitação entre sites (CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) ataques e não interferir no URI para fins de armazenamento em cache.

Veja a seguir um exemplo de um cabeçalho de solicitação:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## Endpoints de API

* [Criar um pacote](#create-a-package)
* [Obter uma lista de pacotes](#get-a-list-of-packages)
* [Obter um pacote por ID](#get-a-package-by-id)
* [Obter a definição de configuração de um pacote](#get-a-packages-configuration-definition)
* [Substituir detalhes e definição do pacote](#replace-package-details-and-definition)
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

A segunda etapa utiliza o método `objectCollections` matriz fornecida no corpo do POST para reunir os registros solicitados do Workfront. Essa etapa pode levar vários minutos para ser concluída, dependendo do número de registros solicitados e da configuração do Workfront. No final desse processo, o pacote de promoção vazio é atualizado com o `packageEntities` e o status é automaticamente definido como &quot;RASCUNHO&quot;.


>[!NOTE]
>
>Observe a estrutura do `objectCollections`  matriz.
>
>Cada item na matriz contém um `objCode` chave que corresponde ao código de objeto documentado no Workfront API Explorer.
>
>Cada item também contém um `entities` coleção. Espera-se que o `ID` e `name` para que as chaves estejam presentes.
>
>Para que a lista de códigos de objeto permitidos seja solicitada no `objectCollections` , consulte a [Objetos compatíveis com a promoção do ambiente](#supported-objects-for-environment-promotion) neste artigo.

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
    "packageName": "Agency Onboarding - 2023-06-06",
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
        "status": "ASSEMBLING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
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

_Empty_

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
            "version": 1,
            "installationCounts": {},
            "createdAt": "2023-06-06T17:29:21.600Z",
            "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
            "publishedAt": null,
            "customerId": "61aa9d090005fa42152c1cb66659f38d"
        },
        {...}
    ]
}
```

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

_Empty_

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
        "status": "DRAFT",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
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

### Obter a definição de configuração de um pacote

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}/definition</code></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/definition
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

_Empty_

#### Resposta

```
200
```

```json
{
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

### Substituir detalhes e definição do pacote

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PUT /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Essa chamada substitui todo o conteúdo do pacote promocional.

A solicitação espera que todos os campos editáveis sejam fornecidos.

Os atributos editáveis são:

1. nome (sequência de caracteres)
1. descrição (sequência de caracteres)
1. origem (string com validação de URL)
1. status (string com validação de valor)
1. versão (número inteiro)
1. packageEntities (coleção)

As opções de status incluem:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>MONTAGEM</td> 
   <td><p>Esse status é atribuído automaticamente enquanto os objetos estão sendo montados.</p><p>Este status não pode ser definido diretamente por um cliente.</p></td> 
  </tr> 
  <tr> 
   <td>RASCUNHO</td> 
   <td><p>Esse status é atribuído na conclusão de um processo de montagem ou ao criar um pacote de promoção vazio.</p><p>É possível que um cliente mova o pacote promocional de volta para esse status.</p><p>Enquanto estiver nesse status, o pacote de promoção não poderá ser instalado em nenhum ambiente.</p></td> 
  </tr> 
  <tr> 
   <td>TESTE</td> 
   <td><p>Esse status permite que um pacote de promoção seja instalado em qualquer sandbox de Pré-visualização ou Atualização personalizada. Enquanto estiver nesse status, o pacote não poderá ser instalado na Produção.</p></td> 
  </tr> 
  <tr> 
   <td>ATIVO</td> 
   <td><p>Esse status permite que um pacote de promoção seja instalado em qualquer ambiente, incluindo Produção.</p><p>Quando o status de um pacote é definido como ATIVO, a variável <code>publishedAt</code> A data é automaticamente definida para o carimbo de data e hora atual da solicitação.</p></td> 
  </tr> 
  <tr> 
   <td>DESATIVADO</td> 
   <td><p>Esse status será usado para ocultar pacotes de promoção usados anteriormente que não serão instalados em nenhum ambiente no futuro.</p><p>Quando um pacote está nesse status, ele não pode ser instalado em nenhum ambiente.</p><p>Quando o status de um pacote é definido como DESATIVADO, a variável <code>retiredAt</code> A data é automaticamente definida para o carimbo de data e hora atual da solicitação.</p><p>O uso deste status é recomendado em vez do uso de<code>DELETE /package</code> endpoint porque ele é recuperável e o histórico de instalação é retido para todas as implantações feitas com esse pacote.</p></td> 
  </tr> 
  <tr> 
   <td>FALHA_NA_MONTAGEM</td> 
   <td><p>O pacote promocional será colocado automaticamente nesse status se a etapa MONTAGEM falhar.</p><p>Para retornar o pacote para a etapa MONTAGEM, acione o processo de extração novamente.</p></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
PUT https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Cabeçalhos

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corpo

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes... with a description change",
    "source": "https://{domain}.{environment}.workfront.com",
    "status": "TESTING",
    "version": 1,
    "metadata": {
        "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"],
        "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
        "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
        "summaryOrder": ["GROUP","ROLE","TMPL"], 
        "shapeVersion": 2
    },
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
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
        "status": "TESTING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
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
1. origem (string com validação de URL)
1. status (string com validação de valor)
1. versão (número inteiro)
1. packageEntities (coleção)

   ou

   objectCollections (matriz)

Fornecer a `packageEntities` atualizará o pacote de promoção com a definição de configuração fornecida.

Fornecer a `objectCollections` iniciará uma reextração da variável `source` ambiente associado ao pacote de promoção. A variável `source` O campo deve ser fornecido quando a variável `objectCollections` é fornecido.

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
        "status": "ACTIVE",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
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

_Empty_

#### Resposta

```
200
```

```
Deleted
```

### Executar uma pré-execução

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

Para cada objeto de promoção, uma das seguintes opções `actions`  será definido:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>CRIAR</td> 
   <td><p>Quando um registro correspondente não pode ser encontrado no ambiente de destino, a ação é definida como CRIAR.</p><p>Quando esta ação é definida na variável <code>translationmap</code> que é fornecido ao <code>/install</code> ponto de acesso, o serviço de instalação criará o registro.</p></td> 
  </tr> 
  <tr> 
   <td>USAREXISTENTE</td> 
   <td><p>Quando um registro correspondente é encontrado no ambiente de destino, a ação é definida como USEEXISTING e uma <code>targetId</code> também é capturado na variável <code>translationmap</code>.</p><p>Quando esta ação é definida na variável <code>translationmap</code> que é fornecido ao <code>/install</code> ponto de extremidade, o serviço de instalação não criará o registro. No entanto, utilizará o <code>targetId</code> incluído na entrada do mapa para outros objetos que podem ter uma referência a este registro.</p><p>Por exemplo, um "Grupo padrão" pode ser encontrado no ambiente de destino no qual um pacote está sendo implantado. Não é possível ter dois registros de "Grupo padrão", portanto, o serviço de instalação usará o GUID do grupo existente em qualquer outra ação de criação de objeto que inclua uma referência ao "Grupo padrão", como um projeto, formulário ou qualquer outra entidade relacionada a esse grupo.</p><p><b>Nota:</b> <ul><li><p>Quando a ação USEEXISTING é atribuída, o registro existente no ambiente de destino não é modificado. </p><p>Por exemplo, se a descrição do "Grupo padrão" tiver sido alterada na sandbox de onde o pacote foi criado e o valor da descrição for diferente no ambiente de destino, o valor permanecerá inalterado após uma instalação com esse <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>IGNORAR</td> 
   <td><p>Esta ação não será definida automaticamente.</p><p>Ele permite fazer uma substituição manual de uma ação CREATE ou USEEXISTING atribuída antes de executar a <code>/install</code> chame.</p><p><b>Notas: </b><ul><li><p>Se um registro originalmente definido como CREATE for definido como IGNORE, quaisquer registros secundários também deverão ser definidos como IGNORE.</p><p>Por exemplo, se um registro de Modelo foi mapeado com uma ação CRIAR e o usuário que estiver instalando deseja excluí-lo da implantação, ele pode definir a ação do Modelo como IGNORAR.</p><p>Nesse caso, se o usuário que estiver instalando também não definir as Tarefas de Modelo, Atribuições de Tarefa de Modelo, Predecessoras de Tarefa de Modelo, Definição de Fila, Tópicos de Fila, Regras de Roteamento etc. como IGNORAR, a implantação resultará em uma falha na tentativa de instalação.</p></li><li><p>Se um registro originalmente definido como USEEXISTING for definido como IGNORE, poderá haver alguns efeitos adversos durante o processo de instalação.</p><p>Por exemplo, se um registro de Grupo foi mapeado com a ação USEEXISTING e o usuário que instalou altera a ação para IGNORE, para objetos que exigem um grupo (por exemplo, um Projeto não pode existir sem um grupo atribuído), o grupo padrão do sistema será atribuído a esse projeto.</p></li><li><p>Se um registro originalmente definido como USEEXISTING for definido como CREATE, poderá haver alguns efeitos adversos durante o processo de instalação, pois muitas entidades do Workfront têm restrições de nome exclusivo.</p><p>Por exemplo, se um registro "Grupo padrão" foi mapeado com a ação USEEXISTING e o usuário que instalou altera a ação para CREATE, porque já existe um "Grupo padrão", a tentativa de instalação não concluirá todas as etapas. Os nomes dos grupos devem ser exclusivos.</p><p>Algumas entidades não têm uma restrição de nome exclusivo. Para esses objetos, fazer essa alteração resultará em dois registros com nomes idênticos. Por exemplo, Modelos, Projetos, Visualizações, Filtros, Agrupamentos, Relatórios e Painéis não exigem restrições de nome exclusivo. É uma prática recomendada ter nomes exclusivos para esses registros, mas não é aplicada.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

No momento, não há suporte para uma ATUALIZAÇÃO `action` nos recursos alfa deste serviço. A opção para permitir um UPDATE `action` é algo que estamos pesquisando.

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
{}
```

### Executar uma instalação

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Esta chamada inicia uma tentativa de instalação de um pacote de promoção no ambiente de destino identificado no URL do POST.

#### Opções

Se um `translationmap` não for fornecido no corpo do POST, o processo iniciará automaticamente o `/prepare-installation` chame. A variável `translationmap` que é devolvido será usado como está, sem a oportunidade de revisar ou fazer ajustes nele.

Se um `translationmap` for fornecido no corpo do POST, o processo de instalação usará o mapeamento fornecido. Isso dá ao usuário que está instalando a oportunidade de revisar e fazer ajustes, conforme necessário, antes de executar uma tentativa de instalação.

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
200
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

_Empty_

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
        "status": "COMPLETED",
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

Esta chamada retornará a versão final `translationMap` produzido pelo serviço de instalação para uma instalação específica.

Cada registro indicará o que o prescrito `action` e se essa ação foi ou não bem-sucedida.

Para registros com um CREATE `action` o `targetId` O campo será definido com o valor do registro recém-criado no sistema de destino. Além disso, a `installationStatus` será definido como INSTALADO.

Para registros com o valor USEEXISTING `action` o `targetId` também será definido, e o campo `installationStatus` O campo será definido como REGISTRADO. Isso significa que o processo de mapeamento foi concluído e o serviço de instalação reconhece que avaliou o registro e não há nada para ser feito.

Se o registro tiver um CREATE `action` mas não conseguir criar o registro com êxito, a variável `installationStatus` será definido como FALHA e o motivo da falha também será fornecido.

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

_Empty_

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
    "status": "COMPLETED",
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