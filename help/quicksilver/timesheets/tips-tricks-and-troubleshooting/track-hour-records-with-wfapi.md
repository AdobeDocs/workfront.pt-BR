---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Rastrear registros de horas com a API do Adobe Workfront
description: Se sua organização usar o Adobe Workfront para inserir horas trabalhadas, mas usar outra ferramenta como o sistema de registro para esses dados, você poderá usar a API do Workfront para sincronizar dados entre os dois sistemas.
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Rastrear registros de horas com a API do Adobe Workfront

Se sua organização usar o Adobe Workfront para inserir horas trabalhadas, mas usar outra ferramenta como o sistema de registro para esses dados, você poderá usar a API do Workfront para sincronizar dados entre os dois sistemas.

O simples rastreamento do registro de hora não é viável porque, se a entrada de hora for removida, o registro inteiro será excluído, o que exige que você extraia o conjunto de dados inteiro e o compare ao conjunto de dados antigo. Felizmente, todas as transações de hora são registradas nas Entradas de Lançamento da Workfront.

Após recuperar um conjunto inicial de todas as horas atuais no sistema, é possível rastrear qualquer e todas as alterações por meio das Entradas de Lançamento.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HORA",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2": "Brad Littler",<br>"newNumberVal": null,<br>"oldNumberVal": 1,<br>"subObjCode": "HORA",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f008db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HORA",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Littler",<br>"newNumberVal": 2,<br>"oldNumberVal": 1,<br>"subObjCode": "HORA",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>Veja a seguir uma descrição dos campos incluídos:

* **changeType:** O tipo de alteração que está sendo feita no objeto:

   * **A:** Adicionar

   * **E:** Editar

   * **D:** Excluir

* **aux2:** O nome do usuário para o qual o registro de hora é.

* **newNumberVal:** Novo valor do registro de hora (Isso será nulo se o changeType for D).

* **oldNumberVal:** Valor anterior do registro de hora.

* **subObjCode:** Tipo de registro sendo modificado (deve sempre ser HORA).

* **subObjID:** ID do registro de Hora.

Você pode usar essas informações para descobrir quais registros de hora foram alterados, editados ou excluídos. Em seguida, você pode usar o subObjID para recuperar mais informações dos registros de hora, se necessário.
