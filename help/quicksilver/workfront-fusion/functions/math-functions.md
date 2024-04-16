---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funções matemáticas no Adobe Workfront Fusion
description: As seguintes funções matemáticas estão disponíveis no painel Mapeamento do Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# Funções matemáticas em [!DNL Adobe Workfront Fusion]

<!--Audited: 4/2024-->

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plano</td>  
   <td> <p>Qualquer</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licença</td>  
   <td> <p>Novo: [!UICONTROL Padrão]</p><p>Ou</p><p>Atual: [!UICONTROL Trabalho] ou superior</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td>  
   <td> 
   <p>Atual: Não [!DNL Workfront Fusion] requisito de licença.</p> 
   <p>Ou</p> 
   <p>Herdados: Qualquer um </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produto</td>  
   <td> 
   <p>Novo:</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] Plano: sua organização deve comprar [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plano: [!DNL Workfront Fusion] está incluído.</li></ul> 
   <p>Ou</p> 
   <p>Atual: sua organização deve comprar [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
>   Devoluções 2
>
>* `ceil(` `4` `)`
>
>   Devoluções 4

## [!UICONTROL andar (número)]

Retorna o maior inteiro menor ou igual a um número especificado.

>[!INFO]
>
>**Exemplos:**
>
>* `floor(` `1.2` `)`
>
>   Devoluções 1
>
>* `floor(` `1.9` `)`
>
>   Devoluções 1
>
>* `floor(` `4` `)`
>
>   Devoluções 4

## [!UICONTROL máx ([matriz de valores]), max(valor1;valor2; ...)]

Retorna o maior número em uma matriz especificada ou o maior número entre os números inseridos individualmente.

## [!UICONTROL min ([matriz de valores]), min(valor1; valor2; ...)]

Retorna o menor número em uma matriz especificada ou o menor número entre os números inseridos individualmente.

## [!UICONTROL round (número)]

Arredonda um valor numérico para o número inteiro mais próximo.

>[!INFO]
>
>**Exemplos:**
>
>* `round(` `1.2` `)`
>
>   Devoluções 1
>
>* `round(` `1.5` `)`
>
>   Devoluções 2
>
>* `round(` `1.7` `)`
>
>   Devoluções 2
> 
>* `round(` `2` `)`
>
>   Devoluções 2

## [!UICONTROL soma ([matriz de valores]), sum(valor1; valor2; ...)]

Retorna a soma dos valores em uma matriz especificada ou a soma dos números inseridos individualmente.

## [!UICONTROL parseNumber (número; separador decimal)]

Analisa uma string com um número e retorna o número. Por exemplo, parseNumber(1 756,456;,)

## [!UICONTROL formatNumber (número; pontos decimais; [separadorDecimal]; [SeparadorMilhares])]

Retorna um número no formato solicitado. Por padrão, o ponto decimal é uma vírgula (,) e o separador de milhares é um ponto (.).

>[!INFO]
>
>**Exemplo:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Retorna 123.456.789.000
