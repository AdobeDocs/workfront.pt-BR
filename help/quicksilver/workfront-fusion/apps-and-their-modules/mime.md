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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# [!UICONTROL MIME] módulos

Você pode usar tipos MIME no Adobe Workfront Fusion. Os tipos MIME (Multipurpose Internet Mail Extension) são rótulos que permitem que o software identifique diferentes tipos de dados compartilhados na Internet. Servidores da Web e navegadores usam o tipo MIME para determinar o que deve ser feito com um arquivo. Por exemplo, um arquivo com o tipo MIME `text/html` serão processados em um navegador de forma diferente de um arquivo com tipo MIME `image/jpeg`. Os tipos MIME funcionam independentemente do sistema operacional e do hardware.

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

## [!UICONTROL MIME] módulos e seus campos

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
     <li> <p><strong>[!UICONTROL Caminho do arquivo]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Nome do arquivo]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>image.jpeg</p> </li> 
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
