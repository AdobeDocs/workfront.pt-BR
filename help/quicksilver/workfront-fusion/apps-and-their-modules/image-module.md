---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de imagem
description: Os módulos de Imagem do Adobe Workfront Fusion permitem obter informações sobre uma imagem específica (dimensões, tipo e assim por diante), converter uma imagem para outro formato de arquivo e alterar diretamente o tamanho da imagem.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Módulos de imagem

[!DNL Adobe Workfront Fusion] [!UICONTROL Imagem] os módulos permitem obter informações sobre uma imagem específica (dimensões, tipo e assim por diante), converter uma imagem para outro formato de arquivo e alterar diretamente o tamanho da imagem.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Imagem] módulos e seus campos

Ao configurar esse módulo, os seguintes campos são exibidos. Um título em negrito em um módulo indica um campo obrigatório.

* [[!UICONTROL Redimensionar]](#resize)
* [[!UICONTROL Converter um formato]](#convert-a-format)
* [[!UICONTROL Extrair metadados]](#extract-metadata)

### [!UICONTROL Redimensionar]

Esse módulo transformador altera a altura e a largura de uma imagem de acordo com os critérios que você especificar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione a fonte da imagem que deseja converter. Você pode selecionar saída de um módulo anterior ou mapear o arquivo de dados e o nome do arquivo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dados]</td> 
   <td>Mapeie o arquivo que deseja converter. Este campo estará disponível se você tiver selecionado o [!UICONTROL Map] no campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do arquivo]</td> 
   <td>Insira um nome para o arquivo convertido. Este campo estará disponível se você tiver selecionado o [!UICONTROL Map] no campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL I want to]</td> 
   <td>Selecione se deseja manter a relação altura-largura ou alterar as dimensões para uma altura e largura especificadas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL de acordo]</td> 
   <td> <p>Selecione como deseja que o módulo determine o novo tamanho da imagem. Este campo será exibido se você tiver selecionado a manutenção da taxa de largura de altura no campo I want to . Outros campos são exibidos com base na seleção neste campo.</p> 
    <ul> 
     <li> <p>[!UICONTROL Largura máxima]</p> <p>Reduz uma imagem para uma largura especificada. A altura é calculada automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altura máxima]</p> <p>Reduz uma imagem para uma altura especificada. A largura é calculada automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altura ou largura máxima]</p> <p>Reduz uma imagem de forma que sua altura e largura não excedam os valores especificados. Como essa opção mantém a relação altura-largura, uma das dimensões pode ser menor do que o especificado. Por exemplo, se a altura e a largura forem especificadas como 40, uma imagem 400x300 será reduzida para 40X30.</p> </li> 
     <li> <p>[!UICONTROL Largura mínima]</p> <p>Amplia uma imagem para uma largura especificada. A altura é calculada automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altura mínima]</p> <p>Amplia uma imagem para uma altura especificada. A largura é calculada automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altura ou largura mínima]</p> <p>Amplia uma imagem de forma que sua altura e largura não sejam menores do que os valores especificados. Como essa opção mantém a relação altura-largura, uma das dimensões pode ser maior do que o especificado. Por exemplo, se a altura e a largura forem especificadas como 300, uma imagem 40x30 será ampliada para 400X300.</p> </li> 
     <li> <p>[!UICONTROL Porcentagem]</p> <p>Altera o tamanho da imagem em uma porcentagem com base no valor especificado. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Largura]</td> 
   <td>Insira ou mapeie a largura desejada da imagem redimensionada em pixels.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Altura]</td> 
   <td>Insira ou mapeie a altura desejada da imagem redimensionada em pixels.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converter um formato]

Esse módulo transformador altera o formato de um arquivo de imagem. Esse módulo é compatível com os seguintes formatos:

* Imagem PNG
* JPG
* GIF
* BMP

O arquivo de origem e a saída devem estar em um desses formatos. Por exemplo, a variável [!UICONTROL Imagem] >[!UICONTROL Converter um formato] pode transformar um arquivo PNG em um arquivo BMP ou um BMP em um JPG.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione a fonte da imagem que deseja converter. Você pode selecionar saída de um módulo anterior ou mapear o arquivo de dados e o nome do arquivo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dados]</td> 
   <td>Mapeie o arquivo que deseja converter. Este campo estará disponível se você tiver selecionado o [!UICONTROL Map] no campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do arquivo]</td> 
   <td>Insira um nome para o arquivo convertido. Este campo estará disponível se você tiver selecionado o [!UICONTROL Map] no campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de saída]</td> 
   <td>Selecione o formato para o qual você deseja que o módulo converta o arquivo de origem. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extrair metadados]

Esse módulo transformador retorna informações básicas sobre um módulo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione a fonte da imagem que deseja converter. Você pode selecionar saída de um módulo anterior ou mapear o arquivo de dados e o nome do arquivo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dados]</td> 
   <td>Mapeie o arquivo que deseja converter. Este campo estará disponível se você tiver selecionado Mapa no campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do arquivo]</td> 
   <td>Insira um nome para o arquivo convertido. Este campo estará disponível se você tiver selecionado Mapa no campo [!UICONTROL Source file].</td> 
  </tr> 
 </tbody> 
</table>

## Possíveis problemas

### Ação finalizada com um erro

Há três casos em que uma ação pode terminar com um erro:

* Os dados recebidos não estavam no formato JPG/GIF/PNG/BMP
* O limite máximo de largura/altura foi excedido ao alterar as dimensões da imagem. O tamanho da imagem não deve exceder a largura de 3840 px e a altura de 2160 px
* O tamanho máximo permitido de uma imagem foi excedido ao alterar as dimensões ou o formato da imagem.
