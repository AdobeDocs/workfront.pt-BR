---
title: Criptografador
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Criptografador

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Criptografador](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/encryptor-modules.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Os módulos [!DNL Adobe Workfront Fusion] [!UICONTROL Criptografador] permitem criptografar quaisquer dados de texto. Atualmente, eles oferecem suporte à criptografia de mensagens via AES256 e PGP ([!UICONTROL OpenPGP]).

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
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Criptografia e descriptografia de mensagens usando PGP

Ao criptografar e descriptografar via PGP, é necessário usar um chaveiro e criar uma chave privada ou pública (ou ambas).

Para obter mais informações sobre chaves públicas e privadas, consulte [Termos básicos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Para obter mais informações sobre chaveiros, consulte [Chaves em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Módulos {Encryptor] e seus campos

Ao configurar os módulos do [!UICONTROL Encryptor], os campos a seguir são exibidos. Um título em negrito em um módulo indica um campo obrigatório.

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
