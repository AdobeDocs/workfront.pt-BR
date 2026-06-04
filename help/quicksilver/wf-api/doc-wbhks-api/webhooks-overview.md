---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Visão geral de webhooks
description: Visão geral de webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
TQID: https://experienceleague.adobe.com/5bBLva-jIjwc953MVjAnwo4y0nABq1N0HGDTIurXk40
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 193
ht-degree: 4%

---

# Visão geral de webhooks

Os Webhooks de documentos do Adobe Workfront definem um conjunto de endpoints de API pelos quais o Workfront faz chamadas de API autorizadas para um Provedor de documentos externo. Isso permite que qualquer pessoa crie um plug-in middleware para qualquer provedor de armazenamento de documentos.

![Webhooks](assets/mceclip0-350x262.png)

A experiência do usuário para integrações baseadas em webhook será semelhante àquela das integrações de documento existentes, como Google Drive, Box e Dropbox. Por exemplo, um usuário do Workfront poderá executar as seguintes ações:

* Navegar pela estrutura de pastas do provedor de documentos externos
* Pesquisar arquivos
* Vincular arquivos ao Workfront
* Fazer upload de arquivos para o provedor de documentos externos
* Exibir uma miniatura do documento

Implementação de referência do ****

Para ajudar a iniciar o desenvolvimento de uma nova implementação de webhooks, o Workfront fornece exemplos de uma implementação de referência. Estes exemplos podem ser encontrados em [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Os exemplos são baseados em Java e permitem que o Workfront conecte documentos em um sistema de arquivos de rede. 

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
