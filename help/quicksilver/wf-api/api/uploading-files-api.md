---
content-type: api
navigation-topic: api-navigation-topic
title: Upload de arquivos por meio da API
description: Upload de arquivos por meio da API
author: John
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 03df0ad329255e86780c03bbb4541e0a0a526381
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Upload de arquivos por meio da API

Você pode fazer upload de arquivos usando APIs do Workfront com ferramentas de API, como Postman, ou com comandos cURL simples.

Para fazer upload de documentos, consulte as instruções para **Fazer upload de documentos** no Workfront [Comportamento da publicação](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWF_API%2FGeneral%2Fapi-basics.html). Também é possível usar essas mesmas instruções para solicitações de cURL.

**Ao usar ferramentas de API para fazer upload de arquivos, siga estas diretrizes:**

* Use a opção da ferramenta de API para carregar o arquivo. Geralmente, essa é uma **Escolher arquivo** na tela de solicitação.

* Use o método POST HTTP para fazer a solicitação para fazer upload do arquivo.

* Sua solicitação deve resultar em uma resposta que inclua um valor para seu identificador.

* Use o valor de identificador, o tipo de objeto e o valor de GUID para objID em uma carga JSON para fazer uma chamada subsequente. Isso é para criar o objeto para o arquivo, como no exemplo a seguir:

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

Você deve receber uma ID para o objeto na resposta.

Consulte a ajuda da ferramenta de API específica que você está usando para obter mais informações.
