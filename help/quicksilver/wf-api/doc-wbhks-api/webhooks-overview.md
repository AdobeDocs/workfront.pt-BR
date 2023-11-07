---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Visão geral do Webhooks
description: Visão geral do Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# Visão geral do Webhooks

Os Webhooks de documentos do Adobe Workfront definem um conjunto de endpoints de API pelos quais o Workfront faz chamadas de API autorizadas para um Provedor de documentos externo. Isso permite que qualquer pessoa crie um plug-in middleware para qualquer provedor de armazenamento de documentos.

![](assets/mceclip0-350x262.png)

A experiência do usuário para integrações baseadas em webhook será semelhante àquela das integrações de documento existentes, como Google Drive, Box e Dropbox. Por exemplo, um usuário do Workfront poderá executar as seguintes ações:

* Navegar pela estrutura de pastas do provedor de documentos externos
* Pesquisar arquivos
* Vincular arquivos ao Workfront
* Fazer upload de arquivos para o provedor de documentos externos
* Exibir uma miniatura do documento

**Implementação de referência**

Para ajudar a iniciar o desenvolvimento de uma nova implementação de webhooks, o Workfront fornece exemplos de uma implementação de referência. Esses exemplos podem ser encontrados em [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Os exemplos são baseados em Java e permitem que o Workfront conecte documentos em um sistema de arquivos de rede. 

>[!NOTE]
>
>Os recursos no GitHub são apenas exemplos e não podem executar uma implementação.

## Versões

* Versão 1.0 (Data de lançamento - maio de 2015): especificação inicial

* Versão 1.1 (Data de lançamento - junho de 2015). Atualização de /uploadInit - documentId e documentVersionId adicionados

* Versão 1.2 (Data de lançamento - outubro de 2015): adição de /createFolder

* Versões futuras (Data de lançamento - a ser definida):

   * Adição/exclusão
   * Adição de /rename
   * Adição de /serviceInfo
   * Adição de /customAction
   * Adicionar paginação e parentId a /search
