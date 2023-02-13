---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funções de storage no Adobe Workfront Fusion
description: As seguintes funções de matriz estão disponíveis no painel de mapeamento do Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Funções de storage no Adobe Workfront Fusion

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

## [!UICONTROL add (array; valor1; valor2; ...)]

Adiciona valores especificados em parâmetros a uma matriz e retorna essa matriz.

## [!UICONTROL contém (matriz; value)]

Verifica se uma matriz contém o valor .

## [!UICONTROL distinct (array; [key])]

Remove duplicatas dentro de uma matriz. Use o &quot;[!UICONTROL key]&quot; para acessar propriedades dentro de objetos complexos. Para acessar propriedades aninhadas, use a notação de pontos. O primeiro item em uma matriz é o índice 1.

>[!INFO]
>
>**Exemplo:** `distinct(Contacts[];name)`
>
>Remove duplicatas dentro de uma matriz de contatos comparando a propriedade &quot;name&quot;

## [!UICONTROL flatten (matriz)]

Cria uma nova matriz com todos os elementos de submatriz concatenados nela, recursivamente, até a profundidade especificada.


## [!UICONTROL join (array); separador)]

Concatena todos os itens de uma matriz em uma string, usando o separador especificado entre cada item.

## [!UICONTROL chaves (objeto)]

Retorna uma matriz das propriedades de um determinado objeto ou matriz.

## [!UICONTROL length (matriz)]

Retorna o número de itens em uma matriz.

## [!UICONTROL mapa (matriz complexa; chave;[chave para filtragem];[valores possíveis para filtrar])]

Retorna uma matriz primitiva contendo valores de uma matriz complexa. Essa função permite filtrar valores. Use nomes de variáveis brutos para chaves.

>[!INFO]
>
>**Exemplos:**
>
>* `map(Emails[];email)`
  >
>  Retorna uma matriz primitiva com emails
>
>* `map(Emails[];email;label;work;home)`
  >
>  Retorna uma matriz primitiva com emails com um rótulo igual a trabalho ou casa

Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL mesclar (array1; array2; ...)]

Mescla uma ou mais matrizes em uma matriz.

## [!UICONTROL remover (matriz; valor1; valor2; ...)]

Remove valores especificados nos parâmetros de uma matriz. Essa função só é eficaz em arrays primitivos de texto ou números.

## [!UICONTROL inverso (matriz)]

O primeiro elemento da matriz se torna o último elemento, o segundo se torna o próximo a último e assim por diante.

## [!UICONTROL fatia (matriz; Início; [end])]

Retorna uma nova matriz contendo apenas itens selecionados.

## [!UICONTROL classificação (matriz; [pedido]; [key])]

Classifica valores de uma matriz. Os valores válidos da variável `order` são:

* `asc`

   (padrão) - ordem crescente: 1, 2, 3, ... para o tipo Número. A, B, C, a, b, c, ... para o tipo de texto

* `desc`

   ordem decrescente: ..., 3, 2, 1 para o tipo Número. ..., c, b, a, C, B, A para texto do tipo.

* `asc ci`

   ordem crescente não diferencia maiúsculas de minúsculas: A, a, B, b, C, c, ... para o tipo de Texto.

* `desc ci`

   ordem decrescente não diferencia maiúsculas de minúsculas: ..., C, c, B, b, A, a para o tipo Texto.

Use o `key` para acessar propriedades dentro de objetos complexos.

Use nomes de variáveis brutos para chaves.

Para acessar propriedades aninhadas, use a notação de pontos.

O primeiro item em uma matriz é o índice 1.

>[!INFO]
>
>**Exemplos:**
>
>* `sort(Contacts[];name)`
   >
   >    Classifica uma matriz de contatos pela propriedade &quot;name&quot; em ordem crescente padrão
>
>* `sort(Contacts[];desc;name)`
   >
   >   Classifica uma matriz de contatos pela propriedade &quot;name&quot; em ordem decrescente
>
>* `sort(Contacts[];asc ci;name)`
   >
   >    Classifica uma matriz de contatos pela propriedade &quot;name&quot; em ordem crescente que não diferencia maiúsculas de minúsculas
>
>* `sort(Emails[];sender.name)`
   >
   >    Classifica uma matriz de emails pela propriedade &quot;sender.name&quot;


## [!UICONTROL arrayDiferença [array1, array2, modo]]

Retorna a diferença entre duas matrizes.

Insira um dos valores a seguir para a variável `mode` parâmetro.

* `classic`: Retorna uma nova matriz que contém todos os elementos de `array1` que não existem no `array2`.

* `symmetric`: Retorna uma matriz de elementos que não são comuns a ambas as matrizes.

   Em outras palavras, a função retorna uma matriz que contém todos os elementos de `array1` que não existem no `array2`e todos os elementos de `array2` que não existem no `array1`.

   >[!INFO]
   >
   >**Exemplos:**
   >
   >Considerando os seguintes arrays:
   >
   >
   ```
   >myArray = [1,2,3,4,5]
   >```
   >
   >
   ```
   >yourArray = [3,4,5,6,7]
   >```
   >
   >* `arrayDifference [myArray, yourArray, classic]`
      >
      >    Devoluções `[1,2]`
   >
   >* `arrayDifference [yourArray, myArray, classic]`
      >
      >    Devoluções `[6,7]`
   >
   >* `arrayDifference [myArray, yourArray, symmetric]`
      >
      >    Devoluções `[1,2,6,7]`

