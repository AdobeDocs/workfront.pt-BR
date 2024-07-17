---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configuração de opções para OPTASK copyIssue
description: Uma explicação dos valores inteiros esperados pelo ponto de extremidade copyIssue.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 4%

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
