---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Recuperar informações de moeda de um projeto quando a moeda for nula
description: Recuperar informações de moeda de um projeto quando a moeda for nula
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

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
