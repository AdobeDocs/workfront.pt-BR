---
content-type: api
navigation-topic: wf-api
title: Obter API de tempo disponível dos usuários
description: Obter API de tempo disponível dos usuários
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 0%

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
