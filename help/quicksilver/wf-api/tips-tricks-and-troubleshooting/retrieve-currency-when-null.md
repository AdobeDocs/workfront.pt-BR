---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Recuperar informações de moeda de um projeto quando a moeda for nula
description: Recuperar informações de moeda de um projeto quando a moeda for nula
author: Becky
feature: Workfront API
source-git-commit: a9af457793e123a60172fe4baf5ae5def472b026
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Recuperar informações de moeda de um projeto quando a moeda for nula (não atribuída)

O objeto do projeto com o campo de moeda pode ser recuperado usando a seguinte solicitação:

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

Se a moeda não estiver definida para o projeto, essa resposta incluirá uma moeda com o valor `null`:

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

Se você precisar da moeda do projeto (como para cálculos), poderá recuperar a moeda padrão do cliente:

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

A resposta inclui a moeda que o usuário definiu como padrão, que seria usada por quaisquer projetos para esse cliente que não tivessem a moeda definida:

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
