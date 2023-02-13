---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos MIME
description: Você pode usar tipos MIME no Adobe Workfront Fusion. Os tipos MIME (Multipurpose Internet Mail Extension) são rótulos que permitem ao software identificar diferentes tipos de dados compartilhados na Internet. Os servidores e navegadores da Web usam o tipo MIME para determinar o que deve ser feito com um arquivo. Por exemplo, um arquivo com o tipo MIME text/html será processado em um navegador de forma diferente de um arquivo com o tipo MIME image/jpeg. Os tipos MIME funcionam independentemente do sistema operacional e do hardware.
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# [!UICONTROL MIME] módulos

Você pode usar tipos MIME no Adobe Workfront Fusion. Os tipos MIME (Multipurpose Internet Mail Extension) são rótulos que permitem ao software identificar diferentes tipos de dados compartilhados na Internet. Os servidores e navegadores da Web usam o tipo MIME para determinar o que deve ser feito com um arquivo. Por exemplo, um arquivo com o tipo MIME `text/html` será processado em um navegador de forma diferente de um arquivo com o tipo MIME `image/jpeg`. Os tipos MIME funcionam independentemente do sistema operacional e do hardware.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> <p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL MIME] módulos e seus campos

### [!UICONTROL Obter um tipo MIME]

Esse módulo transformador retorna o tipo MIME associado a um determinado nome, caminho ou extensão.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo]</td> 
   <td> <p>Insira ou mapeie o arquivo para o qual deseja determinar o tipo MIME. </p> <p>É possível inserir o arquivo usando:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Caminho do arquivo]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Nome do arquivo]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Extensão de arquivo]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>jpeg</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obter uma extensão de arquivo]

Esse módulo transformador retorna a extensão de arquivo original para um determinado tipo MIME.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL tipo MIME]</td> 
   <td> <p>Insira ou mapeie o tipo MIME para o qual deseja determinar a extensão de arquivo. </p> </td> 
  </tr> 
 </tbody> 
</table>
