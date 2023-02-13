---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: As pastas vinculadas não são compatíveis com o objeto DOCU
description: As pastas vinculadas não são compatíveis com o objeto DOCU
author: Becky
feature: Workfront API
source-git-commit: 9bdc433158e471729bd27d701947d6ae41aa06e7
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---


# Não há suporte para o uso da API para adicionar uma pasta vinculada

Não há suporte para o uso da API para adicionar uma pasta vinculada à matriz de pastas para um objeto de Documento (DOCU). A solicitação será bem-sucedida, mas o documento pode ser removido do sistema por alguns provedores externos. Isso porque o sistema externo será usado como a fonte final da verdade. Portanto, se o documento for removido do provedor externo, o documento será considerado como não existe mais. Os documentos não encontrados na pasta vinculada (externa) podem ser removidos automaticamente de [!DNL Workfront] não tem como recuperá-los.
