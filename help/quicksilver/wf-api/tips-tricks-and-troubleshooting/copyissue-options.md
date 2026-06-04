---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configuração de opções para OPTASK copyIssue
description: Uma explicação dos valores inteiros esperados pelo ponto de extremidade copyIssue.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
TQID: https://experienceleague.adobe.com/9cDJFoKl6zqpaAvqzpGqzflcbGZNrAWvEnUAFuqD-Rc
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
source-wordcount: 122
ht-degree: 16%

---

# Configuração de opções para OPTASK copyIssue


Uma das propriedades para uma chamada da API copyIssue é um campo chamado `options`. Este campo espera um número inteiro.

Para incluir uma das seguintes opções, insira o número inteiro correspondente. Para incluir mais de uma opção, insira a soma dos números inteiros correspondentes.

| opção | valor* |
|---|---|
| Limpar atribuições | 2 |
| Limpar progresso | 4 |
| Limpar documentos | 128 |
| Limpar atualizações | 65536 |
| Limpar permissões | 524288 |
| Limpar dados personalizados | 1048576 |

*Todos os valores são potências de 2.

Exemplos:

* Para limpar o progresso ao copiar o problema, insira um valor de `options` de `4`.

* Para limpar o andamento e os documentos, insira um valor de `options` de `132`.

  Limpar progresso = 4

  Limpar documentos = 128

  4 + 128 = 132
