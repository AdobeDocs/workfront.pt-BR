---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Rastrear registros de horas com a API do Adobe Workfront
description: Se sua organização usar o Adobe Workfront para inserir horas trabalhadas, mas usar outra ferramenta como sistema de registro desses dados, você poderá usar a API do Workfront para sincronizar dados entre os dois sistemas.
author: Lisa
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Rastrear registros de horas com a API do Adobe Workfront

Se sua organização usar o Adobe Workfront para inserir horas trabalhadas, mas usar outra ferramenta como sistema de registro desses dados, você poderá usar a API do Workfront para sincronizar dados entre os dois sistemas.

O simples rastreamento do registro de horas não é viável porque, se a entrada de horas for removida, o registro inteiro será excluído, exigindo que você extraia todo o conjunto de dados e o compare ao conjunto de dados antigo. Felizmente, todas as transações de horas são registradas em Lançamentos do Workfront.

Depois de recuperar um conjunto inicial de todas as horas atuais no sistema, você pode rastrear todas as alterações por meio das Entradas do diário.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": nulo,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2": "Brad Littler",<br>"newNumberVal": nulo,<br>"oldNumberVal": "sub",<br> "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f008db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": nulo,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"LitjLECode": 2,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}<br><br><br><br></pre>Veja a seguir uma descrição dos campos incluídos:

* **changeType:** O tipo de alteração que está sendo feita no objeto:

   * **A:** Adicionar

   * **E:** Editar

   * **D:** Excluir

* **aux2:** o nome do usuário para o qual o registro de hora é.

* **newNumberVal:** Novo valor do registro de hora (será nulo se changeType for D).

* **oldNumberVal:** Valor anterior do registro de hora.

* **subObjCode:** Tipo de registro que está sendo modificado (sempre deve ser HORA).

* **subObjID:** ID do registro de Hora.

É possível usar essas informações para descobrir quais registros de horas foram alterados, editados ou excluídos. Em seguida, você pode usar o subObjID para recuperar mais informações dos registros de horas, se necessário.
