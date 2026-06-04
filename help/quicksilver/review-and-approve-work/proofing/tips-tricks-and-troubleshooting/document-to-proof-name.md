---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: O nome do documento foi alterado após o upload e contém um caractere inválido
description: Determinados documentos não podem ser convertidos em provas.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
TQID: https://experienceleague.adobe.com/bE5iUIG7rFpIIa3zXt-5pO0sgfbEO-3QDVFVLwkayIo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 135
ht-degree: 16%

---

# O nome do documento foi alterado após o upload e contém um caractere inválido

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
