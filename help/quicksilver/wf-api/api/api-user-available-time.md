---
content-type: api
navigation-topic: wf-api
title: Obter API de tempo disponível dos usuários
description: Obter API de tempo disponível dos usuários
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
TQID: https://experienceleague.adobe.com/JPvalH2RQRfMeqbYyWXyjyXCx-bdaZwRoR6WDRerZ5U
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 95
ht-degree: 4%

---

# API de tempo disponível dos usuários

**URI: attask/api/v15.0/user/getUsersAvailableTime**

O ponto de extremidade de tempo disponível do usuário recupera dados sobre o tempo disponível do usuário. Isso permite integrações para agregação de dados de acordo com atributos do usuário e intervalos de tempo.

## Exemplo de solicitação

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Parâmetros de solicitação

* **userIDs**: matriz de cadeias de caracteres. Obrigatório. Exemplo: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. string. Obrigatório. Exemplo: `"2022-07-10T00:00:00"`.

* **toDate**: datetime. string. Obrigatório. Exemplo `"2022-07-20T23:59:59"`.

## Exemplo de resposta:

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}
```

## Parâmetros de resposta

* **AVL**: horas disponíveis reais. Matriz de números.
* **PAVL**: horas puramente disponíveis para agendamento que não inclui dias não úteis ou folga do usuário. String.
