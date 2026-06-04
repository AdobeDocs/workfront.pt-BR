---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Mensagem de erro de API 400 Solicitação incorreta
description: Mensagem de erro de API 400 Solicitação incorreta
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
TQID: https://experienceleague.adobe.com/19PIdv4u8de0BlasXD0Yy6GssO3vv6Jt8BzcljB-m1w
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
source-wordcount: 93
ht-degree: 2%

---

# Erro de API: &quot;O servidor remoto retornou um erro (400) Solicitação inválida&quot;

## Problema

Você recebe o seguinte erro ao tentar usar a API para importar um campo personalizado para um problema:

`The remote server returned an error: (400) Bad Request`

## Causa

Esse erro ocorre ao tentar importar, por meio da API, um campo personalizado de um projeto que não tem um formulário personalizado associado a um Tópico da fila.

## Solução

Adicione o formulário personalizado correto ao Tópico da fila.

Para saber mais sobre Tópicos da Fila, consulte [Criar Tópicos da Fila](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
