---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Visão geral dos Webhooks
description: Visão geral dos Webhooks
author: John
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: a62ae524f922326811423cd17d0656920b7cc9d3
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Visão geral dos Webhooks

O Adobe Workfront Document Webhooks define um conjunto de endpoints de API através dos quais a Workfront faz chamadas de API autorizadas para um Provedor de Documentos Externo. Isso permite que qualquer pessoa crie um plug-in middleware para qualquer provedor de armazenamento de documentos.

![](assets/mceclip0-350x262.png)

A experiência do usuário para integrações baseadas em webhook será semelhante à das integrações de documentos existentes, como Google Drive, Box e Dropbox. Por exemplo, um usuário do Workfront poderá executar as seguintes ações:

* Navegar pela estrutura de pastas do provedor de documentos externo
* Pesquisar arquivos
* Vincular arquivos ao Workfront
* Fazer upload de arquivos para o provedor de documentos externo
* Exibir uma miniatura do documento

**Implementação de referência**

Para ajudar a iniciar rapidamente o desenvolvimento de uma nova implementação de webhooks, o Workfront fornece uma implementação de referência. O código para isso pode ser encontrado em [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) . Essa implementação é baseada em Java e permite que o Workfront conecte documentos em um sistema de arquivos de rede. 

## Versões

* Versão 1.0 (Data de lançamento - maio de 2015): Especificação inicial

* Versão 1.1 (Data de lançamento - junho de 2015). Atualizado /uploadInit - Adição de documentId e documentVersionId

* Versão 1.2 (Data de lançamento - outubro de 2015): Adição de /createFolder

* Versões futuras (Data de lançamento - TBD):

   * Adicionado /delete
   * Adicionado /rename
   * Adição de /serviceInfo
   * Adição de /customAction
   * Adicionar paginação e parentId a /search
