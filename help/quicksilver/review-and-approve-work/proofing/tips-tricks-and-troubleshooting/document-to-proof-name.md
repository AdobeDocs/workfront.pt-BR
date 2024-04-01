---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: O nome do documento alterado após o upload contém um caractere inválido
description: Determinados documentos não podem ser convertidos em provas.
author: Courtney
source-git-commit: a01c2e42dad1a7c00ac73fcaeb1202c56238a8bb
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---


# O nome do documento alterado após o upload contém um caractere inválido

## Problema

Determinados documentos não podem ser convertidos em provas.

## Causa

Os arquivos carregados no Workfront não podem conter determinados caracteres nos nomes de arquivo. Se um arquivo contiver qualquer um dos seguintes caracteres no nome do arquivo, eles serão removidos do nome do arquivo quando ele for carregado: `! # % * \ | ' " / ? < > { } [ ]`.

Se um Nome de documento for atualizado para incluir um caractere inválido após o upload inicial, a geração da prova falhará.

## Solução

Remova o caractere inválido do nome do documento:

1. Selecione o documento e clique em **Detalhes do documento**.
1. Clique no nome do documento, remova o caractere inválido e pressione Enter.

   Caracteres inválidos: `! # % * \ | ' " / ? < > { } [ ]`

   ![](assets/doc-name.png)

1. Atualize a página e gere a prova.