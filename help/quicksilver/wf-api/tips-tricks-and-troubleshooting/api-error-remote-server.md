---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Mensagem de erro de API 400 Solicitação incorreta
description: Mensagem de erro de API 400 Solicitação incorreta
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%

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
