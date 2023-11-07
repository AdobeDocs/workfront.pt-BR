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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

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
