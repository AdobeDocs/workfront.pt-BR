---
content-type: api
navigation-topic: api-navigation-topic
title: Upload de arquivos por meio da API
description: Upload de arquivos por meio da API
author: Becky
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 3db01c329c005570b782ae3445f83b7c44ced676
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Upload de arquivos por meio da API

Você pode fazer upload de arquivos usando APIs do Workfront com ferramentas de API, como o Postman, ou com comandos cURL simples.

Para fazer upload de documentos, consulte as instruções de **Carregando Documentos** no Workfront [Comportamento da publicação](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). Você também pode usar essas mesmas instruções para solicitações cURL.

**Ao usar ferramentas de API para fazer upload de arquivos, siga estas diretrizes:**

* Use a opção da ferramenta API para fazer upload do arquivo. Muitas vezes, trata-se de uma **Escolher arquivo** na tela de solicitação.

* Use o método HTTP POST para fazer a solicitação para carregar o arquivo.

* Sua solicitação deve resultar em uma resposta que inclui um valor para o identificador.

* Use o valor do identificador, o tipo de objeto e o valor da GUID para a objID em uma carga JSON para fazer uma chamada subsequente. Isso é para criar o objeto para o arquivo, como no exemplo a seguir:

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
