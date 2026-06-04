---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Tratamento de erros de webhooks de documentos
description: Tratamento de erros de webhooks de documentos
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
TQID: https://experienceleague.adobe.com/KoMJXXZbDdywLGIwYTu7o8GigPxQ5RG6sNQpOTMHWY0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 123
ht-degree: 9%

---

# Tratamento de erros de webhooks de documentos

Problemas podem surgir ao processar solicitações de API. Isso deve ser tratado de forma consistente em todos os endpoints da API. Quando ocorre um erro, o provedor de webhook deve incluir um código de erro no cabeçalho de resposta. Os códigos de erro incluem:

* 403 - Proibido. Indica que os tokens de solicitação estão ausentes ou são inválidos, ou que as credenciais associadas aos tokens não têm acesso ao recurso especificado. Para provedores de webhook baseados em OAuth, o Adobe Workfront tentará recuperar novos tokens de acesso.

* 404 - Não encontrado. Indica que o arquivo ou pasta especificada não existe.

* 500 - Erro interno do servidor. Qualquer outro tipo de erro.

* Descrição do erro no corpo da resposta usando o seguinte formato:

  ```
  {status: "error"
   error: "Sample error message"}
  ```
