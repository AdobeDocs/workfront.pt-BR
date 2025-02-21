---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: O nome do documento alterado após o upload contém um caractere inválido
description: Determinados documentos não podem ser convertidos em provas.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '135'
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

1. Selecione o documento e clique em **Detalhes do Documento**.
1. Clique no nome do documento, remova o caractere inválido e pressione Enter.

   Caracteres inválidos: `! # % * \ | ' " / ? < > { } [ ]`

   ![Nome do documento](assets/doc-name.png)

1. Atualize a página e gere a prova.
