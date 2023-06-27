---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funções de matriz no Adobe Workfront Fusion
description: As seguintes funções de matriz estão disponíveis no painel de mapeamento do Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Funções de matriz no Adobe Workfront Fusion

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
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
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

## [!UICONTROL adicionar (matriz; valor1; valor2; ...)]

Adiciona valores especificados em parâmetros a uma matriz e retorna essa matriz.

## [!UICONTROL contains (matriz; valor)]

Verifica se uma matriz contém o valor.

## [!UICONTROL distinct (matriz; [key])]

Remove duplicatas dentro de uma matriz. Use o &quot;[!UICONTROL key]&quot; para acessar propriedades dentro de objetos complexos. Para acessar propriedades aninhadas, use a notação de pontos. O primeiro item em uma matriz é o índice 1.

>[!INFO]
>
>**Exemplo:** `distinct(Contacts[];name)`
>
>Remove duplicatas dentro de uma matriz de contatos comparando a propriedade &quot;name&quot;

## [!UICONTROL nivelar (matriz)]

Cria uma nova matriz com todos os elementos de submatriz concatenados nela, recursivamente, até a profundidade especificada.


## [!UICONTROL junção (matriz; separador)]

Concatena todos os itens de uma matriz em uma cadeia de caracteres, usando o separador especificado entre cada item.

## [!UICONTROL chaves (objeto)]

Retorna uma matriz das propriedades de um determinado objeto ou matriz.

## [!UICONTROL length (matriz)]

Retorna o número de itens em uma matriz.

## [!UICONTROL map (matriz complexa; chave;[chave para filtragem];[valores possíveis para filtragem])]

Retorna uma matriz primitiva contendo valores de uma matriz complexa. Esta função permite filtrar valores. Use nomes de variáveis brutos para chaves.

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
>  Retorna uma matriz primitiva com emails com rótulo igual a trabalho ou casa

Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL mesclar (matriz1; matriz2; ...)]

Mescla uma ou mais matrizes em uma matriz.

## [!UICONTROL remover (matriz; valor1; valor2; ...)]

Remove valores especificados nos parâmetros de uma matriz. Esta função só é eficaz em matrizes primitivas de texto ou números.

## [!UICONTROL inverter (matriz)]

O primeiro elemento da matriz se torna o último elemento, o segundo se torna o próximo ao último e assim por diante.

## [!UICONTROL fatia (matriz; início; [fim])]

Retorna uma nova matriz contendo apenas itens selecionados.

## [!UICONTROL sort (matriz; [pedido]; [key])]

Classifica os valores de uma matriz. Os valores válidos de `order` parâmetros são:

* `asc`

  (padrão) - ordem crescente: 1, 2, 3, ... para o tipo Número. A, B, C, a, b, c, ... para texto

* `desc`

  ordem decrescente: ..., 3, 2, 1 para o tipo Number. ..., c, b, a, C, B, A para texto.

* `asc ci`

  ordem crescente que não diferencia maiúsculas de minúsculas: A, a, B, b, C, c, ... para o tipo Text.

* `desc ci`

  ordem decrescente que não diferencia maiúsculas de minúsculas: ..., C, c, B, b, A, a para tipo de Texto.

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
>   Classifica uma matriz de contatos pela propriedade &quot;name&quot; em ordem descendente
>
>* `sort(Contacts[];asc ci;name)`
>
>    Classifica uma matriz de contatos pela propriedade &quot;name&quot; em ordem crescente que não diferencia maiúsculas de minúsculas
>
>* `sort(Emails[];sender.name)`
>
>    Classifica uma matriz de emails pela propriedade &quot;sender.name&quot;

## [!UICONTROL arrayDifference [matriz1, matriz2, modo]]

Retorna a diferença entre duas matrizes.

Insira um dos seguintes valores para a variável `mode` parâmetro.

* `classic`: retorna uma nova matriz que contém todos os elementos de `array1` que não existem no `array2`.

* `symmetric`: retorna uma matriz de elementos que não são comuns a ambas as matrizes.

  Em outras palavras, a função retorna uma matriz que contém todos os elementos de `array1` que não existem no `array2`e todos os elementos de `array2` que não existem no `array1`.

  >[!INFO]
  >
  >**Exemplos:**
  >
  >Considerando as seguintes matrizes:
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
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
