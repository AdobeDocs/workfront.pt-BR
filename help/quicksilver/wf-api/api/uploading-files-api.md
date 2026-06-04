---
content-type: api
navigation-topic: api-navigation-topic
title: Upload de arquivos por meio da API
description: Upload de arquivos por meio da API
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
TQID: https://experienceleague.adobe.com/Yd7byYJ1pYDXwdKvINXh4fKy-pWoEiNMj345jr1HHNs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 176
ht-degree: 8%

---

# Upload de arquivos por meio da API

É possível fazer upload de arquivos usando APIs do Workfront com ferramentas de API, como o Postman, ou com comandos cURL simples.

Para carregar documentos, consulte as instruções para **Carregar Documentos** no [Comportamento da publicação](/help/quicksilver/wf-api/general/api-basics.md#post-behavior) do Workfront. Você também pode usar essas mesmas instruções para solicitações cURL.

**Ao usar as ferramentas de API para carregar arquivos, siga estas diretrizes:**

* Use a opção da ferramenta API para fazer upload do arquivo. Frequentemente, há um botão **Escolher Arquivo** na tela de solicitação.

* Use o método POST HTTP para fazer a solicitação para carregar o arquivo.

* Sua solicitação deve resultar em uma resposta que inclui um valor para o identificador.

* Use o valor do identificador, o tipo de objeto e o valor da GUID para a objID em uma carga JSON para fazer uma chamada subsequente. Isso é para criar o objeto para o arquivo, como no exemplo a seguir:

```
{
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "1", "fileName" : "TestPDF"},
}
```

Você deve receber uma ID para o objeto na resposta.

Consulte a ajuda da ferramenta de API específica que você está usando para obter mais informações.
