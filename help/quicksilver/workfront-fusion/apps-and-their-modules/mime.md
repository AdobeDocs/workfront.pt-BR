---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos MIME
description: Você pode usar tipos MIME no Adobe Workfront Fusion. Os tipos MIME (Multipurpose Internet Mail Extension) são rótulos que permitem que o software identifique diferentes tipos de dados compartilhados na Internet. Servidores da Web e navegadores usam o tipo MIME para determinar o que deve ser feito com um arquivo. Por exemplo, um arquivo com o tipo MIME text/html será processado em um navegador de forma diferente de um arquivo com o tipo MIME image/jpeg. Os tipos MIME funcionam independentemente do sistema operacional e do hardware.
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# Módulos [!UICONTROL MIME]

Você pode usar tipos MIME no Adobe Workfront Fusion. Os tipos MIME (Multipurpose Internet Mail Extension) são rótulos que permitem que o software identifique diferentes tipos de dados compartilhados na Internet. Servidores da Web e navegadores usam o tipo MIME para determinar o que deve ser feito com um arquivo. Por exemplo, um arquivo com o tipo MIME `text/html` será processado em um navegador de forma diferente de um arquivo com o tipo MIME `image/jpeg`. Os tipos MIME funcionam independentemente do sistema operacional e do hardware.

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
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Módulos [!UICONTROL MIME] e seus campos

### [!UICONTROL Obter um tipo MIME]

Esse módulo de transformador retorna o tipo MIME associado a um determinado nome, caminho ou extensão.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo]</td> 
   <td> <p>Insira ou mapeie o arquivo para o qual você deseja determinar o tipo de MIME. </p> <p>Você pode inserir o arquivo usando:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Caminho do Arquivo]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Nome do Arquivo]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Extensão de Arquivo]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>jpeg</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obter uma extensão de arquivo]

Este módulo de transformador retorna a extensão de arquivo original para um determinado tipo de MIME.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL tipo MIME]</td> 
   <td> <p>Insira ou mapeie o tipo MIME para o qual você deseja determinar a extensão de arquivo. </p> </td> 
  </tr> 
 </tbody> 
</table>
