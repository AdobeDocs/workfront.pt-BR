---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funções matemáticas no Adobe Workfront Fusion
description: As seguintes funções matemáticas estão disponíveis no painel de mapeamento do Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# Funções matemáticas em [!DNL Adobe Workfront Fusion]

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL média ([matriz de valores]) average(value1; [value2], ...)]

Retorna o valor médio dos valores numéricos em uma matriz específica ou o valor médio dos valores numéricos inseridos individualmente.

## [!UICONTROL ceil (número)]

Retorna o menor inteiro maior ou igual a um número especificado.

>[!INFO]
>
>**Exemplos:**
>
>* `ceil(` `1.2` `)`
   >
   >   Retorna 2
>
>* `ceil(` `4` `)`
   >
   >   Retorna 4


## [!UICONTROL piso (número)]

Retorna o maior inteiro menor que ou igual a um número especificado.

>[!INFO]
>
>**Exemplos:**
>
>* `floor(` `1.2` `)`
   >
   >   Retorna 1
>
>* `floor(` `1.9` `)`
   >
   >   Retorna 1
>
>* `floor(` `4` `)`
   >
   >   Retorna 4


## [!UICONTROL formatNumber (número; pontos decimais; [decimalSeparator]; [milharesSeparator])]

Retorna um número no formato solicitado. Por padrão, o ponto decimal é uma vírgula (,) e o separador de milhar é um ponto final (.).

>[!INFO]
>
>**Exemplo:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Retorna 123.456.789.000

## [!UICONTROL max ([matriz de valores]), max(value1; value2; ...)]

Retorna o maior número em uma matriz especificada ou o maior número entre os números inseridos individualmente.

## [!UICONTROL min ([matriz de valores]), min(valor1; valor2; ...)]

Retorna o menor número em uma matriz especificada ou o menor número entre os números inseridos individualmente.

## [!UICONTROL parseNumber (número; separador decimal)]

Analisa uma string com um número e retorna o número. Por exemplo, parseNumber(1 756,456;,)

## [!UICONTROL round (número)]

Arredonda um valor numérico para o número inteiro mais próximo.

>[!INFO]
>
>**Exemplos:**
>
>* `round(` `1.2` `)`
   >
   >   Retorna 1
>
>* `round(` `1.5` `)`
   >
   >   Retorna 2
>
>* `round(` `1.7` `)`
   >
   >   Retorna 2
> 
>* `round(` `2` `)`
   >
   >   Retorna 2


## [!UICONTROL soma ([matriz de valores]), sum(value1; valor2; ...)]

Retorna a soma dos valores em uma matriz especificada ou a soma dos números inseridos individualmente.
