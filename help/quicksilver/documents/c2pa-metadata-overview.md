---
product-area: documents
navigation-topic: documents-navigation-topic
title: Metadados C2PA no Adobe Workfront
description: Saiba o que são metadados C2PA e como o Adobe Workfront os preserva nos documentos carregados, armazenados e baixados.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 3510218fb179a0852ad22abe2a753ccdb261205a
workflow-type: tm+mt
source-wordcount: 215
ht-degree: 0%

---

# Metadados C2PA no Adobe Workfront

Os metadados C2PA são informações seguras e invioláveis que viajam com um conteúdo. Quando a IA gerativa (GenAI) é usada para criar ou alterar uma imagem, vídeo ou arquivo de áudio, os metadados do C2PA registram esse fato para que qualquer pessoa que receba o arquivo possa ver como ele foi feito.

Os metadados C2PA são baseados no padrão [C2PA](https://c2pa.org/) aberto.

## O que os metadados C2PA contêm

Os metadados C2PA incluem:

* O nome do provedor que forneceu a ferramenta GenAI.
* O nome e o número da versão do sistema GenAI usado para criar ou alterar o conteúdo.
* A data e a hora em que o conteúdo foi criado ou alterado.
* Um identificador exclusivo.

Os metadados C2PA não incluem informações de identificação pessoal (PII).

## Como o Workfront lida com metadados C2PA

O Adobe Workfront não modifica os metadados dos arquivos com os quais você trabalha. Ao fazer upload de um arquivo que já tem metadados C2PA, o Workfront preserva essas informações inalteradas, pois o arquivo é armazenado e baixado do Workfront.

Como os metadados são incorporados ao próprio arquivo, eles permanecem intactos por meio dos fluxos de trabalho do Workfront, de modo que as informações de origem permanecem com o conteúdo quando saem do Workfront.
