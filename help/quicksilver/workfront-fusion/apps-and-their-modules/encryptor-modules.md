---
title: Criptografador
description: Os módulos Adobe Workfront Fusion Encryptor permitem criptografar quaisquer dados de texto. Atualmente, eles oferecem suporte à criptografia de mensagens por meio do AES256 e PGP (OpenPGP).
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Criptografador

[!DNL Adobe Workfront Fusion] [!UICONTROL Criptografador] permitem criptografar quaisquer dados de texto. Atualmente, eles oferecem suporte à criptografia de mensagem por meio do AES256 e PGP ([!UICONTROL OpenPGP]).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td>
  <td> <p>[!UICONTROL Pro] ou superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td>
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Criptografia e descriptografia de mensagens usando PGP

Ao criptografar e descriptografar via PGP, é necessário usar um chaveiro e criar uma chave privada ou pública (ou ambas).

Para obter mais informações sobre chaves públicas e privadas, consulte [Termos básicos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Para obter mais informações sobre chavões, consulte [Teclas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Criptografador] módulos e seus campos

Ao configurar [!UICONTROL Criptografador] , os seguintes campos são exibidos. Um título em negrito em um módulo indica um campo obrigatório.

### Criptografar uma mensagem PGP

Esse módulo permite criptografar uma mensagem usando chaves públicas e privadas.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Chave privada]</td>
        <td>Insira a chave privada do remetente. Isso pode autenticar a identidade do remetente.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Chave pública]</td>
        <td>Insira a chave pública do recipient.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Mensagem]</td>
        <td>Insira a mensagem que deseja criptografar.</td>
    </tr>

### Descriptografar uma mensagem PGP

Esse módulo permite descriptografar uma mensagem usando chaves públicas e privadas.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Chave privada]</td>
        <td>Insira a chave privada do recipient.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Chave pública]</td>
        <td>Insira a chave pública do recipient. Isso pode autenticar a identidade do remetente.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Mensagem]</td>
        <td>Mapeie a mensagem que deseja descriptografar.</td>
    </tr>
</table>
