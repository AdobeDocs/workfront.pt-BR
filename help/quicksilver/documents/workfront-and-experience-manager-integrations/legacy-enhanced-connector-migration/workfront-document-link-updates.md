---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrar pastas e documentos vinculados
description: Você pode usar a API para migrar pastas e documentos vinculados para o Adobe Experience Manager Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: aad8f4648a57c93047a1a691d5e608c327d78c1b
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Migrar pastas e documentos vinculados

Você pode usar a API para migrar pastas e documentos vinculados para o Adobe Experience Manager Assets.

## Procedimento

1. Identifique todos os documentos e pastas vinculados ao provedor de armazenamento de documentos externo anterior, anotando seus identificadores internos de documentos ou pastas do Workfront, bem como a ID da pasta de qualquer pasta contêiner.

   >[!NOTE]
   >
   > Você deve verificar todas as pastas ou documentos descobertos para verificar se eles ainda não criaram um link para eles com o novo provedor.

1. Localize os documentos e pastas no novo repositório por caminho e, em seguida, procure sua identidade no sistema externo.

1. Crie um mapeamento da Workfront ID interna para a ID no novo armazenamento externo. Você precisa disso para criar um novo link na etapa a seguir.

1. Crie um novo link de documento ou pasta de documentos no Workfront, apontando para o recurso em seu novo local por meio da nova ID externa.

   1. **Documentos**: adiciona uma nova versão do documento existente com o novo provedor de documentos externos.
   1. **Pastas**: crie uma nova pasta no mesmo local com o mesmo nome.

>[!CAUTION]
>
>   Não exclua as pastas vinculadas existentes. Isso pode resultar em perda de dados. Para remover links de pastas antigos do aplicativo Workfront, desative a integração de documentos personalizados na área Configuração.


## Exemplo de processo para migrar links

![fluxo de link simplificado](assets/links-flow-simplified.png)

## Informações da API

Para obter mais informações sobre as APIs do Workfront nesta seção, consulte [Documentação do desenvolvedor:Documents](https://developer.workfront.com/documents.html).

### Localizar todos os documentos

Localizar tudo **Documentos (DOCU)** Vinculado a **Provedor do documento** de **providerType** com **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[Referência de API DOCS](https://developer.workfront.com/documents.html#get-/docu/search)

### Localizar todas as pastas

Localizar tudo **Pastas de documentos (DOCFDR)** Vinculado ao provedor do documento de **providerType** com **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API DOCS: (Endpoints de pasta de documentos não cobertos atualmente em developer.workfront.com)

### Vincular documentos

Link **Documentos (DOCU)** de **Provedor de Documento Externo** de **providerType** com **documentProviderID**.

>[!IMPORTANT]
>
>Os documentos são armazenados temporariamente. Ou seja, você tem acesso a todas as versões do documento. Ao criar o link, você pode especificar a ID do documento existente, de modo que esteja apenas gravando uma nova versão nesse documento, com os dados sendo hospedados externamente no novo provedor. Essa ID do documento é a mesma ID encontrada no link do documento que você está substituindo. É o mesmo documento conceitual. Você está simplesmente indicando que os bytes desta nova versão são armazenados com um provedor diferente.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

DOCUMENTOS DA API: (Endpoints de link internos não cobertos atualmente em developer.workfront.com)

### Vincular pastas

Link **Pastas de documentos (DOCFDR)** de **Provedor de Documento Externo** de **providerType** com **documentProviderID**.

>[!IMPORTANT]
>
>Para links de pastas, ao contrário de links de documentos, você precisa do &quot;documentFolderId&quot; da pasta no Workfront para a qual deseja colocar o novo link. Esta é a mesma pasta pai, provavelmente, que a pasta vinculada que estamos copiando.

>[!CAUTION]
>
>As pastas não são armazenadas temporariamente. Não exclua as pastas antigas. Desative a integração de documentos personalizados na área de configuração para remover pastas antigas.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

DOCUMENTOS DA API: (Endpoints de link internos não cobertos atualmente em developer.workfront.com)

## Termos importantes

* **Documento**: um ativo digital no Workfront

* **Pasta de documentos**: um container para ativos digitais no Workfront

* **ID do documento**: ID interna do Workfront para um ativo digital

* **ID da pasta de documentos**: ID interna do Workfront para uma pasta de ativos digitais

* **ID do provedor de documentos**: ID associada a provedores de documentos específicos

>[!IMPORTANT]
>
> Para qualquer Tipo de provedor de documento, um cliente pode ter várias instâncias conectadas. Eles podem ter vários repositórios AEM vinculados, por exemplo. Ou várias instâncias do Google Drive vinculadas. A ID do provedor de documentos indica a instância específica do tipo de conexão que queremos substituir ou para a qual queremos alternar.

* **Tipo de Provedor de Armazenamento de Documentos (também &quot;Tipo de Integração Externa&quot;)**: o tipo de integração do provedor de armazenamento de documentos compatível com o Workfront. Por meio de uma integração dedicada ou uma &quot;integração personalizada&quot;.

* **Tipos de Provedor de Armazenamento de Documentos Atuais ( providerType)**:

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

* **Documento vinculado**: um ativo digital hospedado em um provedor de armazenamento de documentos externo. O Workfront terá sua própria &quot;ID do documento&quot; interna para o ativo, mas os bytes são armazenados externamente. Para facilitar isso, o Workfront também armazena uma &quot;ID de documento externa&quot; para ajudar a localizar o recurso referenciado externamente no repositório ou armazenamento remoto.

* **Pasta de documentos vinculada**: um container para ativos digitais hospedados em um provedor de armazenamento de documentos externo. O Workfront terá sua própria &quot;ID da pasta de documentos&quot; interna para o ativo, mas os bytes são armazenados externamente. Para facilitar isso, o Workfront também armazena uma &quot;ID de documento externa&quot; para ajudar a localizar o recurso referenciado externamente no repositório ou armazenamento remoto.

* **ID do documento externo**: ID atribuída quando os ativos são armazenados fora do Workfront. O Workfront mapeia seu identificador interno para o identificador usado para localizar o ativo no sistema externo, por meio desse campo &quot;identificador de documento externo&quot;. Portanto, ao vincular o documento ou a pasta de um novo armazenamento externo, um novo identificador de documento externo deve ser composto, no formato apropriado para o provedor de documentos externos identificar o documento no novo repositório ou armazenamento.

  >[!NOTE]
  >
  > O Workfront ainda não tem um padrão para identificadores de documentos externos. Uma nova especificação está sendo usada para IDs AEM, mas para outras IDs, a ID do documento externo pode assumir diferentes formas, dependendo do tipo de provedor.


* **Tipo de objeto**: Este é um termo somente para API para fins deste documento. É um tipo de objeto genérico no Workfront com o qual você deseja interagir. Nesse caso, você interagirá com documentos e pastas que têm os tipos &quot;DOCU&quot; e &quot;DOCFDR&quot;, respectivamente.

* **ID do objeto**: o identificador interno do Workfront para o objeto genérico com o qual você deseja interagir. Você interagirá com documentos e pastas, portanto, essa será a ID do documento ou a ID da pasta do documento, respectivamente.
