---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Pastas vinculadas não têm suporte para o objeto DOCU
description: Pastas vinculadas não têm suporte para o objeto DOCU
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# Não há suporte para o uso da API para adicionar uma pasta vinculada

Não há suporte para o uso da API para adicionar uma pasta vinculada à matriz de pastas para um objeto Documento (DOCU). A solicitação será bem-sucedida, mas o documento poderá ser removido do sistema por alguns provedores externos. Isso ocorre porque o sistema externo será usado como a fonte final da verdade. Portanto, se o documento for removido do provedor externo, ele será considerado como não existindo mais. Os documentos não encontrados na pasta vinculada (externa) podem ser removidos automaticamente do [!DNL Workfront] sem como recuperá-los.
