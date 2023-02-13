---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configuração de opções para OPTASK copyIssue
description: Uma explicação dos valores inteiros esperados pelo ponto de extremidade copyIssue.
author: Becky
feature: Workfront API
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 93a67b3dbd59f188dad6b060ec93c3f137c981b2
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 6%

---

# Configuração de opções para OPTASK copyIssue


Uma das propriedades de uma chamada à API copyIssue é um campo chamado `options`. Este campo espera um número inteiro.

Para incluir uma das opções a seguir, insira o número inteiro correspondente. Para incluir mais de uma opção, insira a soma dos números inteiros correspondentes.

| opção | value* |
|---|---|
| Limpar atribuições | 2 |
| Limpar progresso | 4 |
| Limpar documentos | 128 |
| Limpar atualizações | 65536 |
| Limpar permissões | 524288 |
| Limpar dados personalizados | 1048576 |

*Todos os valores são poderes de 2.

Exemplos:

* Para apagar o progresso ao copiar o problema, insira um `options` valor de `4`.

* Para limpar o progresso e os documentos, insira um `options` valor de `132`.

   Limpar progresso = 4

   Limpar documentos = 128

   4 + 128 = 132
