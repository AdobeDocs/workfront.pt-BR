---
title: Criptografador
description: Os módulos do Adobe Workfront Fusion Encryptor permitem criptografar quaisquer dados de texto. Atualmente, eles suportam criptografia de mensagens via AES256 e PGP (OpenPGP).
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Criptografador

[!DNL Adobe Workfront Fusion] [!UICONTROL Criptografador] Os módulos do permitem criptografar quaisquer dados de texto. Atualmente, eles são compatíveis com a criptografia de mensagens via AES256 e PGP ([!UICONTROL OpenPGP]).

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
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Criptografia e descriptografia de mensagens usando PGP

Ao criptografar e descriptografar via PGP, é necessário usar um chaveiro e criar uma chave privada ou pública (ou ambas).

Para obter mais informações sobre chaves públicas e privadas, consulte [Termos básicos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Para obter mais informações sobre chaveiros, consulte [Chaves em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Criptografador] módulos e seus campos

Ao configurar [!UICONTROL Criptografador] , os campos a seguir serão exibidos. Um título em negrito em um módulo indica um campo obrigatório.

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
        <td>Informe a mensagem que deseja criptografar.</td>
    </tr>

### Descriptografar uma mensagem PGP

Este módulo permite descriptografar uma mensagem usando chaves públicas e privadas.

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
