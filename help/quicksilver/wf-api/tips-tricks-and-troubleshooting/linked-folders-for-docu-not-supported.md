---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Pastas vinculadas não têm suporte para o objeto DOCU
description: Pastas vinculadas não têm suporte para o objeto DOCU
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
TQID: https://experienceleague.adobe.com/iPjiffn9QLDldjWRdxMyf8RTaZaB9X6axc7UVY1B3Bg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 118
ht-degree: 9%

---

# Não há suporte para o uso da API para adicionar uma pasta vinculada

Não há suporte para o uso da API para adicionar uma pasta vinculada à matriz de pastas para um objeto Documento (DOCU). A solicitação será bem-sucedida, mas o documento poderá ser removido do sistema por alguns provedores externos. Isso ocorre porque o sistema externo será usado como a fonte final da verdade. Portanto, se o documento for removido do provedor externo, ele será considerado como não existindo mais. Qualquer documento não encontrado na pasta vinculada (externa) pode ser removido automaticamente de [!DNL Workfront] sem nenhuma maneira de recuperá-lo.
