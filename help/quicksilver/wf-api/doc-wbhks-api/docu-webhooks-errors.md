---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Tratamento de Erros de Webhooks de Documentos
description: Tratamento de Erros de Webhooks de Documentos
author: John
feature: Workfront API
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 338cc745a7660ffed8e4d44e19dcadfdc13bc345
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# Tratamento de Erros de Webhooks de Documentos

Problemas podem surgir ao processar solicitações de API. Isso deve ser feito de maneira consistente em todos os pontos de extremidade da API. Quando ocorre um erro, o provedor do webhook deve incluir um código de erro no cabeçalho de resposta. Os códigos de erro incluem:

* 403 - Proibido. Indica que os tokens de solicitação estão ausentes ou são inválidos ou que as credenciais associadas aos tokens não têm acesso ao recurso especificado. Para provedores de webhook baseados em OAuth, a Adobe Workfront tentará recuperar novos tokens de acesso.

* 404 - Não encontrado. Indica que o arquivo ou pasta especificado não existe.

* 500 - Erro interno do servidor. Qualquer outro tipo de erro.

* Descrição do erro no corpo da resposta usando o seguinte formato:

   ```
   {status: “error”
    error: “Sample error message”}
   ```
