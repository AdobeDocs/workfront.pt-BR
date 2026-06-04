---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Recuperar informações de moeda de um projeto quando a moeda for nula
description: Recuperar informações de moeda de um projeto quando a moeda for nula
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
TQID: https://experienceleague.adobe.com/fWBcEeqoJFK6WzcEE2Ajqv6cdxk0J9IN1CiPPGU6pIg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 9%

---

# Recuperar informações de moeda de um projeto quando a moeda for nula (não atribuída)

O objeto de projeto com o campo de moeda pode ser recuperado usando a seguinte solicitação:

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

Isso retornaria o seguinte corpo de resposta:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

Se a moeda não for definida para o projeto, essa resposta incluirá uma moeda com o valor `null`:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

Se você precisar da moeda para o projeto (como para cálculos), poderá recuperar a moeda padrão para o cliente:

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

A resposta inclui a moeda que o usuário definiu como padrão, que seria usada por qualquer projeto para esse cliente que não tem a moeda definida:

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```
