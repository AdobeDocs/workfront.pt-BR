---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrar pastas e documentos vinculados
description: Você pode usar a API para migrar pastas e documentos vinculados para o Adobe Experience Manager Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Migrar pastas e documentos vinculados

Você pode usar a API para migrar pastas e documentos vinculados para o Adobe Experience Manager Assets.

## Procedimento

1. Identifique todos os documentos e pastas vinculados ao provedor de armazenamento de documentos externo anterior, anotando seus identificadores internos de documentos ou pastas do Workfront, bem como a ID da pasta de qualquer pasta que contenha.

   >[!NOTE]
   >
   > Você deve verificar todas as pastas ou documentos descobertos para verificar se eles ainda não criaram um link para eles com o novo provedor.

1. Localize os documentos e as pastas no novo repositório por caminho e, em seguida, procure sua identidade no sistema externo.

1. Crie um mapeamento da Workfront ID interna, para a ID na nova loja externa. É necessário criar um novo link na etapa a seguir.

1. Crie um novo link de documento ou pasta de documento no Workfront, apontando para o recurso em seu novo local por meio da nova ID externa.

   1. **Documentos**: Adicione uma nova versão do documento existente com o novo provedor de documento externo.
   1. **Pastas**: Crie um novo filtro no mesmo lugar com o mesmo nome.

>[!CAUTION]
>
>   Não exclua as pastas vinculadas existentes. Isso pode resultar em perda de dados. Para remover links de pastas antigas do aplicativo Workfront, desative a integração de documento personalizado na área Configuração.


## Exemplo de processo para migração de links

![fluxo simplificado de links](assets/links-flow-simplified.png)

## Informações da API

Para obter mais informações sobre as APIs do Workfront nesta seção, consulte [Documentação do desenvolvedor:Documentos](https://developer.workfront.com/documents.html).

### Localizar todos os documentos

Localizar tudo **Documentos (DOCU)** Vinculado a **Provedor de documentos** de **providerType** com **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[Referência de API DOCS](https://developer.workfront.com/documents.html#get-/docu/search)

### Localizar todas as pastas

Localizar tudo **Pastas de documentos (DOCFDR)** Vinculado ao Provedor de Documentos de **providerType** com **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

DOCUMENTOS DA API: (Pontos de extremidade da pasta de documento não cobertos no momento em developer.workfront.com)

### Vincular documentos

Link **Documentos (DOCU)** from **Provedor de documentos externos** de **providerType** com **documentProviderID**.

>[!IMPORTANT]
>
>Os documentos são armazenados temporariamente. Ou seja, você tem acesso a todas as versões do documento. Ao criar o link, você pode especificar a ID do documento existente, de modo que esteja apenas gravando uma nova versão nesse documento, com os dados sendo hospedados externamente no novo provedor. Essa ID do documento é igual à ID do documento encontrada no link do documento que você está substituindo. É o mesmo documento conceitual. Você está simplesmente indicando que os bytes desta nova versão são armazenados com um provedor diferente.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

DOCUMENTOS DA API: (Endpoints de link interno não cobertos no momento em developer.workfront.com)

### Pastas de links

Link **Pastas de documentos (DOCFDR)** from **Provedor de documentos externos** de **providerType** com **documentProviderID**.

>[!IMPORTANT]
>
>Para links de pastas , ao contrário de Links de documento, você precisa do &#39;documentFolderId&#39; da pasta no Workfront em que deseja colocar o novo link. Essa é a mesma pasta principal, provavelmente, como a pasta vinculada que estamos copiando.

>[!CAUTION]
>
>As pastas não são armazenadas temporariamente. Não exclua as pastas antigas. Desative a integração de documento personalizado na área de configuração para remover pastas antigas.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

DOCUMENTOS DA API: (Endpoints de link interno não cobertos no momento em developer.workfront.com)

## Termos importantes

* **Documento**: Um ativo digital no Workfront

* **Pasta de documentos**: Um contêiner de ativos digitais no Workfront

* **ID do documento**: ID interna da Workfront para um ativo digital

* **ID da pasta do documento**: ID interna da Workfront para uma pasta de ativos digitais

* **ID do Provedor de Documentos**: ID associada a provedores de documento específicos

>[!IMPORTANT]
>
> Para qualquer Tipo de Provedor de Documentos, um cliente pode ter várias instâncias conectadas. Eles podem ter vários Repositórios AEM vinculados, por exemplo. Ou várias instâncias do Google Drive vinculadas. A ID do Provedor de Documentos indica a instância específica do tipo de conexão para a qual queremos substituir ou alternar.

* **Tipo de Provedor de Armazenamento de Documentos (também &quot;Tipo de Integração Externa&quot;)**: O tipo de integração do provedor de armazenamento de documentos compatível com o Workfront. Por meio de uma integração dedicada ou de uma &quot;integração personalizada&quot;.

* **Tipos de Fornecedor de Armazenamento de Documentos Atuais ( providerType)**:

   ```
   ATTASK
   BOX
   GOOGLE
   SHAREPOINT
   WEBDAM
   WORKFRONTDAM
   INFERNO
   WIDEN
   DROPBOX
   DROPBOX_BUSINESS
   ONEDRIVE
   QUIP
   WEBHOOKS
   AEM
   MOCK
   ```

* **Documento vinculado**: Um ativo digital hospedado em um provedor externo de armazenamento de documentos. A Workfront terá sua própria &quot;ID de documento&quot; interna para o ativo, mas os bytes são armazenados externamente. Para facilitar isso, o Workfront também armazena uma &quot;ID de documento externo&quot; para auxiliar na localização do recurso externamente referenciado no repositório remoto ou no armazenamento.

* **Pasta de documentos vinculados**: Um contêiner de ativos digitais hospedados em um provedor externo de armazenamento de documentos. A Workfront terá sua própria &quot;ID da pasta de documentos&quot; interna para o ativo, mas os bytes serão armazenados externamente. Para facilitar isso, o Workfront também armazena uma &quot;ID de documento externo&quot; para auxiliar na localização do recurso externamente referenciado no repositório remoto ou no armazenamento.

* **ID de Documento Externo**: ID atribuída quando os ativos são armazenados fora da área de trabalho. O Workfront mapeia seu identificador interno para o identificador usado para localizar o ativo no sistema externo, por meio desse campo &quot;identificador de documento externo&quot;. Portanto, ao vincular o documento ou a pasta a partir de um novo armazenamento externo, um novo identificador de documento externo deve ser composto, no formato adequado para que o provedor de documento externo identifique o documento no novo repositório ou armazenamento.

   >[!NOTE]
   >
   > O Workfront ainda não tem um padrão para identificadores de documentos externos. Uma nova especificação está sendo usada para IDs de AEM, mas para outras IDs, a ID de documento externo pode assumir formulários diferentes dependendo do tipo de provedor.


* **Tipo de objeto**: Este é um termo de API somente para os fins deste documento. É um tipo de objeto genérico dentro do workfront com o qual você deseja interagir. Nesse caso, você interagirá com documentos e pastas que tenham os tipos &quot;DOCU&quot; e &quot;DOCFDR&quot;, respectivamente.

* **ID do objeto**: O identificador interno do Workfront para o objeto genérico com o qual você deseja interagir. Você interage com documentos e pastas para que isso seja a ID do documento ou a ID da pasta do documento, respectivamente.
